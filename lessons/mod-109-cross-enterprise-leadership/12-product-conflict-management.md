# Managing the Product-Owner Conflict Pattern — Stop-Ship, Delayed-Release, Feature-Scope-Reduction, and the Rehearsed Escalation Ladder

## Motivation

The AI-governance function's authority is tested, in every
enterprise, on the release-decision surface. Product owners
run their systems on delivery timelines with commercial
commitments — quarterly-earnings scope, contractual release
dates, customer-facing announcement windows, competitive-
positioning moves. The head's function stands at the release
gate with the AIA, the evaluation results, the risk register,
the exception discipline, and — sometimes — the substantive
finding that says "this cannot ship as scoped".

Three specific conflict scenarios recur enough to be treated
as named patterns rather than one-off arguments:

- **Stop-ship.** The head's function concludes an AI system
  cannot be released at all in its current form. The finding
  is severe enough to warrant halting the release entirely,
  pending remediation the head names.
- **Delayed-release.** The head's function concludes an AI
  system cannot ship on the planned date but can ship after
  specific remediation on a named timeline. The scope of the
  system is preserved; the timing moves.
- **Feature-scope-reduction.** The head's function concludes
  an AI system can ship on the planned date but only with a
  specific feature or capability removed, throttled, or
  restricted to a specific population. The timing is
  preserved; the scope narrows.

Every one of these decisions puts the head into conflict with
a product owner whose incentives run the other direction. The
conflict is not a symptom of a broken governance function; it
is the *predictable operating cost* of a functioning one.

