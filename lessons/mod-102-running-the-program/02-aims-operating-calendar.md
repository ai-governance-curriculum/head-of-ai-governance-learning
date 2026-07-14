# The ISO/IEC 42001 AIMS Operating Calendar

## Motivation

An AI Management System (AIMS) that has been *designed* — with a
statement of applicability, a scope boundary, a policy taxonomy, and a
control library — is not the same as one that is *operating*. An AIMS
operates when its cadence artefacts (internal audit rounds,
management-review meetings, risk-treatment plan refreshes, competence
assessments, corrective-action follow-through, non-conformity closure)
are actually happening on the calendar, on time, with named owners and
retained evidence.

The head of AI governance owns the operating calendar. The level-50
architect designed the AIMS scope and statement of applicability under
[[mod-101-role-scope-and-leadership-shape]]; the head runs it. When an
ISO/IEC 42001 certification body — accredited under ISO/IEC 42006 —
arrives for a stage-1, stage-2, surveillance, or recertification visit,
what they inspect is the calendar. Missed audit rounds, stale
management-review minutes, unclosed non-conformities beyond their
target dates, competence assessments that never happened — those are
non-conformities against ISO/IEC 42001 itself, not against the
enterprise's own policies. That is the level-60 accountability.

This chapter is the operating calendar the head runs.

## Core concept: management-system clauses map to calendar events

ISO/IEC 42001:2023 follows the ISO Harmonised Structure (formerly
Annex SL) common to ISO 9001, ISO/IEC 27001, ISO 22301, ISO 14001,
and the rest of the management-system family. Its ten clauses — with
the operative clauses running from 4 through 10 — each impose
recurring obligations that the head must schedule as calendar events
with owners and evidence retention.

The mapping the head must be able to defend on any Tuesday morning:

- **Clause 4 (Context of the organization).** Scope-of-AIMS review as
  a scheduled event, not a one-off; interested-party and issue register
  refreshed at least annually and on trigger.
- **Clause 5 (Leadership).** Top-management commitment demonstrated
  through the governance-council cadence (chapter 01), the AI policy
  approval-and-review cycle, and evidence of resource allocation.
- **Clause 6 (Planning).** AI risk assessment and AI system impact
  assessment cadence (per ISO/IEC 23894 and ISO/IEC 42005); the
  AIMS-objectives-and-planning refresh; the risk-treatment plan
  refresh.
- **Clause 7 (Support).** Competence, awareness, and communication —
  competence assessments, training completion tracking, awareness
  campaigns, and the documented-information / document-control
  discipline.
- **Clause 8 (Operation).** Operational planning and control — the
  running of MAP / MEASURE / MANAGE per NIST AI RMF vocabulary, or the
  ISO 8-level operational controls, at per-system cadence.
- **Clause 9 (Performance evaluation).** Monitoring, measurement,
  analysis, evaluation, internal audit, and management review.
- **Clause 10 (Improvement).** Non-conformity, corrective action, and
  continual improvement.

Each of those seven clauses converts into one or more recurring
calendar events. The head's operating calendar is the union.

## The annual AIMS calendar — the ten anchors

A defensible operating calendar has ten anchor events across the
year. Their exact scheduling is enterprise-specific (regulatory
year-end, financial year-end, and the parent ISMS calendar under
ISO/IEC 27001 all constrain placement). The invariant is that each
anchor exists, has an owner, has a pre-read discipline, and produces a
minuted output.

1. **Annual AIMS-scope review** — clause 4. Confirms the AIMS scope
   boundary, interested-parties list, and internal-issues register are
   current. Owned by the head; ratified by the AI governance council;
   feeds into the following year's plan. Typically at start of the
   AIMS operating year.
2. **AIMS objectives and risk-treatment plan refresh** — clause 6.
   Updates the AIMS objectives, the AI risk assessment at
   enterprise-portfolio scope (chapter 03), and the risk-treatment
   plan. Consumes the risk taxonomy the level-50 architect owns and
   produces the year's treatment commitments. Typically Q1.
