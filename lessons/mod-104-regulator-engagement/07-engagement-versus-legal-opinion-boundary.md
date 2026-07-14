# Engagement Versus Legal Opinion — the General Counsel Boundary

## Motivation

There are two boundaries a head of AI governance most frequently gets
wrong. One is the head-and-CRO boundary — where enterprise risk
ownership stops and program ownership begins — covered in
[[mod-101-role-scope-and-leadership-shape]] chapter 06 and revisited
in [[mod-103-board-and-audit-committee-reporting]] chapter 04. The
other is the head-and-General-Counsel boundary, and it is the one
this chapter closes the module with, because every prior chapter of
mod-104 has quietly assumed the hand-off works.

The failure modes are recognisable. A head takes a legal position
they are not qualified to take — a written characterisation of what a
statute *means* rather than what the enterprise *does* about it —
and creates legal exposure the enterprise did not agree to accept. A
head defers to GC on a technical position they should own — what the
system does, how the enterprise knows, what the safeguards are — and
loses regulator credibility the moment a career staff examiner
figures out the person in the chair cannot answer their own
questions. Or, worst, head and GC give different answers to the
same regulator on the same day, because they never sat down and
agreed which one of them owns which sentence.

None of these are recoverable in the moment. All of them are
avoidable with a boundary discipline that both parties rehearsed
before the interaction. This chapter is that discipline.

The reference frame is the IIA Three Lines Model (2020), which
places General Counsel as an assurance and advisory function to the
first and second lines rather than as a first-line operator, and the
ABA Model Rules of Professional Conduct, which govern what a legal
"opinion" formally is when a lawyer delivers one to a client. The
head is not a lawyer, does not deliver opinions, and does not want
to be mistaken for one.
<!-- needs-research: verify ABA Model Rule reference for the
     formal definition of a legal opinion (Rule 2.1 Advisor;
     Rule 2.3 Evaluation for Use by Third Persons) against the
     current ABA Model Rules text. -->

## Core concept — the four-quadrant map

Every regulator interaction the head is involved in fits into one of
four quadrants. The axes are *what kind of position is being taken*
(technical or legal) and *what kind of exposure the interaction
creates* (operational or legal / litigation). The map does not
resolve every edge case, but it resolves the ones that generate
same-day disagreements.

| Quadrant | Nature | Owner | Head's artefact | GC's artefact |
|---|---|---|---|---|
| Q1 | Technical position, no legal exposure | Head | The response | (none) |
| Q2 | Technical position with legal exposure | Head, framed by GC | The technical response | Framing review; privilege cover |
| Q3 | Legal position on technical facts | GC | Technical fact brief; ratification of GC's characterisation | The legal opinion |
| Q4 | Litigation posture / adverse action | GC end-to-end | Witness statement; evidence; briefing input | The pleading, settlement position, or defence |

A useful rehearsal for the head is: for every scheduled regulator
touch in the next quarter, name the quadrant before naming the
authoring team. If nobody can name the quadrant, the interaction is
not ready to happen.

## Walking the quadrants

### Q1 — technical position, no legal exposure

