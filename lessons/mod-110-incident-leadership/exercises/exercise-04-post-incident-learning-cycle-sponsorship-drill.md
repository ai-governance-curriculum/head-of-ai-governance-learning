# exercise-04: Post-Incident Learning Cycle Sponsorship Drill

**Estimated effort:** 3 hours

## Objective

Author the **sponsorship-package artefact set** that shows the head of AI
governance *sponsoring* — not executing — the post-incident learning
cycle for a specific incident. The package is what closes the incident
on the audit-committee register with evidence rather than performance:
the RCA charter that names the specific control-or-policy question, the
commissioning briefs to the level-25 AI Risk Engineer and the level-50
Senior AI Governance Architect, the five-artefact production plan, the
programmatic-coherence review checklist the head applies to the
architect's proposed control and policy revisions, the depth-review
discipline note the head consults in real time, the sector-share
decision memo, the verbatim closure announcement, and the open-incident
tracking cadence. The learner produces ten artefacts, none of which are
the RCA itself — the head does not author the RCA, and this exercise
enforces the boundary.

The artefact set has to survive three stress tests. First, the level-25
AI Risk Engineer reads the RCA charter and confirms the question is
specific enough to produce a control or policy answer — a charter that
reads as "why did this happen" fails the engineer's craft, produces a
narrative rather than a causal analysis, and does not survive first
contact with the evidence. Second, the level-50 Senior AI Governance
Architect reads the commissioning briefs and confirms the artefact
scope is executable — a brief that reads as a delegation note rather
than a sponsorship stake produces an architect who owns neither the
depth nor the coherence of what lands. Third, the audit committee
reads the closure announcement and can trust the incident is genuinely
closed — a closure announcement that fails to name specific controls,
specific policy references, specific register rows, and a specific
sector-share disposition produces a closure that the next audit reads
as ceremonial.

The sponsorship discipline is what closes the incident on the
audit-committee register with evidence, not with performance. The
failure mode is the incident that produced a filing but no learning:
the SOC contained it, the regulator was notified, the customer-facing
statement went out, the war-room retrospective happened the following
week, and six months later an isomorphic incident materialised because
the register never gained a row and the control library never gained
a control. The head owns that failure mode. This exercise is the drill
that builds the sponsorship muscle before the head has to use it under
post-incident political pressure to declare closure.

## Prerequisites

- Chapter [[05-post-incident-learning-cycle-sponsorship]] read and
  internalised — the sponsorship-versus-execution distinction, the
  five artefacts, the RCA discipline elements (charter, team,
  timeline, depth, evidence, sign-off), the commissioning patterns
  for control and policy, the sector-share decision inputs, and the
  audit-committee closure discipline.
- [[mod-102-running-the-program]] chapter 03 (AI risk register),
  chapter 05 (maturity model), chapter 06 (AIMS inventory), chapter
  08 (evaluation discipline) — the running cadences the RCA-driven
  artefacts land into.
- [[mod-103-board-and-audit-committee-reporting]] cluster 3 (the
  incident-and-near-miss reporting cluster) — the board-facing
  summary format and audit-committee register discipline.
- [[mod-106-external-positioning-and-voluntary-codes]] — the
  sector-share posture the specific sharing decision is one instance
  of.
- [[mod-107-program-measurement-and-maturity]] — the KRI / KPI
  portfolio the RCA-derived metrics (RCA cycle time, control-library
  update velocity, incident-to-closure duration) feed.
- This module's chapters 01 through 04 — the incident-command,
  cross-function coordination, Article 73 filing, and US serious-
  incident disclosure disciplines the learning cycle picks up from.
- A specific incident scenario in mind. The scenario from exercise-03
  is a defensible reuse — the filing has been made, containment is
  complete, and the learning cycle is the next phase — but any
  concrete scenario at chapter-01 incident-class specificity works.

## Steps

1. **Scenario recap.** Author a one-page recap of the specific
   incident. Name the incident class per chapter 01 (training-data
   poisoning, RAG-corpus poisoning, prompt-injection escalation,
   drift-triggered failure, evaluation-gap failure, agent tool-use
   failure, model-extraction incident, or the specific class the
   scenario surfaces). Name the containment posture (contained;
   contained with residual risk; ongoing). Name the filing status
   (Article 73 filing lodged on [date]; US serious-incident
   disclosure lodged on [date]; no external filing required). Name
   the affected population estimate at the specificity the head
   would carry to the audit committee. Every subsequent artefact
   references this recap.

