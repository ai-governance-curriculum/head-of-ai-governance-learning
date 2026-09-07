# Chairing the AI Governance Council — Agenda Discipline, Decision-Forcing, Dissent-Capture, and the Escalation Pathway

## Motivation

Chapters 01 through 10 turn *outward*, to the CxO peer
adjacencies. This chapter turns *inward*. The AI Governance
Council is the standing decision-making body the head chairs
inside the enterprise's own governance architecture. Its
purpose is to hold the enterprise's AI-governance decisions —
policy ratifications, tier assignments, exception approvals,
material dissent surfacings, escalations to the board — in a
single forum with a documented process, a named membership, a
predictable cadence, and a decision log the audit committee
can read.

Councils fail in predictable ways. The council with a wandering
agenda that never forces the substantive decision the head
convened it for. The council that captures decisions but not
dissent, so the audit committee later learns that a decision
was "made unanimously" when three members had reservations they
never got to name. The council whose escalation-to-board
pathway is improvised in the moment, so material AI risks
either reach the board too late (after the incident) or too
early (before the substantive question is framed). The council
whose minutes are the head's personal notes rather than a
document-controlled record.

Chairing well is a craft. It is not the same craft as running
the AI-governance program (that is
[[mod-102-running-the-program]]) or as reporting to the audit
committee (that is [[mod-103-board-and-audit-committee-
reporting]]). It is the discipline of the *forum itself* —
what goes on the agenda, how the decision is forced, how
dissent is captured, how the minute becomes a decision, how
the escalation to the board is triggered, how the council's
own effectiveness is reviewed.

The pattern in this chapter draws on Robert's Rules of Order
(Newly Revised) as the parent-parliamentary reference many
enterprises defer to, the ICSA / Chartered Governance Institute
guidance on committee chairing, ISO/IEC 42001 clause 5.3
(organisational roles, responsibilities, and authorities) and
clause 9.3 (management review) as the parent-standard
requirements the council operationalises, the OECD Corporate
Governance Principles (2023) on board-committee discipline
adjacent to the audit-committee-reporting pathway, the IIA's
guidance on governance-committee discipline, and the practice
literature on high-performing executive committees (Charan,
Useem, and adjacent references cited in `resources.md`).

## Core concept — the council is a decision-forcing forum, not
## a status meeting

The load-bearing move is to run the council as a decision-
forcing forum. Every substantive agenda item is a decision the
council will take at this meeting or is a decision the council
has explicitly deferred with a named next-decision date. The
council does not accept "we discussed this" as an outcome. It
accepts "we decided this", "we decided to defer to <date> with
these specific inputs to be delivered", or "we escalated this
to <named body> because it exceeds our authority". No agenda
item leaves the room in the "we discussed this" state without
the chair naming the deferral or the escalation.

The distinction matters because the alternative — the status-
meeting drift — is the most common council failure mode. A
council in status-meeting mode reads updates, asks
clarifying questions, notes concerns, and adjourns. The
decisions that were meant to be forced were not forced. The
policy that needed ratification remains unratified. The tier
assignment that needed adjudication remains ambiguous. The
exception that needed approval or rejection remains in the
"under review" state. Six months later, the CAE's audit
finding names the pattern: "The AI Governance Council does
not evidence decision-forcing discipline."

The chair's craft is what prevents this. It is not aggression
or force of personality; it is the discipline of running the
agenda against a named decision at every item, capturing
dissent transparently on the record, and closing the item
with an unambiguous outcome before moving on.

## Council architecture — membership, quorum, and voting

The council's architecture is written in the charter (the
artefact this chapter produces; see the exercise
[[exercise-05-governance-council-chair-drill]]). Four
architectural decisions carry the load.

### Membership

