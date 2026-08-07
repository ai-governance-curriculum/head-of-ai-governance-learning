# The Voluntary-Code Sign-on Decision Process

## Motivation

A voluntary code is not a regulation the enterprise has to comply
with. It is a public commitment the enterprise elects to take on,
in a form third parties can measure the enterprise against for the
life of the commitment. That distinction is what makes the sign-on
decision harder than a regulatory-compliance decision, not easier.

For a regulation, the head's question is *how do we comply*. For a
voluntary code, the head has to answer four questions the
enterprise does not get to skip: *should we sign, what do we
commit to when we sign, who inside the enterprise signs off on
signing, and what happens if we later have to withdraw*. None of
the four is a legal question — GC advises, GC does not decide.
The head is the accountable executive for the answer, and the CEO,
CRO, and CFO are on the accountable-sign-off ledger for the answer
the head recommends.

The failure mode this chapter opens with is not signing something
the enterprise cannot live up to. It is *signing without process*
— an executive team's press-release-ready move that skipped the
architect's attachment analysis, the CRO's appetite check, the
CFO's cost estimate, and GC's exposure read. The public commitment
lands, the operating gap is discovered six months later, and the
enterprise either quietly under-delivers (the reputational failure
mode) or publicly withdraws (the credibility failure mode). Both
are avoidable. Neither is avoided by refusing to sign; both are
avoided by refusing to sign *without process*.

This chapter builds the sign-on decision process. Chapter 02
carries the same discipline over to standards-body participation.
Chapter 03 covers the public-trust posture the sign-on decisions
feed. Chapter 05 rehearses the harder decisions — declining and
withdrawing.

## Core concept — the voluntary-code portfolio

The head does not decide sign-on code by code. The head runs a
*portfolio*, and every code the enterprise has heard of sits in
one of four states.

- **Signed and active.** The enterprise is a public signatory or
  member. The commitments are named, the operating owner is
  named, the evidence-production discipline is running, and the
  code is on the audit-committee reporting cadence
  ([[mod-103-board-and-audit-committee-reporting]] cluster 4-
  adjacent).
- **Considered and declined, with recorded rationale.** The
  enterprise has considered signing and, at a specific date, on a
  specific written rationale, decided not to. Chapter 05 covers
  how to defend a decline that later attracts external questioning.
- **Under active consideration.** The sign-on decision is in the
  head's pipeline; the artefacts described below are being
  authored; a decision date is on the calendar.
- **Watched.** The code exists and the head tracks it, but no
  sign-on decision is in scope. The regulatory-change discipline
  in [[mod-105-regulatory-change-management]] chapter 01 owns the
  watch tier.

Every code the head is aware of is in exactly one of the four
states, and the state is recorded. A code the enterprise "will
think about later" is either at watch or under active
consideration — the head does not run an undifferentiated
"unknown" tier. Regulators, journalists, and industry peers who
ask "did the enterprise consider signing X" get the answer from
the register, not from the head's memory.

## The standing voluntary-code portfolio the head considers

The bodies below are the current landscape as of the research
window. New surfaces will appear; retired surfaces will drop off.
The list is what the head defends at an audit committee if asked
"what codes has the enterprise considered".

### EU AI Office — General-Purpose AI Code of Practice

The GPAI Code of Practice is the Commission-convened,
multi-stakeholder code developed by the EU AI Office under Article
56 of Regulation (EU) 2024/1689. Signatory GPAI providers can use
adherence to the Code as evidence of compliance with the Article
53 (transparency) and Article 55 (systemic-risk) obligations that
apply to general-purpose AI model providers.
<!-- needs-research: verify the current published version and
signatory roster of the EU AI Office's GPAI Code of Practice
against digital-strategy.ec.europa.eu/en/policies/ai-code-practice.
Confirm the specific Article 56 mechanism by which adherence
substantiates compliance with Articles 53 and 55, and the current
list of signatories. -->

The Code is not neutral for an enterprise that provides GPAI
models. Article 55 obligations for providers of GPAI models with
systemic risk are substantial; the Code is the negotiated, ready-
to-run version of what "compliance" looks like. An enterprise that
declines the Code has to build its own defensible compliance
posture from the Article 55 text, without the presumption the Code
provides. That is possible; it is expensive; and it may be
adversarial vis-à-vis the AI Office in a way the enterprise did
not intend.

