# exercise-03: Enterprise Change Management Plan Drill

**Estimated effort:** 3 hours

## Objective

Author the **seven-lane enterprise change-management plan** for one
specific regulatory change the enterprise is landing, and produce
the artefact the head personally signs and the AI governance council
approves. The plan is the thing that turns the interpreted
obligation (exercise 02) and the level-50 architect's crosswalk
update into landed operating change across the enterprise.

The deliverable is not a template with placeholders. It is a
scenario-specific, fully-populated plan for one named regulatory
change, with named owners per lane, dated milestones, evidence-of-
completion definitions, sign-out capture, and the escalation
triggers under which the plan escalates to the audit committee or
the CEO. A plan a delegate could operate the rollout from without
the head in the room.

The plan has to pass three tests. First, an ISO/IEC 42006
certification body reviews it and recognises it as AIMS clause 8.1
operational-planning evidence. Second, a regulator asks in
examination "when did the enterprise decide to make this change and
who decided" — the plan's governance-authority lane answers with a
date and a committee. Third, a functional peer (CIO / CCO / CHRO)
picks up the plan and can see their own lane's expectations without
having to be briefed by the head.

## Prerequisites

- Chapter [03](../03-change-management-plan-shape.md) — the
  seven-lane plan shape (governance authority, communications,
  training, exceptions, board reporting, regulator notification,
  supply-chain) — read and internalised.
- Chapter [02](../02-interpretation-and-prioritisation.md) — the
  interpretation output is the plan's input. Exercise 02's three
  worked packages are strong prerequisites; pick one of them as
  the scenario for this exercise.
- [[mod-102-running-the-program]] chapters 01 (AI governance
  council), 03 (risk register and exception register), 04
  (regulatory crosswalk), 06 (AI system inventory), 07 (supply-
  chain evidence).
- [[mod-103-board-and-audit-committee-reporting]] chapters 01
  (quarterly pack clusters), 02 (audit-committee deep-dive
  shape), 04 (CxO sign-off flow).
- [[mod-104-regulator-engagement]] chapters 02 (Article 72/73
  filings), 05 (regulator exam runbook), 06 (public-consultation
  submissions) — where lane 6 draws from.
- A specific interpreted regulatory change to plan against.
  Options from the rehearsal roster (chapters 06 and 07): EU AI
  Act GPAI Article 53 obligations landing, JTC 21 harmonised
  standard citation in the OJEU, Colorado SB 24-205 developer /
  deployer obligations, Texas TRAIGA obligations, OSFI E-23 2027
  effective date, Korea AI Basic Act. Choose one that has scope
  wide enough to exercise all seven lanes.

## Steps

1. **Scenario setup — the change identifier.** Author the plan
   header: change identifier (short slug), regulator, obligation
   citation, effective date, authorising decision reference (fill
   in after step 2), plan version, plan date, plan owner (the
   head), plan-desk owner (the analyst from exercise 02). If the
   change's effective date is uncertain at the knowledge cutoff,
   use `<!-- needs-research: verify [obligation] current
   effective date and any implementing regulations against
   [official source] -->` — do not guess.
2. **Lane 1 — governance authority.** Author the authorising
   decision record: the committee (typically the AI governance
   council from [[mod-102-running-the-program]] chapter 01, or
   the risk / executive committee for enterprise-scale changes),
   the meeting date (choose a plausible one relative to the
   effective date), the minute-record extract (obligation and
   citation, GC opinion reference by title and author only —
   the opinion itself is privileged, proposed change and scope,
   the decision with reasoning, authorised authority to
   execute). If the change is material enough to require an
   audit-committee briefing, name the briefing date and the
   audit-committee chair's awareness posture.
