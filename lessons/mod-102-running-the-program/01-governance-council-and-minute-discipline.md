# Chairing the AI Governance Council and Adjacent Committee Cadences

## Motivation

The AI governance council is where the head of AI governance either
becomes an executive or becomes a coordinator with a fancy title. A
council that meets, discusses, and disperses without decisions is a
staff meeting; a council that produces dated decisions, named owners,
tracked actions, and traceable minutes is a governing body. The
difference is not personality. The difference is *cadence, agenda
discipline, and minute-keeping* — the mechanics the head owns.

The head does not just chair the AI governance council. The head is
also the second-line voice at the audit committee, the risk committee,
the technology committee (where one exists), and the executive
committee's AI standing item. Each of those bodies has its own charter,
its own quorum, its own minute-taking convention, and its own
document-retention obligation. Getting one of them wrong — a decision
recorded ambiguously, a quorum missed, an escalation not booked into
the next up-committee cycle — is how a defensible program becomes an
audit finding.

This chapter is how to run the council the level-50 architect chartered,
and how to interface to the four adjacent committees without dropping a
stitch.

## Core concept: the council is a governing body, not a working group

The level-50 architect (see the mod-101 level-ladder chapter) delivered
the operating model — the RACI, the council charter, the cadence, the
escalation paths. The head *runs* the council under that charter. The
distinction the head must hold in their head at all times is:

- A **working group** produces recommendations, options, and analysis.
  It does not decide, it does not commit resources, and its output is
  input to a decision-maker somewhere else.
- A **governing body** decides. It commits resources, sets appetite,
  approves policies, ratifies exceptions, and its minutes are the
  audit trail regulators, third-line auditors, and ISO/IEC 42001
  certification bodies read.

The AI governance council is a governing body. Its charter names the
decisions it takes (policy approval, appetite ratification, exception
approval, escalation acceptance, incident containment approval,
release-gate escalations) and the decisions it *does not* take
(strategy, portfolio P&L, personnel — those live above; engineering
methodology, control implementation — those live below). Running the
council means holding that boundary agenda by agenda.

## The council's operating skeleton

A defensible AI governance council operates on a monthly primary
cadence with the following invariants. The specific numbers vary by
enterprise; the invariants do not.