For enterprises that are *deployers* of GPAI models, not
providers, the Code is not the enterprise's to sign — but the
Code's content matters because it shapes what the enterprise's
GPAI-provider suppliers commit to, which flows into the
enterprise's own supply-chain evidence discipline
([[mod-102-running-the-program]] chapter 07).

### G7 Hiroshima Process — International Code of Conduct

The G7 Hiroshima Process International Code of Conduct for
Organisations Developing Advanced AI Systems was published in
October 2023 as the operational annex to the Hiroshima Process
Guiding Principles. It is a voluntary code addressed to
organisations developing "advanced AI systems" (frontier-model
scope, deliberately). Enterprises endorse the Code publicly; the
OECD.AI observatory hosts a monitoring reporting framework the
signatories report against on a periodic cadence.
<!-- needs-research: verify the current signatory roster of the G7
Hiroshima Code of Conduct and the current cadence and format of
the OECD.AI monitoring reports the signatories submit. Confirm the
current status of the Hiroshima Process AI Reporting Framework. -->

The Code is a lighter-touch instrument than the EU GPAI Code —
narrative rather than measurable — but its public-facing
commitments (transparency reporting, incident sharing, red-teaming
disclosure) are testable enough that a signatory that does not run
them is visibly not running them.

### White House Voluntary AI Commitments

The July and September 2023 White House Voluntary AI Commitments
were signed by an initial group of AI companies and expanded to a
further wave. The Commitments cover safety testing, information
sharing, security investment, watermarking research, and public
reporting.
<!-- needs-research: verify the current status of the White House
Voluntary AI Commitments given that Executive Order 14110 was
rescinded by Executive Order 14179 in January 2025. Confirm
whether the Voluntary Commitments carry forward as a standing
public commitment for their signatories independent of the
rescinded EO, or whether they are treated as historical by
signatories and by the current administration. -->

The head who was operating in 2023 remembers the Commitments as
front-page news. The head operating in the research window has to
determine, before treating the Commitments as a live sign-on
option, whether they are still a live commitment framework for
the enterprises that signed and whether new signatories are being
accepted. Chapter 05's withdrawal discipline is directly relevant
here — the Commitments' evolving political context is the archetypal
case for the "circumstances change" withdrawal rationale.

### Frontier Model Forum

The Frontier Model Forum was launched in July 2023 by Anthropic,
Google, Microsoft, and OpenAI as an industry body focused on
frontier-model safety research, evaluation methodology, and
information sharing. Membership expanded in the following months
and the Forum publishes working-group outputs and safety-research
grants.
<!-- needs-research: verify the current membership of the Frontier
Model Forum, its current published workstreams, and any published
membership criteria against frontiermodelforum.org. Confirm
whether membership is limited to frontier-model developers or
whether adjacent industry participation is accepted. -->

The Forum is a frontier-lab body in scope. For an enterprise that
develops a frontier model, membership is a live sign-on question
running through the full process described later in this chapter.
For an enterprise that is not a frontier-model developer,
membership is not on the table — but the Forum's publications are
tracked (via the scanning system in
[[mod-105-regulatory-change-management]]) because they shape the
methodology conversation the enterprise's own safety-evaluation
function operates against.

### Partnership on AI

Partnership on AI (PAI) is a multi-stakeholder body founded in
2016 with academic, civil-society, and industry members. PAI
publishes shared frameworks on responsible AI, synthetic media,
labour, and safety.
<!-- needs-research: verify PAI's current membership tiers,
current published workstreams, and the specific membership-
commitment framework members sign against partnershiponai.org. -->

PAI membership is a materially different sign-on commitment than
the frontier-lab bodies. It is a multi-stakeholder commitment;
peer members include civil society organisations whose
positioning may diverge from the enterprise's on any given
issue. The head's stance question is whether the enterprise
wants that adjacency — for the credibility it lends the
enterprise's own positioning, and for the exposure it creates
when the enterprise's positioning diverges from a fellow
member's.

### MLCommons AI Safety Working Group

MLCommons is an open engineering consortium best known for MLPerf
benchmarks. The AI Safety Working Group develops evaluation suites
for AI safety, including the AILuminate benchmark for text-based
safety hazards.
<!-- needs-research: verify the current published workstreams of
the MLCommons AI Safety Working Group, including the AILuminate
benchmark's current version and coverage, against
mlcommons.org/working-groups/ai-safety/ai-safety/. -->