The council's membership is small enough to make decisions and
representative enough that the decisions stick. Typical shape:
- **Chair.** The head of AI governance. Non-voting on
  substantive items (the chair runs the discipline; the vote
  is the members'); voting only in tie-break, and only where
  the charter grants the chair the tie-break vote.
- **Voting members.** The C-suite peers the AI-governance
  function's decisions materially affect. Typical set: CIO
  or CTO (representing the AI platform), CDO (data
  governance), CISO (AI security), CPO / DPO (privacy),
  General Counsel (legal), CRO (risk framework), CCO (chief
  compliance officer), CFO (budget-material items), CAIO
  where the enterprise has one. Where the enterprise has a
  Chief Medical Officer (health-and-medical-device sector),
  Head of Model Risk Management (banking / insurance), or
  other sector-specialist executive whose function overlaps
  materially, that officer is a voting member.
- **Standing invitees.** The CAE (in observer capacity —
  the CAE does not vote because the CAE is third-line
  assurance on decisions the council makes; the CAE's
  presence preserves the CAE's audit-committee reporting
  visibility). The Chief Human Resources Officer as invitee
  when AI-in-HR items are on the agenda. The Chief
  Communications Officer as invitee when public-trust or
  incident-communications items are on the agenda. Business-
  unit leaders as invitees for items concerning their
  business unit.
- **Rotating attendees.** Product-owner leads and
  engineering-lead delegates on the specific items concerning
  their systems.
- **Secretariat.** A named secretariat — usually a delegate
  from the head's function at the level-35 or level-50 layer
  — responsible for agenda circulation, pre-read
  distribution, minute-keeping, decision-log maintenance,
  action-item tracking. The secretariat role is fixed;
  turnover risk on this role is a load-bearing concern.

The membership size is bounded — a council larger than twelve
to fifteen voting members loses decision-forcing discipline
because too many perspectives compete for the room's time.
Where the enterprise's C-suite is larger, the charter names
which officers are members and which are standing invitees.

### Quorum

The charter specifies quorum. Typical: two-thirds of voting
members present (in person or remote) for substantive
decisions; a lower threshold for informational items and
minute ratification. Where quorum is not met, substantive
decisions cannot be taken; the chair reschedules or takes the
decision to written resolution (see below). Running an
important vote below quorum is a chapter [[05-cae-
coordination]] audit finding in waiting.

### Voting and consensus

Two voting models to choose between in the charter.

The **consensus** model: decisions are taken by consensus,
with the chair testing consensus explicitly ("do we have
consensus to ratify this policy") and named dissent captured
against the decision. Where a member dissents, the decision
still proceeds if consensus is otherwise present, and the
dissent is recorded with the member's name and the
substantive reason. Consensus does not mean unanimity; it
means "no member insists on blocking".

The **formal-vote** model: substantive decisions are taken by
formal vote. Each voting member votes for, against, or
abstains. Named votes are recorded. Majority decides
(typically simple majority, sometimes a supermajority for
material items).

Most enterprises run consensus at the standing council with
formal-vote fallback for genuinely contested items and for
policy-ratification of the highest material significance
(where the charter mandates formal vote). The choice is
enterprise-specific. The load-bearing move is that the
charter names the model and applies it consistently.

### Written resolution

For decisions that cannot wait for the next council meeting,
the charter permits written resolution: the chair circulates
the proposed decision with the pre-read materials, voting
members respond within a named window (typically 3 to 5
business days), the resolution passes if the required
threshold is met. Written resolutions are a load-bearing
release valve — used sparingly, they prevent the "we couldn't
convene the council so we made the decision ad hoc" pattern
that undermines the council's authority.

## Agenda-setting discipline

The chair owns the agenda. The agenda is not co-authored by
whoever wants an item on it; the chair curates and sequences.
Three moves make agenda-setting work.

**Standing items and rotating items.** The agenda has a small
set of standing items that appear every meeting — decision-
log review from prior meeting; action-item status;
regulatory-change surfacing from
[[mod-105-regulatory-change-management]]; incident and near-
miss review; KRI / KPI portfolio dashboard from
[[mod-107-program-measurement-and-maturity]]. And a larger
set of rotating items — policy ratifications, tier
assignments, exception approvals, sector-overlay adoptions,
regulator-correspondence briefings — that cycle on the AIMS
operating calendar cadence from [[mod-102-running-the-
program]] chapter 02.

**Every substantive item names a decision.** No item goes on
the agenda without a named decision or a named informational
outcome. "Discussion of the fairness testing programme" is
not an agenda item; "Ratification of the fairness testing
policy v2.0" is. Where the item is genuinely informational
(a briefing on a regulator development, a horizon-scanning
signal), the agenda names it as informational and the chair
does not allow it to drift into decision-making without a
name change and appropriate pre-read.

**Pre-read discipline.** Substantive items have a pre-read
circulated the standard number of business days ahead
(typically five). Members are expected to have read the pre-
read; the chair does not permit the meeting to be used to
brief the material the pre-read covered. Where a member is
unprepared, the item may be deferred at the chair's
discretion (with the deferral logged); the chair does not
walk the council through pre-read material as a courtesy
because that is the discipline that lets pre-reads be
skipped next time.

## Decision-forcing at the meeting

The chair's craft at the meeting itself is the discipline of
closing every agenda item. Four moves.

**Frame the decision.** At the start of each substantive
item, the chair frames the decision precisely: "The council
is asked to ratify the AI Third-Party Standard v1.3, effective
[date], with the following material changes from v1.2:
[named]. The council may (a) ratify as drafted, (b) ratify
with named amendments to be delegated to the head's function,
or (c) defer to a named next date with named inputs. The
substantive author of the standard is [head's level-50
architect]; the recommending party is the head."

**Solicit substantive input.** The chair invites named voting
members to speak in a considered order — typically the
functionally-adjacent member first (the CCO on a policy item,
the CDO on a data-governance item, the CISO on a security-
scoped item), then the remaining voting members. The chair
does not permit the loudest voice to dominate; the chair
names members who have not spoken and asks for their view.

**Test for decision.** The chair tests for decision explicitly.
"We have heard [named substantive positions]. Do we have
consensus to ratify with the following amendments: [named]".
Or, in formal-vote mode: "I call the vote on ratification as
amended. Voting for: [names]. Voting against: [names].
Abstaining: [names]. The motion passes / fails / is deferred
with the following inputs to the next meeting: [named]".

**Capture and close.** The secretariat records the decision
verbatim; the chair reads it back before moving on. If a
member had a substantive concern that was not fully addressed,
the chair names the dissent explicitly: "[Named member]'s
dissenting view was [summarised]; that dissent is recorded
against the decision". The item closes; the agenda moves on.

## Dissent-capture discipline

The single most audit-committee-visible feature of a well-run
council is the dissent record. Dissent is not a problem to be
managed away; dissent is the signal that the council heard
more than one view before deciding, and the record of the
dissent is what lets the audit committee, the CAE, and the
board later reconstruct why a decision was taken as it was.

Three specific disciplines.

**Named dissent on the record.** Where a voting member
dissents on a substantive decision, the dissent is recorded
with the member's name, the substantive reason (in one or two
sentences), and any specific request the dissenting member
has (a re-examination trigger, a monitoring commitment, an
escalation flag). Anonymised or aggregated dissent — "some
members expressed concern" — is not enough; the record names
the member.

**Dissent does not delay decision.** Where consensus (or
majority vote) is otherwise present, the dissent is recorded
and the decision proceeds. The dissent is not a veto. This
is what prevents the council from becoming hostage to a
single member's persistent objection; and it is what makes
dissent safe to voice, because the dissenting member is not
blocking the room's business.

**Post-hoc dissent invitation.** Where a member did not raise
dissent in the room but on reflection wishes to record one, the
chair accepts a written dissent up to a named window (typically
48 hours) that attaches to the decision in the minute. This
prevents the meeting-dynamics failure where a member could not
find the moment to voice a concern under pressure and is
denied the record because the meeting has adjourned.

**Escalation on structural dissent.** Where dissent is
persistent across meetings — the same member dissenting on the
same substantive line across multiple items — the chair
initiates a peer conversation with the dissenting member, and,
where the underlying disagreement is genuinely irresolvable at
the council, initiates an escalation to the CEO or audit
committee. The chair does not permit persistent dissent to
become political noise or to be answered by exclusion from
the council.

## Minute-keeping and decision-log discipline

Minutes are not the chair's personal notes. They are the
document-controlled record of the council's business. Four
disciplines.

**Decision log.** A separate, cumulative decision log —
distinct from the minute — carries every substantive decision
the council has taken since its founding, with the date,
the decision text, the material context, the named dissent,
and the current status (in force, superseded by a later
decision, revoked with named reason). The decision log is
the reference the audit committee reads when they want to
know "when did the enterprise decide this".

**Action-item register.** Every action item — every "the head
will deliver X by date"; "the CDO's function will report Y at
the next meeting" — is captured in a separate action-item
register with the assignee, the due date, and the status.
Action items are reviewed at the top of the next meeting as
a standing item; late items are flagged with a reason.

**Minutes.** The minutes carry the attendance record (voting
members present, invitees present, secretariat present), the
material discussion on each item (not verbatim but sufficient
to reconstruct the substantive positions), the decision taken
(referenced to the decision log entry), and the dissent
recorded. Minutes are circulated for member review within a
named window (typically 5 business days), ratified at the
next meeting under the standing "minute ratification" item,
and archived in document control.

**Document control.** The decision log, action-item register,
and minutes are stored in the enterprise's document-control
system (typically the CCO's compliance-library platform,
tied to chapter [[09-chief-compliance-officer-coordination]])
with versioning, distribution, and retention. The audit
committee's secretariat has standing access. The CAE has
standing access.

## Escalation-to-board pathway

The council's decisions do not always fit within the council's
own authority. Some material AI risks require board-level
awareness or ratification. The charter names the escalation-
to-board pathway explicitly.

Three pathways.

**Standing report to the audit committee.** The council's
decisions are surfaced at the audit committee on the
reporting cadence from [[mod-103-board-and-audit-committee-
reporting]] — typically quarterly. The head is the
substantive presenter; the CAE (as observer) may comment
on the council's discipline; the CCO (chief compliance
officer) is present for the compliance dimension. Material
decisions since the last audit-committee session are
summarised; material dissent is reported; the forward-look
of the council's next-cycle items is previewed.