3. **Lane 2 — communications cadence.** Author the four-wave
   cadence:
   - **Wave A (internal alignment)** — the CxO-peer briefing
     memo the head circulates ahead of any broader move.
     Attendees (specific CxO roles), delivery date relative to
     the effective date, and the ask of each function.
   - **Wave B (enterprise-scale CEO letter)** — the CEO letter
     the head drafts and the CEO or CAIO signs. Include the
     one-page letter itself (three things: what is changing,
     why, and the enterprise's posture on readiness). GC review
     status, Communications tone review status.
   - **Wave C (function-and-team rollout)** — the function-
     level communications and team-level runbook updates each
     affected function issues. List the affected functions
     (product, engineering, sales, procurement, HR, sector-
     facing regulatory relations) and the completion register
     the head monitors.
   - **Wave D (external posture)** — the external position
     Communications holds if asked by a journalist, customer, or
     prospect. GC review, Communications sign-out, whether a
     proactive statement (blog post, trust-centre update, ISO/IEC
     42001 public statement) is authored.
   Include the discipline that the head does not make compliance
   claims — external claims about compliance belong to
   Communications and GC jointly with the head as substance
   owner.
4. **Lane 3 — training refresh.** Author the three-tier training
   refresh:
   - **Tier 1 (function refresh)** — AI-governance function is
     briefed. Delivery mechanism (staff meeting or called
     session), record-keeping (minute entry).
   - **Tier 2 (role-based first-line refresh)** — role-based
     populations (name the roles — product managers, data
     scientists, ML engineers, evaluators, procurement
     specialists, sales engineers on regulated deals). LMS-
     tracked completion SLA (typically 30–60 days from wave C),
     escalation on gaps.
   - **Tier 3 (enterprise-wide policy refresh)** — the AI
     acceptable-use or adjacent enterprise-wide policy update.
     Coordination with HR / L&D, next quarterly refresh cycle
     integration.
   For each tier: content accuracy sign-off (head), timing owner
   (HR under SLA), completion evidence owner (HR/L&D, audited
   by head).
5. **Lane 4 — exception window.** Author the exception-window
   posture:
   - **Existing-exception re-scoring.** How the desk re-scores
     every open exception in the affected control area against
     the new obligation. Output: annotated exception register
     with invalidated / more-material / unaffected marks.
   - **Transition-window posture.** For affected systems that
     cannot achieve the new obligation by the compliance date
     without disrupting operations, the specific transition-
     window posture — which systems, how long, contingent on
     what interim safeguards (specific, evidenced), which
     committee approves.
   - **New-exception moratorium.** Whether a time-boxed new-
     exception moratorium is imposed in the affected control
     area during rollout. Duration, lift criteria.
   Cross-reference: [[mod-102-running-the-program]] chapter 03
   on exception discipline;
   [[mod-103-board-and-audit-committee-reporting]] chapter 04 on
   CxO sign-off for transition-window postures.
6. **Lane 5 — board and audit-committee reporting.** Author the
   pack-cluster feed:
   - Which pack clusters carry the change (regulator-engagement
     summary, regulatory-change tracking, portfolio risk-appetite,
     KRI dashboard).
   - Whether the change triggers an audit-committee deep-dive
     briefing at the quarter of finalisation, and if so, the
     brief agenda and co-briefers (head, GC, level-50 architect).
   - The KRIs the change introduces or reshapes, with a baseline
     ([[mod-107-program-measurement-and-maturity]] chapter 01
     supplies the KRI portfolio).
   - The risk-appetite tolerance the change shifts, if any, and
     the risk-committee coordination path.
7. **Lane 6 — regulator-facing notification.** Author the
   regulator-facing sequencing:
   - **Required filings.** Whether the obligation requires a
     filing (Article 72 post-market monitoring update, Article
     73 serious-incident report, sector-regulator notification,
     state AG registration). Filing timeline, artefact
     production, sign-out (GC-led per
     [[mod-104-regulator-engagement]] chapter 02).
   - **Supervisory-dialogue updates.** Where the enterprise is
     in ongoing supervisory dialogue on a related matter, the
     head's advance signal and the update within the next
     scheduled dialogue.
   - **Public-consultation participation.** Whether the
     enterprise submits to an open consultation on interpretive
     guidance ([[mod-104-regulator-engagement]] chapter 06).
   - **Voluntary transparency.** Any proactive communication
     (public statement, joint-industry statement, customer FAQ),
     coordinated with lane 2 wave D.
   - **What the enterprise does not communicate.** The specific
     internal drafting disagreements, tentative
     interpretations, and unsettled transition-window
     extensions the enterprise holds off on communicating —
     communicate from a settled position, not from work-in-
     progress.
8. **Lane 7 — third-party and supply-chain.** Author the
   supplier-propagation moves:
   - **Contract audit.** Which material AI-supplier contracts
     are audited against the new obligation, on what timeline.
   - **Amendment negotiation.** For contracts that do not cover
     the obligation, the amendment ask and the negotiation
     timeline. Procurement runs; head supplies substance and GC
     supplies drafting.
   - **New-contract template update.** The enterprise's standard
     AI-supplier contract template incorporates a new-obligation
     clause (one-shot, pays back on every subsequent
     procurement).
   - **Supplier communication.** The formal communication to
     material suppliers naming the change and the enterprise's
     expectation.
   - **Post-change verification.** How procurement verifies each
     material supplier has moved, on what cadence, feeding into
     the third-party audit interface
     ([[mod-102-running-the-program]] chapter 04).
9. **Interdependencies, escalation triggers, and sign-out.**
   Wrap the plan with:
   - **Interdependencies.** Where lane N's completion depends on
     lane M's output (e.g. lane 3 training needs lane 5
     board briefing to have landed the KRIs first; lane 7
     supplier communication needs lane 2 wave D external
     posture to be settled).
   - **Escalation triggers.** The specific conditions that
     escalate the plan to the AI governance council (SLA miss
     on any lane), to the audit committee (transition-window
     scope expansion, exception moratorium extension), or to the
     CEO (public-posture change, material cost overrun).
   - **Sign-out block.** Head's signature, and CxO sign-out
     per lane where material — CIO / CTO for engineering-
     carried lanes, CHRO for training lanes, CCO for external-
     facing lanes, GC for regulator-facing lanes.

