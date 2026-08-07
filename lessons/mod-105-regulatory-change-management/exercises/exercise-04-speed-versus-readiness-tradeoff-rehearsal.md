# exercise-04: Speed Versus Readiness Tradeoff Rehearsal

**Estimated effort:** 2 hours

## Objective

Author the **compliance-date posture** the head proposes for one
specific in-flight regulatory change, using the two-column ledger
from chapter 04, and then rehearse defending the posture in the
four rooms chapter 04 names — the CEO room, the board / audit-
committee room, the regulator room, and the enterprise room.

The deliverable is a written posture proposal and four short room
briefings the head would take into each of the four rooms. It is a
speed-versus-readiness rehearsal, not a plan authoring exercise —
the change-management plan is exercise 03. This exercise is about
the head's *adjudication move*: the specific combination of full
readiness, transition window, exception, deferred scope, and
accepted residual risk that the head proposes, defended with the
same substance translated to each audience.

The rehearsal has to survive three tests. First, the CEO reads the
CEO briefing and could sign the wave B letter (chapter 03 lane 2)
without asking the head for more information. Second, the audit-
committee chair reads the committee briefing and can see the
process was followed, the residual-risk acceptance is appropriate
to appetite, and the KRI that would move first if the posture were
wrong is named. Third, the regulator briefing is a posture the
head could deliver in an examination without the regulator later
citing an inconsistency between what the head said and what the
enterprise did.

## Prerequisites

- Chapter [04](../04-speed-versus-readiness-tension.md) — the
  two-column ledger, the five-move aligned posture, and the
  four-room defense discipline — read and internalised.
- Chapter [02](../02-interpretation-and-prioritisation.md) — the
  interpretation output that produced the packaged obligation and
  the priority ranking. Exercise 02 is a strong prerequisite.
- Chapter [03](../03-change-management-plan-shape.md) — the plan
  shape that the posture will operationalise. Exercise 03 is a
  strong prerequisite; using the same scenario across exercises
  03 and 04 lets the posture and the plan align.
- [[mod-102-running-the-program]] chapters 03 (risk register and
  exception discipline), 06 (AI system inventory that supplies
  the current-state evidence), 07 (supply-chain evidence).
- [[mod-103-board-and-audit-committee-reporting]] chapters 02
  (audit-committee deep-dive), 03 (risk-appetite framework), 04
  (CxO sign-off flow).
- [[mod-104-regulator-engagement]] chapters 05 (regulator exam
  runbook — the regulator-room posture disclosure), 07 (the head-
  and-GC boundary).
- [[mod-107-program-measurement-and-maturity]] chapter 01 — the
  KRI portfolio the head names as the "first-to-move" indicator
  if the posture is wrong.
- A specific regulatory change to rehearse against. Options from
  chapters 06 and 07: EU AI Act GPAI Article 55 systemic-risk
  provider obligations landing, JTC 21 harmonised standard
  moving to OJEU citation, Colorado SB 24-205 developer /
  deployer obligations, Texas TRAIGA effective date, OSFI E-23
  2027 effective date, Korea AI Basic Act enforcement. Pick a
  change where the honest readiness gap is non-trivial —
  rehearsing against a change the enterprise is already fully
  ready for teaches nothing.

## Steps

1. **Scenario setup — the change and the honest gap.** Author
   the one-paragraph scenario: the change (regulator, obligation,
   citation, effective date — use `<!-- needs-research: ... -->`
   where the date is uncertain), the enterprise's current
   position at a high level, and the honest gap between the
   compliance date's demands and the enterprise's readiness
   capacity. The gap is the reason this exercise exists — if
   there is no honest gap, pick another scenario.
2. **The compliance-side column.** Author the compliance-side
   read against the three questions chapter 04 names:
   - **What has the regulator said, in its own words?** Cite the
     regulator's specific supervisory statements, published
     FAQs, speeches, press releases naming enforcement
     priorities on this obligation. Mark
     `<!-- needs-research: verify [regulator statement]
     against [source] -->` where the statement's citation is
     uncertain. Do not paraphrase the regulator; quote or cite.
   - **What has the regulator done in analogous cases?** Cite
     the enforcement history against peers on analogous
     obligations. Where the enforcement history is thin (a new
     obligation with no analogue), state that explicitly.
   - **What have peers announced?** Cite peer disclosures on
     their own readiness posture — public statements, industry-
     body reporting, trade press. Where peer disclosures are
     thin, state that explicitly. Peer disclosures are a
     program-management input, not a regulatory floor.
