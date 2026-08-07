# CIO / CTO / CDO Coordination Pattern — The AI Platform Runs on Their Systems

## Motivation

The head of AI governance does not build the AI platform. The
CIO owns the enterprise's information technology; the CTO owns
the technology delivery and often the AI platform specifically;
the CDO owns the enterprise data governance parent framework
and, where the enterprise has designated the role, the AI
platform's data side. In many enterprises the AI platform is
delivered through a joint CIO / CTO organisation, sometimes
under a Chief AI Officer (see the CAIO adjacency in
[[mod-101-role-scope-and-leadership-shape]] chapter 06). In
any of these arrangements, the head's AIMS runtime — the
control-testing pipelines, the evaluation harness, the
evidence collection, the audit-ready inventory queries — is a
*consumer* of the platform, not its owner.

The failure mode this chapter is written against is the head
who tries to build a parallel AI platform. The reasoning is
usually reasonable — "the CIO's platform does not have the
governance hooks we need, so we will build them ourselves" —
and the outcome is uniformly bad: two model registries with
divergent metadata, two evidence stores that neither the CAE
nor an EU AI Act notified body knows which to trust, two
deployment paths that produce two provenance chains, and a
CIO / CTO organisation that treats the head's function as an
adversary rather than a partner. The coordination pattern in
this chapter is what prevents that.

The pattern draws on ISO/IEC 42001 clause 8 (operational
planning and control), the MLOps discipline as described in
the various vendor and open-source references (MLflow, Kubeflow,
Vertex AI Model Registry, Databricks Unity Catalog, SageMaker
Model Registry, and enterprise offerings), NIST AI RMF MAP and
MEASURE functions, and the data-governance dimensions of DAMA-
DMBOK 2 and ISO/IEC 38505. It is executed against a specific
governance-runtime specification the head's level-50 architect
authors and the `ai-infra-mlops` role (level 25) implements on
the CIO / CTO / CDO side.

## Core concept — the governance runtime plugs into the platform

The load-bearing move is to write down, precisely, what the
governance runtime needs from the AI platform and what the
governance runtime returns to the platform. This is not "we
need better MLOps"; it is a technical specification, jointly
authored and jointly owned, that treats the AIMS operating
runtime as a *plugin* into the platform's runtime rather than
as a separate stack.

The three sub-specifications the head co-authors:

1. **The metadata contract.** What the model registry, the
   feature store, the training-data catalogue, and the
   deployment platform expose to the governance runtime, in
   what schema, at what freshness. Without the contract, the
   AIMS inventory ([[mod-102-running-the-program]] chapter
   06) drifts against the reality on the platform.
2. **The evidence contract.** What deployment events, training
   runs, evaluation runs, and inference traces are emitted
   into the governance evidence store, in what format, with
   what retention. Without the contract, evidence completeness
   (KPI 8 in [[mod-107-program-measurement-and-maturity]]
   chapter 01) will trend down over time as the platform
   changes and no one re-wires the evidence flows.
3. **The gate contract.** Which release, promotion, and
   configuration events call the governance-runtime check
   before proceeding, in what synchronous or asynchronous
   mode, with what fail-open or fail-closed semantics. Without
   the gate contract, "governance sign-off" becomes an out-of-
   band ticket that release engineers work around under
   deadline pressure.

The three contracts are the interface. The CIO / CTO's
platform team implements them. The head's level-50 architect
maintains them. The `ai-infra-mlops` role at level 25 (see the
adjacent role in the curriculum) executes the wiring on the
platform side.

## The three coordination surfaces

### Surface 1 — model registry integration

The AIMS inventory is a governance view of the models,
datasets, evaluation results, and deployment records that live
in the AI platform's own registries. It is *not* a separate
database the head's team maintains by hand. The failure mode
the interface prevents is the "shadow inventory" — a
governance-team spreadsheet that names models the platform
does not have and misses models the platform does have.

The metadata contract is the interface. At minimum, the
governance runtime queries the model registry for: model
identifier (stable across the model's lifecycle, including
retraining), semantic version, upstream training pipeline
reference, training-data version, evaluation-suite pass
record, deployment environment, current production status,
lineage back to prior versions, and the responsible product
owner. The contract specifies field names, freshness
guarantees, and access methods (API, event stream, database
view). Where the platform's registry does not carry a field
the governance runtime needs — e.g., the responsible product
owner, or a link to the AIA reference — the interface
specifies whether the field is added to the platform's schema
or maintained in a governance-side extension linked by
identifier. The head does not force the platform's schema; the
head and the platform lead negotiate the extension pattern.

Cadence: quarterly joint review of the metadata contract at
the AIMS operating calendar cycle; ad-hoc when the platform's
registry schema changes materially. Joint owner: the head's
level-50 architect and the CIO / CTO's ML platform lead;
`ai-infra-mlops` executes the schema-integration work.

### Surface 2 — data-governance interface (the CDO adjacency)

