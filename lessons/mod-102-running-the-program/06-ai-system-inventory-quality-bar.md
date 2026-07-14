# Owning the AI System Inventory Quality Bar

## Motivation

Every regulator, certification body, and third-line auditor asks
essentially the same first question: *what AI systems do you operate,
and where are they in their lifecycle?* An enterprise that cannot
answer that question on demand — completely, currently, and
consistently — has already failed the audit before any control has
been sampled.

The AI system inventory is the answer. It is the authoritative
enumeration of every AI system the enterprise builds, deploys, or
consumes, with the metadata required to link every system to its
impact assessment, its risk register entries, its supply-chain
evidence, its release-decision packet, its post-market surveillance
telemetry, its incident history, and its retirement plan. Under the
EU AI Act, Articles 12 and 26 impose logging and record-keeping
obligations on providers and deployers; Article 60 imposes registration
of high-risk systems in the EU database; the AIMS under ISO/IEC 42001
imposes documented information covering the AI systems the AIMS is
scoped to. The inventory is the substrate for all of it.

The level-50 architect designed the inventory schema (see
[[mod-101-role-scope-and-leadership-shape]] chapter 01). The head owns
the *operating discipline* that the inventory is complete, current,
and defensible under regulator inspection. This chapter is that
operating discipline.

## Core concept: three quality properties, one operating bar

The inventory has three quality properties the head owns and defends,
each with a specific meaning:

- **Complete.** Every AI system that meets the enterprise's
  in-scope definition is present. No shadow systems, no
  business-unit-specific inventories that never surface, no
  procurement-purchased AI services outside the tracked
  perimeter.
- **Current.** Every material change to any system — release,
  version upgrade, retraining, retirement, ownership change,
  regulatory classification change — is reflected within a bounded
  window (typically 5 to 10 business days for non-material changes,
  same-day for material changes).
- **Consistent.** Every field is populated to the same depth for
  every system; every dropdown value comes from the schema's
  controlled vocabulary; every cross-reference (to impact assessment,
  to risk register, to ML-BOM, to model card) resolves to a live
  artefact.

An inventory that is only two of the three fails. Complete and
current but inconsistent is unusable as evidence. Complete and
consistent but not current is a snapshot, not an inventory. Current
and consistent but not complete is a fiction because shadow systems
are exactly where the material risk lives.

The head is the accountable executive for all three.

## What "in-scope" means — the definition the head enforces

The inventory's in-scope definition is derived from the level-50
architect's AIMS scope statement (chapter 02) and specialised to
enterprise practice. The head does not personally decide what is in
scope; the head enforces the derived definition consistently across
business units.

A workable definition typically includes:

- Any system that uses machine learning, foundation-model inference,
  agentic behaviour, or algorithmic decisioning to produce output
  that affects an enterprise decision, customer experience, employee
  experience, or regulated outcome.
- Any procured or contracted AI service where the enterprise is the
  deployer under EU AI Act terminology or the user of an outsourced
  model under sector rules.
- Any research or experimental AI system that has left the pure-
  research boundary (touched real data, touched real users, touched
  real production infrastructure).
- Any AI-adjacent decision-support system whose outputs are trusted
  as if they were AI-produced, regardless of its underlying
  implementation.

Explicitly *excluded* from the inventory — with the exclusion
documented so a regulator can see the reasoning:

- Pure classical statistical models under the enterprise's parent
  MRM framework where the AIMS scope statement excludes them
  (common in banking where SR 11-7 pre-dates ISO/IEC 42001 and the
  scope statement carves out classical MRM).
- Rule-based systems with no learned parameters (though
  documentation of the exclusion is itself an artefact).
- Personal-productivity AI usage by employees under the enterprise
  acceptable-use policy, unless it produces enterprise decisions
  (in which case it is in scope regardless of who provisioned it).

The head reviews the in-scope definition annually and any time the
level-50 architect updates the AIMS scope. Every business unit knows
the definition; every intake channel (procurement, engineering,
research, business-unit product) applies it.

## The inventory schema — what the architect specified

The architect specified the schema. The head reads it well enough to
defend it. A defensible schema — the operative fields the head
enforces at intake and update — typically contains:

- **System ID.** Monotonic identifier, unique across all business
  units and lifecycle stages.