**Escalation on material single decisions.** Where the
council takes (or defers) a decision the chair judges is
material enough to require audit-committee ratification
before it takes effect, the head escalates independently to
the audit-committee chair within a named window (typically
one week), with the decision, the council's rationale, and
the named dissent. The audit committee ratifies, requests
amendment, or requests the decision to be re-taken.

**Emergency escalation on material risk.** Where a matter
before the council reveals a material AI risk the enterprise
was not carrying in its risk register — a discovery-time
finding, a live incident escalating, a regulator
correspondence changing the enterprise's obligation set — the
chair escalates to the audit-committee chair within a named
window (24 to 48 hours depending on severity), independent of
the standing reporting cadence. This is the invariant that
the head retains audit-committee access on any material
second-line matter, from
[[mod-101-role-scope-and-leadership-shape]] chapter 07
engagement-contract discipline.

The escalation pathway is not a substitute for the council's
own decision authority. Most decisions the council takes are
within the council's authority; the escalation pathway
governs the specific subset where board-level ratification or
awareness is required.

## The council's own effectiveness review

The council reviews its own effectiveness at least annually.
The review is a standing agenda item (typically at the first
meeting of the calendar year or fiscal year). The review
covers:

- **Attendance discipline.** How consistently voting members
  attended. Where attendance is falling, the chair engages
  the CEO or the reporting-line executive to restore
  discipline.