- **Quorum and voting.** A named quorum threshold (typically simple
  majority of voting members, with a fixed floor — e.g. "no fewer than
  five voting members present, including at least one of head, CRO
  delegate, GC delegate"). Whether decisions are consensus,
  simple-majority, or head-with-veto-and-appeal. Whether attendance by
  delegation is permitted and whom a delegate may bind.
- **Voting members and standing attendees.** Voting members are the
  people whose accountability is on the record for the decision.
  Standing attendees are advisory — CAE observer, external counsel on
  standing invitation, CISO's AI-security lead, and so on. Everyone
  present is named in the minutes; everyone who voted is named
  separately.
- **Standing agenda.** A fixed structure so the same categories are
  visited every cycle and drift is visible. A workable structure:
  1. Approval of previous minutes.
  2. Action-tracker review (open, closed-since-last, aged, escalated).
  3. AIMS operating-calendar dashboard (audit round status, management
     review preparation, non-conformity closure ageing, competence
     assessment ageing).
  4. Portfolio risk register — new-since-last, appetite deviations,
     escalation triggers, closed risks with root cause.
  5. Incident-and-near-miss review.
  6. Third-party evidence review — vendor onboardings, tier-1
     continuous-monitoring exceptions, terminations.
  7. Release-decision escalations from the release-assurance function
     (level 35).
  8. Policy exceptions and waivers requested / expiring / breached.
  9. Regulator engagement summary (correspondence in the period).
  10. External positioning items requiring council approval
      (voluntary-code sign-ons, consultation submissions).
  11. Standing risks (a rolling five to seven risks the council has
      resolved to revisit every meeting until closed).
  12. AOB and forward calendar.
- **Timeboxing.** Every agenda item has a book-ahead timebox. Items
  that consume their timebox without decision are either escalated,
  deferred with a named owner and a next-meeting date, or ratified as
  "no change, revisit at [date]". They do not linger without a verb.
- **Pre-read discipline.** No item without a pre-read older than the
  timebox required to read it. A ten-page pre-read for a ten-minute
  decision fails the discipline. If it is not written down, it is not
  on the agenda; if it is not read, the decision is deferred.
- **Written-decision discipline.** Every decision is recorded as
  *decision + rationale + owner + date + expiry-or-review-trigger*.
  A decision without an expiry-or-review trigger is not a decision;
  it is an intention.

The council chair — the head — owns all six invariants.

## Chairing behaviour: what the head does at the head of the table

Two chairing habits distinguish a governing body from a working
group.

First, **the chair states the question**. Before discussion opens on
any agenda item, the chair reads aloud (or restates in their own words)
the specific question the council is being asked to decide. Not "let's
discuss the vendor issue" — "the council is asked to decide whether to
accept vendor X's post-remediation attestation as sufficient to move
the vendor from suspended-tier-1 back to tier-1, or to require an
additional independent evaluation before reinstatement." Ambiguity in
the question is ambiguity in the decision, and ambiguity in the
decision is the audit finding.

Second, **the chair closes the question**. Before moving on, the chair
reads back the decision, the rationale, the owner, and the review
trigger. If any voting member objects to the read-back's accuracy,
that objection is captured in the minutes. Decisions that cannot be
read back are re-opened, re-drafted, or deferred with an owner. The
chair does not permit the meeting to move on with an ambiguous
decision on the record.

The head runs the meeting so that a person who joined halfway
through, or reads the minutes six months later, or is an
ISO/IEC 42006 auditor sampling the minutes two years later, can tell
exactly what was decided, by whom, on what evidence, and when it will
be revisited.

## Minute-keeping discipline the certification body will inspect

Minutes are the primary audit-trail artefact of the council. Under
ISO/IEC 42001 the AIMS is expected to keep documented information;
under ISO/IEC 42006 a certification body inspects that documented
information for evidence of top-management commitment, management
review, and continual improvement. Minutes are how that inspection
succeeds or fails.

A defensible minute template contains, per item:

- **Item ID** — a monotonic identifier so the minute is referenceable
  elsewhere (a decision log, an action tracker, a control-evidence
  attachment). Do not restart numbering per meeting; use
  `AIGC-YYYY-NNN` or equivalent.
- **Item title** — one line.
- **Category** — policy approval / exception / risk-appetite change /
  escalation acceptance / incident / third-party / release-gate /
  regulator / external-positioning / other.
- **Presenting owner** — the person who brought the item.
- **Pre-read reference** — document control number and revision of the
  paper the council read.
- **Question stated** — the exact question the council was asked to
  decide.
- **Discussion summary** — three to eight lines, non-attributive
  unless attribution is material.
- **Decision** — the exact wording of the decision.
- **Vote record** — voting members named, abstentions noted, dissent
  captured in the words of the dissenter.
- **Owner and review trigger** — the person accountable for the
  decision's execution and the date or event at which the council
  revisits.
- **Cross-references** — related risks, controls, incidents, or open
  actions.

Minutes are drafted by a named secretariat, reviewed by the chair
before circulation, circulated to members within a fixed window (five
business days is typical), and approved at the following meeting.
Approved minutes are locked. Amendments after approval are recorded as
errata with the reason. That last discipline — no silent edits to
approved minutes — is what a certification body will test by sampling.

## The four adjacent committees the head interfaces to

Beyond chairing the AI governance council, the head is a *reporting-in
voice* to four adjacent bodies. Each has a different mandate and a
different audit-trail expectation.

- **Audit committee.** The board's audit committee is the ultimate
  oversight body for the AIMS, the AI risk framework, and third-line
  audit findings related to AI. The head appears on the audit
  committee's calendar at a defined cadence (quarterly is common,
  monthly for heavily regulated enterprises), presents the AI risk
  register at portfolio scope, reports on audit-round findings and
  closure, and takes escalations back down. See
  [[mod-103-board-and-audit-committee-reporting]] for the pack
  authoring discipline.
- **Enterprise risk committee.** Under the CRO. The head takes AI
  risks that cross AI-family scope or interact with the parent
  enterprise risk taxonomy (operational risk, technology risk, credit
  risk in banking, actuarial risk in insurance, patient-safety risk
  in health) into the enterprise risk committee. Escalations from the
  AI governance council with parent-enterprise-risk implications
  land here.
