# CAE Coordination Pattern — Being a Third-Line Subject, Not Its Owner

## Motivation

The Chief Audit Executive is the accountable executive for the
enterprise's third-line internal audit function under the IIA
Three Lines Model (2020), the IIA CAE guidance, and the IIA
International Professional Practices Framework (IPPF, now
Global Internal Audit Standards, effective 2025). The CAE
authors the audit plan, executes audits with independent
tenure, reports functionally to the audit committee, and
maintains independence from first-line management and second-
line functions.

The head of AI governance is a *subject* of third-line audit,
not its owner. This is the invariant the head does not confuse
themselves about. The head does not sit on the CAE's audit
planning committee. The head does not approve audit-plan
inclusion or exclusion of specific engagements. The head does
not review or edit audit reports before they are issued to the
audit committee. The head *coordinates* with the CAE — provides
evidence access, offers subject-matter input on audit scoping
when the CAE requests it, responds to audit findings on the
CAE's schedule, appears jointly at the audit committee's
annual audit-programme review — but the head does not
influence the CAE's independence.

The failure mode is the head who is too close to the CAE and
compromises the CAE's independence, or the head who is too
distant from the CAE and produces a defensive posture that
makes third-line audit engagement painful for both sides. The
coordination pattern in this chapter is the middle path.

The pattern draws on the IIA Global Internal Audit Standards
(effective January 2025), the IIA Three Lines Model (2020), the
IIA CAE Guidance, the IPPF standards on audit independence
(specifically the safeguards against impaired objectivity),
the audit committee's charter typical of listed and regulated
enterprises, and — where sector-specific — the supervisory
guidance on internal audit (e.g., Basel Committee's principles
on internal audit for banks, EBA Guidelines on internal
governance).

## Core concept — the head is audited, the head is not the auditor

The load-bearing move is a single-sentence discipline: the head
is audited by the CAE; the head does not audit themselves; the
head does not audit the CAE; the head does not co-author the
CAE's plan.

Three consequences.

- **The head does not assure the head's own numbers.** The
  KRIs and KPIs in
  [[mod-107-program-measurement-and-maturity]] chapter 01, the
  maturity plot in chapter 03, the ROI pack in chapter 04, the
  cost pack in chapter 05 — the head produces them; the CAE
  (or an external assurance provider engaged by the CAE)
  assures them. The head's own second-line function does not
  self-assure.
- **The head does not co-author the audit plan.** The head can
  propose an area to the CAE as being worth an audit look;
  the CAE decides. The head does not have veto power over the
  CAE's inclusion or exclusion of specific engagements. The
  audit plan is the CAE's, ratified by the audit committee, and
  it is authored independently of the head's preferences.
- **The head does not edit audit reports.** When the CAE
  issues an audit finding, the head responds through the
  management-response mechanism the audit-report format
  provides. The head does not negotiate the finding out of
  the report before issuance. The head can dispute the finding
  in the management response, and the CAE can revise or leave
  the finding as the CAE judges appropriate; the audit
  committee reads both the finding and the response.

## The three coordination surfaces

### Surface 1 — audit-plan coordination (input, not co-authorship)

The CAE builds an audit plan against a risk-based methodology
(typically an annual audit-plan cycle, with continuous risk
assessment). The methodology draws on the enterprise risk
register (chapter [[04-cro-coordination]]), the CAE's own
risk assessment, the audit committee's guidance, prior audit
findings, and — for AI-specific engagements — subject-matter
input from the head's function.

The head's input is *input*, not co-authorship. Practically:

- **The head provides an annual AI-audit-priority note** to the
  CAE ahead of the audit-plan cycle. The note lists the areas
  in the head's function where the head believes third-line
  audit engagement would add material assurance value —
  typically the areas where the second-line function's own
  assurance is weakest (e.g., self-assurance on control-testing
  pass rate is inherently limited), the areas of highest AI
  risk (top-of-portfolio risks per chapter [[04-cro-coordination]]),
  and the areas where recent audit findings have not yet been
  fully closed. The note is a *proposal*, not a plan.
- **The CAE considers the note along with other inputs.** The
  CAE may adopt the head's proposal, adopt part of it, extend
  it, or decline it in favour of other audit priorities. The
  CAE's decision is not appealed by the head to the audit
  committee.