The CDO owns the enterprise data governance framework — data
catalogue, data lineage, data-quality controls, data-
classification taxonomy, master-data management. The head's
AI-specific extension: training-data provenance and consent,
evaluation-data curation (test-set contamination controls,
representativeness, held-out integrity), synthetic-data
governance, and data-poisoning-resistance controls at ingest.

The interface is a joint chapter in the enterprise data
governance policy — authored by the CDO's data-governance
lead and the head's level-50 architect, ratified in the data
governance council (which the CDO chairs) and in the AI
governance council (which the head chairs, per chapter
[[11-chairing-the-governance-council]]). The chapter names:

- **Training-data provenance requirements.** For each AI
  system tier (see [[mod-102-running-the-program]] chapter
  06), the required provenance depth — source system, consent
  basis (if personal data), licence terms (if third-party),
  ingest date, transformation lineage.
- **Evaluation-data curation requirements.** The requirements
  for held-out evaluation sets — how they are separated from
  training, how contamination is prevented, how
  representativeness is measured, how the sets are versioned
  and rotated.
- **Synthetic-data governance.** Where synthetic data is
  used, the disclosure requirement, the fidelity/utility/
  privacy trade-off documentation, and the specific approvals
  needed at each AI system tier.
- **Data-poisoning controls.** For AI systems ingesting
  external data (web scraping, third-party feeds, RAG source
  registries), the poisoning-resistance controls the ingest
  pipeline enforces and the monitoring the CDO's data-quality
  function runs.

Cadence: annual joint review at the data governance council;
quarterly on new AI system onboarding. Joint owner: CDO's
data-governance lead and the head's level-50 architect.

### Surface 3 — MLOps runtime and release-assurance gate

The MLOps runtime is where the governance gate physically
lives. When a model is promoted from staging to production, or
when a production model is retrained and re-released, or when
a feature-flagged agentic capability is enabled for a new
population, the release event is what triggers the governance-
runtime check. The gate contract governs how.

Two design choices carry the load. First, whether the gate is
*synchronous* (the release pipeline waits for the governance
runtime's answer before proceeding) or *asynchronous* (the
release proceeds; the governance runtime evaluates in parallel
and can trigger rollback if the check fails). Second, whether
the gate is *fail-open* (a governance-runtime timeout permits
the release) or *fail-closed* (a governance-runtime timeout
blocks the release). Different AI system tiers may warrant
different design choices; the interface specifies which tier
uses which combination and why.

The gate check itself is a joint-authored specification. The
level-50 architect authors it; `ai-infra-mlops` implements the
integration on the platform's CI/CD; the CIO / CTO's release
engineering lead owns the release pipeline's overall
correctness. Typical checks: AIMS inventory current for this
model, AIA on file for this system at the required tier depth,
evaluation-suite most-recent-run at required pass rate,
required approvals recorded, no open blocking exception
against this system.

Cadence: gate specification versioned; changes ratified at the
AI governance council and communicated to the release-
engineering function in advance of the release cycle they
apply to. Joint owner: level-50 architect and the CIO / CTO's
release engineering lead.

## The AI-platform ownership handoff

