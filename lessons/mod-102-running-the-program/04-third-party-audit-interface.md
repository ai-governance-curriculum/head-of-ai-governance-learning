# Leading the Third-Party Audit Interface

## Motivation

Any AI governance function running at level-60 scope is inspected by
someone external at least twice a year, often more. The
ISO/IEC 42001 certification body arrives for stage-1, stage-2,
surveillance, and recertification visits under ISO/IEC 42006
accreditation rules. A ForHumanity Independent Audit of AI Systems
(IAAIS) auditor or a BABL AI Algorithm Bias Auditor may arrive under
a specific NYC Local Law 144 or EU AI Act conformity-assessment
mandate. In banking, insurance, health, pharma, or critical
infrastructure a sector regulator's examiner arrives on a
supervisory cycle. The third-line internal audit function arrives on
the CAE's audit plan.

Every one of these visits is a moment where the AI governance
function is either defensible or not. The design is upstream — the
level-50 architect built the AIMS, the control library, the evidence
architecture, the third-party program. The visit's success or failure
depends on the head's operating discipline: how evidence is packaged,
how sampling access is administered, how findings are received,
remediation plans are agreed, and audit-committee reporting on
findings is structured.

The head is the enterprise's *audit interface*. Not the auditor, not
the auditee — the interface. This chapter is that interface's shape.

## Core concept: five distinct external audit relationships

The head must not treat the five external audit relationships as one
undifferentiated "audit" category. Each has a different mandate, a
different independence posture, a different sampling scope, and a
different reporting-line back into the enterprise. Getting one wrong
usually looks like getting all of them wrong.

- **ISO/IEC 42001 certification body.** Conformity assessment of the
  AIMS against ISO/IEC 42001. Accredited under ISO/IEC 42006 by a
  national accreditation body (UKAS in the UK, ANAB in the US,
  DAkkS in Germany, and equivalents; the international coordinating
  body is the IAF). Scope: the enterprise's own AIMS as documented.
  Output: certification decision (grant, maintain, suspend,
  withdraw) and non-conformities. Reporting-line: to the head, then
  to the audit committee.
- **ForHumanity IAAIS auditor.** ForHumanity's Independent Audit of
  AI Systems programme certifies auditors to conduct specific
  criteria-based audits against ForHumanity criteria (GDPR-AI, EU
  AI Act, NYC LL144, Colorado SB21-169, and others). Scope: as
  contracted, typically per-system or per-obligation. Output: audit
  report against the specific criteria set. Reporting-line: to the
  head or to the first-line owner, per contract.
- **BABL AI Algorithm Bias Auditor.** BABL AI trains and certifies
  algorithm auditors under its own certification. Scope: as
  contracted; frequently NYC LL144 bias audits and similar. Output:
  audit report with statistical bias metrics per the audit
  criteria. Reporting-line: as contracted; often published in
  summary form under LL144's public-disclosure requirement.
- **Sector regulator examiner.** Federal Reserve, OCC, FDIC, NCUA,
  or state banking supervisor for banks; state insurance regulators
  under the NAIC AI Model Bulletin; FDA for medical devices under
  GMLP; FCA / PRA in the UK for financial services; OSFI in Canada;
  BaFin in Germany; MAS in Singapore; and equivalents. Scope:
  regulatory examination scope, typically prescribed by the
  examiner. Output: examination findings and matters-requiring-
  attention. Reporting-line: through the enterprise's regulatory
  affairs / compliance function to the head and the board.
- **Third-line internal audit.** The enterprise's own internal
  audit function under the CAE, per the IIA International
  Professional Practices Framework. Scope: audit plan approved by
  the audit committee. Output: audit reports with findings and
  management-response plans. Reporting-line: functionally to the
  audit committee, administratively often to the CEO or CFO.

The head owns the interface to all five. The head is *audited by* the
first four (as the accountable executive for the AIMS and the AI
control library) and *coordinated with* the fifth (third-line
independence prohibits the head from directing internal audit but
requires coordination on scope and access).

## Preparing the evidence bundle — the OSCAL / evidence-architecture story

The level-50 architect delivered the evidence architecture (see
[[mod-101-role-scope-and-leadership-shape]] chapter 01) — the
machine-readable evidence store keyed to control IDs, using OSCAL for
controls and assessments, CycloneDX ML-BOM and SPDX 3.0 AI for
supply-chain, model / system / dataset cards for AI-specific
artefacts, and SLSA attestations for build-pipeline integrity.

