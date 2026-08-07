# Sponsoring the Post-Incident Learning Cycle

## Motivation

The incident is not closed when the SOC declares containment complete.
The incident is not closed when the filing lands with the national
competent authority under Article 73. The incident is not closed when
the customer-comms function retires the holding statement. The incident
is closed when the enterprise has *learned* from it — root-cause
analysis complete and signed, risk register updated, control library
revised, policy re-published, board briefed on both the incident and
the changes it produced, and (where the enterprise chooses) the lesson
shared with sector peers through the appropriate voluntary channel.

The failure mode this chapter defends against is specific and common:
the incident that produced a filing but no learning. The SOC contained
it. The regulator was notified within the statutory window. The
customer-facing statement went out. The war-room retrospective happened
the following week and the head-of-role's calendar moved on. Six months
later the same incident, or an isomorphic one — a different model, the
same class of failure at a different point in the stack — happens again.
The audit committee asks why. The honest answer is that the enterprise
did not commission the learning cycle. The RCA was never written to a
depth the next incident could have been designed against. The risk
register did not gain a row. The control library did not gain a
control. The policy did not gain a clause. The near-miss briefing to
the board did not include the delta between the incident and the
program.

The head of AI governance owns this failure mode. Not because the head
does the RCA — the AI Risk Engineer (level 25) does the RCA
engineering; the Senior AI Governance Architect (level 50) commissions
the artefact updates. The head owns the fact that the learning cycle
happens at all, that it runs at the right depth, that it produces the
five artefacts, that it closes on the audit-committee register with
evidence, and that the enterprise carries the lesson forward.

This chapter is how the head sponsors that cycle without executing it,
and how the head keeps the cycle running past the political incentive
to declare closure.

## Core concept — sponsorship, not execution

The head sponsors the learning cycle. The head does not execute it. The
distinction is the load-bearing move in this chapter and the one heads
most commonly get wrong under post-incident pressure.

**Sponsorship** is: chartering the RCA with a specific question,
naming the engineer-in-charge and the review chain, setting the target
completion date, reviewing the RCA at depth and pushing back if it
stops at proximate cause, ratifying the artefact updates the RCA
implies, signing the RCA report, and closing the incident on the
audit-committee register once the artefacts land.

**Execution** is: doing the timeline reconstruction, running the
Five-Whys, drafting the control-library revision, writing the policy
clause, filing the change into the register cadence. Execution is the
level-25 AI Risk Engineer's craft, the level-50 Senior Architect's
commissioning discipline, and the running program's cadences (per
`[[mod-102-running-the-program]]`).

Confusing sponsorship with execution produces one of two failures. The
first is the head who tries to do the RCA. This head has no time to do
it well, does it badly, and loses credibility with the technical
function whose respect the interface depends on. The RCA that lands is
thinner than the one the AI Risk Engineer would have produced, and the
Senior Architect's review adds nothing because the head who authored
it also owns the review chain.

The second is the head who is absent from the RCA. This head signs
what lands on the desk, does not push back on shallow findings, does
not force the control-library update, and treats the RCA as a
compliance artefact rather than a learning artefact. Six months later
the audit committee gets the isomorphic-incident briefing and the head
has no defensible answer for why the class of risk was not treated
after the first occurrence.

