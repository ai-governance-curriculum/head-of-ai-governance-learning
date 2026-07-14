# exercise-02: Article 73 Serious-Incident Filing Runbook

**Estimated effort:** 4 hours

## Objective

Produce the **leadership-scope runbook** the head of AI governance
keeps ready-to-run for an Article 73 serious-incident filing under
the EU AI Act. The architect (paired level-50 role) owns the
operational incident workflow that lands in
[[mod-110-incident-leadership]]; this runbook is the head's face of
that workflow — the artefacts, decisions, sign-offs, and briefings
the head personally executes when Article 73 is triggered.

The deliverable is not a policy document and is not a training
narrative. It is a step-by-step script the head executes under time
pressure, in the moment, with named roles, named artefacts, named
timelines, and named escalation paths. A colleague picking up the
runbook cold, mid-incident, has to be able to run it.

## Prerequisites

- Chapter [02-article-72-and-73-filings](../02-article-72-and-73-filings.md)
  — Owning the Article 72 and Article 73 Filings at Leadership
  Scope — read and internalised. The seven-question filing-defence
  discipline in particular is load-bearing.
- [[mod-102-running-the-program]] chapter 04 on the post-market
  monitoring operating discipline that feeds incident detection.
- [[mod-103-board-and-audit-committee-reporting]] cluster 3 on the
  incident-and-near-miss briefing shape the runbook writes into.
- [[mod-110-incident-leadership]] on the operational incident
  workflow the architect runs; the runbook is the leadership face
  of that workflow, not a substitute for it.
- Chapter [07-engagement-versus-legal-opinion-boundary](../07-engagement-versus-legal-opinion-boundary.md)
  on the GC boundary the runbook has to respect at every step
  where legal interpretation is required.
- A concrete enterprise in mind, with an assumed sector, an assumed
  jurisdictional footprint inside the Union, and an assumed lead
  NCA (or multi-Member-State configuration if that is the reality).

## Steps

1. **Definition-and-triggering discipline.** Open the runbook with
   the Article 3(49) definition of a serious incident restated in
   plain form the head can read out in a triage meeting. Below
   that, author the enterprise's own **triggering rule** — the
   internal test that decides when the definition is met for a
   given event. The triggering rule names the decision-makers (who
   calls it), the evidence they need in front of them, and the
   escalation path if the call is contested. Mark any point where
   you are uncertain of the exact statutory wording with a
   `needs-research` note; do not paraphrase around uncertainty.
2. **Timeline compliance one-pager.** Author the three Article 73
   timelines on a single page: the general rule (approximately 15
   days from awareness under Article 73(2)); the shorter rule for
   widespread infringement or serious-and-irreversible
   fundamental-rights breach (approximately 2 days under Article
   73(3)); the rule for death of a person (approximately 10 days
   under Article 73(4)). Beside the statutory clock, author the
   enterprise's own **internal clock discipline** — the T-minus
   milestones (evidence lock, GC review, CxO sign-off window, NCA
   submission window, board notification window) that make the
   external timeline meetable rather than aspirational. Mark
   `needs-research` on any specific timeline wording you are not
   confident is verbatim.
3. **Seven-question filing defence, worked.** Take the seven
   questions from chapter 02 (what happened factually; when we
   became aware and how we dated that; causal link or reasonable
   likelihood; containment and remediation; who is affected and
   notified; current root-cause view and evidence; corrective
   action committed with dates). Answer all seven for **one
   hypothetical incident scenario** you construct for the drill.
   The scenario is clearly labelled hypothetical at the top of the
   runbook and is chosen to exercise the runbook, not to describe
   any real event. Do not use a real incident from your enterprise
   or a public incident you cannot fully characterise.
4. **Sign-off flow.** Author the named-signature routing for the
   filing. Every signer has: the role title, the specific decision
   that signer makes (not "review" — the actual go/no-go call they
   own), the SLA for their turnaround, and the escalation path if
   the signer is unavailable inside the SLA. At minimum: head of
   AI governance; General Counsel (legal interpretation, including
   whether the event meets Article 3(49)); senior AI governance
   architect (technical accuracy of the account of events); CISO
   (if the incident is cyber-adjacent); DPO (if the incident is
   privacy-adjacent); CRO (enterprise-risk register update); CEO
   (for reputationally significant incidents); board chair (for
   material incidents). Specify the **sequence** the signatures run
   in — parallel where possible, serial where a downstream signer
   needs the upstream call.
5. **Briefing outputs.** Specify each internal briefing the runbook
   produces and the artefact for each: the board briefing (shape
   from [[mod-103-board-and-audit-committee-reporting]] cluster
   3); the interim audit-committee-chair briefing (issued before
   the next scheduled board pack, not held for it); the CEO
   briefing (shape and length); the internal all-hands
   communication drafted with Comms (with the split of what the
   head owns versus what Comms owns). For each briefing, name
   who drafts, who signs, who distributes, and by when relative to
   the NCA filing.