3. **The readiness-side column.** Author the readiness-side read
   against the four questions chapter 04 names:
   - **Current state, evidenced.** The AIMS evidence on the
     current state — control-testing pass rate, exception count,
     incident record, evaluation coverage — specific to the
     obligation's attachment. "Control C.4.2 is implemented on N
     of M in-scope systems" language, not "we are 80% ready".
     For the exercise, evidence values can be plausible-scenario
     values, not real telemetry — but they have to be *specific
     numbers* consistent with the enterprise-context assumption,
     not "several" or "most".
   - **Honest completion probability.** For each in-flight
     change the enterprise is running against the obligation,
     the honest completion-by-date probability. Distinguish the
     50th-percentile date (planning date) from the 80th-
     percentile date (sprint-plan date) from the 20th-percentile
     date (worst-plausible date). Chapter 04's discipline: plan
     against the 50th and 20th, not the 80th.
   - **Operating-team capacity picture.** What the operating
     teams (engineering, product, procurement, HR) are already
     carrying. What the marginal cost of the readiness push is
     on top. What gives if the push takes priority.
   - **Transitional safeguards actually available.** For each
     lane where full readiness will slip, the specific interim
     safeguard — currently operating, reducing the specific
     risk, measurable, auditable, named-owner. Vague
     "compensating controls" language does not survive this
     test.
4. **The aligned posture — the five-move breakdown.** Author the
   posture as a specific combination of the five moves chapter
   04 names, mapped to specific subsets of the obligation's
   attachment:
   - **Full readiness on lane A** — the systems / controls the
     enterprise is fully ready on by the date. Name them.
   - **Transition-window posture on lane B** — the systems /
     controls the enterprise is not ready on by the date, the
     specific interim safeguard package, the window-close date,
     and the disclosure posture to the regulator if the
     regulator's supervisory framework requires it.
   - **Exception with time limit on lane C** — the narrow
     subset with a documented, dated, committee-approved
     exception; the compensating-control identification; the
     revisit date (not "closed").
   - **Deferred scope on lane D** — the subset that is out of
     scope for the compliance date because attachment analysis
     or GC opinion shows it does not attach. Write the reason.
   - **Accepted risk with board notice on lane E** — the
     residual package that neither achieves readiness, nor
     benefits from an interim safeguard, nor is out of scope,
     and that the enterprise accepts as residual risk with
     audit-committee notice. This subset should be small; if it
     is large, note the program problem explicitly.
   Each lane is bounded (specific systems / controls), dated
   (specific milestone dates or windows), and evidenced (the
   evidence supporting that this is the right posture for the
   subset).
5. **Room briefing one — the CEO room.** Author the CEO
   briefing: three sentences (one per question chapter 04 names
   — what is the enterprise's overall posture, is it defensible,
   what is the risk if wrong and what is the cost of doing more)
   and one appendix (the five-move breakdown from step 4). The
   briefing should be readable in three minutes; the appendix
   should be readable in ten. If the CEO will sign the wave B
   letter, the substance in the briefing is the substance in the
   letter — chapter 03 lane 2 wave B.
6. **Room briefing two — the audit-committee room.** Author the
   audit-committee briefing on the compact chapter 04 shape:
   - The obligation and the date.
   - The five-move breakdown (referring back to step 4's
     document, not restating it).
   - The KRIs that would move first if the posture is wrong
     (name them, name their baseline).
   - The escalation triggers under which the head brings the
     posture back to the committee mid-cycle.
   The briefing is where the CxO peer with the largest exposure
   (CRO for appetite, GC for legal, CIO / CTO for engineering-
   carried lanes, CCO for external-facing lanes) either co-signs
   by presence or explicitly does not. Name the peer and the
   presence-signing expectation.