2. **RCA charter.** Author the RCA charter as a written document
   the head signs before the AI Risk Engineer starts. The charter
   contains, at minimum:
   - The specific question, phrased so the answer is a control or a
     policy, not a story. "What allowed X to persist past Y, and
     what change to control Z or policy W would have detected or
     blocked it?" is the shape. "Why did this happen?" is not.
   - The named engineer-in-charge (the level-25 AI Risk Engineer)
     and the named reviewer (the level-50 Senior AI Governance
     Architect).
   - The data-source contributors named by role: the AI Evaluation
     Engineer at level 35, the product manager and engineering
     lead of the affected system, the SOC contact, and the legal
     contact.
   - The target completion date, expressed as a specific date four
     to eight weeks from containment, with explicit rationale for
     the specific date chosen (incident complexity, regulator
     follow-up commitment, next audit-committee meeting, engineer
     load).
   - The review chain: draft to architect, architect review to
     head, head sign-off.

3. **Five-artefact production plan.** For each of the five
   artefacts the learning cycle produces — signed RCA report,
   updated risk-register entry, updated control-library entries,
   updated policy entries, board-facing summary — produce a row
   with:
   - Authoring owner (named role or named person).
   - Review chain (named reviewers in sequence).
   - Delivery date (specific date, referenced against the RCA
     target completion in the charter).
   - Tracking status (not started; in progress; in review;
     complete).
   Name explicitly that a missing artefact does not close the
   incident on the audit-committee register — the row on the plan
   *is* the register-closure gate.

4. **Commissioning brief to the level-25 AI Risk Engineer.**
   Author the written brief the head hands to the engineer at
   RCA kickoff. The brief covers:
   - The specific RCA question (referenced against the charter).
   - The evidence discipline required — every claim evidenced,
     timelines cite timestamps, counterfactual claims cite the
     specific artefacts they rest on, unavailable evidence
     documented as a finding.
   - The timeline target (referenced against the charter's
     completion date), with the intermediate milestones the head
     will review against.
   - The review checkpoints — draft-one review with architect,
     depth-review with head, evidence-review with head, final
     sign-off.
   - The escalation path when the engineer surfaces evidence
     gaps, scope creep, or a finding that implicates a peer
     function whose cooperation the RCA depends on.
   The brief is a written brief — a document with a filename —
   not a note in the task tracker and not a Slack message.

5. **Commissioning brief to the level-50 Senior AI Governance
   Architect.** Author the written brief the head hands to the
   architect for the control-library revision commissioning and
   the policy revision commissioning. The brief covers:
   - The scope of the control-library revision commissioning
     (which controls are candidates for revision, retirement, or
     new authorship, based on the anticipated RCA findings).
   - The scope of the policy revision commissioning (which policy
     clauses are candidates for revision).
   - The programmatic-coherence review criteria the head will
     apply (referenced against the checklist in step 6).
   - The delivery cadence — the architect returns drafts to the
     head on a named cadence; the head reviews and signs.
   - The escalation path where the architect surfaces a proposed
     control the operating function (CISO, CPO, HR, product)
     cannot commit to operate.
   Same format discipline as step 4: written brief, filename,
   sponsorship stake visible on the page.

6. **Programmatic-coherence review checklist.** Author the
   checklist the head applies to each of the architect's proposed
   control-library and policy updates. The checklist covers, for
   each proposed control or clause:
   - **Conflict with existing control** (yes / no + rationale) —
     does the new control require behaviour that contradicts an
     existing control?
   - **Duplication of existing control** (yes / no + rationale) —
     does the new control cover a surface an existing control
     already covers, implying the RCA finding is really that the
     existing control was not operating?
   - **Maturity implication** per [[mod-102-running-the-program]]
     chapter 05 — which maturity level does the new control
     assume, and does the program currently operate at that
     level?
   - **Taxonomy fit** — does the control compose cleanly with the
     ISO 42001 clause structure and the enterprise's control
     taxonomy?
   - **Cross-function composition** — does the control compose
     with the CISO's security stack, the CPO's privacy controls,
     HR's employment controls, and the other adjacent-function
     control stacks the AI stack sits alongside?
   The checklist is the head's review artefact — the head fills it
   in for each proposed control or clause before signing.