- **Decision-forcing discipline.** How many agenda items
  closed with named decisions versus how many drifted to
  "discussed". A drift ratio above a threshold triggers a
  chair-led corrective.
- **Dissent-capture discipline.** How many decisions carried
  named dissent. A dissent rate of zero across a year is a
  signal the council is not surfacing dissent; the chair
  investigates whether the council is genuinely aligned or
  the meeting dynamics are suppressing dissent.
- **Action-item completion.** How consistently action items
  closed on time. A completion rate below a threshold
  triggers a review of ownership.
- **Escalation-pathway usage.** How often the council
  escalated to the audit committee — both standing and
  emergency. Zero escalations across a year with material
  events on the AI landscape is a signal the pathway is
  underused.
- **Member feedback.** A short structured feedback round from
  voting members and the secretariat on the chair's craft,
  the agenda quality, the pre-read quality, and the meeting
  discipline. The chair reads the feedback with an open
  posture and adjusts.

The effectiveness review is the discipline that keeps the
council itself honest across time. Councils that do not
review themselves degrade quietly.

## The council charter

The council's architecture is written in the charter — a
short document (5 to 10 pages) that names:

1. **Purpose.** The specific decisions the council makes and
   the decisions it does not (delegated to the head's function,
   escalated to the CEO or audit committee, held elsewhere).