The head's job at audit time is to package a subset of that
evidence into an audit-ready bundle for the specific auditor's
scope. Concretely, that means:

- **Statement of applicability.** The AIMS statement of applicability
  (which Annex A controls are in scope, which are excluded and why)
  under document control, at the revision the auditor is examining.
- **Control-mapping table.** For each control the auditor will
  sample, the internal control ID, its ownership, its evidence
  pointers, and its date of last effective-operation confirmation.
- **Evidence packages per sampled control.** OSCAL assessment plans
  and results where the enterprise has adopted OSCAL; equivalent
  structured evidence otherwise. Not a folder of screenshots.
- **Management-review minutes and internal-audit reports.** The
  latest cycle, ISO/IEC 42001 clause 9.2 and 9.3 outputs (chapter
  02), with follow-through evidence for any prior findings.
- **Risk register extract.** The relevant portfolio-scope risk
  register extract (chapter 03), at the granularity the auditor
  asks for.
- **AI system inventory extract.** The AI system inventory
  extract (chapter 06) scoped to the auditor's population of
  interest.
- **Incident and non-conformity register.** The relevant window,
  with corrective actions and effectiveness reviews.
- **Third-party evidence.** For any sampled AI vendor: the
  tiering assessment, the vendor's model/system/dataset cards,
  ML-BOM, SLSA attestation, and continuous-monitoring evidence
  (chapter 07).

The bundle is assembled to a documented convention. The head does
not personally assemble it every visit; a named audit-liaison role
(often housed in the GRC operating team) executes to the convention
under the head's oversight. When the level-50 architect updates the
evidence architecture, the audit-bundle convention updates in step.

## Administering sampling access

Auditors sample. They sample AI systems, model cards, evidence
records, personnel to interview, third-party vendors, incidents. The
head administers sampling access as an operating discipline with
three properties:

- **Un-tampered access.** Auditors receive access to the sampling
  population — the actual, current AI-system inventory; the actual,
  current risk register; the actual, current incident log — not a
  curated subset. Curation is exactly the failure mode the sampling
  is designed to detect. The head enforces this even when it
  surfaces uncomfortable content; that is what independence means.
- **Documented access channels.** Access to systems and evidence is
  provisioned through a documented channel (typically a
  read-only auditor account with logged actions, or an escorted
  live-view session, per the CISO's policy). Ad-hoc sharing is
  prohibited; every access is logged and retained.
- **Interview scheduling and observer discipline.** Where the
  auditor conducts interviews, scheduling is coordinated through the
  head's audit-liaison; a note-taker attends every interview to
  capture what was said and shared. The head does not attend
  interviews of first-line staff (that would compromise the
  independence of the interview) but reviews notes for accuracy
  after the fact.

Under ISO/IEC 42006 a certification body will observe the sampling-
access discipline and treat curation, obstruction, or
undocumented-access as itself a non-conformity finding.

## Receiving findings — the discipline before defence

When an auditor issues findings, the head has one job before any
defence: read them accurately. Two habits.

First, **do not defend in the exit meeting**. Exit meetings surface
draft findings for factual clarification, not for negotiation of
substance. The head asks questions of clarification, corrects factual
misunderstandings on the record, and receives the finding. Substantive
disagreement is registered in writing after the exit meeting
through the auditor's stated appeal or dispute process.

Second, **triage findings by class before response**. A finding may
be:

- **Non-conformity (major).** A significant failure to meet a
  requirement — for ISO/IEC 42001 audits, an absence of a required
  process, or a systemic failure to implement, or a breakdown that
  causes AIMS objectives to be unachievable. Requires a corrective-
  action plan and typically a re-audit before a certification
  decision can be made.
- **Non-conformity (minor).** A single lapse in an otherwise
  operating process. Requires a corrective-action plan; closure
  verified at the next surveillance visit.
- **Observation or opportunity for improvement.** Not a
  non-conformity; a documented signal the enterprise may act on.
- **Matter requiring attention or supervisory finding.** In sector-
  regulator language, a finding requiring management response and
  remediation.
- **Third-line internal audit finding.** Categorised per the
  enterprise's own internal-audit rating scheme (high / medium /
  low, or equivalent) with management responses tracked.

The head does not conflate classes. A major non-conformity is not
"opportunities for improvement in bulk"; a supervisory finding is
not "a certification-body observation." Each class has its own
regulatory or contractual weight and its own reporting-line back to
the audit committee.