7. **RCA depth-review discipline note.** Author the head's own
   note capturing the four signals that tell the head the draft
   RCA has stopped at proximate cause. The learner writes the note
   as a checklist the head consults in real time when reading the
   draft. The four signals per chapter 05:
   - The finding is a single technical fix without a systemic
     finding above it.
   - The finding does not connect to any control-library entry —
     implying the AIMS did not carry a control for this class of
     failure and the RCA has not surfaced that gap.
   - The finding blames a person without asking why the alert
     design or process design allowed a competent person under
     normal load to miss it.
   - The finding does not distinguish between the incident's
     proximate trigger and the conditions that allowed the
     trigger to have this consequence.
   For each signal, the note names the specific pushback the head
   will send to the architect (who pushes back to the engineer) —
   the head does not rewrite the RCA.

8. **Sector-share decision memo.** For the specific incident,
   author the memo that weighs the four inputs per chapter 05 —
   legal exposure, competitive exposure, regulator context, and
   sector-good calculus — and produces a signed decision. The
   memo names:
   - The specific channel the enterprise will contribute through,
     if sharing: Partnership on AI, Frontier Model Forum,
     MLCommons AI Safety Working Group, the sector ISAC where an
     AI-specific channel exists, or a regulator-hosted forum.
   - The specific artefact the enterprise will contribute:
     anonymised RCA summary, control-library delta, evaluation-
     gap description, or telemetry pattern.
   - The reasoned rationale where the decision is to decline —
     naming which of the four inputs carried the decision, and
     what the audit-committee register records instead.
   The memo is signed by the head; the sharing decision is not
   delegated.

9. **Audit-committee closure announcement.** Author the verbatim
   text the head reads to the committee at the closure meeting:
   "Incident [ref] is now closed on the register. RCA signed on
   [date]. Register row [ref] updated. Controls [refs] revised.
   Policy [ref] republished. Sector-share decision: [contributed
   via / declined for reason]. Committee to note." The learner
   fills in every bracket for the specific scenario — the
   verbatim text is what the head will actually read, not a
   template.

10. **Open-incident-tracking cadence.** Author the cadence
    document that names how the head reports open-incident counts
    and gaps to the audit committee at each cycle until closure.
    The document covers:
    - The report format at each cycle (open-incident count,
      per-incident age against the target closure window,
      per-incident named gap).
    - The target closure window (typically twelve weeks from
      containment for serious incidents — the head names the
      specific window for the enterprise's incident-severity
      taxonomy).
    - The slippage discipline: at what age the head names the
      specific stall (RCA stalled; artefact update stalled;
      sector-share decision unresolved) and drives it to
      closure.
    - The escalation path when a specific closure gate cannot
      be met inside the target window.

## Deliverables

- `scenario-recap.md` — the one-page incident recap.
- `rca-charter.md` — the signed RCA charter with the specific
  question, named team, and target completion date.
- `five-artefact-production-plan.md` — the production plan across
  the five artefacts with authoring owner, review chain, delivery
  date, and tracking status.
- `brief-to-ai-risk-engineer.md` — the written commissioning brief
  to the level-25 AI Risk Engineer.
- `brief-to-senior-architect.md` — the written commissioning brief
  to the level-50 Senior AI Governance Architect.
- `coherence-review-checklist.md` — the programmatic-coherence
  review checklist across the five criteria.
- `rca-depth-review-discipline.md` — the head's real-time checklist
  of the four proximate-cause signals and the named pushback for
  each.
- `sector-share-decision-memo.md` — the signed sector-share
  decision memo weighing the four inputs.
- `closure-announcement-text.md` — the verbatim audit-committee
  closure text with every bracket filled in.
- `open-incident-tracking-cadence.md` — the cadence document for
  reporting open incidents until closure.

## Acceptance criteria

- The RCA charter question is a specific question whose answer is
  a control or a policy. A charter that phrases the question as
  "why did this happen" fails the criterion.
- The target completion date on the charter has explicit rationale
  (not just a date, but the reasoning that produced the date —
  complexity, regulator follow-up, board cadence, engineer load).
- All five artefacts on the production plan have a named
  authoring owner and a specific delivery date. An artefact with
  an unnamed owner or a "TBD" date fails the criterion.
- The commissioning briefs to the AI Risk Engineer and the
  Senior Architect are written briefs — documents with filenames
  in the deliverables — not notes in a task tracker.
- The coherence-review checklist covers all five criteria
  (conflict, duplication, maturity, taxonomy, cross-function).
  A checklist missing any of the five fails the criterion.
- The depth-review discipline note covers all four proximate-cause
  signals and names the specific pushback for each. A note that
  names the signals without naming the pushback fails the
  criterion.