The sponsorship posture is closer to how the head handles the Article
73 filing (per `[[mod-104-regulator-engagement]]` chapter 02 and this
module's chapter 03) — the head signs, does not draft, but reviews at
sufficient depth that the signature carries weight. The RCA is the
same shape: the head signs, does not author, but reviews at sufficient
depth that the signature is not ceremonial.

## The five artefacts the learning cycle produces

A complete learning cycle produces five artefacts. Enumerate them.
When any of the five is missing at incident closure, the cycle is not
complete and the audit-committee register stays open.

1. **The RCA report itself.** Authored by the AI Risk Engineer, reviewed
   by the Senior AI Governance Architect, signed by the head. The RCA
   is the document the next audit reads. It is the document the next
   RCA — for the next incident — reads as prior art. It carries the
   incident timeline, the causal analysis, the evidence trail, the
   findings, and the commissioned changes.

2. **The updated risk register entry.** A new row on the enterprise AI
   risk register, or a revised existing row, per the running discipline
   in `[[mod-102-running-the-program]]` chapter 03. If the incident
   surfaced a class of risk the register did not carry, the row is new.
   If the incident materialised a risk the register already carried at
   a residual score, the row is re-scored and the treatment plan is
   revised.

3. **The updated control library entries.** New or revised entries in
   the enterprise's control library — the ISO 42001 controls the
   enterprise operates against, mapped to the specific controls the
   Senior Architect designed under the AIMS. The Senior Architect
   commissions the revision; the head reviews for programmatic
   coherence; the head signs off.

4. **The updated policy entries.** New or revised clauses in the
   enterprise AI-governance policy taxonomy. Same commissioning
   pattern as controls: architect drafts, head reviews for coherence,
   head signs, policy re-published on the enterprise's policy portal.

5. **The board-facing summary.** Per the board-and-audit-committee
   reporting cluster 3 in `[[mod-103-board-and-audit-committee-reporting]]`
   — the incident-and-near-miss reporting cluster. The summary carries
   the incident description, the RCA finding at a level appropriate to
   the audit committee, the changes commissioned, and the sector-share
   decision.

The head confirms each artefact against a checklist before closing the
incident on the audit-committee register. Missing artefacts do not
close the incident; they extend the tracking window.

## The RCA discipline the head sponsors

The head's sponsorship of the RCA covers six substantive elements. The
head does not do any of them, but the head sets each one at the
chartering stage and inspects each one at the review stage.

### Charter — the specific question

The RCA charter names the specific question the RCA answers. Not "why
did the incident happen" — that framing produces an RCA that stops at
the proximate cause and reads as a narrative rather than a causal
analysis. The charter names a specific question the RCA has to
answer, phrased so that the answer is a control or a policy, not a
story.

Examples of well-phrased RCA charters:

- "What allowed the RAG-corpus poisoning to persist past the
  corpus-verification stage of the ingestion pipeline, and what control
  design would have detected or blocked it before it reached
  production?"
- "What allowed the drift-triggered failure to remain undetected for
  six weeks past the drift-monitoring threshold, and what change to
  the monitoring interface, the on-call rotation, or the escalation
  taxonomy would have surfaced it earlier?"
- "What allowed the prompt-injection payload to escalate past the
  prompt-hardening layer to an agent-tool call, and what change to the
  tool-authorisation boundary would have contained it?"
- "What allowed the training-data class imbalance to reach the
  production model without evaluation-set coverage, and what change to
  the pre-deployment evaluation gate would have caught it?"

The head charters the RCA with one such question, in writing, before
the AI Risk Engineer starts. If the incident surfaces more than one
class of failure — most non-trivial incidents do — the head charters
more than one RCA, or explicitly scopes the single RCA to the
enumerated set of questions. What the head does not do is leave the
question unstated and hope the RCA discovers it.

### Team — named participants and roles

The RCA charter names the participants and their roles. A defensible
RCA team includes:

- **Engineer-in-charge:** the AI Risk Engineer (level 25). Authors the
  RCA. Runs the timeline reconstruction, the causal analysis, the
  evidence gathering. Owns the artefact.
- **Reviewer:** the Senior AI Governance Architect (level 50). Reviews
  the RCA for depth, for evidence discipline, for consistency with the
  control library and taxonomy the architect owns. Commissions the
  control-library and policy revisions the RCA implies.
- **Data source — evaluation function:** the AI Evaluation Engineer
  (level 35) provides evaluation data, red-team findings, and
  benchmark comparisons relevant to the incident.
- **System owner — product / engineering:** the product manager and
  engineering lead of the affected AI system provide access to logs,
  code, deployment history, and incident-time context.
- **Data source — SOC:** the SOC provides containment telemetry,
  attacker-side reconstruction where applicable, and the DFIR
  artefacts that compose with the RCA (per `[[mod-109-cross-enterprise-leadership]]`
  chapter 01 — the CISO coordination pattern).
- **Data source — legal:** legal provides constraints on what can be
  written into the RCA where litigation or regulatory exposure exists,
  and reviews the RCA before external circulation (per this module's
  chapter 03 on the filing regime).

The head does not sit on the RCA team. The head charters it, reviews
the draft, and signs the final. Sitting on the team collapses the
review chain — the head cannot review a document the head co-authored.

### Timeline — target completion date

The head sets an explicit target completion date at chartering. A
defensible RCA on a serious AI incident typically takes four to eight
weeks from containment. Faster than four weeks and the evidence
discipline usually slips; slower than eight and the political momentum
to act on the findings dissipates. The specific date the head sets
depends on:

- The complexity of the incident (single-system versus multi-system,
  contained versus ongoing residual risk).
- The regulator's expected posture on the follow-up (an Article 73
  filing that promised an RCA delivery date creates a hard external
  constraint).
