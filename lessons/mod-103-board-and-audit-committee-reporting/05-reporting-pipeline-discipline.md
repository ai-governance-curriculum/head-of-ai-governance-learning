# The Reporting Pipeline Discipline

## Motivation

A board pack that is a scramble every quarter is a program that is
one adverse-quarter away from missing a distribution date, which is
one distribution miss away from an audit finding, which is one audit
finding away from the head being replaced. The reporting-pipeline
discipline exists so that assembling the pack is a *predictable
operational cadence*, not a heroic effort.

Chapter 04 covered *who signs off on what*. This chapter covers
*what evidence is collected from whom, by when, in what form,
against what quality bar*, so that when the sign-off flow starts
the inputs are already there.

The discipline is boring, and it is precisely because it is boring
that a reader can tell whether the head is running a program or
running a story. A pack whose evidence pipeline is documented and
in force is a pack an ISO/IEC 42006 auditor can trace back to
source in fifteen minutes. A pack whose evidence pipeline is not
documented is a pack the head cannot defend.

## Core concept: the pipeline is a scheduled cadence with named owners

Every input to the pack has three attributes: a *producer* (the
first-line owner, second-line function, or external party who
generates the evidence), a *cadence* (how frequently the evidence
is produced), and a *retention path* (where the evidence lives so
it is retrievable by cross-reference from the pack).

The pipeline is the document that lists every input, its producer,
its cadence, and its retention path. It is authored once, ratified
by the CxO peer group, and referenced by every pack cycle. It
lives under AIMS document control.

## The evidence categories

The pack's clusters (chapters 01-03) draw on a limited set of
evidence categories. Naming them explicitly is how the pipeline is
structured.

### AI-system inventory evidence

The current point-in-time inventory of AI systems in scope, with:

- System identifier, owner, capability tier, deployment posture,
  and jurisdiction footprint.
- Risk-taxonomy classification.
- Impact-assessment status and last-refresh date.
- Model card / system card / dataset card citations.
- Third-party dependency footprint.

Producer: the AI system inventory function (typically inside the
head's own team, or the level-50 architect's function where scope
overlaps — see [[mod-102-running-the-program]] chapter 06).

Cadence: continuous (inventory is a living register) with a
month-end snapshot for reporting.

Retention: the inventory system of record, with the month-end
snapshot filed as an immutable extract.

### Portfolio risk-register evidence

The AI risk register at portfolio scope, with:

- Risk items open in period, opened in period, closed in period.
- Movement in risk position (likelihood, impact, residual position
  after treatment).
- Appetite-tracker state per appetite statement.
- Escalation events in period.

Producer: the head's risk-register function.

Cadence: council-cycle cadence (typically monthly, matching the
governance-council cycle in [[mod-102-running-the-program]] chapter
01) with a period-end snapshot for reporting.

Retention: the risk-register system of record, with the period-end
snapshot filed under document control.

### KRI telemetry

Numeric values for each KRI on the dashboard, with:

- Current-period value.
- Prior-three-period trend.
- Source system reference and query used to produce the value.
- Data-quality confidence and any known gaps.

Producer: mixed. Some KRIs come from the head's own function
(exceptions live and aged; audit-round posture). Some come from
first-line telemetry (control operation coverage; evaluation cadence
against expectation; model-monitoring drift). Some come from the
CISO (security-signal KRIs). Some come from the CAE (finding-ageing
KRIs). Each KRI's producer is named in the pipeline document.

Cadence: monthly at minimum for period-comparison, weekly or daily
for KRIs feeding operational monitoring. Board pack takes
period-end values.

Retention: the KRI values are produced from live systems; the
pack-cycle snapshot is filed under document control with query
and timestamp.

### Incident and near-miss log

Every incident meeting the pre-agreed logging threshold, with:

- Incident identifier, dates, systems, category, factual summary.
- Reportability determination and the rationale.
- Containment, remediation, and closure status.
- Post-incident review reference where completed.

Producer: the incident-management function (see
[[mod-110-incident-leadership]] for the operating discipline).

Cadence: continuous with a period-end summary for reporting.

Retention: the incident-management system of record with immutable
audit trail.

### Third-party vendor evidence

Vendor posture summarised for reporting, with:

- Vendor identifier, tier, dependency footprint (systems depending
  on this vendor), attestation status (SOC 2 Type 2, ISO 27001,
  ISO/IEC 42001, sector attestations).
- Contractual status (in force, in renegotiation, in remediation,
  in termination).
- Concentration position.
- Change events in period.

Producer: the third-party risk function (jointly held by procurement,
the head's own function, and the CISO for security posture — the
pipeline document names the primary producer per field).

Cadence: continuous with a period-end snapshot for reporting.

Retention: the third-party-risk system of record with pack-cycle
snapshot filed under document control.

### Regulator engagement log

Every active regulator engagement, with:

- Regulator, jurisdiction, instrument at play.
- Nature of engagement, enterprise counterpart, status.
- Correspondence in period.
- Board-decision-needed flag.

Producer: General Counsel (or Chief Compliance Officer per
reporting-line — see [[mod-101-role-scope-and-leadership-shape]]
chapter 06) with the head's coordination on AI-specific content.

Cadence: continuous with a period-end summary for reporting.

Retention: the legal or compliance system of record with a
pack-cycle summary filed under document control; privileged
material is retained separately and referenced but not quoted in
the pack.

### Regulatory-change monitoring log

New and pending obligations in period, with:

- Regulator or law-making body, instrument.
- Coming-into-force date.
- Assessed enterprise exposure.
- Current program response.