- The sector-share memo weighs all four inputs (legal exposure,
  competitive exposure, regulator context, sector-good calculus)
  and produces a signed decision with a named channel and a named
  artefact (or a reasoned decline with the input that carried the
  decision named).
- The closure announcement text is verbatim (the head could read
  it aloud without editing) and covers all five artefact
  confirmations (RCA signature, register row, controls, policy,
  sector-share disposition).
- Any factual claim about a specific sharing channel's current
  membership or contribution mechanism, a specific regulator's
  current posture on incident-sharing as evidence of maturity, or
  a specific enterprise's incident-closure discipline carries a
  `<!-- needs-research: verify [specific fact] against [official
  source] -->` marker where the fact is not independently
  verifiable from cited primary sources. No practice is guessed.

## Stretch goals

- Extend the depth-review discipline into a **rehearsed pushback
  conversation** where the head sends the RCA back to the
  architect a second time and the AI Risk Engineer resists —
  authored as a two-page transcript that carries the specific
  language the head uses to hold the line without rewriting the
  RCA, and the specific language the head uses to name the
  proximate-cause signal that triggered the second send-back.
- Extend the sector-share memo into a **two-scenario compare**:
  share now (before the regulator engagement closes) versus share
  after the regulator engagement closes. The compare weighs how
  the four inputs shift across the two scenarios and produces
  the head's preferred sequencing with rationale.
- Author the **control-library commit message** that ties the
  control revision to the incident, with the change-history
  annotation the running library carries. The commit message is
  the artefact the next audit reads to reconstruct the
  incident-to-control causal chain.
- Author the **six-months-later audit-committee brief** showing
  the revised control's operating effectiveness — the KPI trend
  since the control landed, the near-miss count in the class the
  control addresses, and the evidence the head presents that the
  learning was real, not ceremonial. The brief composes with
  [[mod-103-board-and-audit-committee-reporting]] cluster 3.
- Extend the exercise into a **multi-incident RCA** where the
  RCA charter covers two related incidents (same class,
  different systems; or same system, different failure modes
  within a bounded window) — the charter names the shared
  question and the specific-per-incident sub-questions, and the
  production plan carries the shared-versus-per-incident split
  across the five artefacts.

## Notes and starter guidance

The most common first-cut failure on this exercise is the RCA
charter that reads as a story-question rather than a
control-question. "Why did the RAG corpus get poisoned?" produces
a narrative RCA that stops at the proximate cause and does not
connect to the control library. "What allowed the corpus
poisoning to persist past the corpus-verification stage of the
ingestion pipeline, and what control design would have detected
or blocked it before it reached production?" produces an RCA
whose finding is a specific control the architect can commission.
Force the control-or-policy phrasing on the charter question.
Where the incident surfaces more than one class of failure —
most non-trivial incidents do — either charter more than one RCA
or explicitly scope the single RCA to the enumerated set of
questions. What the head does not do is leave the question
unstated and hope the RCA discovers it.

The second common failure is the head who tries to author the
RCA. This collapses the review chain — the head cannot review a
document the head co-authored — and the RCA that lands is
thinner than the one the AI Risk Engineer would have produced.
This exercise deliberately excludes the RCA itself from the
deliverables. If the learner finds themselves drafting the RCA
in one of the ten artefacts, the drill is being missed. The
head sponsors; the engineer authors; the architect reviews and
commissions the follow-on revisions.

The third common failure is the commissioning briefs written as
delegation notes ("please run the RCA on incident X, target
completion in six weeks, thanks") rather than as the head's
sponsorship stake. The brief the level-25 engineer receives is
what carries the head's judgement about depth, evidence
discipline, escalation posture, and review checkpoints. A brief
that does not visibly carry the head's stake produces an engineer
who owns the artefact but not the discipline the head expects
around it. The same holds for the architect brief on
control-library and policy revisions — the brief has to name the
coherence criteria the head will apply, not just the scope of
the revision.

The fourth common failure is the sector-share memo that skips the
legal-exposure input. Legal's view on external contribution is
binding, not advisory — an RCA finding that an operational
control was not operating, shared externally, is a document
plaintiff's counsel will subpoena. The memo that documents the
sector-good calculus and the regulator-posture read without
documenting the legal read is a memo that the general counsel
will refuse to sign against. The fifth common failure is the
closure announcement that fails to name which specific controls,
which specific policy references, and which specific register
rows are updated — "we have completed the learning cycle" is not
a closure announcement; naming the artefact identifiers verbatim
is. Force the specificity, even where the exercise scenario
requires inventing plausible identifier formats.