The failure mode this chapter is written against is the
conflict that turns political. When the escalation ladder is
not written down, product owners appeal directly to the CEO
or the board on the merits of the individual system, framing
the head as an obstacle. Peers pick sides. The audit
committee reads the conflict as a governance failure ("why
is your AI-governance function fighting with your product
organisation") rather than as a governance success ("your
AI-governance function surfaced a material finding and the
enterprise's escalation discipline resolved it on the
merits"). Once the pattern becomes political, the head's
authority erodes; the next stop-ship finding is harder to
carry; the pattern gets worse until it hits an incident that
was preventable and the function loses its remit.

The pattern in this chapter is what prevents that. It rests on
three moves. First, the **asked-and-answered discipline** — a
named substantive question with a named substantive answer,
carried through the escalation without redefinition. Second,
the **rehearsed escalation ladder** — a written ladder with
named steps, named participants, and named timings, rehearsed
before the live case rather than improvised at the moment.
Third, the **decision-and-dissent discipline** — the ladder
closes with a named decision on the record, with the head's
substantive position preserved as dissent where the decision
proceeds against it. The ladder does not require the head to
win every escalation; it requires the head to carry every
escalation on the merits, and the record to reflect the
substance.

The chapter draws on the negotiation-and-conflict literature
adjacent to executive practice (Fisher and Ury's *Getting to
Yes* on principled negotiation; Patterson et al.'s *Crucial
Conversations* on the discipline of high-stakes exchanges),
the IIA's guidance on second-line function escalation, the
BSA / OECD guidance on responsible-AI deployment gates, and
the enterprise-governance literature on decision-rights
architecture (RACI / RAPID conventions), each cited in
`resources.md`. The composition with the AI Governance Council
from chapter [[11-chairing-the-governance-council]] and the
audit-committee reporting cluster from
[[mod-103-board-and-audit-committee-reporting]] is
load-bearing.

## Core concept — the asked-and-answered discipline

The load-bearing move is the asked-and-answered discipline.
When the head's function surfaces a stop-ship, delayed-
release, or feature-scope-reduction finding, the finding is
framed as a named substantive question with a named
substantive answer. The question and the answer travel
through the escalation ladder together, unmodified in
substance; the ladder decides what to do with the answer, not
whether the question was validly asked or the answer honestly
given.

An example. The head's evaluation function finds that a
production recommendation system's fairness metric on
protected-class exposure has degraded past the enterprise's
own AI Third-Party Standard threshold since the last
retraining. The system is scheduled to release a new model
version tomorrow. The head's substantive question: "does the
enterprise's AI Third-Party Standard threshold on protected-
class exposure permit this release". The head's substantive
answer: "no; the current metric exceeds the threshold by X
percentage points on the protected class named; the standard
requires the release to be delayed until the metric is within
threshold, per section [named] of the standard".

The question and the answer are load-bearing because they
frame the escalation as a *policy question* — is the standard
applied — not as an *authority question* — does the head have
the authority to stop the release. The policy question can be
answered on the merits by any escalation level. The authority
question invites political framing ("the head is exceeding
their remit", "the head is being unreasonable", "the product
organisation needs to move faster").

The head's discipline: every conflict conversation starts by
naming the question and the answer, and every escalation step
carries the same question and the same answer forward. Where
the product owner or an escalation level wants to reframe the
question ("the real question is whether we can ship on time";
"the real question is whether the head's threshold is
calibrated correctly"), the head returns the frame ("the
policy question is X; we can also examine the calibration
question separately, but that examination does not change the
answer to the policy question as it stands").

## The three conflict types

The three conflict types share the discipline but differ in
severity, framing, and remediation shape.

### Stop-ship

The stop-ship finding is the highest-severity of the three.
The head's function concludes the system cannot release at
all in its current form. Typical triggers:
- An evaluation surfaces a fairness, safety, or security
  finding severe enough to warrant halting.
- The AIA is not on file at the required tier depth and the
  system has been miscategorised in intake.
- A red-team finding routed under chapter [[01-ciso-
  coordination]] is unremediated and mapped to a severity
  that blocks release.
- A regulatory-obligation finding under
  [[mod-105-regulatory-change-management]] concludes the
  system's release without specific controls violates a
  named obligation.

Framing: "The enterprise's [named policy or obligation]
requires that this system does not release in its current
form. The specific finding is [X]. The remediation is [Y].
The system may release when [Y] is complete."

Remediation shape: named substantive remediation with a
named criterion for release readiness. Not "release when the
head is comfortable"; "release when [named metric] is at
[named threshold] against [named evaluation set]".

### Delayed-release

The delayed-release finding is lower-severity than stop-ship
but blocks the planned release date. The system can ship
after specific remediation on a named timeline. Typical
triggers:
- An evaluation surfaces a finding that is not release-
  blocking at the highest severity but is not within the
  standard's threshold at the current release scope.
- A required approval, evidence artefact, or documentation
  is not yet complete, and completion has a named timeline.
- A pre-existing exception is expiring and re-approval has
  not been completed at the required cadence.

Framing: "The enterprise's [named policy or obligation]
requires [specific remediation] before this release proceeds.
The remediation is on a [named timeline]. The system may
release on [named date] when [remediation] is complete."

Remediation shape: named remediation on a named timeline,
often with the product owner and the head's level-50
architect co-scoping the remediation to compress the timeline
where possible without compromising the substance.

### Feature-scope-reduction

The feature-scope-reduction finding permits the release but
narrows the scope. The system ships on the planned date
without one or more features, capabilities, populations, or
integrations. Typical triggers:
- A specific feature (an agentic tool-call capability, a
  high-risk output modality, an integration with an
  unsanctioned data source) has an unresolved governance
  finding while the rest of the system is release-ready.
- A specific customer population (a jurisdiction with a
  regulatory obligation the enterprise is not ready to
  meet; a demographic segment where the fairness evaluation
  has surfaced a material gap) is out of scope pending
  remediation.
- A specific use case (a high-risk downstream use the
  enterprise is not ready to sanction; a use case that
  requires a specific consent flow that is not yet built)
  is disabled at feature-flag level.

Framing: "The system may release on the planned date with
[specific scope reduction]. The reduced scope is [named
feature, population, or use case]. The reduced scope may be
restored when [named remediation] is complete."

Remediation shape: feature-flag or capability-gating that is
enforceable in production, with a named re-scoping trigger
and a named audit trail on the reduction.

## The rehearsed escalation ladder

The escalation ladder is a five-step written ladder with named
steps, named participants, and named timings. The ladder is
rehearsed in tabletop drills at least annually (see the
exercise [[exercise-06-product-conflict-escalation-
rehearsal]]).

### Step 1 — Head-to-product-owner working session

The first step is a working session between the head's level-
50 architect and the product owner (or the product owner's
technical lead). The session's purpose is to establish the
asked-and-answered pair — is the substantive question and
answer agreed to, or is there a genuine substantive
disagreement.

Three outcomes:
- **Agreed and resolved.** The product owner accepts the
  finding, the remediation, and the timeline. The item goes
  to the standing exception register (chapter
  [[mod-102-running-the-program]] chapter 05 exception
  discipline) and the release plan updates. No further
  escalation.
- **Agreed with re-scoping.** The product owner and the
  architect agree the finding stands, and jointly re-scope
  the remediation to compress the impact — a feature-scope-
  reduction may substitute for a delayed-release where
  the substantive finding is preserved. The re-scoping is
  documented and the release plan updates. No further
  escalation.
- **Disagreed on the substance.** The product owner does not
  accept the finding, the standard's application, the
  remediation, or the timeline. The item goes to Step 2.

Timing: same day for a live release-gate item; within one
business day for a routine finding.

### Step 2 — Head-to-product-organisation-lead conversation

Step 2 elevates from the working-level to the leadership-
level. The head personally engages the product organisation's
lead — the VP of Product for the product line, or the
General Manager of the business unit. The purpose is not to
override the product owner but to establish whether the
leadership layer sees the same substantive question and answer
the working-level session did.

Three outcomes:
- **Resolved at leadership level.** The product-organisation
  lead accepts the finding as it stands or with a co-scoped
  amendment. The item closes.
- **Resolved with escalation-to-council commitment.** The
  product-organisation lead does not resolve at this level
  but agrees the item goes to the AI Governance Council
  (Step 3) with both positions documented. The head does
  not proceed to a unilateral stop-ship at this step; the
  discipline is that the council decides.
- **Attempted end-run.** The product-organisation lead
  bypasses the head and escalates to the CEO or the CAIO
  directly, framing the head as the obstacle. The head
  responds by requesting the CEO or CAIO route the item to
  the council rather than deciding bilaterally; where the
  end-run is a pattern, the head raises the pattern as a
  named escalation to the audit committee under the
  audit-committee-access invariant
  ([[mod-101-role-scope-and-leadership-shape]] chapter 07
  engagement-contract discipline).

Timing: within one business day for a live release-gate item;
within three business days for a routine finding.

### Step 3 — AI Governance Council decision

Step 3 is the standing forum. The head brings the item to the
AI Governance Council (chapter [[11-chairing-the-governance-
council]]) with the pre-read including the substantive
finding, the product owner's substantive position, the
remediation the head recommends, and the release plan impact.
The council decides.

The council's decision options:
- **Uphold the head's finding.** The stop-ship, delayed-
  release, or feature-scope-reduction stands. The release
  plan updates; the remediation begins; the item is
  monitored on the council's action-item register.
- **Modify the head's finding.** The council amends the
  scope of the reduction, the remediation, or the timeline.
  The head accepts the amendment; the release plan updates.
- **Grant a documented exception.** The council grants an
  exception to the standard the head applied, on the terms
  named in the exception discipline. The exception has a
  named expiry, named compensating controls, named residual-
  risk owner, and named re-review trigger. The exception is
  logged; the CAE reads it as part of the standing exception
  register.
- **Escalate to the audit committee.** Where the material
  significance exceeds the council's authority (a stop-ship
  on a system of high strategic importance; a finding with
  material regulatory implications; a pattern of exceptions
  the council does not want to accumulate without board
  visibility), the council escalates to the audit committee
  under the chapter [[11-chairing-the-governance-council]]
  material-single-decision escalation pathway.

The head's substantive position is preserved in the record
regardless of the council's decision. Where the council
decides against the head, the dissent-capture discipline
from chapter [[11-chairing-the-governance-council]] captures
the head's dissent in the council minute, and — where the
decision has material AI-safety, fairness, or regulatory-
compliance implications the head cannot support in silence —
the head triggers Step 4.

Timing: at the next scheduled council or by written
resolution (chapter [[11-chairing-the-governance-council]])
for time-critical items; typically within one to two weeks.

### Step 4 — Escalation to CEO / CAIO

Step 4 is peer escalation above the council. The head raises
the item personally to the CEO (or the CAIO where the CAIO
holds the reporting line for the AI-governance function).
The purpose is to surface either (a) a material substantive
disagreement the head cannot support in silence, or (b) a
pattern of end-runs, exceptions, or dismissals that
undermines the governance function's authority in a way that
the head is professionally obligated to name.

The head prepares Step 4 as a written brief — one to three
pages — with the specific finding, the substantive question
and answer, the escalation trail through Steps 1 through 3,
the head's professional recommendation, and the head's
proposed resolution. The head does not use Step 4 as a
routine escalation for items the council has properly
adjudicated against the head's preference; Step 4 is for
material questions where the head's professional obligation
is engaged.

The CEO / CAIO's decision options:
- **Uphold the council's decision.** The head accepts and
  the item closes at Step 4.
- **Overturn the council's decision.** The CEO / CAIO
  overrides in the head's direction. The item closes at
  Step 4.
- **Route to the audit committee.** The CEO / CAIO routes
  the item to the audit committee for board-level
  ratification. The item goes to Step 5.
- **Route to the general-counsel for legal-authority
  determination.** Where the underlying question includes a
  legal-obligation dimension the CEO / CAIO wants GC's
  opinion on, the item routes through GC (chapter
  [[06-general-counsel-coordination]]) and returns for
  final resolution at Step 4 or Step 5 as applicable.

Timing: within one week of the council decision, or
compressed for live release-gate items.

### Step 5 — Audit-committee escalation

Step 5 is the final step. The head, under the audit-
committee-access invariant, escalates to the audit-committee
chair on any second-line-material item where the escalation
ladder has not resolved the substantive question and where
the head's professional obligation requires the audit
committee's read.

Step 5 is the invariant preserved by
[[mod-101-role-scope-and-leadership-shape]] chapter 07
engagement-contract discipline. It is not a routine
escalation. Using it degrades its value; not using it when
the professional obligation requires it is the failure the
invariant exists to prevent.

The audit-committee chair's decision options include: full
audit-committee session on the item, private meeting with the
head to gather additional context, request to the CEO / CAIO
to reopen at Step 4 with additional inputs, or acceptance of
the escalation record for the audit committee's forward
attention. The head accepts the audit-committee chair's
process choice.

Timing: at the audit committee's next scheduled session, or
sooner for emergency-escalation items (per chapter
[[11-chairing-the-governance-council]] emergency escalation).

## The rehearsed-not-improvised discipline

The ladder is written *before* the live case, and rehearsed at
least annually against tabletop scenarios covering the three
conflict types. Rehearsal produces three specific benefits.

**Rehearsal builds the muscle for the substantive question.**
Live conflict conversations are high-stakes and time-
pressured. The habit of naming the substantive question and
answer explicitly — and of resisting the reframe — is a
muscle the head builds in rehearsal, not on the first live
case. Heads who improvise on their first live stop-ship
lose the substance under pressure.

**Rehearsal builds the peer-network familiarity.** The
product-organisation leads, the CEO / CAIO's office, and the
audit-committee chair see the ladder in tabletop before they
see it live. The first time they read the head's substantive
finding is not in an incident. This is the same discipline
the CISO applies to incident-response tabletops and that
[[mod-110-incident-leadership]] applies to AI-incident
tabletops; the escalation ladder is the same class of
artefact.

**Rehearsal surfaces ladder-design failures.** A step whose
timing is unrealistic, a participant who cannot be reached
in the timing, an outcome that was not anticipated — these
surface in tabletop. Fixing them in tabletop is far cheaper
than discovering them on the first live case.

The tabletop cadence is annual at minimum, with additional
tabletops when the ladder is updated, when the head's
function has turnover at the level-50 architect layer, or
when the product-organisation's structure changes materially.

## The escalation-ladder document

Consolidated in a single escalation-ladder document owned by
the head, co-signed by the CEO or CAIO (as the enterprise's
executive-authority reference), reviewed at the AI Governance
Council on the annual review cadence, and stored in the
CCO's enterprise policy library (chapter [[09-chief-
compliance-officer-coordination]]). The document has, at
minimum:

1. **The three conflict types.** Stop-ship, delayed-release,
   feature-scope-reduction — with the framing template and
   the remediation shape per type.
2. **The asked-and-answered discipline.** The template for
   how a finding is framed as a substantive question and
   answer, with the head's obligation to carry the question
   and answer unmodified through the ladder.
3. **The five ladder steps.** Named steps, named
   participants, named timings, named outcomes per step.
4. **The council pathway.** Reference to chapter
   [[11-chairing-the-governance-council]] — how the item is
   brought to the council, the pre-read format, the decision
   options.
5. **The audit-committee-access invariant.** Reference to
   [[mod-101-role-scope-and-leadership-shape]] chapter 07
   engagement-contract discipline — how Step 5 is invoked,
   what it is used for, what it is not used for.
6. **The tabletop-rehearsal cadence.** Named cadence, named
   scenarios, named participants in rehearsal.
7. **The record-keeping discipline.** How each escalation is
   logged — the substantive question, the answer, the
   ladder steps taken, the timing, the outcome — for the
   annual council effectiveness review and the CAE's audit
   scope.
8. **The review cadence.** Annual review of the escalation-
   ladder document at the council; ad-hoc on material
   organisational or program changes.

## Anti-patterns the head does not permit

**The unilateral stop-ship at Step 1.** The head's function
declares a stop-ship at the working-level session and treats
the declaration as final without the escalation ladder
running. The product organisation experiences the finding
as an ambush; the CEO / CAIO reads it as the head exceeding
authority; the substantive merits are lost under the
authority conflict. The remedy is: the head's function
articulates the substantive finding at Step 1 and carries it
through the ladder; the stop-ship *outcome* is decided by
the ladder, not asserted unilaterally by the head.