- **System name and description.** Human-readable name; three-to-
  five-line description covering purpose, users, and decisioning role.
- **Business unit and executive owner.** The first-line accountable
  executive at SVP or above for material systems, at director for
  non-material.
- **Second-line owner.** The AI governance analyst (level 15) or
  risk engineer (level 25) with second-line responsibility.
- **Lifecycle stage.** Concept / development / evaluation / staging
  / production / post-market / retiring / retired.
- **Regulatory classification.** EU AI Act classification
  (prohibited / high-risk / limited-risk / minimal-risk / GPAI / not
  in scope); sector classifications (banking model materiality
  tier under SR 11-7, medical device class under FDA, high-risk
  under the Colorado AI Act, etc.); jurisdictional applicability.
- **Provider / deployer role.** The enterprise's role under
  EU AI Act terminology (provider, deployer, distributor,
  importer) and equivalent sector terminology, per system.
- **Impact assessment reference.** Pointer to the impact assessment
  under ISO/IEC 42005 or equivalent (banking model validation,
  medical-device design history file, algorithmic impact assessment
  under the Canadian AIA, DPIA where applicable).
- **Risk register cross-reference.** Pointers to open and closed
  register rows (chapter 03) touching the system.
- **Model cards, system cards, dataset cards.** Pointers to the
  authored cards under evidence-architecture document control
  (chapter 07).
- **ML-BOM and SBOM.** Pointer to the CycloneDX ML-BOM and SPDX
  3.0 AI profile document for the system (chapter 07).
- **SLSA level and attestations.** Build-pipeline supply-chain
  integrity level and attestations (chapter 07).
- **Data sources and lineage.** Enumerated data sources, with
  regulatory tags (personal data, sensitive personal data, health
  data, biometric data, etc.) and data-lineage evidence.
- **Third-party dependencies.** Foundation models, vector stores,
  MLOps services, and other AI-family third-party dependencies
  keyed to the third-party program (chapter 07).
- **Post-market surveillance state.** For high-risk systems,
  Article 72 post-market monitoring plan state and Article 73
  serious-incident reporting posture.
- **Retirement plan and date.** Plan for retirement or refresh at
  the end of the intended-use window.
- **Last review date and next review date.** Cadence-tracked so
  reviews do not go stale.

The head does not personally populate the fields. The head enforces
that they are populated to the schema's depth for every in-scope
system, and that population is evidenced.

## Intake discipline — how systems land in the inventory

The inventory becomes stale primarily through weak intake. Three
intake channels the head owns:

- **Engineering intake.** Every new AI system entering the SDLC
  registers at project inception. The engineering intake gate is a
  first-line control — no development budget is released without an
  inventory record. The record is bare (name, purpose, tentative
  classification) at inception and populated through the lifecycle.
- **Procurement intake.** Every third-party AI service, model API,
  MLOps tool, or contract with an AI clause routes through the
  vendor-onboarding process (chapter 07) which creates or extends an
  inventory record. Procurement is enforced by the CFO / procurement
  policy; the head confirms the enforcement is real by sampling.
- **Research and experimental intake.** Research groups routinely
  build systems that later become production. A promotion gate — the
  point at which a research artefact leaves the research boundary —
  must be an inventory intake event. The head owns the promotion
  gate criteria and enforces its trigger.

A fourth channel exists in practice — *shadow discovery*. AI systems
built or procured outside the intake gates surface through incidents,
audits, or business-unit self-report. Every shadow discovery is a
non-conformity (chapter 02) with a root cause analysis: which gate
failed, why, and what changes to gate enforcement follow. Repeated
shadow discovery from the same business unit is diagnostic; the head
escalates through the CxO channel to the responsible executive.

## Refresh discipline — keeping the inventory current

The inventory is not populated once. It is refreshed on cadences the
head enforces:

- **Event-driven refresh.** Named events trigger immediate updates —
  version deployment, retraining, ownership change, classification
  change, incident, regulatory reclassification, retirement. The
  event-driven refresh path is automated where possible (integrations
  with the CI/CD pipeline, the MLOps platform, the ticketing system)
  and manual where not.
- **Quarterly system-owner attestation.** Every system's first-line
  owner attests, quarterly, that the inventory record is accurate.
  Attestation is a documented artefact; a failed or missing
  attestation is a non-conformity.