Working-group participation is a lighter commitment than
signatory-body membership. The enterprise commits to
contributing (data, engineering hours, review time) not to a
public position. The head's stance decision here is about
engineering allocation more than about public exposure — but the
working group's outputs are consequential (published benchmarks
become industry-reference material), and the enterprise's
participation history is visible.

### US AI Safety Institute Consortium (AISIC)

The AI Safety Institute Consortium was convened by NIST as the
multi-stakeholder consortium supporting the US AI Safety
Institute's evaluation methodology work.
<!-- needs-research: verify the current organisational status of
AISIC given that Executive Order 14110 was rescinded by Executive
Order 14179 in January 2025 and the US AISI's institutional
positioning is evolving. Confirm current membership requirements,
current active working groups, and whether new applications are
being accepted, against nist.gov/aisi/artificial-intelligence-
safety-institute-consortium-aisic. -->

AISIC membership sits at the intersection of voluntary-code and
standards-body engagement. Members contribute to evaluation
methodology, publish jointly, and — critically — hold a working
relationship with a US federal centre of technical expertise that
is not a regulator. The chapter-03 engagement discipline in
[[mod-104-regulator-engagement]] governs how the head treats the
US AISI itself; AISIC membership is the operating vehicle for
that engagement for enterprises that qualify and elect to join.

### Adjacent industry bodies the head tracks but does not usually sign

Beyond the specific-scope bodies above, the head tracks a longer
list of industry associations whose codes or member commitments
touch AI: DIGITALEUROPE, BSA | The Software Alliance, ITI
(Information Technology Industry Council), the Chamber of
Digital Commerce, sector trade associations (SIFMA, ISDA, PhRMA,
AHIP, and the equivalents in other geographies), and country-
specific bodies. Membership in these bodies is generally a
Government Affairs decision, not a voluntary-code decision — but
the AI-specific code content produced by these bodies overlaps
with the voluntary-code landscape, and the head coordinates with
Government Affairs on which bodies to join and what the enterprise
signs onto through them.

## The four-move stance discipline

For every code in the portfolio, the enterprise's stance is one
of four moves — and only four. The stance is on the register.

- **Sign** — the enterprise takes on the public commitment,
  authors the operating-owner assignment, and runs the evidence
  discipline.
- **Decline with rationale** — the enterprise consciously does
  not sign, records the reason, and can defend the decision if a
  regulator, a journalist, or a customer asks.
- **Defer with a revisit date** — the enterprise is not ready to
  decide, records why (waiting for the next Code version, waiting
  for a specific peer's decision, waiting for a jurisdictional
  clarification), and puts a date on the calendar when the
  decision is retaken.
- **Watch** — the enterprise tracks the code but has no active
  sign-on decision in scope. This state is the same as the watch
  tier in the scanning system.

The discipline is that every code on the portfolio has an
explicit state. "We haven't got round to it" is not a state. If
the enterprise has not got round to it, either the code is at
watch (recorded) or the enterprise is deferring (recorded, with
revisit date). The head enforces the register, not the head's
memory.

## The internal decision process — the seven steps

An enterprise-scale sign-on decision runs through seven steps.
The head owns the process; the CxO peers own their steps. Steps
are sequenced deliberately, and the process does not skip
forward.

### Step 1 — Attachment analysis

The senior AI governance architect (level 50) runs the attachment
analysis: for each of the code's commitments, what does the
commitment attach to inside the enterprise. Which systems, which
model families, which business lines, which suppliers, which
geographies. The output is a table with a row per commitment and
columns for attachment surface, current-state readiness, and
gap. The scanning-and-crosswalk discipline in
[[mod-105-regulatory-change-management]] chapters 02 and 03 is
the same one applied here.

Attachment analysis is not "does this code apply to us". Voluntary
codes always apply to those who sign — that is what "voluntary"
means. The question is *what would the enterprise commit to*, in
terms specific enough that the CFO can cost it and the CRO can
appetite-check it. An attachment analysis that reads "this code
applies to our AI systems" has skipped the work.

### Step 2 — Cost estimate