3. **Competence and awareness assessment round** — clause 7.
   Assesses whether people whose work affects AI-system conformity —
   analysts, engineers, evaluation engineers, agentic-safety
   engineers, first-line AI product owners, third-party procurement
   staff, GRC operators — have the competence documented and
   evidenced. Deficiencies feed the training plan. Typically Q1–Q2.
4. **Internal audit round(s)** — clause 9.2. A planned programme of
   internal audits covering the AIMS. Typically two rounds a year for a
   maturing AIMS, potentially aligned with the ISMS audit programme.
   Owner is a designated internal audit function (first-line risk
   assurance, second-line self-assessment, or third-line internal
   audit depending on the enterprise). See chapter 04 on the
   third-line interface.
5. **Mid-year risk-treatment plan review** — clause 6 / 10.
   Half-way through the treatment plan year, the head reviews progress
   against the risk-treatment commitments made at anchor 2, escalates
   at-risk treatments to the council, and updates the plan. Typically
   Q3.
6. **Non-conformity and corrective-action ageing review** — clause
   10.1 / 10.2. A standing review — happens every council meeting
   (chapter 01) — but with a dedicated deeper cadence (quarterly is
   typical) to look at ageing profiles, root-cause patterns, and
   corrective-action effectiveness.
7. **Supplier / third-party AI evidence refresh** — clause 8 and
   clause 6. The tiered third-party AI supplier programme (chapter 07
   for the supply-chain evidence discipline) is refreshed on a
   defined cadence per tier — tier-1 continuous / quarterly, tier-2
   semi-annual, tier-3 annual is a common shape. See
   [[mod-101-role-scope-and-leadership-shape]] chapter 06 on the CxO
   adjacency and chapter 07 of this module.
8. **Management review** — clause 9.3. Top management reviews the
   AIMS at planned intervals. ISO/IEC 42001 does not specify a
   frequency; annual is minimum, semi-annual is defensible for a
   maturing AIMS in a regulated sector. See the next section for the
   minimum inputs and outputs.
9. **Certification-body engagement window** — the head's calendar
   of stage-1, stage-2, surveillance, or recertification visits from
   the ISO/IEC 42001 certification body, plus preparation and
   post-visit remediation windows. See chapter 04.
10. **Year-end continual-improvement close-out** — clause 10.3.
    Consolidates the year's non-conformity data, corrective-action
    effectiveness, internal- and external-audit findings, management-
    review outputs, and produces the continual-improvement input to
    the next year's planning cycle.

Each anchor gets a document-controlled agenda template, a named
owner, a named accountable executive (the head, in most cases), a
pre-read discipline (chapter 01), and evidence retention rules aligned
to the AIMS document-control policy.

## Management review — clause 9.3 in detail

Management review under clause 9.3 is the single most audit-visible
anchor of the operating calendar. A certification-body assessor will
sample the previous management-review minutes to check that the
required inputs were considered and the required outputs were
produced. The head's job is to make that sample succeed.

Minimum inputs the management review must consider (adapted from ISO
Harmonised Structure clause 9.3):

- Status of actions from previous management reviews.
- Changes in external and internal issues relevant to the AIMS.
- Feedback from interested parties.
- Performance information — the AIMS-objectives dashboard, results
  of monitoring and measurement, internal and external audit results,
  non-conformity and corrective-action status, effectiveness of
  actions taken to address risks and opportunities, third-party
  performance, and — under ISO/IEC 42001's AI-specific extensions —
  AI-impact and AI-risk information.
- Adequacy of resources.
- Opportunities for continual improvement.

Minimum outputs the management review must produce:

- Decisions related to continual-improvement opportunities.
- Any need for changes to the AIMS (scope, policy, objectives, control
  library, resource allocation).
- Actions with owners and dates.

The head chairs (or co-chairs with the executive sponsor — typically
the CAIO or CRO depending on reporting-line configuration; see
[[mod-101-role-scope-and-leadership-shape]] chapter 07). The minute
follows the discipline in chapter 01. Every input and output is
traceable to a control-evidence attachment in the AIMS document
control.

## Internal audit rounds — clause 9.2

Clause 9.2 requires the enterprise to conduct internal audits at
planned intervals to determine whether the AIMS conforms to its own
requirements and to ISO/IEC 42001, and whether it is effectively
implemented and maintained. This is *self-assessment* — distinct from
the third-line internal audit under the IIA Three Lines Model and
distinct from external certification-body audits.