- **Annual full walk-through.** Once a year the head and the level-50
  architect (or their delegate) walk every material system's record
  end-to-end to verify field-level accuracy and cross-reference
  currency. The walk-through catches drift the event-driven and
  quarterly-attestation channels missed.
- **Regulator-triggered refresh.** When a regulator requests
  inventory data (which they will, both in examinations and in
  sector-wide inquiries), the inventory is refreshed against the
  specific ask before responding. The refresh discovers gaps the
  cadences did not.

## Making the inventory audit-defensible — the OSCAL / structured-evidence story

An inventory that lives in a spreadsheet is not defensible. An
inventory that lives in the GRC-for-AI platform, populated from the
authoritative first-line systems (source code repository, MLOps
platform, procurement system, ticketing), with structured evidence
attachments per field, and machine-readable exports (OSCAL for
control mapping, CycloneDX ML-BOM for supply-chain, JSON exports for
regulator queries), is.

The head enforces four properties on the inventory tooling:

- **Single source of truth.** One inventory of record, not several.
  Business-unit tools that hold local inventories feed the central
  inventory; they do not compete with it.
- **Field-level provenance.** Every field's value is traceable to
  its source — the authoritative first-line system, the responsible
  human attestation, or the timestamped ingest event.
- **Change history.** Every change to every record is retained with
  timestamp, author, and reason. Silent edits are not possible.
- **Machine-readable export.** The inventory exports to the formats
  regulators and auditors ask for — CSV for regulators without a
  preferred format, OSCAL for controls, ML-BOM and SPDX for
  supply-chain, custom JSON for the EU AI Act's future high-risk
  system database format when specified.

Under ISO/IEC 42006 a certification body will sample inventory
records and follow the cross-references. When a model-card pointer
does not resolve, or an impact-assessment reference points to a
document under revision without a locked version, the sample fails.

## Composition with the EU AI Act's Article 60 EU database

EU AI Act Article 60 requires providers of high-risk AI systems to
register their systems, and Chapter III Section 4 imposes provider
and deployer obligations that flow through the enterprise's own
records. The EU database registration is a separate artefact from the
enterprise inventory but sources its data from it. The head must:

- Identify which of the enterprise's systems require Article 60
  registration (all high-risk systems the enterprise provides in
  the EU, plus certain public-authority deployments under Article
  60(2)).
- Ensure the inventory record carries every field the registration
  requires, and that the extract-to-registration path is a
  documented process, not a manual re-authoring.
- Track the state of each registration (submitted, live, updated,
  suspended) as a field in the inventory record.
- Feed the registration content into the AI governance council for
  ratification before submission, and to the GC for legal-position
  review.

The head does not personally submit registrations; the regulatory-
affairs function typically does. The head ensures the underlying data
is defensible.

## Composition with post-market surveillance

Under EU AI Act Article 72, providers of high-risk AI systems
establish and document a post-market monitoring system. Under Article
73, providers report serious incidents. The inventory is the surface
against which post-market surveillance runs — telemetry per system,
incident state per system, retraining triggers per system, drift
monitoring per system all attach to the inventory record.

The level-50 architect designed the post-market surveillance
architecture. The head runs it against the inventory, ensuring that:

- Every high-risk system has a documented post-market monitoring
  plan attached to its inventory record.
- Post-market telemetry actually flows into the plan's dashboards
  and the drift, degradation, and incident signals fire against
  the risk register (chapter 03).
- Article 73 serious-incident classification is applied consistently
  and the reporting-decision cadence is documented per system, per
  jurisdiction. See [[mod-110-incident-leadership]] for the incident
  response discipline.

An inventory that stops tracking a high-risk system once it enters
production has failed the post-market obligation. The head ensures
the lifecycle-state field is honestly maintained through the
production stage, and that the retirement path is a controlled event,
not an abandonment.

## Composition with the risk register

The inventory and the risk register (chapter 03) cross-reference
each other. Every risk-register row lists the systems affected;
every inventory record lists its open and closed risks. The
composition is deliberate — a risk without a system is either an
enterprise-scope risk (parent enterprise register) or a taxonomy
placeholder (which should be closed), and a system without any risk
history is either brand-new or under-analysed.

The head runs a periodic reconciliation between the two data
structures and treats orphaned references as debt. Orphaned
references are exactly the inconsistency regulators surface when they
cross-check the inventory against incident records.