## Authoring remediation plans

A defensible remediation plan against an external audit finding
contains:

- **Finding reference.** The exact language of the finding and its
  auditor-assigned ID.
- **Root cause.** Analysed to a depth the auditor accepts; typically
  more than one why-layer deep.
- **Corrective action.** The specific change to policy, procedure,
  control, system, or resource that addresses the root cause.
- **Containment action.** Any interim action taken while the
  corrective action is in flight — a heightened monitoring, a
  temporary policy tightening, a suspension of a specific practice.
- **Owner.** The accountable executive for the corrective action
  (often first-line; sometimes the head or the level-50 architect
  for AIMS-design findings).
- **Target date.** The date the corrective action will be complete.
- **Effectiveness review.** How and when the enterprise will
  confirm the corrective action worked, and what evidence will
  demonstrate that.
- **Council and audit-committee visibility.** How the plan is
  minuted into the AI governance council (chapter 01) and, for
  material findings, reported to the audit committee.

Under ISO/IEC 42001 clause 10.2, corrective-action effectiveness
review is a non-optional part of the plan. Under a sector examiner's
findings, the enterprise's response letter typically commits to the
plan; the letter is a document the head co-authors with the
regulatory-affairs function and the GC. See
[[mod-104-regulator-engagement]] for the correspondence-authoring
discipline.

## Reporting audit findings to the audit committee

The audit committee sees external and third-line audit findings on a
disciplined cadence. The head's reporting shape — used across all
five audit relationships — has consistent structure:

- **Summary.** A single paragraph identifying the auditor, scope,
  window, and overall conclusion.
- **Findings by class.** A table of findings by class (major,
  minor, observation, matter-requiring-attention, etc.), with
  ownership and target dates.
- **Trend.** Comparison to prior audits — improving, worsening,
  stable — with pattern commentary.
- **Systemic themes.** Findings that individually are minor but
  collectively signal a design gap the level-50 architect should be
  asked to address.
- **Management response.** For each material finding, the
  management response as agreed, with ownership.
- **Remediation status.** Ageing of open remediations from prior
  audits, with escalation for any material item overdue.
- **Ask of the committee.** What decision, endorsement, or
  intervention the head is asking the audit committee for.

The audit-committee pack does not present findings without a
management response. That would be the head presenting the auditor's
work as if it were the enterprise's; the audit committee's role is
to see how the enterprise is responding, not to hear the auditor's
finding raw. See [[mod-103-board-and-audit-committee-reporting]]
for the pack-authoring discipline in depth.

## Composing the four external audits — the sampling-overlap problem

The four external audits sample overlapping populations. The
certification body samples across the AIMS; the ForHumanity or BABL
auditor samples specific systems or specific obligations; the sector
examiner samples systems within its remit; the third-line auditor
samples per the audit-committee-approved plan. If the head does not
coordinate, the same AI system may be sampled four times in six
months, each time surfacing overlapping evidence in slightly
different formats to slightly different auditors.

The composition discipline:

- **Coordinate on scope in advance.** The head maintains a
  twelve-month calendar of external and third-line audit windows
  and shares a portfolio-level view with each auditor's engagement
  lead so they can weight their samples toward under-covered
  populations.
- **Publish evidence in a canonical format.** OSCAL assessment
  results, ML-BOM, SLSA attestation, model/system/dataset cards.
  The head produces evidence once; each auditor consumes it in the
  canonical format and takes their own inferences.
- **Coordinate remediation plans.** Where the same underlying gap
  produces findings from two auditors, the enterprise runs a single
  remediation with dual-tracked reporting, not two competing
  remediations.
- **Track sampling coverage.** The head monitors which AI systems
  have been sampled by whom and when, so that a systemic
  under-coverage is visible and can be addressed by proactively
  offering samples to the next audit.

Under-coordination is expensive — in staff time, in inconsistency of
evidence, in remediation confusion. Over-coordination violates
audit independence. The line lies at coordination-of-scope and
evidence-canonicalisation, not at coordination-of-findings.

## Preserving third-line independence

The third-line internal audit function is the one external
relationship where coordination-versus-independence is most
delicate. Under the IIA Three Lines Model the third line's
independence is what makes its findings valuable. The head must not:

- Direct the CAE on scope.
- Suggest or discourage specific findings.
- Approve or edit third-line audit reports before they land at the
  audit committee.
- Attend interviews of first-line staff as an observer.

The head *may* and *should*:

