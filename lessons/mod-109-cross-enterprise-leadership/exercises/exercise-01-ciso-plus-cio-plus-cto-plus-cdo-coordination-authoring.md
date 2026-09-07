# exercise-01: CISO + CIO + CTO + CDO Coordination Authoring

**Estimated effort:** 4 hours

## Objective

Author the **technical-adjacency interface set** — one
document co-signed by the head and each of the CISO, the
CIO / CTO, and the CDO — that operationalises chapters
[01-ciso-coordination](../01-ciso-coordination.md) and
[02-cio-cto-cdo-coordination](../02-cio-cto-cdo-coordination.md).
The deliverables are the two written interface documents,
plus the technical-specification set the interface documents
reference (finding template for SOC routing, metadata /
evidence / gate contract specifications for the AI platform,
data-governance policy chapter for the CDO adjacency, ownership-
handoff protocol). These are the artefacts the head takes to
the CISO, the CIO / CTO, and the CDO for co-signature and then
ratifies in the audit-committee-visible CxO adjacency map from
[[mod-101-role-scope-and-leadership-shape]] chapter 06.

The interface set has to survive three stress tests. First,
the CISO's SOC lead reads the finding template and confirms
the SOC can ingest and triage it under the standard SLA — a
template with fields the SOC cannot parse or a severity
mapping the SOC does not use fails the test. Second, the
CIO / CTO's ML platform lead reads the three contracts
(metadata, evidence, gate) and confirms the platform can
expose the fields at the required freshness — a contract that
requires a schema the platform does not have and that no one
has agreed to build is a contract that will not exist in
practice. Third, the CAE reads the interface set and can
answer, without a walking tour, what is in scope, what is
out of scope, and where the boundaries sit — an interface set
that requires a briefing to interpret fails the audit-committee
readability standard.

The interface set is not a set of PowerPoint slides. It is a
governance artefact.

## Prerequisites

- Chapter [01-ciso-coordination](../01-ciso-coordination.md)
  — the four coordination surfaces with the CISO (AI risk
  register / ISMS composition, red-team finding routing,
  detection engineering, incident joint response), the
  interface-document structure, and the three anti-patterns
  (parallel triage queue, separate incident bridge, head-
  owned detection rule) — read and internalised.
- Chapter [02-cio-cto-cdo-coordination](../02-cio-cto-cdo-coordination.md)
  — the three contracts (metadata, evidence, gate), the
  three coordination surfaces, the AI-platform ownership
  handoff, and the four anti-patterns (shadow inventory,
  parallel evidence store, out-of-band gate, head-authored
  platform requirements) — read and internalised.
- [[mod-101-role-scope-and-leadership-shape]] chapter 06
  (CxO adjacency map) — the boundary map the interface
  documents plug into.
- [[mod-102-running-the-program]] chapter 03 (AI risk
  register), chapter 06 (AIMS inventory), chapter 08
  (evaluation discipline) — the AIMS artefacts the interface
  documents compose with.
- Primary sources cited in `resources.md` — CISA / NCSC
  "Guidelines for Secure AI System Development"; CISA
  "Deploying AI Systems Securely"; MITRE ATLAS; OWASP LLM
  Top 10 v2; NIST SP 800-218A; ISO/IEC 27001 clause 6.1.2;
  ISO/IEC 42001 clause 8; NIST AI RMF MAP and MEASURE
  functions.
- A concrete enterprise in mind — sector, AI-platform
  maturity, whether the enterprise has a CIO / CTO split or
  a combined role, whether the CDO role exists distinctly or
  sits under the CIO, and the current AI system portfolio
  shape (see [[mod-102-running-the-program]] chapter 06).

## Steps

1. **Enterprise context one-pager.** Author the half-page
   context the interface set operates against: sector, AI-
   platform architecture at a summary level (single platform
   versus federated by business unit; on-prem versus cloud
   versus hybrid), current CISO's operating model (SIEM
   platform, vulnerability-management platform, incident-
   response convention), current CIO / CTO's MLOps stack
   (model registry, deployment platform, CI/CD), current
   CDO's data-governance framework (data catalogue, lineage,
   quality controls). Every subsequent artefact references
   this one-pager.