**The reframe accepted.** The head accepts the product
organisation's reframe of the question ("the real question is
whether we can ship on time"). The escalation runs on the
reframed question. The head's original substantive answer
becomes invisible. The remedy is: the asked-and-answered
discipline. The head returns the frame — "the policy
question is X; the timing question is separate; we can
examine both, but the policy question's answer does not
change because the timing question is difficult".

**The end-run without response.** The product-organisation
lead bypasses the head and escalates directly to the CEO or
CAIO. The head learns about the escalation after the fact.
The head does not respond, either because the head does not
know how or because the head believes escalating an end-run
looks defensive. The pattern repeats; the head's authority
erodes. The remedy is: the head responds to every end-run —
substantively at the CEO / CAIO level (requesting the item
route to the council), and structurally by raising the
pattern to the audit committee if end-runs become recurrent.

**The council-decision that the head cannot accept in
silence.** The council decides against the head on a
substantive finding the head's professional obligation
requires the head to escalate further. The head accepts the
council decision publicly to preserve the appearance of
alignment while privately disagreeing. Later, the substantive
finding proves out; the audit committee reads that the head
knew and did not escalate. The remedy is: Step 4 and Step 5
exist for exactly this scenario. Using them is a professional
obligation, not a political move; the head's engagement
contract preserves the invariant precisely because the head
will occasionally need to exercise it.