A specific coordination move worth naming: the *ownership
handoff* when a new AI capability moves from an initial
research or exploration environment (often owned by the AI
research function or a product team's data-science group) into
the CIO / CTO's platform for production. The handoff is where
governance controls are usually first applied, and it is where
they are usually first *skipped* if the handoff protocol is not
written down.

The handoff is a joint procedure between the originating team,
the CIO / CTO's platform lead, and the head's function. At the
handoff, the AIMS inventory record is created, the AIA is
opened (if not already), the required evidence artefacts are
attached (model card, evaluation results, training-data
provenance record), the platform-side onboarding is initiated
(registration in the model registry, wiring into the release
pipeline, integration into the observability stack), and the
governance-gate configuration is applied. The handoff protocol
is jointly authored — head's level-50 architect, CIO / CTO's
platform lead, and the CDO's data-governance lead — and
maintained in the same document control as the interface
document with the CISO.

The load-bearing detail: the handoff protocol is a *gate*, not
a checklist people work around. A production AI system that
did not go through the handoff is a system the head's function
does not have inventoried, is a system the CAE will find in
audit, and is a system the audit committee will read as an
uncontrolled release. The gate discipline is what prevents the
long tail of "shadow AI" — production capabilities that
predate or bypass the governance runtime and never get
regularised.

## The interface document

Consolidated into a single interface document, co-signed by the
head, the CIO, the CTO (where distinct), and the CDO, ratified
in the CxO adjacency map. The document has, at minimum:

1. **Scope statement.** What is in scope for the interface
   (production AI systems on the enterprise AI platform;
   handoff protocol for new systems; MLOps release pipeline;
   data-governance interface). What is not in scope (research
   environments below the handoff threshold; sunset systems
   past retirement).
2. **The three contracts.** Metadata contract, evidence
   contract, gate contract — each with schema references,
   freshness / latency guarantees, fail semantics, and change-
   management protocol.
3. **The three surfaces.** Model registry integration, data-
   governance interface, MLOps runtime and release-assurance
   gate — each with cadence and joint owner.
4. **The handoff protocol.** Named steps, named owners at each
   step, the gate that determines whether production status is
   granted.
5. **The escalation ladder.** When the interface breaks — a
   metadata contract field falls out of freshness, an evidence
   contract stream is disrupted, a gate is bypassed under
   production pressure — how the head, CIO / CTO, and CDO
   escalate. Typically: peer-conversation first, then the CAIO
   or CEO, then the audit committee for material breaches.
6. **The joint audit-committee appearance.** Once a year, the
   head appears jointly with the CIO / CTO on the AI platform
   review at the audit committee, and jointly with the CDO on
   the data-governance review. The joint appearances are the
   discipline that keeps the interface honest across turnover.
7. **The review cadence.** Annual review of the interface
   document itself; ad-hoc on material platform changes.

## Anti-patterns the head does not permit

**The shadow inventory.** The head's team maintains an
inventory spreadsheet that has drifted from the platform's
model registry. The remedy is: the AIMS inventory is a
governance *view* over the platform's registries, not a
separate database. If the view has to be maintained by hand,
the metadata contract is broken and the head's first move is
to fix the contract, not to reconcile spreadsheets.

**The parallel evidence store.** The head's team stores
evidence in its own store that the platform's audit-log
retention does not know about. The evidence is orphaned when
the head's tooling is retired. The remedy is: evidence lives
in the enterprise's evidence-of-record system (typically the
platform's audit-log store extended for governance metadata),
with the AIMS evidence store as a governance-scoped view.

**The out-of-band gate.** The governance sign-off is an email
or a ticket the release engineer processes as a manual step,
not a gate the release pipeline enforces. Under deadline
pressure, the manual step gets skipped and the release
proceeds. The remedy is: the gate lives in the release
pipeline as a machine-enforced check, with fail semantics
appropriate to the AI system tier, and any bypass is logged as
a policy exception that the exception-and-waiver register
picks up ([[mod-102-running-the-program]] chapter 05 exception
discipline).

**The head-authored platform requirement.** The head writes
platform requirements that describe how the platform *should*
be built — architecture prescriptions, tool choices, vendor
selections — outside the CIO / CTO's own architecture-and-
delivery discipline. The CIO / CTO reads this as encroachment
and the requirements get ignored. The remedy is: the head
authors *governance requirements* against the platform's
capabilities; the CIO / CTO decides how the platform meets the
requirements.

## Composition with adjacent modules

- The **CxO adjacency map** in
  [[mod-101-role-scope-and-leadership-shape]] chapter 06 is
  the parent boundary document.
- The **AIMS inventory** in [[mod-102-running-the-program]]
  chapter 06 is the governance view whose freshness the
  metadata contract governs.
- The **AI risk register** in [[mod-102-running-the-program]]
  chapter 03 is where the platform-related risks (gate bypass,
  evidence orphaning) get carried and monitored.
- The **evidence-completeness metric** in
  [[mod-107-program-measurement-and-maturity]] chapter 01 is
  the KPI the evidence contract's effectiveness is measured
  against.
- The **incident-leadership discipline** in
  [[mod-110-incident-leadership]] is where a gate bypass or a
  platform-side incident triggers the joint response.
- The **CISO coordination** in chapter 01 of this module is
  where the platform's telemetry feeds the SOC-side detection
  stack.

## Summary

- The head does not build the AI platform; the CIO / CTO does,
  with the CDO owning the enterprise data-governance parent.
  The head's governance runtime plugs into the platform as a
  consumer.
- Three contracts govern the plug-in: the metadata contract
  (what the platform exposes to the governance runtime); the
  evidence contract (what events flow into the evidence store);
  the gate contract (what release events call the governance
  check, in what mode, with what fail semantics).
- Three coordination surfaces implement the contracts: model
  registry integration, data-governance interface (with the
  CDO), and MLOps runtime and release-assurance gate.
- The AI-platform ownership handoff is the gate that prevents
  the long tail of shadow AI. The handoff protocol is jointly
  owned and machine-enforced.
- Four anti-patterns to refuse: shadow inventory, parallel
  evidence store, out-of-band gate, head-authored platform
  requirements. Each of these fails audit and each of these
  is preventable through the contract discipline.
- The interface document — co-signed by head, CIO, CTO, and
  CDO — is ratified in the CxO adjacency map, reviewed
  annually at the audit committee, and maintained by the
  level-50 architect on the head's side with
  `ai-infra-mlops` executing on the platform side.
- Chapter [[03-cpo-dpo-coordination]] turns to the privacy
  adjacency — the AIA / DPIA interface, the ROPA interface,
  and the GDPR / CPPA / DPDPA obligations that divide across
  the AI-scope and enterprise-scope boundary.