## Example — a shadow-discovery incident, minute-shaped

A worked example. A customer-service team, under pressure to reduce
handle time, procured a third-party generative-AI chatbot on a
credit-card subscription and deployed it into their internal
knowledge-base assistant workflow. It never went through procurement
intake, never touched engineering intake, never appeared in the
inventory. Six months into use, an incident (the chatbot produced a
hallucinated product-recall claim to a customer) surfaces it.

The head's operating discipline plays out as follows.

- The incident triage (see [[mod-110-incident-leadership]]) opens a
  register row (chapter 03) with the standard fields; category
  transparency / robustness, subcategory hallucination on
  customer-facing text.
- The inventory intake gate is triggered retroactively: a new
  inventory record is opened for the system, backdated to the actual
  deployment date, with every field populated to schema depth. The
  system's classification under EU AI Act is assessed (limited-risk
  transparency obligation under Article 50 applies because it
  interacts with humans in a customer-service context; no high-risk
  classification applies because the outcomes are not
  determinative).
- The procurement intake failure — the credit-card procurement path
  bypassed the vendor-onboarding process — is opened as a
  non-conformity (chapter 02) against the procurement policy. Owner:
  CFO's procurement function, with second-line challenge from the
  head. Corrective action: tighten credit-card-purchase
  reconciliation to flag AI-service subscriptions.
- The council reviews (chapter 01). The council ratifies the
  reactive controls (chatbot suspended pending impact assessment,
  customer notification handled by CCO), the non-conformity plan,
  and adds "recurrent shadow-procurement risk" as a standing risk
  row for the coming six months to check whether the corrective
  action is landing.
- The audit committee is briefed at its next cycle (chapter 01 and
  [[mod-103-board-and-audit-committee-reporting]]), including the
  inventory-completeness implication.

Every step is captured. Every step is defensible. The inventory
becomes more complete rather than less credible.

## Common failure modes

- **Spreadsheet-of-record.** An inventory in a shared spreadsheet
  has no field-level provenance, no change history, no
  machine-readable export, and no defensible integrity. This is
  the single most common failure mode. The head insists on
  platform-of-record from day one.
- **Business-unit inventories that never surface.** Business
  units maintain their own inventories for local ops and never
  federate them to the central inventory. The result is a central
  inventory that under-counts, undetectably. The head resolves
  this through mandatory federation, not through duplication.
- **Fields populated to different depths.** Some systems' records
  are complete; others have every field at "TBD." Consistency
  fails; sampling fails. The head enforces schema-depth on every
  in-scope record.
- **Stale cross-references.** A model-card pointer resolves to a
  deleted document; an impact-assessment reference points at a
  draft never approved. The head runs a cross-reference integrity
  check monthly.
- **Shadow discovery as normal.** Repeated shadow discovery is
  taken as unavoidable and not escalated. This is a governance
  failure the audit committee will surface if the head does not.

## Summary

- The AI system inventory is the substrate for regulator inspection,
  certification-body sampling, and the enterprise's own AIMS
  operation; the level-50 architect designed the schema and the
  head owns the operating discipline that it is complete, current,
  and consistent.
- The in-scope definition is derived from the AIMS scope statement,
  reviewed annually, and enforced consistently across engineering,
  procurement, and research intake channels.
- Intake discipline covers three channels — engineering,
  procurement, research — with shadow discovery as a fourth
  channel that is always a non-conformity.
- Refresh discipline is layered — event-driven, quarterly
  attestation, annual walk-through, and regulator-triggered
  refresh — each with a documented cadence and owner.
- The inventory tooling is a single source of truth with
  field-level provenance, change history, and machine-readable
  export in the formats regulators and auditors expect (OSCAL,
  CycloneDX ML-BOM, SPDX AI, CSV, JSON).
- The inventory composes with EU AI Act Article 60 registration,
  Articles 72 / 73 post-market surveillance and serious-incident
  reporting, and the enterprise risk register (chapter 03); each
  composition is a documented cross-reference the head runs
  periodic reconciliation against.
- Five failure modes — spreadsheet-of-record, unfederated
  business-unit inventories, uneven field depth, stale cross-
  references, normalised shadow discovery — are the leading
  indicators of an inventory that will fail an audit. The head
  watches for all five.