2. **Membership.** Voting members, standing invitees,
   rotating attendees, secretariat. Named by role, not by
   incumbent (so the charter survives turnover).
3. **Quorum.** The threshold for substantive decisions and
   the threshold for other business.
4. **Voting model.** Consensus or formal vote, with the
   fallback rule for contested items.
5. **Written resolution.** The conditions under which written
   resolution is permitted and the required threshold.
6. **Agenda-setting authority.** The chair's authority and
   the process by which members may propose items.
7. **Pre-read discipline.** The lead time, the format, and
   the deferral rule for unprepared items.
8. **Decision-log and minute discipline.** The document-
   control location, the review-and-ratification cadence, the
   retention.
9. **Dissent-capture discipline.** The named-dissent
   convention, the 48-hour written-dissent window, the
   escalation on structural dissent.
10. **Escalation-to-board pathway.** The standing report
    cadence, the material-single-decision escalation, the
    emergency escalation.
11. **Effectiveness-review cadence.** The annual review and
    its named artefact.
12. **Charter-review cadence.** Annual charter review at the
    council itself, with material charter changes ratified at
    the audit committee.

The charter is ratified at the audit committee at inception
and at each material revision. The charter is stored in the
CCO's enterprise policy library (chapter [[09-chief-
compliance-officer-coordination]]).

## Anti-patterns the chair does not permit

**The status-meeting drift.** The council reads updates and
discusses without forcing decisions. The remedy is: every
substantive agenda item has a named decision at the top of
the item; the chair closes each item with an unambiguous
outcome before moving on.

**The unanimous decision that hid dissent.** The chair does
not test for consensus explicitly; members with concerns do
not find the moment to raise them; the minute records
"decided unanimously"; a member later writes to the audit-
committee chair with the substantive concern they never got
to voice. The remedy is: the chair tests for consensus
explicitly; the chair names members who have not spoken; the
48-hour written-dissent window is a standing safety valve.

**The wandering agenda.** Items go on the agenda without
named decisions or clear ownership; the meeting drifts; the
material items get compressed at the end and rushed. The
remedy is: the chair curates the agenda; every item has a
named decision or a named informational outcome; the timings
are named and the chair holds them.

**The chair-as-author.** The chair is the substantive author
on every item and the ratifying authority; the council
becomes a rubber-stamp for the chair's own decisions. The
remedy is: the chair distinguishes the chair-role (agenda,
discipline, decision-forcing, dissent capture) from the head-
role (substantive author on AI-governance items); where the
chair is also the substantive author, the chair explicitly
frames the item as "the head is recommending X; the council
is asked to ratify, amend, or defer" and steps back from
advocacy during the deliberation.

**The minute as the chair's notes.** The minute is drafted by
the chair from personal notes, circulated informally,
ratified without member review. The record cannot be trusted;
the audit committee's read is compromised. The remedy is: the
secretariat drafts the minute; the minute is circulated for
member review within the standing window; the minute is
ratified at the next meeting under a standing item.

**The improvised escalation.** A material AI risk surfaces at
the council; the chair does not know whether to escalate
independently, wait for the standing report, or defer; the
escalation is improvised in the moment. The remedy is: the
charter names the three escalation pathways; the chair
selects and executes without improvisation.

**The council that has never reviewed itself.** No annual
effectiveness review; no attendance discipline; no dissent-
capture check; the council degrades and the chair does not
see it until the CAE surfaces the finding. The remedy is: the
effectiveness review is a standing item on the annual first
meeting; the review's outputs are the chair's own performance
inputs.

## Where the discipline earns its keep — the contested policy
## ratification

The load-bearing test of the chair's craft is the contested
policy ratification. The head has brought the AI Third-Party
Standard v1.3 for ratification. The changes from v1.2 include
a new evidence-depth requirement for high-risk vendors that
the CDO's third-party function warns is operationally onerous
and the GC warns is difficult to enforce contractually in
some jurisdictions. Two voting members are prepared to dissent
if the standard is ratified as drafted.