6. **NCA engagement plan.** Author the four-stage engagement plan
   the head expects to run after the filing lands: the opening
   filing itself (channel, format, cover letter, acknowledgement
   discipline); the follow-up written information request the head
   anticipates within weeks (evidence repository posture, response
   SLA, GC review of every response); the on-site inspection
   preparation (host, brief-holders, evidence stations, physical
   or virtual logistics); the remediation-plan drafting stage
   (owner, sign-off, commitment tracking back into
   [[mod-102-running-the-program]] chapter 03 risk register). Each
   stage names the head's personal action and the architect's
   supporting action.

## Deliverables

- `runbook.md` — the full leadership-scope runbook covering steps
  1 through 6, structured so a reader unfamiliar with the drafting
  session can execute it.
- `triggering-rule.md` (may be a section within `runbook.md`) —
  the Article 3(49) plain-form restatement plus the enterprise's
  own triggering test with named decision-makers.
- `timeline-onepager.md` — the three Article 73 timelines beside
  the enterprise's internal T-minus milestone discipline.
- `worked-seven-question.md` — the seven-question filing defence
  answered for the hypothetical scenario, clearly labelled
  hypothetical.
- `signoff-flow.md` — the signature routing table with role,
  decision made, SLA, escalation, and sequence.
- `briefing-outputs.md` — the internal briefing outputs (board,
  audit-committee chair, CEO, all-hands) with drafter, signer,
  distributor, and timing.
- `nca-engagement-plan.md` — the four-stage post-filing engagement
  plan with head's and architect's actions at each stage.

## Acceptance criteria

- Every sign-off in the flow has a named role, a **specific
  decision** the signer makes (not "review" or "approve" in the
  abstract), a **stated SLA**, and an **escalation path** if that
  signer is unavailable inside the SLA.
- The runbook is **executable without further clarification** by a
  reader who was not present for the drafting session. A named
  delegate picking it up cold has enough to run it.
- Every artefact the runbook produces has a **named template** —
  either the NCA's published format where one exists, or the
  enterprise's own internal template named by filename or
  document ID. No artefact is left as "we will draft the format
  when needed."
- The GC hand-off is drawn explicitly at every step where legal
  interpretation is required — meeting the Article 3(49)
  definition, characterising the triggering paragraph of Article
  73, wording that touches parallel obligations (GDPR Article 33,
  sector-regulator incident regimes), and any statutory
  characterisation offered to the NCA in follow-up engagement.
- The hypothetical scenario is clearly labelled as such and is
  not confusable with a real event at the enterprise or in the
  public record.
- Every point where the drafter is uncertain of statutory wording
  is marked `needs-research` inline rather than paraphrased
  around.

## Stretch goals

- Author a **table-top exercise script** the head can run with the
  CxO peer group (CEO, GC, CISO, DPO, CRO, Comms lead, Government
  Affairs lead, architect) that exercises the runbook end-to-end
  against a hypothetical scenario, with an injects timeline, a
  facilitator brief, and a debrief-capture template.
- Author a **variant runbook** for a named non-EU sector-regulator
  incident-reporting regime — for example the UK FCA operational-
  incident reporting duty, the US NYDFS cyber-incident reporting
  regime, the Singapore MAS technology-risk incident-notification
  requirement, or an equivalent regime for the sector you are
  authoring against. Name the specific regime; do not draft
  against a generic "sector regulator." Mark `needs-research` on
  any specific reporting-window or format detail you are not
  confident of.
- Draft the **regulator-facing cover letter** template that
  accompanies the opening filing — the head's personal
  positioning of the filing rather than the mechanical form data —
  in a form GC will pass without material redraft.

## Notes and starter guidance

- The runbook is not a policy document. Policies say what the
  enterprise commits to. This runbook says what the head does, in
  order, with what artefacts and what sign-offs, when Article 73
  is triggered. If the draft starts reading like a policy, cut it
  back to imperatives.
- The most common failure mode in a first-cut runbook is
  under-specified sign-off. "Head signs; GC reviews" is not a
  runbook — it is a placeholder. Push each sign-off to the
  specific decision the signer owns (does this event meet the
  Article 3(49) definition; is the technical account accurate;
  does this event move the enterprise risk position; is this
  reputationally significant enough to require CEO sign-off).
- The head has to be able to recite the three Article 73
  timelines without looking them up. The one-pager is a memory
  aid, not a substitute. If the drafter finds themselves
  paraphrasing the timelines because they are not sure of the
  exact wording, mark `needs-research` and verify against
  Regulation (EU) 2024/1689 before circulating the runbook.
- The hypothetical scenario for the seven-question worked pass
  should be chosen to stress-test the runbook, not to be easy.
  Pick a scenario where the causal-link determination is not
  obvious, or where the affected-population question is
  contested, or where the timeline paragraph in play is arguable.
  The runbook that only handles the easy scenario is the runbook
  that fails on the day.
- Every step where the head might be tempted to freelance across
  the legal-interpretation line under pressure is a step that
  needs GC drawn in the runbook explicitly. Chapter 07 of this
  module extends this boundary; the runbook cites it rather than
  restating it.
- Keep the runbook itself short and dense. A leadership runbook
  that reads as a fifty-page document is a runbook nobody opens
  when the event lands. The supporting artefacts can be longer;
  the runbook proper is the executable spine.