- **The head briefs the CAE on scope questions** when the CAE
  requests briefings. When the CAE is scoping an AI audit, the
  head or the head's team provides subject-matter briefings on
  the audit's technical shape — what an AIA looks like, what
  an AI red-team finding looks like, what MLOps evidence looks
  like, what a foundation-model third-party evidence pack looks
  like. The briefings are educational, not directional; the
  CAE decides the audit's scope.

Cadence: annual note to the CAE ahead of the audit-plan cycle;
ad-hoc briefings on CAE request. Joint owner: the head
personally and the CAE, with the level-50 architect providing
technical briefing content on request.

### Surface 2 — evidence access and audit fieldwork support

The CAE, when auditing the head's function, requires evidence
access — to the AIMS documentation, the risk register, the
KRI/KPI portfolio production pipelines, the AIA and DPIA
inventory, the incident register, the third-party evidence
pack, the exception-and-waiver register, the training-
completion records, and any other artefact that supports the
audit's testing objectives.

The interface specifies:

- **Standing evidence-access rights.** The CAE has standing
  read access to the AIMS evidence store, the KRI/KPI
  dashboards, the incident register, the AIA / DPIA inventory,
  and the exception-and-waiver register. Standing means the
  CAE does not have to request access per engagement; the
  access is provisioned once, maintained by the head's team,
  and revoked only if the CAE role transitions.
- **On-request evidence extraction.** For evidence not held
  in the standing-access surface (e.g., specific working
  papers, level-50 architect's design notes on a control,
  vendor evidence packs), the CAE requests extraction and the
  head's function provides within an agreed SLA (typically
  5 business days for standard extractions, longer for
  extractions requiring technical work).
- **Interview and walkthrough support.** The head's team
  makes members available for interviews and walkthroughs on
  the CAE's schedule, within reason. Interview scheduling is
  managed by the CAE's audit team; the head's team's
  availability is the default posture.
- **Evidence integrity discipline.** The head's team does not
  alter evidence after the CAE has begun testing on it. If
  evidence needs correction (an error in a KRI production
  run, a missing artefact discovered mid-audit), the head's
  team notifies the CAE, produces the correction transparently,
  and the audit record captures the correction and its
  provenance.

Cadence: standing access maintained continuously; extraction
and interview support on the CAE's audit schedule. Joint
owner: the head's level-15 analyst on the evidence-production
side (evidence store hygiene, extraction execution) and the
head's level-50 architect on the technical-content side, with
the head personally accountable for the evidence-access
posture overall.

### Surface 3 — audit-finding response and remediation tracking

When the CAE issues an audit finding against the head's
function, the head responds through the management-response
mechanism the audit report format provides. The response has
disciplines the head follows.

- **Accept, mitigate, or dispute — pick one.** The management
  response either accepts the finding (with a specific
  remediation plan and a specific target closure date),
  mitigates the finding (accepts the underlying observation
  but disputes the severity or the specific corrective the
  CAE recommends, with a substituted remediation), or
  disputes the finding (rejects the observation with a
  substantive counter-argument the audit committee can
  evaluate).
- **Do not equivocate.** The response is one of the three
  above; it is not "we will consider" or "we agree there is
  work to do here" without a specific remediation. Vague
  responses fail the audit committee's review of the
  management-response quality.
- **Remediation is time-bound.** Every accepted finding has a
  target closure date. The head does not accept findings with
  open-ended remediation; open-ended remediation is what the
  CAE reports back to the audit committee as unclosed at
  every subsequent read.
- **Remediation is tracked to closure.** The head's function
  maintains a tracker of accepted findings, remediation
  status, and closure evidence. The CAE re-tests on the
  CAE's cycle, and the head's tracker matches the CAE's
  tracker. Disagreement between the two trackers is a
  discipline break the head fixes.
- **Disputed findings escalate to the audit committee.** When
  the head disputes a finding, the audit committee is the
  arbitrator. The head presents the dispute in the head's
  own words at the audit-committee meeting where the audit
  report is discussed; the CAE presents the audit team's
  view; the audit committee decides. The head does not
  campaign the audit committee off-line to reject the
  finding — that behaviour compromises the CAE's
  independence and the audit committee will notice.