**The escalation as routine.** The head runs every finding
through Steps 4 and 5 rather than accepting council
decisions at Step 3. The escalation ladder loses its
gravity; the CEO / CAIO's office and the audit committee
disengage; when the head genuinely needs Step 4 or Step 5 for
a material finding, the escalation lands with reduced
weight. The remedy is: the head reserves Steps 4 and 5 for
material findings; routine council-adjudicated items close
at Step 3 with named dissent in the record.

**The improvised ladder.** The escalation-ladder document
does not exist, or it exists but has never been rehearsed.
The first live stop-ship is the first exercise of the
ladder; participants improvise; the substantive question
gets lost. The remedy is: the ladder is written and
rehearsed before the first live case.

**The finding that never enters the ladder.** The head
identifies a substantive finding but does not bring it
forward because the product owner's likely resistance is
uncomfortable to face. The system ships; the finding proves
out later; the audit committee's post-mortem reads that the
head knew and did not escalate. The remedy is: the head
brings every finding forward. The ladder decides what
happens; the head decides what to raise.

## Where the discipline earns its keep — the live stop-ship

The load-bearing test of the ladder is the live stop-ship on
a strategically important release. The enterprise has
announced a new AI-powered product tier that ships next
Tuesday, with customer commitments in place, marketing
running, and quarterly earnings scope depending on the
launch. The head's evaluation function, in the final pre-
release run, surfaces a fairness finding on protected-class
exposure that exceeds the enterprise's Third-Party Standard
threshold. The head concludes stop-ship is warranted pending
remediation the head's team estimates at three to six weeks.