The CFO's office costs the sign-on decision. Not just direct
compliance cost (headcount to run the reporting, engineering to
build any missing instrumentation, third-party evaluation spend)
but *opportunity cost* — what does the enterprise not get to
build if it commits this capacity to code-driven compliance. And
*risk-adjusted cost of misfire* — what does the enterprise expect
to spend if a signed commitment is later missed and remediation
is required.

The cost estimate has to be a *number*, not a range. Ranges hide
the CFO's actual position. If the estimate is honestly uncertain,
the number carries a confidence band; the band is not the answer.
The head does not accept a cost estimate that reads "significant
but manageable" — that is a phrase, not an estimate.

### Step 3 — Appetite check

The CRO checks the sign-on against the enterprise AI risk
appetite ([[mod-103-board-and-audit-committee-reporting]]
chapter 03). Two directions: does signing take the enterprise
*outside* the appetite (unusual — voluntary codes usually
compress the enterprise toward tighter controls, not looser),
and does *not* signing leave the enterprise outside a defensible
posture the appetite implicitly requires.

The second direction is the harder one. If the enterprise's
declared appetite is "we operate at the frontier of safe AI
practice", and the frontier of safe AI practice as evidenced by
peers is Code-adherent, then not signing is outside appetite.
The CRO makes that call, not the head. The head packages the
question.

### Step 4 — Legal exposure read

GC reads the code for legal exposure. Two questions: does the
code create a legally-enforceable commitment (usually no — that
is what "voluntary" means, and the code's text is generally
careful to say so, though the details matter and vary by
jurisdiction) and does the code create *ancillary* legal exposure
— a public statement that could be cited in a later regulatory
proceeding, a private litigation, or a shareholder action.

The GC output is not a "sign / don't sign" recommendation. It is
a legal-exposure characterisation the head then weighs against
the other steps. [[mod-104-regulator-engagement]] chapter 07 is
the governing boundary — GC opines on legal exposure, the head
owns the sign-on decision.

### Step 5 — Public-positioning read

Communications and Government Affairs jointly read the code for
public-positioning implications. Where is the code in the
current political conversation. Who signed. Who declined. What
happened to peers who signed and later missed. What would the
enterprise's signing (or not signing) look like on a competitor's
next earnings call, in a congressional hearing, in a Financial
Times article. What would the enterprise's messaging on the
sign-on need to look like to be defensible.

This read is not the head's own. The head consults it. Chapter
03 of this module covers the head's own public-trust posture in
detail; the public-positioning read at step 5 is the
Communications-and-Government-Affairs contribution to the
sign-on decision, not a substitute for the head's chapter-03
work.

### Step 6 — The head's recommendation

The head, with the outputs of steps 1 through 5 in hand, writes
a one-page recommendation. The recommendation has:

- The stance recommendation — sign, decline, defer, watch — with
  the specific rationale in one paragraph.
- The commitment scope, if signing — which of the code's
  commitments the enterprise takes on in full, which with
  qualification, which if the code permits partial sign-on.
- The operating-owner assignment, if signing — who inside the
  enterprise owns evidence production, at what cadence, with
  what reporting to the head.