- The board cadence (the next audit-committee meeting is a natural
  target if it falls in a defensible window).
- Available engineer time on the AI Risk Engineer (a serious RCA
  competes with the engineer's steady-state risk-engineering load).

The head reviews progress against the target at a bounded cadence
(typically weekly). Slippage of more than one week from the target
triggers a re-charter conversation, not a silent extension.

### Depth — pushing past proximate cause

The head reviews the RCA for depth. The specific discipline the
enterprise uses — Five-Whys with contextual analysis, Ishikawa /
fishbone, HFACS-adjacent human-factors analysis, or the systemic
analysis discipline the architect designed — is a choice the Senior
Architect makes when the AIMS is designed. The head does not choose
the method for a given RCA. The head reads the RCA and asks whether
the analysis stopped at the proximate cause.

Signals the RCA stopped at proximate cause and needs to go deeper:

- The finding is a single technical fix ("we added a filter") with no
  systemic finding above it.
- The finding does not connect to any control-library entry — implying
  the AIMS did not carry a control for this class of failure and the
  RCA has not surfaced that gap.
- The finding blames a person ("the on-call engineer missed the alert")
  without asking why the alert was designed such that a competent
  engineer under normal load could miss it.
- The finding does not distinguish between the incident's proximate
  trigger and the conditions that allowed the trigger to have this
  consequence.

Where the head sees one of these signals in the draft RCA, the head
pushes back to the Senior Architect, who pushes back to the AI Risk
Engineer. The head does not rewrite the RCA. The head names the depth
gap and requires the engineer-in-charge to close it.

### Evidence discipline — every claim evidenced

Every claim in the RCA is evidenced. The evidence trail is what the
next audit reads. Timelines cite log entries with timestamps. Causal
claims cite the specific artefacts they rest on. Counterfactual claims
("if the drift threshold had been set at 0.05 instead of 0.15, the
incident would have surfaced at day nine instead of day forty-two")
cite the drift-trace data. Where an evidence trail is unavailable —
because logs were not retained, because a system was decommissioned,
because the incident-time telemetry was insufficient — the RCA states
the gap explicitly, and the gap itself becomes a finding.

The head reviews the evidence discipline as a first pass before
reviewing the analytical content. If the evidence trail is thin, the
analysis on top of it is unreliable regardless of how compelling it
reads. The head sends the RCA back to strengthen evidence before
engaging with findings.

### Sign-off — the head signs the final RCA

The head signs the final RCA. The signature is not ceremonial. The
head signs the specific claim that the RCA is complete, is evidenced,
answers the chartered question, and carries the findings the enterprise
will act on. The signature is what the audit committee, the regulator
(where the RCA is shared externally), and the next audit read as
head-of-role ratification of the causal account.

A signed RCA the head has not read is worse than no signature — it
represents a false ratification. The head reads every RCA the head
signs, at whatever depth is needed for the signature to be defensible.

## Control-library update commissioning

The RCA produces findings. The findings imply control-library changes.
The head commissions the Senior Architect to draft those changes. The
commissioning pattern is deliberate and separates the head's review of
programmatic coherence from the architect's craft of control design.

The architect returns a proposed change — a new control, a revision
to an existing control, or (occasionally) the retirement of a control
the RCA has shown to be ineffective. The head reviews for programmatic
coherence, asking:

- Does this proposed control conflict with an existing control? If
  two controls now cover the same failure surface with incompatible
  requirements, one has to yield.
- Does this proposed control duplicate an existing control? If the
  existing control already covers this surface, the RCA finding is
  that the existing control was not operating, not that a new control
  is needed. The action is different — enforcement of the existing
  control versus authoring of a new one.
- Does this proposed control change the maturity model per
  `[[mod-102-running-the-program]]` chapter 05? A new control at
  level 4 maturity when the program is at level 3 maturity creates a
  gap the program cannot close on the current staffing plan; the
  architect and head resolve the maturity implication before the
  control lands.
- Does this proposed control compose cleanly with the ISO 42001
  clause structure and the enterprise's control taxonomy? A control
  that does not fit the taxonomy structure invites drift in the next
  review cycle.
- Does this proposed control compose with the CISO's security controls
  where the failure surface overlaps (per `[[mod-109-cross-enterprise-leadership]]`
  chapter 01)? A control that the SOC has to operate but was not
  co-designed with the CISO does not land in the SOC's stack.

Once the head signs off, the new or revised control enters the running
library on the next scheduled cadence. The Senior Architect commissions
the operational implementation (training, tooling, evaluation coverage,
audit trail). The head confirms at the next running-program review
that the control is operating, not just documented.

## Policy update commissioning

The same pattern runs for policy. The RCA may imply a policy change —
a new clause in the enterprise AI-governance policy, a revised threshold
in an existing clause, a new obligation on a downstream function, or a
new exemption where the RCA shows a clause to be over-broad.

The Senior Architect drafts the policy revision. The head reviews for
programmatic coherence, asking:

- Does the policy revision create a conflict with any other enterprise
  policy — the data-governance policy, the model-development standard,
  the third-party-risk policy, the acceptable-use policy for the
  enterprise's own AI systems?
- Does the policy revision create an obligation that another function
  cannot operationally meet? A policy clause that requires a function
  to do something the function is not staffed for creates paper
  compliance without operational compliance.
- Does the policy revision trigger cross-functional review? Any clause
  that affects the obligations of another function (legal, HR,
  procurement, product) requires that function's sign-off before
  publication.
- Is the policy revision at the right level of the policy hierarchy?
  A tactical control belongs in the standard beneath the policy, not
  in the policy itself; the head enforces the boundary.

The head signs the revised policy. The policy is re-published on the
enterprise's policy portal on the standard publication cadence, with
change-history annotation that ties the revision to the incident (with
the incident anonymised or redacted per the enterprise's disclosure
posture). Where the policy update affects other functions' obligations,
cross-functional review is triggered explicitly.

## The sector-share decision

Where the RCA surfaces a lesson that could prevent isomorphic incidents
at sector peers, the head faces a decision: share, or do not share.
The decision is the head's, informed by the Senior Architect, legal,
communications, and the external-relations function. The decision is
not delegated.

### The channels available

Where the enterprise chooses to share, the practical channels include:

- **Partnership on AI** — the head's enterprise, where a member,
  contributes an anonymised lesson through the appropriate PAI working
  group. <!-- needs-research: verify current PAI membership channels
  and lesson-sharing mechanisms; verify against PAI's incident-sharing
  guidance where published -->
- **Frontier Model Forum** — where the enterprise is a member (the
  Forum's membership is a bounded set of frontier developers), the
  incident pattern is contributed through the Forum's information-
  sharing channels. <!-- needs-research: verify current FMF membership
  requirements and information-sharing mechanisms -->
- **MLCommons AI Safety Working Group** — where the enterprise
  participates in the working group's benchmarks and evaluations, the
  incident may inform a new evaluation category or benchmark
  contribution. <!-- needs-research: verify MLCommons AI Safety WG
  current scope and contribution channels -->
- **Sector ISAC where an AI-specific channel exists** — the financial-
  services ISAC (FS-ISAC), the health-ISAC (H-ISAC), and other sector
  ISACs increasingly operate AI-specific working groups or channels.
  Where the sector has one, the ISAC channel is the natural route for
  operational-security-adjacent AI incidents. <!-- needs-research:
  verify which sector ISACs currently operate AI-specific channels and
  their contribution norms -->
- **Regulator-hosted sharing forums** — some regulators operate
  voluntary information-sharing forums (AI safety institutes, sandbox
  cohorts, sector supervisor working groups). Contribution here often
  composes with the general regulator engagement discipline in
  `[[mod-104-regulator-engagement]]`.

The head names the specific channel and the specific artefact the
enterprise will contribute — anonymised RCA summary, control-library
delta, evaluation-gap description, telemetry pattern — not "we will
share our learnings" as a general commitment.

### The four inputs to the decision

The decision to share, or not, weighs four inputs:

- **Legal exposure.** Does sharing create litigation exposure? An
  RCA finding that an operational control was not operating, shared
  externally, is a document a plaintiff's counsel will subpoena.
  Legal's view is a binding input, not an advisory one. Where legal
  determines that sharing creates unmanageable exposure, the head
  does not share, and documents the reason on the audit-committee
  register.
- **Competitive exposure.** Does sharing reveal a competitive
  advantage (the enterprise has a detection capability peers do not
  and sharing telegraphs it) or a competitive weakness (the enterprise
  had a control gap peers do not have and sharing highlights it)?
  Competitive exposure is a real consideration, and the honest
  version of the answer is not always "share anyway".
- **Regulator context.** Does the regulator, in the enterprise's
  jurisdiction, interpret sharing as evidence of maturity (the
  enterprise is a good citizen contributing to sector safety) or as
  an admission of failure (the enterprise has just documented a
  control gap the regulator can inspect against)? Regulator posture
  varies by jurisdiction, sector, and current enforcement priority.
  The head reads the regulator context through the same lens as the
  general regulator-engagement discipline (`[[mod-104-regulator-engagement]]`).
- **Sector-good calculus.** Would sharing prevent isomorphic incidents
  at peers? Where the answer is clearly yes and the other three
  inputs allow it, the sector-good calculus tips the decision toward
  sharing. Where the sector-good calculus is weak (the incident is
  idiosyncratic to the enterprise's stack, or the lesson is already
  in public discourse), the calculus does not carry the decision.

The head weighs the four, documents the weighing on the audit-
committee register, and signs the sharing (or non-sharing) decision.
The general voluntary-engagement discipline in
`[[mod-106-external-positioning-and-voluntary-codes]]` covers the
posture the enterprise takes on external contribution across all
channels; the sector-share decision on a specific incident is one
instance of that discipline.

## The audit-committee closure discipline

The incident is not closed on the audit-committee register until:

- The RCA report is complete, signed by the head, and summarised to
  the audit committee at a level appropriate to the committee.
- The risk register update is live on the running register.
- The control-library update is live on the running library.
- The policy update is published on the policy portal.
- The sector-share decision is documented — either the shared artefact
  reference, or the reasoned decision not to share.
- The board-facing summary has been presented to the audit committee
  per the incident-and-near-miss reporting cluster in
  `[[mod-103-board-and-audit-committee-reporting]]` cluster 3.

The head does not close the incident on the register without evidence
of each. The tracking window stays open, and the head reports the
open-incident count to the audit committee at each cycle until closure.
An incident that has been open on the register for more than the
enterprise's target closure window (typically twelve weeks from
containment for serious incidents) is itself a signal — either the RCA
is stalled, or the artefact updates are stalled, or the sector-share
decision is unresolved. The head names the specific gap and drives it
to closure.

Closure is announced explicitly at the audit committee: "Incident
[reference] is now closed on the register. RCA signed on [date].
Register row [reference] updated. Controls [references] revised.
Policy [reference] republished. Sector-share decision: [contributed
via / declined for reason]. Committee to note." The explicit
announcement creates the record the next audit reads for closure
discipline evidence.

## Composition with adjacent modules

- `[[mod-102-running-the-program]]` chapter 03 — the risk register
  cadence into which the RCA-driven register update lands.
- `[[mod-102-running-the-program]]` chapter 05 — the maturity model
  the control-library update composes against; the head does not
  land a control that pushes the program past its current maturity
  without a plan to close the gap.
- `[[mod-102-running-the-program]]` chapter 08 — the evaluation
  discipline the RCA may commission new evaluation coverage from.
- `[[mod-103-board-and-audit-committee-reporting]]` cluster 3 — the
  incident-and-near-miss reporting cluster the board-facing summary
  is authored into.
- `[[mod-104-regulator-engagement]]` chapter 02 — the Article 73
  filing regime the RCA may compose with where the filing promised
  a follow-up delivery of causal analysis.
- `[[mod-106-external-positioning-and-voluntary-codes]]` — the
  general voluntary-engagement discipline the sector-share decision
  is one instance of.
- `[[mod-107-program-measurement-and-maturity]]` — the KRI / KPI
  portfolio into which incident-derived metrics land (RCA cycle time,
  control-library update velocity, incident-to-closure duration).
- `[[mod-109-cross-enterprise-leadership]]` chapter 01 — the CISO
  coordination pattern that carries the DFIR-side artefacts into the
  RCA and the AI-specific findings back into the CISO's control
  stack.
- This module's chapter 01 through 04 — the incident-command,
  cross-function coordination, Article 73 filing, and US serious-
  incident disclosure disciplines the learning cycle picks up from.
- This module's chapter 06 — the difficult-conversation discipline
  that carries the harder briefings the learning cycle often
  requires (an RCA finding that names a peer function's gap, a
  sector-share decision that a business unit opposes, a control
  revision that a product team resists).

## Summary

- The incident is closed when the enterprise has learned from it, not
  when the SOC declares containment or the filing lands with the
  regulator.
- The head sponsors the learning cycle. The AI Risk Engineer does the
  RCA engineering; the Senior Architect commissions the artefact
  revisions; the head charters, reviews, ratifies, and signs.
- A complete learning cycle produces five artefacts: the signed RCA
  report, the updated risk-register entry, the updated control-library
  entries, the updated policy entries, and the board-facing summary.
- The RCA charter names a specific question phrased so the answer is
  a control or policy, not a story. "Why did this happen" is not a
  charter.
- The RCA team is named at chartering: engineer-in-charge, reviewer,
  and data-source functions. The head does not sit on the team.
- Target RCA completion is typically four to eight weeks from
  containment. The head sets the date, reviews progress at bounded
  cadence, and re-charters on slippage rather than silently extending.
- The head reviews the RCA for depth (does it stop at proximate
  cause?) and evidence discipline (is every claim evidenced?) before
  reviewing findings.
- The head signs the final RCA. The signature is not ceremonial; the
  head reads what the head signs.
- Control-library and policy updates follow the same commissioning
  pattern: architect drafts, head reviews for programmatic coherence
  (conflict, duplication, maturity implication, taxonomy fit,
  cross-function composition), head signs, update lands on the next
  cadence.
- The sector-share decision weighs legal exposure, competitive
  exposure, regulator context, and sector-good calculus. The decision
  is the head's, is documented, and is one instance of the voluntary-
  engagement discipline in `[[mod-106-external-positioning-and-voluntary-codes]]`.
- The incident closes on the audit-committee register only when all
  five artefacts are complete and the sector-share decision is
  documented. Closure is announced explicitly to the committee.
- Chapter 06 covers the difficult conversations the learning cycle
  often generates — the RCA finding that names a peer function's gap,
  the sector-share decision a business unit opposes, the control
  revision a product team resists.