7. **Room briefing three — the regulator room.** Author the
   regulator briefing on the discipline chapter 04 names — share
   the shape of the posture in the regulator's vocabulary, with
   evidence the regulator can verify, without oversharing
   internal drafting disagreements or unsettled process. Cite
   [[mod-104-regulator-engagement]] chapter 05 for the exam
   runbook and chapter 07 for the head-and-GC boundary on what
   the head personally says versus what GC delivers. The
   briefing has:
   - The posture at the level of subsets (lane A / B / C / D /
     E) without internal committee names or personalities.
   - The specific evidence the regulator can inspect (control-
     testing evidence, exception register extract if the
     regulator's supervisory framework contemplates that,
     interim-safeguard operational evidence).
   - The window-close dates on transition-window items.
   - What the enterprise is *not* asking the regulator to do
     (e.g. the enterprise is not asking for a formal extension;
     it is disclosing its planned window-close date under the
     supervisory framework's disclosure regime).
8. **Room briefing four — the enterprise room.** Author the
   enterprise-facing briefing (wave C of chapter 03 lane 2) —
   the substance the operating teams need to understand what
   the posture is and what their lane is. The briefing is
   plain-language, role-specific where necessary, and closes
   with a Q&A capture (the specific questions the head expects
   from operating teams and the head's prepared answers).
   Include the specific trap chapter 04 names: teams that first
   hear the posture in a customer meeting have been failed by
   the head.
9. **The three speed traps and three readiness traps.** For the
   scenario, name specifically which of chapter 04's six traps
   apply and how the posture avoids them:
   - Speed traps: the "we said we would be ready" trap, the
     "we can catch up later" trap, the "regulator won't
     notice" trap.
   - Readiness traps: the "gold-plating" trap, the "everything
     is a priority" trap, the "single-point-of-failure
     heroics" trap.
   For each trap that applies, name the mitigation. Write the
   traps that do not apply as such — silence is a failure to
   consider them.

## Deliverables

- `scenario.md` — the one-paragraph change and honest-gap
  statement.
- `compliance-side.md` — the compliance-side column against the
  three questions (regulator's words, analogous history, peer
  disclosures) with citations and needs-research markers.
- `readiness-side.md` — the readiness-side column against the
  four questions (current state evidenced, honest completion
  probability, capacity picture, transitional safeguards).
- `aligned-posture.md` — the five-move breakdown mapped to
  specific subsets of attachment, bounded / dated / evidenced.
- `ceo-briefing.md` — the three-sentences-plus-appendix CEO
  briefing.
- `audit-committee-briefing.md` — the compact audit-committee
  briefing with KRIs and escalation triggers.
- `regulator-briefing.md` — the regulator-room briefing under
  the exam-runbook discipline.
- `enterprise-briefing.md` — the wave C plain-language briefing
  with Q&A capture.
- `trap-audit.md` — the six-trap audit and mitigations.

## Acceptance criteria

- The compliance-side column cites the regulator's own words
  (with a specific citation or a `<!-- needs-research: ... -->`
  marker naming the fact and the source to verify), not the
  head's paraphrase. GC's opinion is not in the compliance-side
  column — that is chapter 02 step 3, not this exercise.
- The readiness-side column produces **specific numbers** for
  current state (N of M systems on control C) and honest
  completion probabilities at the 50th / 80th / 20th
  percentiles. Language like "mostly ready" or "on track" is a
  defect.
- The transitional-safeguards subsection produces safeguards
  that meet the five properties chapter 04 names (currently
  operating, reduces the specific risk, measurable, auditable,
  named owner). Vague "compensating controls" language is a
  defect.
- The five-move aligned posture assigns every element of the
  obligation's attachment to exactly one of the five lanes.
  Attachment left unassigned is a defect. The lane E (accepted
  risk) subset is small; if it is more than a quarter of the
  attachment, the exercise flags this as a program problem
  rather than pretending the posture is aligned.
- The CEO briefing is genuinely three sentences plus one
  appendix. If it is longer, the head has failed the discipline.
- The audit-committee briefing names the specific KRIs that
  would move first, with baselines. "We will monitor KRIs" is a
  defect.
- The regulator briefing does not include internal committee
  names, drafting disagreements, or unsettled process. The
  substance is settled position, evidence, dates.
- The enterprise briefing is plain-language, role-specific
  where necessary, and closes with a Q&A capture. Teams reading
  the briefing understand their lane.
- The trap audit addresses all six traps explicitly — six
  paragraphs even where three of the traps do not apply.
  Silence on a trap is treated as failure to consider it.

## Stretch goals

- Rehearse the **posture-change decision** — a mid-rollout
  scenario where facts change (a regulator issues an
  interpretive statement narrowing the obligation, a peer
  suffers enforcement on a related matter, an engineering
  slippage shifts the honest completion probability
  materially). Author the posture-change memo the head takes
  back to the audit committee, the sequencing of the update to
  each of the four rooms, and the register entry that records
  the change.
- Author the **posture disclosure to a specific NCA** as a
  fully-drafted supervisory-dialogue update, using the
  [[mod-104-regulator-engagement]] chapter 05 exam-runbook
  discipline. The draft is what GC reviews and the head
  co-signs; it demonstrates the regulator-room posture in
  regulator-facing artefact form.
- Draft the **posture-monitoring dashboard** — a one-page KRI
  view the head reads weekly during the rollout window,
  covering the specific indicators from the audit-committee
  briefing plus lane-completion status against the five-move
  breakdown. Chapter [[mod-107-program-measurement-and-maturity]]
  chapter 01 shapes the KRI portfolio the dashboard draws from.
- Extend the exercise with a **contrasting-posture case** — a
  scenario where the head has to argue for a *slower* rollout
  than product / engineering is pushing for. Chapter 04 covers
  both directions; the exercise as authored is oriented toward
  arguing for a slower-than-full-readiness posture, but the
  head also has to be able to argue for a faster-than-comfort
  posture when the regulator's history and peer disclosures
  demand it. The contrasting-posture case is symmetric and
  equally valuable.

## Notes and starter guidance

The most common first-cut failure is optimism in the readiness-
side column. The head, wanting to present the enterprise well,
reads "88% ready" as "close enough" and rounds it to "ready by
the date". Ninety days later the missing 12% turns out to be the
attachment that mattered most, and the enterprise is caught
unready without a transition-window posture. The discipline
chapter 04 enforces — specific numbers, honest completion
percentiles, credible interim safeguards — is not pessimism.
It is program planning against how change actually lands.

The second common failure is asymmetry across the four rooms.
The head says one thing to the CEO (posture is strong), a
different thing to the audit committee (posture is contingent
on transition-window operating), a different thing to the
regulator (posture is settled), and a different thing to the
operating teams (posture is a stretch). When any two of the
four rooms hear from each other — which happens — the head is
caught misaligned. The discipline: same substance in every
room, translated to the room's vocabulary. Force yourself to
draft all four briefings and read them side by side; if the
substance drifts, the posture drifts.

On the CEO room — resist the pull to write a longer briefing
than the discipline allows. Three sentences plus one appendix
is a discipline that forces the head to know the posture well
enough to compress it. A CEO briefing that runs to four pages
is a head who does not yet know the posture and is hiding it in
prose.

On the audit-committee room — the KRIs matter more than the
briefing. A briefing that names the wrong KRIs (metrics that
will not move first if the posture is wrong) is a briefing
that leaves the audit committee unable to see the failure
coming. Consult [[mod-107-program-measurement-and-maturity]]
chapter 01 explicitly; do not invent KRIs for the exercise.

On the regulator room — the temptation is to overshare. The
head who says "we had a lot of internal disagreement about
whether this obligation attaches to X" thinks they are being
transparent; the regulator hears "the enterprise does not have
a settled position". Settle first, disclose from the settled
position. Chapter 04 and [[mod-104-regulator-engagement]]
chapter 07 are both explicit on this.

On the trap audit — the six traps are named because they are
common, not because they are exotic. The head who has run a
material regulatory change through to the compliance date has
almost always encountered at least two of them. Force yourself
to name specifically which apply, with the specific mitigation
in place, so a reviewer can see the discipline was applied
rather than glossed.

The posture is not a compromise between speed and readiness.
It is the head's *aligned proposal* — the specific combination
that is defensible in all four rooms. A posture that survives
in three rooms but not the fourth is not yet aligned. Rewrite
until it is.