Cadence: management response inside the audit report's
required window (typically 30 calendar days); remediation
tracked on the head's KPI cadence and reported in the head's
own board pack; CAE re-testing on the CAE's schedule. Joint
owner: the head personally on the accountability side; the
level-50 architect on the substantive remediation authoring;
the level-15 analyst on the tracker maintenance.

## The joint audit-committee appearance rhythm

The IIA discipline is that the CAE has direct access to the
audit committee. That is preserved. In addition, the head and
the CAE appear *jointly* at specific audit-committee moments,
which the interface document specifies.

Typical joint appearances:

- **Annual audit-committee review of the AI-governance
  programme.** Once a year, the head presents the programme's
  effectiveness (KRIs / KPIs / maturity plot / incidents / ROI)
  and the CAE presents the audit-programme view (the audits
  conducted, findings and closures, the audit-plan for the
  coming year as it relates to the AI-governance function).
  The joint appearance is the discipline that ensures the
  audit committee reads a coherent view.
- **Annual AI-audit-plan review.** Where the CAE has an AI-
  audit-plan sub-portfolio, the audit committee reviews it
  with the CAE and the head jointly. The head does not vote
  on the plan; the head is present so the audit committee
  has the head's context on the areas the CAE is prioritising.
- **Material AI-incident post-mortem.** Where the CAE has
  conducted an audit or advisory engagement following a
  material AI incident, the head and the CAE appear jointly
  to present the finding and the enterprise's response. The
  Chief Communications Officer (chapter 10) may be present
  for the disclosure dimension; the CISO (chapter 01) may be
  present for the security dimension.

Between joint appearances, the CAE retains standing executive-
session rights with the audit committee (without management
present) and the head retains equivalent rights. Executive-
session rights are not exercised as a routine posture; they
are exercised when either function has a material issue that
requires committee attention without management filtering.

## The interface document

Consolidated in a single interface document co-signed by the
head and the CAE, ratified in the CxO adjacency map. The
document has, at minimum:

1. **The IIA-invariants statement.** The head is a third-line
   audit subject, not its owner; the CAE is the accountable
   executive for the audit programme; the head does not
   compromise the CAE's independence.
2. **The three coordination surfaces.** Audit-plan input,
   evidence access and fieldwork support, audit-finding
   response and remediation tracking — each with the cadence,
   the joint owners, and the specific procedures.
3. **The joint audit-committee appearance rhythm.** The
   specific joint appearances (annual programme review,
   annual audit-plan review, material-incident post-mortem)
   with the expected preparation and delivery pattern.
4. **The independence safeguards.** The specific safeguards
   preserving the CAE's independence: no head influence on
   audit-plan inclusion / exclusion, no head editing of
   audit reports, no head off-line campaigning against
   findings, no head participation in audit-fieldwork
   decisions.
5. **The escalation ladder.** When the interface breaks — the
   head disputes an audit finding in a way that produces
   procedural conflict; the head believes the CAE has
   excluded an AI-audit area of material importance; the CAE
   observes conduct on the head's part that suggests
   independence-impairment attempts — how the head and the
   CAE escalate. Typically: peer conversation, then the
   audit-committee chair.
6. **The review cadence.** Annual review of the interface
   document itself; ad-hoc on changes to the IIA
   standards or the audit-committee charter.

## Anti-patterns the head does not permit

**The audit-plan negotiation.** The head arrives at the CAE
with a list of "audits we want" and expects the plan to
accommodate. The CAE reads this as an attempt to steer the
audit programme and independence is compromised. The remedy
is: the head provides an annual proposal note; the CAE
decides.

**The finding-negotiation-off-line.** After a draft finding
is issued to the head for management response, the head
negotiates with the audit-team engagement lead to soften the
finding before issuance. The CAE (or the engagement lead)
reads this as pressure and the audit committee will hear
about it. The remedy is: the management-response mechanism is
the only path for disagreement; disputes are recorded and go
to the audit committee.

**The evidence-obstruction pattern.** The head's team makes
evidence extraction painful — extended SLAs, missing
artefacts, incomplete responses — as a passive-defensive
posture. The CAE reports the obstruction to the audit
committee and the head's function loses credibility. The
remedy is: standing access maintained; extractions inside
SLA; interviews available; evidence integrity discipline
preserved.