If the chair's craft is working, the following happens: the
pre-read circulates five business days ahead with the material
changes named; the CDO's substantive concern and the GC's
substantive concern are documented in the pre-read; the chair
opens the item with the decision framed (ratify, amend, or
defer); the chair invites the functionally-adjacent members
first (CDO, GC); the chair invites the remaining voting
members; the chair proposes an amendment — the evidence-depth
requirement is retained with a named phased-implementation
schedule that the CDO's function co-authors with the head's
level-50 architect; the chair tests for consensus; consensus
is present with the CDO and GC's concerns addressed by the
amendment; two members who had reservations record named
dissent on specific residual concerns (the enforceability of
the contractual language in one named jurisdiction); the
decision is taken, the dissent is recorded, and the amendment
is captured in the decision log with a named next-review date;
the action item goes to the head's function to update the
standard by a named date and circulate for member sign-off
under written resolution.

If the chair's craft is not working, one of the anti-patterns
above surfaces: the CDO and GC's substantive concerns are not
heard because the chair rushed the item; the standard is
ratified as drafted with the concerns unaddressed; two members
write to the audit-committee chair with dissent that was never
recorded; the standard proves unenforceable in the named
jurisdiction six months later and the CAE surfaces both the
substantive finding and the process finding at the audit
committee.

## Composition with adjacent modules

- The **CxO adjacency map** in
  [[mod-101-role-scope-and-leadership-shape]] chapter 06 is
  the parent boundary document; the council operationalises
  the map through standing decisions.
- The **AIMS operating calendar** in
  [[mod-102-running-the-program]] chapter 02 sets the
  council's meeting cadence and the rotation of standing
  agenda items.
- The **AI policy taxonomy** in chapter
  [[09-chief-compliance-officer-coordination]] is the set of
  policies the council ratifies and re-ratifies on the
  library's lifecycle.
- The **audit-committee reporting cluster** in
  [[mod-103-board-and-audit-committee-reporting]] is the
  forum the escalation-to-board pathway feeds into.
- The **regulatory-change discipline** in
  [[mod-105-regulatory-change-management]] is the source of
  the horizon-scanning items on the standing agenda.
- The **KRI / KPI portfolio** in
  [[mod-107-program-measurement-and-maturity]] chapter 01 is
  the dashboard the council reviews on its standing
  metrics item.
- The **incident-leadership discipline** in
  [[mod-110-incident-leadership]] is where the council is
  activated for material AI incidents in the after-action
  and remediation-ratification phases.

## Summary

- The AI Governance Council is a decision-forcing forum, not
  a status meeting. Every substantive agenda item has a named
  decision; every item closes with an unambiguous outcome
  before moving on.
- Four architectural decisions carry the council: membership
  (voting, standing invitees, rotating attendees,
  secretariat), quorum, voting model (consensus or formal
  vote), and written-resolution rules for out-of-cycle
  decisions.
- Agenda-setting discipline: standing items and rotating
  items on the AIMS operating cadence; every substantive item
  names a decision; pre-read discipline with a named lead
  time and a deferral rule for unprepared items.
- Decision-forcing discipline: frame the decision, solicit
  substantive input in a considered order, test for decision
  explicitly, capture and close before moving on.
- Dissent-capture discipline: named dissent on the record,
  dissent does not delay decision, 48-hour written-dissent
  window, escalation on structural dissent.
- Minute-keeping and decision-log discipline: separate
  decision log, action-item register, minutes drafted by
  secretariat and ratified at the next meeting, document
  control with CAE and audit-committee-secretariat access.
- Escalation-to-board pathway: standing report cadence,
  material-single-decision escalation, emergency escalation
  on material risk.
- Effectiveness-review cadence: annual review of the
  council's own discipline against attendance, decision-
  forcing, dissent-capture, action-item completion,
  escalation-pathway usage, and member feedback.
- Seven anti-patterns to refuse: status-meeting drift,
  unanimous-decision-that-hid-dissent, wandering agenda,
  chair-as-author, minute-as-chair's-notes, improvised
  escalation, and the council that has never reviewed itself.
- The charter (5 to 10 pages) is ratified at the audit
  committee at inception and each material revision, and is
  stored in the CCO's enterprise policy library.
- Chapter [[12-product-conflict-management]] turns to the
  head's *conflict pattern* with product owners — stop-ship,
  delayed-release, and feature-scope-reduction decisions —
  and the escalation ladder that keeps the conflict on
  merits rather than politics.