If the ladder is running, the following happens over the
next forty-eight hours. Step 1: the head's level-50
architect meets with the product owner; the substantive
question is named ("does the Third-Party Standard threshold
permit release with the current metric"); the answer is
named ("no; the metric exceeds threshold by X percentage
points"); the product owner disagrees on the applicability
of the threshold to this system class. Step 2: the head
personally engages the VP of Product for the product line;
the substantive question and answer are re-affirmed; the VP
does not accept, but agrees the item goes to the council
under written resolution given the time constraint. Step 3:
the council convenes by written resolution within 24 hours;
the pre-read includes the substantive finding, the product
owner's position, the head's recommendation (stop-ship for
three to six weeks, with named remediation and a re-
evaluation gate), the CFO's material-event evaluation
(disclosure obligations under the applicable rules), and
GC's legal-exposure evaluation. The council decides: uphold
the head's finding with a compressed remediation timeline
(two to three weeks) that the head's function and the
product owner co-scope; the launch is delayed; the CCO's
crisis-communications runbook (chapter [[10-chief-
communications-officer-coordination]]) is activated for the
customer, investor, and internal communications on the
delay; the CFO's material-event evaluation triggers
appropriate disclosure. The head is not asked whether the
launch will proceed on Tuesday; the ladder decided.

If the ladder is not running, the alternative sequence: the
head asserts stop-ship at Step 1; the product owner escalates
directly to the CEO ("the head is trying to kill our launch");
the CEO makes a bilateral decision under launch-week pressure
without the council's substantive record, GC's evaluation, or
the CFO's disclosure evaluation; the launch proceeds; the
fairness finding proves out post-launch through customer
complaints and — worse — a regulator inquiry; the audit
committee's post-mortem finds that the head raised the
finding but the escalation was not run through the
established ladder because the ladder did not exist or was
not rehearsed. The head loses the argument in the room; the
enterprise loses the argument in the record.

## Composition with adjacent modules

- The **engagement-contract discipline** in
  [[mod-101-role-scope-and-leadership-shape]] chapter 07 is
  where the audit-committee-access invariant is negotiated at
  hiring; Step 5 depends on it.
- The **CxO adjacency map** in
  [[mod-101-role-scope-and-leadership-shape]] chapter 06 is
  the parent boundary document naming the relationship with
  every ladder participant.
- The **AIMS operating cadence** in
  [[mod-102-running-the-program]] chapter 02 and the
  **exception-and-waiver discipline** in
  [[mod-102-running-the-program]] chapter 05 are the source
  of the release-gate findings and the register in which
  exceptions land.
- The **evaluation discipline** in
  [[mod-102-running-the-program]] chapter 08 is where the
  substantive findings that enter the ladder originate.
- The **audit-committee reporting cluster** in
  [[mod-103-board-and-audit-committee-reporting]] is the
  forum Step 5 escalates into.
- The **regulatory-obligation register** in
  [[mod-105-regulatory-change-management]] is the reference
  for findings that involve a named obligation.
- The **AI Governance Council** in chapter
  [[11-chairing-the-governance-council]] is where Step 3
  runs.
- The **General Counsel coordination** in chapter
  [[06-general-counsel-coordination]] is where legal-
  authority determinations under Step 4 route through GC.
- The **CFO coordination** in chapter
  [[07-cfo-coordination]] is where material-event and
  disclosure evaluations for delayed launches and stop-ship
  events run.
- The **Chief Communications Officer coordination** in
  chapter [[10-chief-communications-officer-coordination]] is
  where customer, investor, and internal communications on
  a stop-ship or delayed-release run.
- The **incident-leadership discipline** in
  [[mod-110-incident-leadership]] is where a stop-ship that
  post-dates an incident (as containment or as remediation)
  operates.

## Summary

- Product-owner conflict on AI releases is the predictable
  operating cost of a functioning governance function, not a
  symptom of a broken one. The pattern that keeps the
  conflict on merits is a written, rehearsed escalation
  ladder — not improvisation at the moment.
- Three conflict types recur: stop-ship (release cannot
  proceed), delayed-release (release proceeds after
  remediation on a named timeline), feature-scope-reduction
  (release proceeds with narrowed scope). Each has its own
  framing template and remediation shape.
- The asked-and-answered discipline names every finding as a
  substantive question with a substantive answer, and
  carries the question and answer unmodified through the
  ladder. Reframes are returned, not accepted.
- The five-step ladder: Step 1 head-to-product-owner working
  session; Step 2 head-to-product-organisation-lead
  conversation; Step 3 AI Governance Council decision; Step
  4 CEO / CAIO escalation on material substantive
  disagreements; Step 5 audit-committee escalation under
  the audit-committee-access invariant. Named participants,
  named timings, named outcomes per step.
- The ladder is rehearsed in annual tabletops covering the
  three conflict types. Rehearsal builds substantive-question
  muscle, peer-network familiarity, and surfaces ladder-
  design failures before the first live case.
- The escalation-ladder document is co-signed by the head
  and the CEO / CAIO, ratified at the AI Governance Council,
  reviewed annually, and stored in the CCO's enterprise
  policy library.
- Seven anti-patterns to refuse: the unilateral stop-ship at
  Step 1, the reframe accepted, the end-run without
  response, the council-decision the head cannot accept in
  silence, the escalation as routine, the improvised ladder,
  and the finding that never enters the ladder.
- The ladder does not require the head to win every
  escalation; it requires the head to carry every escalation
  on the merits, with the substantive record preserved. The
  audit committee reads the record; the record's honesty is
  what preserves the function's authority across time.
- This chapter closes mod-109. Chapter
  [[mod-110-incident-leadership]] turns to the *incident*
  discipline where every one of this module's coordination
  patterns comes under time pressure at once — CISO, GC,
  CCO, CFO, DPO, CHRO, CCO (compliance), and the AI
  Governance Council — with the head running the substantive
  spine across all of them.