Producer: the regulatory-change function (see
[[mod-105-regulatory-change-management]] for the operating
discipline).

Cadence: continuous with a period-end summary for reporting.

Retention: the regulatory-change system of record with a pack-cycle
extract filed under document control.

### Audit-plan and third-line findings

The CAE's plan and the findings-ageing view, with:

- Audits completed in period against the plan.
- Findings by severity and by AI-relevant category.
- Management response and remediation status.
- Ageing view against target dates.

Producer: the Chief Audit Executive. The head does not produce this
evidence; the CAE presents it directly (chapter 02).

Cadence: quarterly aligned with the audit-committee cadence.

Retention: the internal-audit system of record.

### External audit and certification-body findings

Findings from ISO/IEC 42001 certification-body audits, financial-
statement external audit AI-adjacent findings, sector regulator
examinations, voluntary attestation-provider results, and material
customer-contractual assurance requests.

Producer: mixed — the head coordinates capture across the assurance
function.

Cadence: driven by the external body's cadence; the head captures
each event as it lands.

Retention: the assurance-function system of record with a
pack-cycle extract filed under document control.

### Maturity-assessment posture

Point-in-time position against the reference maturity plots
(NIST AI RMF Playbook, ISO/IEC 42001 AIMS maturity, OWASP AI
Security & Governance Checklist coverage — see
[[mod-107-program-measurement-and-maturity]]).

Producer: the head's function.

Cadence: annual full assessment with quarterly delta commentary.

Retention: the AIMS document control system.

## The pipeline document

A defensible pipeline document is a table with one row per
evidence category and columns for:

- Evidence category and description.
- Producer (named function or role, not a named individual — roles
  outlast individuals).
- Cadence.
- Retention path (specific system of record and the archival path
  for pack-cycle snapshots).
- Quality bar (what "complete" means for this evidence category —
  a schema, a checklist, or a minimum-fields specification).
- Downstream cluster reference (which cluster of which pack the
  evidence feeds).

The pipeline document is a first-class AIMS artefact. It is
ratified by the CxO peer group (chapter 04's owners), updated when
the pack shape changes, and inspected by the certification body
under ISO/IEC 42006 sampling.

## The reporting-cycle timeline

Working backward from committee distribution (T-0):

- **T-15 business days — evidence-cycle open**. The pipeline
  producers are notified that the cycle has opened. Producers with
  monthly or continuous cadence continue as normal; producers with
  cycle-specific work (period-end snapshots, quarterly summaries)
  schedule the work.
- **T-10 — first-line evidence due**. Control-operation coverage,
  incident-log summary, third-party-status snapshot, KRI values
  from operating systems.
- **T-8 — second-line evidence assembled**. Risk-register
  snapshot, appetite-tracker state, exception posture, regulatory-
  change summary, maturity-assessment delta.
- **T-7 — evidence lock**. Chapter 04 sign-off flow begins. After
  T-7 no new evidence enters the cycle; late-breaking material is
  captured as an addendum with explicit provenance.
- **T-7 to T-0** — the sign-off flow (chapter 04) runs.
- **T-0 — distribution**.
- **T+meeting — post-meeting**. Decisions taken are recorded in
  the decision log, action items assigned, escalations dispatched.
  The next cycle opens.

The exact numbers vary. The invariant is that every input has a
*known deadline* well before the pack has to be written, so pack
assembly is composition of assembled evidence, not evidence
gathering under time pressure.

## The addendum discipline

Between evidence lock (T-7) and distribution (T-0), the world does
not pause. A material incident may occur; a regulator may issue an
enforcement action; a stop-shipping trigger may fire. The pipeline
handles these through *addenda*, not by editing the locked pack:

- The addendum is a dated, named document (`ADD-YYYY-Q#-NN`) that
  accompanies the pack.
- It cites the event, the date and time of detection, the
  provenance, and the current status.
- It states specifically what the head recommends the committee
  do about the event (defer to a subsequent meeting, take
  immediate decision, note without action).
- It is signed off by the relevant CxO content owner on the same
  discipline as the pack itself.

Addenda are visible. They are not corrections to the pack; they are
supplementary. This preserves comparability across pack archives
(chapter 01's cross-quarter comparability discipline).

## What the pipeline discipline buys

Three things:

- **Predictability**. The cycle runs the same way every time. The
  head's team, the first-line producers, and the CxO peer group
  know what is due when. Missed inputs are visible before they
  become missed distributions.
- **Defensibility**. Every value in the pack traces to a source in
  a system of record with a query, a producer, and a timestamp. A
  certification-body auditor asking "where did this KRI value come
  from?" gets an answer in fifteen minutes.
- **Improvability**. The pipeline is a document that can be
  measured, audited, and improved. Cycles that miss inputs generate
  a corrective action; producers that consistently miss deadlines
  are addressed as a competence or capacity issue. The pipeline is
  a program-management instrument in its own right.

## Summary

- The reporting pipeline names every evidence input the pack
  consumes, its producer (as a role, not an individual), its
  cadence, its retention path, and its quality bar.
- The pipeline document is an AIMS artefact ratified by the CxO
  peer group and inspectable by a certification body under
  ISO/IEC 42006 sampling.
- The reporting cycle runs backward from committee distribution,
  with evidence-lock at T-7 preceding chapter 04's sign-off flow;
  late-breaking material is handled through named addenda rather
  than pack edits.
- The pipeline buys predictability, defensibility, and
  improvability; it turns pack production from a heroic effort
  into a scheduled operational cadence.