A defensible internal audit programme has:

- An **audit plan** — coverage over a defined cycle (three years is
  common) that ensures every AIMS clause and every applicable control
  is audited at least once in the cycle, weighted by risk.
- A **round schedule** — the specific rounds within the year, with
  scope, criteria, audit team, and dates.
- **Auditor independence** — auditors are not auditing their own
  work. In a small function this constrains scope more than the head
  usually expects; internal audit of the head's own second-line
  activity requires an independent auditor (often supplied by the
  third-line CAE under a co-source arrangement).
- **Audit reports** — findings recorded per an evidence template,
  categorised (non-conformity major / non-conformity minor /
  observation), with agreed corrective-action plans and target dates.
- **Follow-through** — every finding tracked to closure in the
  non-conformity and corrective-action register. Ageing is reported
  at the council monthly.

The head owns the plan and the follow-through. The head does not
personally perform the audits (that would violate auditor
independence) but does ensure the audit function is resourced and
its findings are acted on.

## Non-conformity and corrective action — clause 10.1 and 10.2

A non-conformity is any failure to meet a requirement — a requirement
of ISO/IEC 42001, of the enterprise's own AIMS policies, or of a
legal / regulatory obligation the AIMS is designed to address. When
one is identified (internal audit, external audit, incident,
regulator inquiry, whistleblower channel, or self-report), clauses
10.1 and 10.2 require the enterprise to:

- React — control it and correct it.
- Evaluate the need for corrective action — analyse root cause,
  evaluate the possibility of similar non-conformities elsewhere.
- Implement any action needed.
- Review effectiveness.
- Update the AIMS if necessary.

The head owns the non-conformity register at operating discipline.
Every non-conformity has: a unique ID, a source, a description, a
severity, an accountable owner, a due date for containment, a due date
for corrective-action plan, a due date for closure, an
effectiveness-review date. Ageing beyond target dates is escalated to
the council and, for material items, to the audit committee. Ageing
patterns — non-conformities of a given type that consistently blow
their target dates — are themselves diagnostic data feeding the
year-end continual-improvement close-out.

## Competence — clause 7.2

Clause 7.2 requires the enterprise to determine the necessary
competence of persons doing work under its control that affects
AIMS performance and AI system performance, and to ensure they are
competent — through education, training, or experience — and to
retain documented information as evidence.

For the head, this converts into a competence matrix: named roles
(the AI governance analyst, the AI risk engineer, the AI evaluation
engineer, the agentic-safety engineer, first-line product owners
for AI systems, third-party procurement, the GRC operators) mapped
to the specific competences required (technical, methodological,
regulatory, sector-specific), and per-person evidence of that
competence.

The competence matrix is a document under document control. The
annual competence assessment (anchor 3 above) samples per person and
identifies deficiencies. Deficiencies feed the training plan and, if
material, become non-conformities in their own right. Under
ISO/IEC 42006 a certification body will inspect the competence
matrix and the sampling evidence.

## How the calendar composes with the ISMS calendar

Most enterprises with an AIMS also have an information-security
management system (ISMS) certified to ISO/IEC 27001. The ISMS has its
own operating calendar with the same clause-4-to-10 anchors. The head
does not run two parallel calendars in isolation; the AIMS calendar
composes with the ISMS calendar under the level-50 architect's AIMS
scope design.

The composition pattern the head must understand:

- **Shared clauses.** Clause 5 (leadership), clause 7 (support), and
  clause 10 (improvement) usually share governance bodies and
  document-control mechanisms with the ISMS. The AIMS should not
  build a parallel document-control apparatus; it should extend the
  ISMS's.
- **Distinct scope.** Clause 4 (context) is where AIMS and ISMS
  scopes are explicitly named. The AIMS scope names AI systems in
  scope, deployment contexts, roles the enterprise plays under
  ISO/IEC 42001 (provider, deployer, distributor, importer,
  affected-party representative), and the interface to the ISMS.
- **Shared audit teams.** The internal audit programme may share
  auditors and audit vehicles with the ISMS; the plan explicitly names
  where a single audit event covers both scopes and where a scope
  is single-management-system.