## Deliverables

- `plan-header.md` — change identifier, regulator, citation,
  effective date, authorising decision reference, plan version /
  date / owner.
- `lane-1-governance-authority.md` — the authorising decision
  record and audit-committee briefing posture.
- `lane-2-communications.md` — the four waves (A alignment memo,
  B CEO letter, C function rollout, D external posture) with
  drafts.
- `lane-3-training.md` — the three-tier refresh plan with LMS
  SLAs and content sign-off.
- `lane-4-exceptions.md` — the re-scoring output, transition-
  window posture, moratorium decision.
- `lane-5-board-reporting.md` — the pack-cluster feed, audit-
  committee deep-dive shape, KRI introductions.
- `lane-6-regulator-notification.md` — the filing / dialogue /
  consultation / transparency sequencing and the do-not-
  communicate discipline.
- `lane-7-supply-chain.md` — the contract audit, amendment,
  template update, supplier communication, post-change
  verification moves.
- `interdependencies-escalation-signout.md` — the wrap-up section
  with interdependencies, escalation triggers, and the sign-out
  block.

## Acceptance criteria

- Every lane has a named owner (specific role, not "the
  enterprise") and a dated milestone timeline anchored to the
  effective date. No lane reads "as soon as possible".
- Lane 1 produces a specific committee, a specific date, and a
  specific decision record extract. The record answers the
  regulator's "when did the enterprise decide and who decided"
  question with a date and a committee.
- Lane 2 wave B contains the actual one-page CEO letter draft,
  not a description of what the letter would say. The letter
  states three things: what is changing, why, and the
  enterprise's posture on readiness. GC review and
  Communications tone review status are called out.
- Lane 3 tier 2 names the specific role-based populations, a
  completion SLA anchored to wave C (30–60 days), and an
  escalation path for gaps. "Training will be rolled out" is
  not enough.
- Lane 4 addresses all three moves (re-scoring, transition-
  window, moratorium) even where the decision on the moratorium
  is "no moratorium because..." — silence on any of the three is
  a defect.
- Lane 5 names the specific pack clusters the change touches,
  the KRIs introduced with baselines, and (where material) the
  audit-committee deep-dive shape.
- Lane 6 addresses all four sub-lanes (filings, dialogue,
  consultation, transparency) and explicitly names what the
  enterprise does not communicate. Silence on the do-not-
  communicate discipline is a defect.
- Lane 7 addresses all five sub-lanes (contract audit,
  amendment, template update, supplier communication, post-
  change verification) with named owners and timelines.
- Interdependencies are stated, not implied. A reviewer can
  trace which lanes block which.
- Escalation triggers are specific conditions (SLA miss, scope
  expansion, cost overrun) not generic "significant issues".
- The sign-out block names specific CxO peers per lane. Peers
  who are not sign-out counterparts are still named in wave A
  alignment so their awareness posture is on record.
- Where the change's effective date or a specific obligation
  detail is uncertain at the knowledge cutoff, a
  `<!-- needs-research: ... -->` marker names the fact and the
  source to verify. No effective date is guessed.

## Stretch goals

- Produce the **audit-committee deep-dive briefing** for the
  change as a standalone artefact — the material change briefing
  pattern from [[mod-103-board-and-audit-committee-reporting]]
  chapter 02. Attendees (audit-committee chair, head, GC, level-
  50 architect, CIO / CTO or CHRO as material), agenda (60
  minutes), pre-reads, one-page summary, follow-up commitments
  template.
- Produce a **90-day rollout-status one-pager** the head brings
  to the AI governance council monthly during the rollout — the
  seven-lane status view with green / amber / red per lane, the
  active escalations, the upcoming board / audit-committee
  touchpoints, and the risk-of-slip flag.
- Author the **post-rollout retrospective** template — what the
  head runs 90 days after the effective date to close the
  plan. Metrics (lane SLA hit rate, exception drift, KRI
  behaviour), what to carry into the next plan
  ([[mod-107-program-measurement-and-maturity]] chapter 04 on
  process improvement).
- Extend the plan with the **sector overlay** — where the
  enterprise operates under a sectoral supervisor (banking,
  insurance, health, telecoms), name how the change intersects
  with sectoral supervision and how the sectoral CxO peer
  ([[mod-109-cross-enterprise-leadership]]) is coordinated in
  the plan.

## Notes and starter guidance

The most common first-cut failure is a plan that looks complete
because every lane has content but the content is generic. Lane
2 says "communicate the change to all employees" without a
draft; lane 3 says "training will be updated" without a role-
based tier; lane 6 says "engage regulators as appropriate"
without naming filings or dialogues. A generic plan is worse
than no plan — the enterprise operates from it, misses the
substance, and cannot defend the miss because "we had a plan."
Force specificity: names, dates, drafts.

The second common failure is under-authoring lane 4. Exception
discipline is invisible until an audit or an enforcement action
surfaces it. A plan that does not re-score the existing
exception register against the new obligation is a plan that
will produce a rollout with exception-covered holes the
regulator finds. Even where the re-scoring output is "no
exceptions in the affected control area", write the sentence —
so a reviewer sees the discipline was applied.

The third common failure is missing lane 7. AI programs run on
suppliers; a change that lands inside the enterprise but not at
the supplier boundary is a change that fails at the supplier
boundary. If the enterprise is a heavy consumer of foundation-
model APIs, vector-database platforms, evaluation services, or
notified-body assessments, lane 7 is where the plan lives or
dies. Draft it explicitly, even where the enterprise is small
and lane 7 is short.

On the CEO letter — resist the pull to draft the letter as a
detailed technical briefing. The CEO's signature is on a
three-sentence executive posture, not on an implementation plan.
The letter's job is to establish that the enterprise is making
the change and to set the tone that later waves refer back to.
Detail belongs in wave C and in the plan itself.

On the do-not-communicate discipline in lane 6 — this is where
enterprises most often trip themselves. A well-meaning
communication about a tentative interpretation, an unsettled
transition-window scope, or an internal drafting disagreement
can commit the enterprise to a posture it has not decided.
Force lane 6 to name what the enterprise does not communicate,
so the plan's operating owners know the boundary.

The plan is a working document, not a polished deliverable.
Version it, date it, keep it in the same repository as the
running-program artefacts, and update it at every AI governance
council review. A plan that never changed during rollout is
either a very small change or a plan the enterprise did not
actually operate from.