- Formally request that a topic be considered for inclusion in the
  third-line audit plan (chapter 01 on sideways escalations).
- Provide un-tampered access to AIMS documentation, control-
  evidence, and the AI system inventory.
- Respond to draft findings with factual clarifications through the
  documented dispute process.
- Present a management response to findings at the audit committee.

That distinction — between coordinating on access and directing on
substance — is a load-bearing invariant of the head's role. Violating
it is a governance failure the audit committee will detect, and it
compromises the head's own independence as a second-line executive.

## Example — a certification-body surveillance visit, end to end

A working example of the head's operating discipline over a
certification-body surveillance visit.

Six weeks out, the certification body confirms the surveillance
scope. The head's audit-liaison assembles the evidence bundle to
the documented convention; the head reviews for completeness two
weeks out. Any known non-conformity from the prior visit that is
not yet closed is separately flagged and the closure evidence is
prepared for re-verification.

The visit runs three days. Day 1 opens with the auditor's opening
meeting; the head chairs the enterprise side, confirming scope,
sampling method, and interview schedule. The audit-liaison
administers sampling access and coordinates interviews. The head
does not attend first-line interviews.

Day 3 closes with the auditor's exit meeting. Draft findings are
presented: one minor non-conformity relating to competence-
assessment ageing (chapter 02); two observations relating to
third-party evidence completeness (chapter 07); no major
non-conformities; certification maintained pending closure of the
minor.

The head takes the exit findings without defence, asks clarifying
questions, and thanks the auditor. Within one business day, the
audit-liaison circulates draft minutes of the exit meeting. Within
one week, the head convenes an internal working session to draft
the corrective-action plan for the minor non-conformity and to
document accepted actions on the observations.

The plan is presented at the next AI governance council meeting
under the standing agenda item for external audit findings (chapter
01). The council ratifies the plan and owners. The plan is added to
the non-conformity register with target dates.

The audit committee is briefed at its next quarterly meeting under
chapter 01's fixed reporting shape. The head presents the finding,
the plan, the ageing table for open remediations from prior visits,
the trend commentary, and the ask of the committee (in this case:
endorsement of the plan and a specific check-in six weeks before the
next surveillance visit).

Every artefact is retained in AIMS document control. When the next
surveillance visit arrives twelve months later, the closure
evidence is ready for re-verification.

## Common failure modes

- **Curating the sample.** Providing the auditor with a subset the
  enterprise thinks is representative rather than the actual
  population. Failure to detect this is one of the certifier's own
  competences; when detected, it produces a major non-conformity of
  its own and can suspend certification.
- **Defending in the exit meeting.** Turning the auditor's draft
  findings into a debate. This burns credibility, does not change
  the findings, and reads as poor governance to any observer.
- **Conflating classes.** Treating an observation as if it were a
  non-conformity (over-response) or a non-conformity as if it were
  an observation (under-response). Both are governance failures.
- **Losing the calendar.** Failing to coordinate the four external
  audits and the third line's schedule until visits collide. This
  usually produces last-minute evidence hunts, staff time
  overruns, and inconsistent evidence — all of which propagate as
  new findings.
- **Weak remediation loop-close.** Remediation plans agreed but
  effectiveness never verified. This is the failure the next
  surveillance visit will find and re-open.

## Summary

- The head runs the interface to five distinct external audit
  relationships — ISO/IEC 42001 certification body under
  ISO/IEC 42006, ForHumanity IAAIS auditor, BABL AI Algorithm Bias
  Auditor, sector regulator examiner, third-line internal audit —
  and treats each on its own mandate and independence posture.
- Evidence bundles are assembled to a documented convention from
  the architect's evidence architecture, in canonical formats
  (OSCAL, ML-BOM, SLSA, model / system / dataset cards).
- Sampling access is un-tampered, documented, and channel-
  administered; curation is itself a non-conformity.
- Findings are received without defence in the exit meeting,
  triaged by class, and answered by defensible remediation plans
  with root-cause analysis and effectiveness reviews.
- Audit-committee reporting has a fixed shape: summary, findings by
  class, trend, systemic themes, management response, remediation
  ageing, and ask of the committee.
- The four external audits' sampling is coordinated by the head on
  scope and canonical evidence; findings and substance are not
  coordinated (that would compromise independence).
- Third-line independence is preserved by strict rules — no
  direction of scope, no attendance at first-line interviews, no
  edit of drafts — while access and evidence-provision are open
  and disciplined.