Getting this composition right is where a certification body will
probe. A head who cannot answer "what is inside AIMS scope that is
not inside ISMS scope, and vice versa" has not internalised the
scope statement the architect delivered.

## Example — a year-in-the-life view

A concrete twelve-month calendar for a mid-size regulated enterprise
running a certified AIMS in its second surveillance year, aligned to
a January AIMS operating year:

- **January.** Anchor 1 (scope review) and anchor 2 (objectives and
  risk-treatment plan refresh) run in the first three weeks. Council
  ratifies the year's plan at the end of January.
- **February.** Competence assessment round (anchor 3) opens.
- **March.** Internal audit round 1 (anchor 4). Scope: AIMS clauses
  4, 5, 6 and a sample of Annex A controls under the risk-treatment
  plan.
- **April.** Non-conformity closures from round 1 track; anchor 3
  competence assessment closes. The AI supplier evidence refresh
  round for tier-1 vendors runs (anchor 7).
- **May–June.** Management review (anchor 8) at end of June, with
  first-half evidence (Q1 objectives progress, audit round 1
  findings, competence assessment outputs, incident and near-miss
  data, third-party performance). Council ratifies the six-month
  scorecard.
- **July.** Certification body surveillance visit (anchor 9).
  Preparation runs through June; the visit is one week; the
  post-visit close-out runs into August.
- **August–September.** Anchor 5 (mid-year risk-treatment plan
  review) runs; any at-risk treatments escalated to the council.
  Non-conformities from the surveillance visit are tracked to closure.
- **October.** Internal audit round 2 (anchor 4). Scope: AIMS
  clauses 7, 8, 9, 10 and the remaining Annex A controls under the
  risk-treatment plan.
- **November.** Anchor 7 tier-2 supplier evidence refresh runs.
  Anchor 6 non-conformity ageing deep-dive.
- **December.** Anchor 10 year-end continual-improvement close-out.
  Draft next-year AIMS plan for the January anchors.

Every anchor's minute and evidence bundle is stamped and retained
per the AIMS document-control policy. Anywhere a certification body
looks in that year, the record is defensible.

## Common failure modes

Three failure modes the head must watch for and defend against.

- **Calendar-without-evidence.** The calendar shows the anchor
  happened; the evidence bundle is missing. A management review
  meeting that produced no minute is not a management review under
  clause 9.3. The head reviews evidence completeness quarterly.
- **Evidence-without-decisions.** The anchor produced a lot of
  documentation but no dated decisions with owners. This is chapter
  01's ambiguity problem; the AIMS operates on decisions, not on
  memos.
- **Ageing debt.** Non-conformities, corrective actions, and risk
  treatments accumulate past their target dates without escalation.
  This is the earliest warning that the operating discipline is
  slipping. The head runs a monthly ageing dashboard at the council.

Each failure mode is a leading indicator of a certification-body
non-conformity finding at the next visit. Catching them early is the
head's job.

## Summary

- The AIMS calendar converts the seven operative clauses of
  ISO/IEC 42001 into recurring calendar events with named owners
  and retained evidence.
- Ten anchor events per year — scope review, objectives and
  risk-treatment refresh, competence assessment, internal audit
  rounds, mid-year plan review, non-conformity ageing review,
  supplier evidence refresh, management review, certification-body
  engagement window, year-end close-out — form the minimum
  defensible cadence.
- Management review under clause 9.3 is the single most
  audit-visible anchor; the head chairs it under a documented
  input-and-output structure that a certification body will
  sample.
- Internal audit under clause 9.2 requires auditor independence,
  planned coverage across a multi-year cycle, and disciplined
  follow-through on findings.
- Non-conformity and corrective-action under clauses 10.1 / 10.2
  operate through a register with dated commitments and effectiveness
  reviews; ageing patterns are diagnostic data.
- The AIMS calendar composes with the ISMS calendar under the
  level-50 architect's scope design; parallel calendars are a
  scope-design failure, not a calendar failure.
- The three failure modes to defend against are calendar-without-
  evidence, evidence-without-decisions, and ageing debt.