Example. The AI Safety Institute (or a peer national body — AISI UK,
US AISI, Singapore's AI Verify Foundation, etc.) asks the enterprise
to share an evaluation methodology for a specific capability tier, as
part of a voluntary evaluation-sharing programme. There is no
statute in play, no enforcement power in the interaction, no
disclosure that would move the enterprise's legal position. The
regulator wants the *technical artefact*.

The head owns this end-to-end. The artefact is a technical write-up
of the evaluation methodology, the datasets used, the thresholds,
the reasoning for the choices, and the observed results. GC is
notified for awareness — because any external disclosure needs to be
inventoried — but GC is not on the drafting team. If the head
routes a Q1 interaction through GC for authoring, the head has
signalled to their own function and to GC that the head does not
trust their technical staff to speak for themselves. Chapter 03 of
this module covers the AISI engagement in operational detail.

### Q2 — technical position with legal exposure

Example. An Article 73 serious-incident filing under the EU AI Act.
The substance of the filing is technical — what the system did, what
the enterprise detected, when, what containment was applied, what
the residual harm looks like. But the filing itself is a mandatory
regulatory disclosure with statutory triggers, and every word in it
will be read against the statute by the national competent
authority, potentially by a court, and by counterparties.

The head authors the substance. GC reviews the framing — the
sequencing of factual statements, the choice between "identified"
and "detected", the placement of any determination language, the
handling of causation attribution, and the assertion of privilege
where an internal investigation is ongoing. The head signs (chapter
02 of this module is explicit that signature does not delegate). GC
does not sign. The two artefacts are (a) the filing, signed by the
head, and (b) an internal GC memo covering the framing review and
any preserved privilege, held by GC.

### Q3 — legal position on technical facts

Example. A CPPA (California Privacy Protection Agency) rulemaking
notice invites written submissions on how proposed automated
decision-making regulations should treat a specific class of
enterprise system. The submission is not merely descriptive. The
enterprise is being asked to take a position on statutory
interpretation — what the words of the proposed rule ought to mean
in context.

GC delivers the opinion. The head produces two upstream artefacts:
a technical fact brief that gives GC the ground truth about how the
enterprise's systems actually operate, and a ratification memo in
which the head confirms that GC's characterisation of those facts is
accurate. The submission itself is signed by GC (or by the enterprise
via GC's authoring), not by the head. If the submission touches
technical claims the head has not ratified, the head does not let it
go out — and this is a boundary GC will respect if the head raises
it early, not late.

### Q4 — litigation posture / adverse regulatory action

Example. A sector regulator issues a Matter Requiring Attention
(MRA) or a formal supervisory letter naming a specific AI system and
alleging a specific inadequacy in the enterprise's governance of it.
The remediation plan the enterprise files in response is a legal
instrument. The follow-on may include a consent order or an
enforcement action.

GC owns end-to-end. The head is a witness — the person who briefed
the remediation team, the person who signed the internal
attestation about the prior state, the person who will be deposed if
this escalates. The head produces evidence and briefings; the head
does not sign anything to the regulator in this quadrant that GC has
not authored or explicitly co-signed. The temptation, in a Q4
matter, is for the head to want to fix the relationship personally.
The discipline is that the relationship is now in the litigation
posture and repair happens on GC's timeline, not the head's.

## The packaging discipline

Between Q2 and Q3 there is a discipline that is easy to under-invest
in and that everything else in this chapter depends on. The head
*packages* regulator obligations for GC. Packaging is neither
lay-legal-analysis (which is out of scope) nor mechanical forwarding
(which is a waste of GC's time and a signal that the head does not
know what the enterprise does). Packaging is the technical-position
work that only the head is uniquely qualified to do.

A well-packaged obligation, delivered from the head to GC, has five
components:

1. **A plain-English summary of what the regulation requires.** The
   head has read the statute or the regulation and can state, in
   two or three sentences, what the obligation is in operational
   terms. Not what it *means* in legal terms — what it *requires*
   the enterprise to do.
2. **The attachment analysis.** The head names the specific systems,
   decisions, actors, business lines, or data flows within the
   enterprise the obligation attaches to. If the obligation is
   scoped to "high-risk" systems, the head names which systems in
   the inventory fall inside and which fall outside, with the
   classification reasoning.
3. **A technical-feasibility assessment.** For each attachment
   point, the head names what the enterprise can technically do to
   comply, what the enterprise cannot yet do, and what the delta
   would take to close.
4. **An operational-cost assessment.** The head brings a defensible
   estimate of what compliance would cost — engineering effort,
   run-cost, vendor spend, opportunity cost from feature scope
   reduction. This is the input GC needs to weigh whether an
   argument for narrower attachment is worth the enforcement risk.
5. **The question for GC.** The head asks GC a specific question:
   does the obligation attach in this way, on these facts, and
   what defences would the enterprise have if a regulator disagreed
   with the attachment analysis. GC's answer is the opinion.

The head then takes GC's interpretation into the running program as
an operational requirement. The head does *not* re-litigate GC's
opinion inside the program, and does not amend it in later
briefings. If the head disagrees with GC's opinion, the disagreement
runs through the disagreement discipline below, not through a
softened restatement in a policy document.

## The technical-position discipline

The mirror of packaging is the discipline of taking a technical
position and holding it. There are questions a regulator will ask
the head that GC should not answer alone, because GC does not have
the standing to answer them. The head is the qualified voice; GC
signs off on framing and privilege, but the substance is the head's.

These are the questions:

- **What does this system do?** The head describes the system in
  operational terms, at the level of specificity the regulator asked
  for. Not the marketing description, not the model card excerpt —
  the technical-operational description the enterprise's own
  engineers would recognise.
- **How did we know?** The head describes the evaluation, monitoring,
  detection, or attestation evidence that gives the enterprise
  confidence in its own claims. This is where the AIMS earns its
  keep — the head has evidence to point to because the program
  produced it.
- **What safeguards are in place?** The head describes the technical
  and organisational controls that reduce the risk, and — this is
  the credibility test — the head can describe what those safeguards
  do not cover.
- **What have we changed since a prior finding?** The head describes
  the remediation, the evidence that it took effect, and the
  monitoring that will detect regression.
- **What is our own view of residual risk?** The head takes a
  technical position on what risk remains after safeguards, with the
  reasoning. Regulators respect a head who names residual risk with
  a straight face; regulators do not respect the "there is no risk"
  answer, which nobody believes anyway.

If the head cannot answer these, the head has a program problem, not
a boundary problem. If GC answers these on the head's behalf, the
head has a positioning problem.

## The disagreement discipline

Head and GC will disagree on framing. It is a healthy sign — the two
functions are pulling from different training and different
incentives, and the friction is doing useful work. The discipline is
in how the disagreement is resolved, not in avoiding it.

- **Escalate to a scheduled joint session, not a rushed hallway
  call.** The stakes of a regulator-facing disagreement are too high
  to resolve on the way to the meeting. The head asks for time on
  GC's calendar with named attendees and a written statement of the
  disagreement.
- **Document the disagreement and the resolution.** The internal
  record captures what the head proposed, what GC proposed, the
  rationale each side gave, and the resolution reached. If the
  disagreement is material, brief the audit-committee chair (see
  [[mod-103-board-and-audit-committee-reporting]] chapter 04 on
  CxO sign-off flow). This documentation is protective for both
  functions if the interaction is later reconstructed.
- **Never present a disagreement to a regulator.** Internal
  disagreement is internal. A regulator who detects a split answer
  from head and GC treats it as a governance failure and expands
  scope on that basis. If a resolution has not been reached before
  the interaction, the interaction is postponed.
- **Where the disagreement cannot be resolved and the matter is
  time-critical**, the default rule is that GC's view prevails on
  legal interpretation and the head's view prevails on technical
  fact. Mixed cases — where a legal interpretation depends on a
  contested technical characterisation — escalate to the CEO with
  both positions written down and the trade-off named. The head
  does not resolve mixed cases alone and does not let GC resolve
  them alone.

The disagreement discipline is where the boundary is actually
tested. A head who has never disagreed with GC on framing has either
a very simple regulatory profile or a boundary that is doing no
work.

## Adjacent boundaries

The head-and-GC boundary is the most-tested, but not the only one
that shows up in regulator engagement. Four adjacent boundaries
deserve naming, because failing to distinguish them is another
mode of the same class of failure.

- **Government Affairs.** GA owns the political-relationship layer
  with regulator leadership — chairs, commissioners, appointed
  officials — as distinct from career staff. When the head is
  arranging a meeting with a commissioner rather than with a
  supervision team, GA is co-ordinating the calendar, not the head.
  See [[mod-101-role-scope-and-leadership-shape]] chapter 06 for
  the CxO adjacency map that names this split.
- **Communications.** External-facing statements about a regulator
  interaction — a press release acknowledging a filing, a response
  to a media enquiry about an enforcement matter, a proactive
  disclosure — belong to Communications, not to the head. The head
  provides the substance; Communications owns the news-cycle
  relationship. The regulator is not the news cycle.
- **Investor Relations.** When a regulator interaction is material
  to shareholders (a consent order, a large civil penalty, a stayed
  product launch), IR owns the disclosure discipline under the
  applicable securities regime. The head briefs IR on materiality
  inputs; IR (with GC and the CFO) decides on disclosure timing and
  wording.
- **CISO.** Cyber-adjacent regulator engagement — CISA in the US,
  NCSC in the UK, national cyber authorities elsewhere — is
  primarily the CISO's relationship. When an AI-security incident
  crosses into that regime (a model-weight exfiltration, a
  prompt-injection incident with data-exposure consequences, a
  red-team finding with public disclosure obligations), the head
  co-ordinates on the AI-specific overlay but does not front the
  primary relationship. See [[mod-110-incident-leadership]] for the
  wider incident-leadership hand-off pattern.

## The one-sentence summary

If the head has to compress this boundary to one sentence for a new
peer, a new board member, or a new GC: *engagement is what the head
does; a legal opinion is what General Counsel delivers, and the head
does not deliver legal opinions.* The four-quadrant map, the
packaging discipline, the technical-position discipline, and the
disagreement discipline are all in service of that sentence.

## Summary

- The head-and-GC boundary is one of the two boundaries the role
  most frequently gets wrong; the other is the head-and-CRO
  boundary in [[mod-101-role-scope-and-leadership-shape]] chapter
  06 and [[mod-103-board-and-audit-committee-reporting]] chapter 04.
- Every regulator interaction fits one of four quadrants: technical
  no-exposure (head owns), technical with legal exposure (head
  authors, GC frames), legal on technical facts (GC opines, head
  ratifies facts), litigation posture (GC end-to-end, head as
  witness).
- Packaging obligations for GC is a five-component discipline: plain
  summary, attachment analysis, technical feasibility, operational
  cost, and the specific question for GC. It is not lay-legal
  analysis and it is not mechanical forwarding.
- The head takes technical positions on what the system does, how
  the enterprise knows, what safeguards exist, what has changed, and
  what residual risk remains. GC covers framing and privilege.
- Disagreement is resolved in scheduled joint session, documented
  internally, and never presented to a regulator. Time-critical
  unresolved disagreement defaults to GC on interpretation, head on
  technical fact, and CEO on mixed cases.
- Adjacent boundaries — Government Affairs, Communications, Investor
  Relations, CISO — apply the same pattern: the head provides
  substance, another function owns the primary relationship.
- The one-sentence compression: engagement is what the head does;
  a legal opinion is what General Counsel delivers, and the head
  does not deliver legal opinions.