2. **The CISO interface document.** Author the co-signed
   interface document (6 to 12 pages) with the seven required
   sections from chapter 01:
   - Scope statement (in-scope: AI-specific security
     concerns per MITRE ATLAS and OWASP LLM Top 10; out-of-
     scope: classical application-security concerns that
     route through the SOC's standard process).
   - The four surfaces, each with inbound/outbound signal
     specification, cadence, and joint owner.
   - Severity mapping (AI-specific severity to CISO
     incident-severity levels, named explicitly).
   - Evidence-sharing protocol (where the AIMS evidence
     store and the CISO's evidence store federate versus
     duplicate).
   - Escalation ladder (when interface breaks — SOC does
     not triage inside SLA; specification does not turn into
     a detection rule inside a quarter; incident co-response
     diverges).
   - Joint annual audit-committee appearance.
   - Review cadence and version discipline.

3. **The finding template for SOC routing.** Author the
   specific finding template every red-team finding uses. At
   minimum:
   - Finding identifier, discovery date, discovering
     principal.
   - Affected AIMS system identifier (referenced against the
     inventory from [[mod-102-running-the-program]] chapter
     06).
   - Finding class (MITRE ATLAS technique IDs where
     applicable; OWASP LLM Top 10 categories where
     applicable).
   - Head's recommended severity (with explicit mapping to
     the CISO's severity taxonomy).
   - Reproducible proof-of-concept (with confidentiality
     controls).
   - Exploitation conditions (what a real-world exploit
     requires).
   - Recommended remediation approach (as input, not as
     decision).
   The template is machine-parseable — the SOC's ingestion
   API can consume it — with a human-readable rendering.

4. **The four AI-specific detection-engineering
   specifications.** Author, at chapter-01 depth, the four
   named specifications:
   - Prompt-injection detection at the API gateway or
     model-serving layer.
   - Model-extraction detection.
   - Training-data leakage detection at inference.
   - Agent tool-use anomaly detection.
   Each specification names the observable, the detection
   window, the expected false-positive rate, and the
   telemetry source the SOC's detection engineer will
   implement against. The specifications are inputs to the
   SOC's implementation, not implementations themselves.

5. **The CIO / CTO / CDO interface document.** Author the
   co-signed interface document (8 to 14 pages, longer than
   the CISO document because of the three-signatory scope)
   with the seven required sections from chapter 02:
   - Scope statement.
   - The three contracts (metadata, evidence, gate) with
     schema references, freshness / latency guarantees, fail
     semantics, and change-management protocol.
   - The three surfaces (model registry integration, data-
     governance interface, MLOps runtime and release-
     assurance gate).
   - The AI-platform ownership handoff protocol.
   - Escalation ladder.
   - Joint annual audit-committee appearance (with the CIO / CTO
     on the AI platform, with the CDO on data-governance).
   - Review cadence and version discipline.

6. **The three contracts.** Author each contract as a
   discrete specification:
   - **Metadata contract.** Named fields the AIMS inventory
     query returns from the model registry, with schema,
     freshness guarantees, and access method. Where the
     platform's registry does not carry a required field, the
     contract names the extension pattern.
   - **Evidence contract.** Named deployment events, training
     runs, evaluation runs, and inference-trace events that
     flow into the governance evidence store, with format
     and retention.
   - **Gate contract.** Named release, promotion, and
     configuration events that call the governance-runtime
     check, with synchronous / asynchronous mode and fail-
     open / fail-closed semantics per AI system tier.

7. **The AI data-governance policy chapter.** Author the
   joint chapter — co-authored with the CDO's data-
   governance lead — that plugs into the enterprise data
   governance policy at the AI-specific rows: training-data
   provenance requirements per AI system tier, evaluation-
   data curation requirements, synthetic-data governance,
   data-poisoning-resistance controls. The chapter is
   drafted here for CDO sign-off; the exercise does not
   require live sign-off but produces the artefact ready for
   it.

8. **The AI-platform ownership handoff protocol.** Author
   the named-steps, named-owners protocol for when a new AI
   capability moves from research or exploration into the
   CIO / CTO's production platform. The protocol includes:
   - AIMS inventory record creation.
   - AIA opening (if not already).
   - Required evidence artefacts attached (model card,
     evaluation results, training-data provenance record).
   - Platform-side onboarding (registration in model
     registry, wiring into release pipeline, integration
     into observability stack).
   - Governance-gate configuration applied.
   - Named handoff owner on each side; named handoff-
     complete criterion.

9. **The failure-mode audit.** Author a short section — one
   paragraph per failure mode — naming how the interface set
   detects and recovers from each of the seven failure
   modes named across chapters 01 and 02:
   - Parallel triage queue (chapter 01).
   - Separate incident bridge (chapter 01).
   - Head-owned detection rule outside the SOC's SIEM
     (chapter 01).
   - Shadow inventory (chapter 02).
   - Parallel evidence store (chapter 02).
   - Out-of-band gate (chapter 02).
   - Head-authored platform requirements (chapter 02).

## Deliverables

- `enterprise-context.md` — the half-page context one-pager.
- `interface-ciso.md` — the co-signed CISO interface document.
- `finding-template.md` — the SOC-routing finding template
  with machine-parseable schema and human-readable rendering.
- `detection-specifications/spec-prompt-injection.md`,
  `spec-model-extraction.md`,
  `spec-training-data-leakage.md`,
  `spec-agent-tool-anomaly.md` — the four detection-
  engineering specifications.
- `interface-cio-cto-cdo.md` — the co-signed CIO / CTO / CDO
  interface document.
- `contract-metadata.md`, `contract-evidence.md`,
  `contract-gate.md` — the three contract specifications.
- `data-governance-ai-chapter.md` — the AI-specific joint
  chapter of the enterprise data-governance policy.
- `handoff-protocol.md` — the AI-platform ownership handoff
  protocol.
- `failure-mode-audit.md` — the seven-failure-mode detection-
  and-recovery paragraphs.

## Acceptance criteria

- The CISO interface document has all seven required
  sections and every surface has the inbound/outbound signal
  specification, cadence, and joint owner named. A section
  missing or a surface with an unnamed joint owner fails the
  criterion.
- The finding template has every field named in the
  chapter-01 minimum set, has an explicit severity mapping
  to the CISO's taxonomy, and is machine-parseable. A
  template without the severity mapping fails the criterion.
- Each detection-engineering specification names the
  observable, the detection window, the expected false-
  positive rate, and the telemetry source. A specification
  without these fails the criterion.
- The CIO / CTO / CDO interface document has all seven
  required sections; the three contracts are separate,
  discrete specifications with schema, freshness, and fail
  semantics; the handoff protocol is a gate, not a
  checklist. A contract expressed as prose without schema
  fails the criterion.
- The AI data-governance chapter is co-authored — the
  document names the head's substantive author and the
  CDO's data-governance lead — even where sign-off is not
  yet live.
- The failure-mode audit names, for each of the seven
  failure modes, at least one specific detection signal and
  one specific recovery action.
- Any factual claim about a specific peer enterprise's
  interface design, a specific tooling vendor's capability,
  or a specific ATLAS / OWASP / SP 800-218A obligation
  carries a `<!-- needs-research: verify [specific fact]
  against [official source] -->` marker where the fact is
  not independently verifiable from the cited primary
  sources. No practice is guessed.

## Stretch goals

- Extend the deliverable with the **rehearsed handoff-
  scenario tabletop**: a specific tabletop exercise walking
  a hypothetical new AI capability through the handoff
  protocol end-to-end, with each named owner playing their
  step, and the artefact identifying the specific timing
  and hand-off failures the protocol is designed against.
- Author the **ATLAS-mapped finding walkthrough** — the
  worked example from chapter 01's "where the discipline
  earns its keep" section, extended to a full narrative:
  the finding is discovered, formatted using the finding
  template, routed to the CISO's platform, triaged, joint-
  scoped for remediation, closed, and reported to the audit
  committee. The walkthrough is a rehearsal artefact for
  the head's function and for the SOC's app-sec lead.
- Draft the **cross-platform variation** — a variant of the
  metadata contract for a federated-platform enterprise
  (each business unit's platform has its own model registry;
  the governance runtime queries across them) versus a
  single-platform enterprise. The variation is a stress
  test on the contract's portability.
- Author the **CAE onboarding brief** — the one- to two-
  page brief the head hands to the CAE at the annual
  interface review, summarising what the interface set is,
  what has changed since last year, and what the CAE should
  read against. The brief composes with the chapter
  [[05-cae-coordination]] discipline.
- Extend the failure-mode audit with a **live-incident dry
  run**: a specific narrative in which one of the seven
  failure modes surfaces during an incident, the interface
  set detects it, and the recovery discipline restores the
  interface. The dry run is a rehearsal artefact for the
  incident-leadership module [[mod-110-incident-leadership]].

## Notes and starter guidance

The most common first-cut failure on this exercise is the
CISO interface document that is written in AI-governance
vocabulary rather than in CISO-operational vocabulary. An
interface document the CISO's SOC lead cannot read on first
pass is an interface document that will not be adopted. The
remedy is to draft the CISO document with a specific SOC
lead in mind — someone with SIEM operational depth, ISO/IEC
27001 fluency, and a functioning triage discipline — and to
translate every AI-governance concept into that reader's
vocabulary. The severity mapping is the most sensitive
translation; get it wrong and every finding routes at
ambiguous severity.

The second common failure is the three contracts written as
prose rather than as specifications. A metadata contract
that says "the model registry should expose sufficient
metadata to support governance queries" is not a contract; a
metadata contract that names field `model_identifier` (type:
string, stable across lifecycle), `semantic_version` (type:
semver), `training_data_version` (type: reference to data
catalogue), and so on, is. Force the specification depth even
where the field set is enterprise-adapted.

The third common failure is the handoff protocol written as
a checklist people work around. A checklist is a document; a
gate is a machine-enforced pipeline step with a named owner
and a named handoff-complete criterion. Force the gate
depth. Where the platform does not have the machinery to
enforce the gate yet, name the interim manual step and the
migration plan; do not write the protocol as if the gate
already exists when it does not.

On the CDO joint chapter — the temptation is to let the
CDO's data-governance lead author it entirely because it
lives in the CDO's document. Do not. The AI-specific
substantive content requires the head's level-50 architect
to author; the CDO's function shepherds the composition. A
CDO-authored chapter without substantive AI depth reads as
generic and fails on the first regulatory examination.

The interface set is a living artefact. Version it, date it,
refresh it annually at the joint audit-committee appearance,
and distribute the current version to the CISO, CIO, CTO,
CDO, CAE, CAIO, and audit-committee secretariat. An
interface set that has not been refreshed in a year is an
interface set that no longer describes the coordination; an
interface set that lives on the head's laptop is an interface
set that no one else can act on when the head is
unavailable.