- The condition set — the specific facts that would move the
  head to reconsider (a peer withdrawal, a Code revision, a
  material change in the enterprise's own footprint).
- The exit path, if signing — how the enterprise withdraws if
  the conditions turn against continued adherence. Chapter 05
  covers withdrawal discipline in detail.

The recommendation is one page. Longer recommendations are the
head having failed to compress the decision to the point where
the sign-off room can decide.

### Step 7 — Sign-off routing

The recommendation routes to the sign-off room. For a material
voluntary code, the sign-off room is the CEO, GC, CRO, and CFO —
and, for a code the audit committee has previously briefed on,
the audit-committee chair as a ratifier.

The routing is not a rubber stamp. Every named sign-off has a
specific accountability:

- **CEO** — the accountable executive for the enterprise's
  public commitment. The CEO signs, or the sign-on does not
  happen. The CEO is who a journalist or a shareholder addresses
  the "why did the enterprise sign X" question to.
- **GC** — the sign-off ratifies that the legal-exposure read
  (step 4) is the enterprise's settled legal position on the
  commitment. GC does not sign the enterprise up; GC ratifies
  that GC has read.
- **CRO** — the sign-off ratifies that the appetite check
  (step 3) is complete and that the sign-on sits within
  appetite (or, if outside, that the board has been notified
  under the exception discipline in
  [[mod-103-board-and-audit-committee-reporting]] chapter 03).
- **CFO** — the sign-off ratifies that the cost estimate
  (step 2) is the enterprise's committed cost estimate and that
  the budget carries the estimate. If the estimate is not in the
  budget, the sign-on does not happen until it is.

Where the sign-off room disagrees, the head does not go around
the disagreement to the CEO. The head convenes the disagreement,
runs it through the head-and-CxO adjacency discipline in
[[mod-101-role-scope-and-leadership-shape]] chapter 06 (extended
in [[mod-104-regulator-engagement]] chapter 07 to the CxO
adjacency ring), and either resolves the disagreement or
withdraws the recommendation. A sign-on that ships with a CxO
peer in silent disagreement is a sign-on the head will not be
able to defend later.

## The register — the sign-on portfolio as an artefact

The voluntary-code portfolio lives in the same register class as
the regulatory-change register
([[mod-105-regulatory-change-management]] chapter 01) and the
regulator-engagement inventory
([[mod-104-regulator-engagement]] chapter 04). One row per code.
The columns:

- Code identifier and canonical citation.
- Current state (signed / declined / deferred / watched).
- State-entry date and rationale.
- Commitment scope, if signed (which commitments, in what form).
- Operating owner, if signed.
- Revisit date, if deferred.
- Audit-committee visibility (last briefing date, next scheduled
  visibility).
- Withdrawal condition set, if signed — the specific facts under
  which the head reopens the sign-on decision.
- Public-facing artefact link — the enterprise's own web page,
  press release, or public commitment document that carries the
  sign-on.

The register is a governance artefact, not the head's private
notes. It is auditable, versioned, and readable by the CxO
peers, the audit-committee chair, and (under access controls)
by outside auditors under NDA.

## What the head does not confuse

Three category errors the head does not make:

- A voluntary code is not a regulation. GC does not opine on
  compliance; GC opines on legal exposure. The enterprise
  chooses whether to be bound.
- A voluntary code is not a marketing artefact. The head does
  not sign the enterprise up so the CEO can name-drop the
  signing in a keynote. The commitment is durable and the
  operating cost is durable; the marketing surface is not the
  driver.
- A voluntary code is not the same as standards-body
  participation. Chapter 02 covers the standards-body posture,
  which is a different kind of engagement (technical
  contribution, procedural voting, working-group leadership)
  with a different sign-off shape. The two portfolios interact
  — the GPAI Code cites CEN-CENELEC standards; the AISIC
  membership sits next to NIST AI RMF work — but the head
  keeps them on separate registers because the decision
  discipline is different.

## Summary

- Voluntary codes are public commitments the enterprise elects
  into. The sign-on decision is a governance decision the head
  owns; GC advises but does not decide.
- The head runs a portfolio: every code the enterprise is aware
  of sits in one of four states — signed, declined with
  rationale, deferred with revisit date, or watched.
- The standing portfolio as of the research window covers the
  EU AI Office GPAI Code of Practice, the G7 Hiroshima Process
  Code of Conduct, the White House Voluntary AI Commitments
  (where the enterprise is or was a signatory), the Frontier
  Model Forum, Partnership on AI, MLCommons AI Safety Working
  Group, and the US AISI Consortium; each carries a
  needs-research marker to confirm current status.
- Every code has one of four stances — sign, decline with
  rationale, defer with revisit date, watch — and the stance is
  on the register with rationale.
- The internal decision process is seven sequenced steps —
  attachment analysis (level-50 architect), cost estimate
  (CFO), appetite check (CRO), legal exposure (GC), public-
  positioning read (Comms + Government Affairs), head's
  one-page recommendation, and sign-off routing to CEO / GC /
  CRO / CFO (and audit-committee chair for material codes).
- The sign-off room is not a rubber stamp; each CxO ratifies a
  specific accountability, and disagreement is convened and
  resolved before sign-on, not after.
- The register is the durable artefact — one row per code, with
  state, commitment scope, operating owner, withdrawal
  conditions, and public-facing link — auditable and readable
  by CxO peers, the audit-committee chair, and external
  auditors under NDA.
- Chapter 02 turns to the standards-body participation
  portfolio; chapter 03 to the public-trust posture the sign-on
  decisions feed; chapter 05 to the harder decisions to decline
  or withdraw.
