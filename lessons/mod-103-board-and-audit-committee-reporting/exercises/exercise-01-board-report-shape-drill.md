# exercise-01: Board Report Shape Drill

**Estimated effort:** 3 hours

## Objective

Produce a defensible **quarterly board AI-risk pack template**, plus
a worked example of the pack for one hypothetical (or actual)
quarter, for the enterprise you would run — or already run — the
program at. The pack has to answer the three board questions from
chapter 01 in order, structure the seven content clusters, and be
comparable across quarters if archived and re-read six months later.

The deliverable is not "notes about what the board should see." It
is the template the head would put in front of the board next
cycle, plus a worked one-quarter instance the head could defend to
the audit-committee chair as a first cut.

## Prerequisites

- Chapter [01-board-report-shape](../01-board-report-shape.md) read
  and internalised.
- The running-program artefacts from [[mod-102-running-the-program]]
  — specifically the risk-register cadence (chapter 03), the
  AI system inventory (chapter 06), and the AI supply-chain
  evidence discipline (chapter 07) — in view. Where these are
  hypothetical for the enterprise you are working against, hold a
  working assumption.
- A concrete enterprise in mind, with an assumed sector (banking,
  insurance, health, pharma, public sector, frontier lab, tech
  platform, industrial) and a board reporting-line configuration
  (mod-101 chapter 06).

## Steps

1. **Enterprise context one-pager.** Write a half-page setting the
   context the pack will operate against: sector, jurisdictional
   footprint, approximate AI portfolio scale (systems in
   inventory, by capability tier if you are running tiers),
   dominant regulator regimes, and the current appetite framework
   in force (from mod-102 chapter 03). This is the scenario for
   the drill; every subsequent artefact refers back to it.
2. **Pack template — seven-cluster shape.** Author the template
   with the seven content clusters from chapter 01
   (appetite-and-heat-map, KRI dashboard, incident summary,
   regulator engagement, third-party status, regulatory change
   and maturity, decisions requested). For each cluster, specify:
   the specific artefacts it contains, the length budget in
   pages, the layout convention (heat map, table, prose,
   dashboard), and the cross-references to other clusters.
3. **KRI dashboard cut.** Draft the specific KRI list the
   dashboard will carry. Each KRI has: a one-line definition; a
   producer (the function or system of record from which the
   value is drawn); a threshold band structure (green / amber /
   red or the equivalent from your CRO's framework); a trend
   representation. Aim for eight to twelve KRIs, no more —
   dashboards that carry twenty KRIs are dashboards no board
   reads.
4. **Worked one-quarter pack.** Draft a worked example of the
   pack for one hypothetical quarter. Populate each cluster
   at the depth the template requires. The heat map has cell
   counts and captions; the KRI dashboard has values and trends;
   the incident summary has at least one incident at the
   template's full depth; the regulator engagement summary has
   at least one active engagement; the third-party cluster shows
   concentration; the decisions-requested cluster has at least
   one specific ask (or an explicit no-ask statement).
5. **Comparability discipline.** Author the short (one-page)
   discipline that keeps the pack comparable across quarters —
   which fields do not change without formal rationale, how KRI
   definition changes are tabled, how heat-map cell definitions
   are versioned, how archived packs are locked. See chapter 01
   on archive comparability.
6. **Three-board-question test.** Read your worked pack back
   against the three board questions from chapter 01 (has risk
   moved and is it inside appetite; where are we exposed; what
   decisions are requested). Annotate each cluster with the
   question(s) it answers. Any cluster that answers none is
   either cut or rewritten.

## Deliverables

- `enterprise-context.md` — the scenario one-pager.
- `board-pack-template.md` — the seven-cluster template with
  artefacts, length budgets, layout conventions, and cross-
  references per cluster.
- `kri-dashboard.md` — the KRI list with definitions, producers,
  thresholds, and trend representations.
- `worked-quarter-pack.md` (or `.pdf`) — the populated worked
  example.
- `comparability-discipline.md` — the archive-and-comparability
  one-pager.
- `three-question-annotation.md` — the mapping of clusters to
  board questions with any cluster changes flagged.

## Acceptance criteria

- The seven clusters are present with concrete content
  specifications, not headers with "TBD."
- Every KRI on the dashboard has a producer named — a role or a
  system of record, not "TBD" or "various."
- Every heat map cell has a caption; every KRI has a trend;
  every incident has reportability status; every regulator
  engagement has a next-action-by-date; every decision requested
  has an owner and a review trigger.
- The comparability discipline is specific enough that an
  incoming head reading the archive six months later can tell
  whether a change was formally tabled.
- The three-question annotation shows every cluster mapping to
  at least one of the three board questions. Clusters mapping to
  none are cut or rewritten before submission.

## Stretch goals

- Author the monthly-delta shape — the one-page written update
  between formal quarters — with the exact fields it carries and
  the distribution list. Chapter 01 flags monthly deltas as the
  common heavier-regulated-enterprise cadence.
- Draft the addendum shape (from chapter 05 of this module) for
  a material event between evidence-lock (T-7) and distribution
  (T-0). Include one worked addendum.
- Produce the pack in a form directly importable into whichever
  GRC-for-AI platform the enterprise has selected (Credo AI,
  Holistic AI, ModelOp, Monitaur, ServiceNow AI Control Tower,
  IBM watsonx.governance, or the actual platform), so the
  template is machine-parseable rather than only human-readable.
- Circulate the pack to a peer at head-of-role or audit-committee-
  chair level and incorporate one round of critique before
  submission.

## Notes and starter guidance

- Resist the urge to make the KRI list comprehensive. Every KRI
  costs the board attention; a KRI that never moves is a KRI
  that has been retained past its useful life. Cut aggressively.
- The most common failure of a first-cut board pack is that it
  reads like an internal ops report — everything the head's
  function does, presented as achievement. The pack is not about
  what the function did; it is about what the *risk position* is
  and what the board must know or decide.
- The worked quarter is where the template is stress-tested. If
  you find yourself unable to populate a cluster because the
  template did not tell you what belongs in it, the template is
  under-authored. Revise.
- Keep the pack under twenty pages including annexes. Board
  attention is finite; longer packs are read less carefully, not
  more.