- **Technology committee.** Under the CIO / CTO / CDO stack, where it
  exists. Interfaces to build-versus-buy decisions on AI platforms,
  the choice of the GRC-for-AI platform, and enterprise engineering
  standards that compose with the AI control library. The head brings
  the AI supply-chain evidence discipline into scope here and takes
  engineering-standard implications back.
- **Executive committee AI standing item.** Under the CEO. Where a
  Chief AI Officer designation exists, the head reports through the
  CAIO; where it does not, the head reports directly on the standing
  item. The purpose is not deep-dive risk analysis; it is executive
  visibility of the top three to five AI-risk items and the two or
  three cross-CxO issues that need coordination.

The head does not attend all four with the same pack. Each committee's
charter constrains what is in scope. The head owns knowing which paper
lands with which committee, in what depth, in what timeframe. That
mapping is a document — the head's committee interface map — that
lives in the AIMS document control.

## Escalation choreography — up, down, and sideways

Escalations from the AI governance council go up to (typically) the
audit committee or the executive committee, and down to (typically) the
control-library owner (level-50 architect) or the release-assurance
owner (level-35 evaluation engineer) for execution. Sideways
escalations — to CRO, CCO, CPO / DPO, GC, CISO — are also common.

A defensible escalation record contains: the originating council
decision reference, the destination body, the specific ask, the
by-when, the owner accountable for the destination-body follow-through,
and the loop-close mechanism (how the head knows the destination body
took the ask). Without a loop-close, escalations become sinkholes and
the council loses authority.

An underappreciated escalation is *sideways to the CAE*. Under the
IIA Three Lines Model the third line is independent — the head does
not direct it — but the head can and should formally request that a
matter be considered for third-line audit inclusion. That written
request is itself an artefact the audit committee expects to see; it
is how the second line signals to the third that a topic warrants
independent assurance without violating third-line independence.

## Example — a policy-exception decision, minute-shaped

A worked example. The council is asked to approve an exception to the
enterprise AI policy allowing the marketing team to deploy a
third-party generative model to draft social-media copy without a
formal impact assessment, for a 60-day pilot.

The chair states the question: *the council is asked to decide whether
to grant a 60-day exception to policy AI-POL-001 s.4.3 (impact
assessment required prior to production deployment of any
customer-facing generative model), scoped to the marketing team's
social-copy drafting use, subject to compensating controls X, Y, Z*.

Discussion surfaces: the compensating controls (a human-in-the-loop
approval gate, a content policy filter, no PII in inputs) are
adequate; the 60-day window is longer than the four-week impact
assessment would take; the CPO delegate objects on grounds that
brand-safety risk is under-analysed.

The chair reads the decision back: *exception approved with three
amendments: window shortened to 30 days; compensating controls
extended to include a daily human-review sample; brand-safety concern
recorded as a standing risk for the next meeting. Owner: head of
marketing operations. Review trigger: 30 days from today or
immediately on any incident. Dissent: CPO delegate on
brand-safety grounds.*

Minutes reference item `AIGC-2026-047`, pre-read `AIP-EXCEPT-0047 rev
2`, standing risk `AIR-SR-013 (brand safety on GenAI-drafted
content)`, and the follow-through action `ACT-2026-091 (30-day
review)`.

That minute survives an audit-committee challenge, a CAE sample, and
a certification-body inspection. The exception is bounded, owned,
loop-closed, and traceable. That is the shape.

## Summary

- The AI governance council is a *governing body*, not a working
  group; the head runs it under the level-50 architect's charter with
  the specific discipline of quorum, standing agenda, timeboxing,
  pre-read, and written decisions.
- The chair states the question before discussion and reads back the
  decision before moving on; ambiguity in either is the audit
  finding.
- Minutes are the primary AIMS audit-trail artefact; they are drafted
  by a named secretariat, chair-reviewed, member-approved, locked,
  and errata-tracked — never silently edited.
- Four adjacent committees (audit, enterprise risk, technology,
  executive) receive the head's paper on differing cadences and in
  differing depths; the head owns the committee interface map that
  makes those interfaces predictable.
- Escalations always specify the destination body, ask, by-when,
  owner, and loop-close; sideways written requests to the CAE are
  first-class artefacts that preserve third-line independence while
  signalling assurance interest.