**The self-assurance substitute.** The head's function
publishes "assurance results" on its own numbers and cites
them at the audit committee as if they were third-line
assurance. The CAE and the audit committee notice the
category error. The remedy is: the head publishes second-
line assurance results as second-line — with the label — and
does not cite them as substitutes for third-line assurance.

**The reactive-only response to findings.** The head only
responds to CAE findings after issuance, without a proactive
posture on emerging areas the CAE has flagged in advance as
of concern. The head's function then repeatedly appears
"caught off guard" at the audit committee. The remedy is:
when the CAE signals an area of emerging concern in advance
of an engagement, the head's function takes the signal as
a management indicator and acts on it before the audit
finding lands.

## The head's own three-lines-of-defence posture

The head runs a second-line function. The AI Governance
Council chaired by the head (chapter
[[11-chairing-the-governance-council]]) is a second-line
governance body. The KRI/KPI portfolio the head produces is a
second-line telemetry pipeline. The AI risk register the head
maintains is a second-line register.

First-line functions in AI are the product, engineering, and
platform teams building and operating AI systems. The head's
second-line function challenges first-line decisions where
appetite is at stake; provides governance-runtime services
first-line consumes (AIA templates, evaluation harness
integration, evidence pipelines); and reports second-line-
material events into the risk and audit committees.

Third-line is the CAE's. The head coordinates with the CAE per
this chapter and does not confuse the head's function with
third-line. When an AI system needs assurance beyond what the
head's second-line function can defensibly provide (because
self-assurance has an inherent independence limit), the
engagement is a third-line engagement — by the CAE's team or
by an external assurance provider (an ISO/IEC 42001
certification body, a ForHumanity IAAIS auditor, a BABL AI
auditor, or an equivalent) engaged by the CAE — not by the
head's own team.

## Composition with adjacent modules

- The **CxO adjacency map** in
  [[mod-101-role-scope-and-leadership-shape]] chapter 06 is
  the parent boundary document; the three-lines-at-leadership-
  scope chapter (chapter 04) is the invariant statement this
  chapter operates against.
- The **third-line-and-CAE coordination** in
  [[mod-108-leading-the-governance-function]] chapter 05
  covers the personnel-and-function-leadership dimension of
  the CAE coordination.
- The **CRO coordination** in chapter 04 of this module
  covers the second-line composition into the CRO's
  enterprise risk framework — the CAE audits both functions.
- The **KRI/KPI portfolio** in
  [[mod-107-program-measurement-and-maturity]] chapter 01 is
  where the third-line-assurance-of-the-metric ownership row
  appears.
- The **audit-committee reporting cluster** in
  [[mod-103-board-and-audit-committee-reporting]] is the
  forum where joint appearances occur.

## Summary

- The head is a third-line audit *subject*, not its owner.
  The CAE is the accountable executive for the audit
  programme. The head does not co-author the audit plan,
  does not edit audit reports, does not negotiate findings
  off-line, and does not compromise the CAE's independence.
- Three coordination surfaces carry the work: audit-plan
  input (proposal, not co-authorship), evidence access and
  fieldwork support (standing access, extraction SLAs,
  interview availability, evidence integrity), and audit-
  finding response and remediation tracking (accept /
  mitigate / dispute, time-bound remediation, tracked to
  closure).
- The joint audit-committee appearance rhythm — annual
  programme review, annual audit-plan review, material-
  incident post-mortem — is the discipline that keeps the
  audit committee's read of the AI-governance function
  coherent between the head's and the CAE's views.
- Five anti-patterns to refuse: audit-plan negotiation,
  finding-negotiation-off-line, evidence-obstruction pattern,
  self-assurance substitute, reactive-only response to
  findings.
- The head runs a second-line function; the CAE runs third
  line. Where an AI system needs assurance beyond second-
  line's defensible reach, the engagement is third-line — the
  CAE's team or an external assurance provider the CAE
  engages — not the head's own team.
- The interface document — co-signed by head and CAE — is
  ratified in the CxO adjacency map, reviewed annually, and
  the head and CAE appear jointly at the audit committee on
  the specified rhythm.
- Chapter [[06-general-counsel-coordination]] turns to the
  General Counsel adjacency — the engagement-versus-legal-
  opinion boundary, litigation posture, and the SAR / MOU /
  MRA management the head coordinates with GC on.
