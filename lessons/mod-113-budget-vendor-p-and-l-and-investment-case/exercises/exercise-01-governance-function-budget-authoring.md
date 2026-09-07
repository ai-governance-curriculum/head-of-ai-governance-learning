# exercise-01: Governance Function Budget Authoring

**Estimated effort:** 2 hours

## Objective

Author the **three-year rolling budget model** for the enterprise's
AI-governance function against the nine cost categories authored
in chapter [01-governance-function-budget-line](../01-governance-function-budget-line.md).
The model carries year-1 line-item detail (specific lines,
specific quantities, per-line defence), year-2 committed
trajectory (line-item shape at less granularity but with
substantive per-line movement and ratified target), and year-3
planning trajectory (higher-level shape as the trajectory the
function is on). Every line carries the four-component defence-of-
ask — first-order justification, peer-benchmark reference (or the
explicit absence of one), growth driver, and compression cost —
and every line carries a multi-year trajectory rather than a
year-1-only detail with year-2/year-3 as inflation-plus-X.

The deliverable is the artefact the head takes to the CFO in the
Q4 budget-authoring cycle, the artefact the CFO's business-partner
finance lead reads for coherence and models against in the
enterprise's own FP&A machinery, the artefact the CAE reads for
the external-audit-fee coordination, the artefact the procurement
category managers work against on the vendor-renewal cadences,
and the artefact the audit committee reads (through the CFO's
disclosure) as evidence the function is being run as a business
rather than as a queue of asks.

The model has to survive three stress tests. First, the
**compression pressure test** — the CFO opens the cycle with a
posture of "trim 15% off the aggregate" and the head has to
walk the CFO through the specific compression cost per line
without defaulting to "the function fails" on every line. Second,
the **portfolio-growth-outrun test** — the CFO's FP&A analyst
asks how the model handles the case where the enterprise's AI
portfolio grows twice as fast as the ratified year-2 shape
contemplated, and the head has to answer with the specific
growth-driver mechanism and the specific re-baselining trigger
rather than with a promise of good-faith reforecasting. Third,
the **hostile-audit-committee test** — a newly-seated audit-
committee member with an internal-audit background asks the CFO
why the incident-response reserve exists at all given the
enterprise's low historical AI-incident rate, and the head has
to have equipped the CFO with the specific answer that
distinguishes the retainer that unlocks the reserve from the
contingent reserve capacity itself.

The model is the head's substantive negotiating instrument
across the enterprise's own annual cost-authoring calendar; it
is the substrate every other artefact in this module sits on
top of.

## Prerequisites

- Chapter [01-governance-function-budget-line](../01-governance-function-budget-line.md)
  — the multi-year budget model shape, the nine cost categories,
  the line-item defence discipline, the budget-cycle calendar,
  the upstream and downstream interfaces, and the seven anti-
  patterns the head does not permit — read and internalised.
- Sibling chapters [02-multi-year-investment-case](../02-multi-year-investment-case.md)
  through [08-caio-and-cxo-budget-envelope-coordination](../08-caio-and-cxo-budget-envelope-coordination.md)
  skimmed so the head understands which artefacts sit on top of
  this exercise's model and which do not.
- [[mod-108-leading-the-governance-function]] chapter 02 (the
  multi-year hiring plan) because the plan is the substantive
  source for the headcount line-items and the year-2 / year-3
  headcount trajectory. The exercise inherits the plan's
  trigger-contingent shape rather than re-authoring it.
- [[mod-108-leading-the-governance-function]] chapter 03 (the
  coaching-and-career-pathing cadence) because the specific
  development plans against named team members are the
  substantive source for the training-and-certification line-
  items.
- [[mod-107-program-measurement-and-maturity]] chapters 01 and
  03 because the KRI/KPI portfolio and the maturity trajectory
  are the growth-driver substrate the head reads to defend the
  multi-year trajectory.
- [[mod-105-regulatory-change-management]] chapter 01 for the
  regulatory-trigger signals that drive year-2 and year-3 line-
  item movement across the assurance, training, and headcount
  categories.
- [[mod-110-incident-leadership]] because the incident-response
  reserve funds the retainer-and-reserve pairing that module
  develops, and because the incident-load history is the
  growth driver on the reserve line.
- The enterprise-context one-pager from the head's own
  onboarding artefact (or the exercise-01 context artefact
  from [[mod-108-leading-the-governance-function]]) as the
  input the model's specifics inherit — sector, jurisdictional
  footprint, AI portfolio scope, maturity stage, and audit-
  committee risk-appetite disposition.

## Steps

1. **Inherit the enterprise context.** Confirm the enterprise-
   context one-pager is current and reference it. The model's
   specifics — the headcount composition, the vendor-category
   mix, the assurance-body engagement pattern, the training
   cohort shape — depend on the sector, jurisdictional
   footprint, AI portfolio scope, maturity stage, and audit-
   committee risk-appetite disposition on the one-pager.
   Where the one-pager carries a `<!-- needs-research -->`
   marker the head has not yet resolved, carry the marker
   through into the model rather than filling in a placeholder
   the CFO will discover.

2. **Author the year-1 headcount line.** Consume the year-1
   headcount detail from the multi-year hiring plan
   ([[mod-108-leading-the-governance-function]] chapter 02).
   For each named position on the plan, populate the specific
   headcount sub-lines the model carries — salary, employer
   taxes and benefits, equity and variable, recruiter fees
   where applicable, and the position's share of the backfill
   reserve. Do not re-author salary bands; consume the
   enterprise's own compensation-band structure and carry
   `<!-- needs-research -->` markers where the specific band
   is not yet available. Read the composition explicitly — the
   proportion of level-15 through level-60 — so the CFO reads
   the headcount cost as a composition of levels rather than
   as a flat FTE count.

3. **Author each of the eight remaining cost categories with
   per-line detail.** Walk the categories in the order the
   chapter enumerates them — GRC-for-AI vendor spend, AI-
   observability vendor spend, AI-runtime security vendor
   spend, external assurance and audit spend, tooling
   depreciation, training and certification, incident-response
   reserve, and external-benchmarking-and-community-leadership.
   For each category:
   - Enumerate the specific line-items the chapter names for
     the category (the platform licence, the implementation
     cost, the growth-in-usage escalators, and so on).
   - Author each line with placeholder specifics the head can
     defend once the enterprise's own procurement and vendor-
     P&L data are wired in, or with `<!-- needs-research -->`
     markers where the specific figure genuinely depends on
     data the head does not yet carry.
   - Name the category-specific interface (the CISO's team
     for runtime-security, the CAE for external-audit-fee
     coordination, procurement's category manager for the
     technology-vendor categories, HR for headcount) so the
     line-item ownership is legible.

4. **Author the year-2 committed trajectory per line.** For
   each line in the year-1 detail, author the year-2 shape.
   The year-2 shape is at less line-item granularity than
   year-1 but carries substantive per-line movement — the
   direction (growth, hold, compression), the magnitude
   (small / moderate / material), and the specific mechanism
   driving the movement. Where the year-2 shape depends on a
   trigger-contingent event (a hiring-plan trigger firing,
   a regulatory obligation moving from horizon-scanned to
   in-force, a vendor contract's multi-year term rolling to
   renewal, a maturity-model transition ratified with the
   CRO), name the trigger explicitly. The year-2 shape is
   what the CFO ratifies at the previous cycle; the head
   authors it substantively rather than as inflation-plus-X.

5. **Author the year-3 planning trajectory per line.** For
   each line, author the year-3 shape at higher-level
   granularity than year-2. The year-3 shape is the
   trajectory the function is on and the shape the CFO can
   plan against, with the explicit understanding that year-3
   detail will emerge as year-3 becomes year-2 in the next
   cycle. Name the trajectory-shaping assumptions the year-3
   shape depends on — the AI portfolio's expected inference-
   volume growth, the regulatory-horizon events on the
   horizon-scanning artefact, the ISO/IEC 42001 re-certification
   year cadence, the incident-load baseline the reserve is
   sized against — so the year-3 shape is defensible rather
   than aspirational.

6. **Author the four-component defence per line.** For every
   line in year-1, year-2, and year-3, author the four-
   component defence-of-ask:
   - **First-order justification** — regulatory, contractual,
     risk-appetite, or strategic-imperative — with the specific
     source authority the justification rests on.
   - **Peer-benchmark reference** — with the specific
     benchmarking source (a named exchange, a named
     professional-body publication, a named consulting-firm
     study, a named regulator publication) where a defensible
     benchmark exists, or with an explicit named absence
     where one does not. Never fabricate a benchmark; carry
     a `<!-- needs-research -->` marker where the benchmark
     is nominally available but the head has not yet run
     the specific query.
   - **Growth driver** — the specific mechanism (AI portfolio
     growth, regulatory change, incident-load history,
     maturity trajectory) that drives the line's year-over-
     year trajectory, with the specific input signal (the
     KRI/KPI, the horizon-scanning artefact, the incident
     register, the maturity-assessment output) the head reads
     to detect the driver firing.
   - **Compression cost** — the specific capability that
     breaks at 10%, 25%, and 50% compression on the line.
     Refuse the reflexive "the function fails" answer on
     every line; author the specific consequence per band.

7. **Run the compression pressure test.** With the model
   authored, simulate the CFO opening the cycle with a
   posture of "trim 15% off the aggregate". Walk each of the
   nine categories in turn and author the specific compression
   posture the head takes — which lines the head volunteers
   for compression (typically because the compression cost
   is genuinely modest at the requested band), which lines
   the head refuses to compress (with the specific
   compression cost as the refusal's substance), and which
   lines the head offers to re-baseline conditionally on a
   trigger not firing. The output is a `compression-scenarios.md`
   artefact the head can walk the CFO through line by line
   rather than reflexively defending the aggregate.

8. **Run the portfolio-growth-outrun test.** Simulate the
   CFO's FP&A analyst asking how the model handles the case
   where the AI portfolio grows twice as fast as the year-2
   shape contemplated. Walk the model's growth-in-usage
   escalators (the observability data-volume escalator, the
   GRC platform's per-AI-system charge, the runtime-security
   licence's per-model-deployment charge, the assurance
   category's per-scope-expansion fee), author the specific
   re-baselining trigger (the specific portfolio-size
   threshold on the AI system inventory, the specific
   inference-volume threshold on the observability platform,
   the specific incident-rate threshold on the incident
   register) that fires a mid-year re-baselining
   conversation, and author the pre-negotiated contingent
   authorisation shape so the head does not have to reopen
   the budget cycle from a green field when the trigger
   fires. Output is a `growth-trigger-map.md` artefact.

9. **Run the hostile-audit-committee test.** Simulate a
   newly-seated audit-committee member with an internal-audit
   background challenging the CFO on why the incident-response
   reserve exists at all. Author the specific answer that
   distinguishes the retainer that unlocks the reserve (the
   modest recurring cost that maintains the DFIR, external-
   counsel, and crisis-communications capacity ready to
   engage in hours) from the contingent reserve capacity
   itself (the authorised draw the CFO's finance team has
   budgeted against). Author the composition with
   [[mod-110-incident-leadership]] so the audit-committee
   member reads the reserve as the substantive incident-
   preparedness posture the module develops rather than as
   discretionary contingency. Output is a
   `reserve-defence-brief.md` artefact the head briefs the
   CFO with ahead of the audit-committee cycle.

10. **Author the line-item defence discipline artefact and
    the failure-mode audit.** Consolidate the four-component
    defence per line into a `line-item-defence.md` artefact
    the head can walk any interlocutor through on demand.
    Then author the failure-mode audit — one paragraph per
    anti-pattern the chapter names, with the specific
    detection signal and specific recovery action per
    anti-pattern:
    - Line-item-first with no model.
    - Vendor-spend abdication to procurement.
    - One-year horizon posture.
    - Absent incident reserve.
    - Community-and-training soft-cut pattern.
    - Budget-as-inflation defence.
    - Disclosure-cycle-only forecast posture.
    The audit is the head's discipline against the head's
    own drift; the head runs it at each Q4 authoring cycle
    and at the mid-year refresh.

## Deliverables

- `budget-model.md` — the multi-year rolling budget model
  itself. Rows are the nine cost categories and their line-
  items; columns are year-1 (detailed), year-2 (committed
  trajectory), and year-3 (planning trajectory). Where
  quarterly granularity matters within year-1 (typically for
  vendor renewals, ISO/IEC 42001 audit cycles, and the CFO's
  own quarterly refresh cadence), the model carries the
  quarterly detail; elsewhere annual detail suffices.
- `line-item-defence.md` — the four-component defence-of-ask
  (first-order justification, peer-benchmark reference,
  growth driver, compression cost) per line, walkable end-
  to-end.
- `compression-scenarios.md` — the compression pressure test
  output. Per line, the head's compression posture at 10%,
  25%, and 50% compression bands, with the specific
  capability consequence per band.
- `growth-trigger-map.md` — the portfolio-growth-outrun test
  output. The specific re-baselining triggers, the specific
  input signals the head reads to detect them firing, and
  the pre-negotiated contingent authorisation shape.
- `reserve-defence-brief.md` — the hostile-audit-committee
  test output. The retainer-versus-reserve distinction, the
  composition with [[mod-110-incident-leadership]], and the
  specific briefing the head equips the CFO with.
- `interfaces-map.md` — the upstream and downstream
  interfaces the model runs against (CFO's finance business-
  partner, procurement's category managers, HR, CAE, audit
  committee), with the specific substantive contact per
  interface and the cadence the head engages the interface at.
- `budget-cycle-calendar.md` — the head's annual calendar
  against the enterprise's own CFO cycle (Q4 authoring,
  mid-year refresh, quarterly refresh, mid-year re-baselining
  triggers), with the specific artefact the head brings to
  each window and the specific decision the head takes out
  of each window.
- `failure-mode-audit.md` — the seven anti-pattern detection-
  and-recovery paragraphs.
- `research-registry.md` — the enumerated `<!-- needs-research -->`
  markers carried in the model, with the specific data source
  the head will consult to resolve each marker and the
  cadence the head will refresh the marker on.

## Acceptance criteria

- Every line-item in the model has all three year columns
  populated (year-1 detail, year-2 committed, year-3
  planning). A line with year-1 detail and year-2/year-3 as
  "TBD" or blank fails the criterion — the model is the
  multi-year negotiating instrument and cannot carry year-2
  or year-3 as a hole.
- Every line-item carries all four components of the defence-
  of-ask (first-order justification, peer-benchmark reference
  or explicit absence, growth driver, compression cost). A
  line with a blank component fails the criterion; a line
  whose peer-benchmark reference is fabricated fails
  emphatically — the head resolves the absence with a
  `<!-- needs-research -->` marker rather than inventing.
- Every year-2 and year-3 line-item movement carries a
  specific mechanism (a specific trigger event, a specific
  KRI/KPI trajectory, a specific vendor-contract term
  structure, a specific maturity-model transition). A line
  whose year-2 movement reads as "3% inflation" or "same as
  last year plus growth" fails the criterion — the chapter's
  budget-as-inflation anti-pattern is what the criterion
  refuses.
- Every line-item's compression cost is specific at each of
  the 10%, 25%, and 50% bands. A line whose compression cost
  is "the function fails" at every band fails the criterion;
  the reflexive answer is what the CFO discounts and what
  the discipline replaces.
- The nine cost categories are all populated. A model that
  omits the incident-response reserve, or the external-
  benchmarking-and-community-leadership category, or the
  tooling depreciation category fails the criterion —
  omitting a category signals the head has adopted a
  chapter-refused posture (absent-reserve, community-and-
  training-soft-cut, or line-item-first-with-no-model).
- The compression pressure test output enumerates the head's
  specific posture per line at each of the three compression
  bands. A "trim across the board pro rata" posture fails
  the criterion — the discipline is per-line substantive
  engagement with the trade-off, not proportional
  compression.
- The portfolio-growth-outrun test output enumerates specific
  re-baselining triggers with specific measurable signals.
  A trigger authored as "if the portfolio grows a lot" fails
  the criterion; the trigger has to be a specific measurement
  on a specific input signal.
- The reserve-defence-brief distinguishes the retainer from
  the contingent reserve capacity explicitly and composes
  with [[mod-110-incident-leadership]] as the substantive
  incident-preparedness posture. A defence that reads the
  reserve as generic contingency fails the criterion.
- The failure-mode audit names, for each of the seven anti-
  patterns the chapter enumerates, at least one specific
  detection signal and one specific recovery action.
- Any factual claim about a vendor's specific fee structure,
  a specific accredited certification body's fee schedule, a
  specific benchmarking exchange's per-participant fee, or a
  specific credential program's cohort tuition carries a
  `<!-- needs-research: verify [specific fact] against [named
  source] -->` marker where the fact is not independently
  verifiable. The chapter itself carries such markers around
  ISO/IEC 42001 CB fees, IFRS and US GAAP treatment of SaaS
  implementation costs, and incident-reserve sizing; the
  exercise inherits the discipline.

## Stretch goals

- Author the **CFO-facing budget-cycle pack** — the specific
  two-page pack the head takes to the CFO in the Q4
  authoring window. The pack compresses the model into: the
  year-1 aggregate against the previous cycle's authorised
  budget line, the year-2 committed shape as ratified at the
  previous cycle and any material deltas the head is
  raising, the year-3 planning shape as the trajectory the
  CFO is being asked to plan against, the head's specific
  asks per category (the year-1 authorisation, the year-2
  contingent authorisations, the reserve authorisation, and
  any classification decisions the head is asking the CFO's
  finance team to ratify), and the three stress-test
  postures the head has run the model through. The pack is
  what the CFO reads before the head is in the room; the
  head does not walk the CFO through the full model in the
  window.
- Author the **procurement-category-manager pack** — the
  specific brief the head hands to procurement's technology-
  vendor and professional-services category managers ahead
  of the vendor-renewal cadences. The pack carries the head's
  substantive view on each vendor category (what the category
  purchases, what the acceptable price movement is at
  renewal, what the substantive capability question is at
  renewal), the head's escalation posture on renewals that
  fall outside the acceptable band, and the head's request
  for the category managers' own market intelligence on
  peer-enterprise renewals in each category.
- Author the **audit-committee disclosure support brief** —
  the specific brief the head prepares for the CFO ahead of
  the audit committee's annual budget disclosure cycle. The
  brief does not disclose line-item detail (that is the
  CFO's disclosure); it equips the CFO with the specific
  answers to the substantive audit-committee questions the
  brief anticipates — the reserve question, the assurance-
  mix question, the community-leadership question, the
  training-and-certification question, and the vendor-
  concentration question.
- Draft the **classification-decision case** — a specific
  case study in which the head negotiates the capex-vs-opex
  classification of a specific vendor implementation with
  the CFO's finance team. Walk the substantive input the
  head brings (a faster implementation with more expensed
  cost in year-1 versus a phased implementation with more
  capitalised cost amortised over years 2-5), the CFO's
  finance team's authority (the classification decision
  itself is theirs, not the head's), and the audit-committee
  surfacing where the classification materially changes the
  year-1 cost profile the committee is reading.
- Author the **third-year retrospective template** — the
  short template the head will run at the end of year-3 to
  assess whether the model's ratified year-2 shape held,
  which lines moved outside the ratified shape and why,
  which growth-driver mechanisms fired as authored and which
  did not, and what the year-4 planning shape should look
  like given the trajectory data. The retrospective is the
  discipline that turns the model from a cycle artefact into
  a living instrument.

## Notes and starter guidance

The most common first-cut failure is a model that authors
year-1 at line-item fidelity and treats year-2 and year-3 as
inflation-plus-X. Inflation is a placeholder the head has
substituted for substantive per-line trajectory reasoning, and
the CFO reads it correctly as absence-of-thought — the CFO's
FP&A analyst will run their own inflation-plus-X model at less
cost than the head's, and the head's version adds nothing to
the conversation. Force the growth-driver discipline. Every
line's year-over-year movement is driven by a specific
mechanism — the AI portfolio's inference-volume growth, a
specific regulatory obligation coming into force, an incident-
load rise past a specific threshold, a maturity-model
transition ratified with the CRO — and the head names the
mechanism rather than defaulting to inflation. The line whose
mechanism the head genuinely cannot name is the line the head
has authored without substance and the line the CFO will
compress first.

The second common failure is the model that treats vendor
categories as procurement's problem. The head enumerates a set
of vendor line-items, hands the specific renewal negotiations
to procurement's category managers, and never opens the vendor
categories as a portfolio the head substantively engages with.
The vendor categories drift — capabilities compress at renewal
because procurement's category-management posture defaults to
compress-the-line-item, price increases get accepted where they
should be resisted and resisted where they should be accepted,
and the function's tooling posture erodes invisibly. Force the
substantive-engagement discipline. The head reads the vendor
category as a portfolio, brings the substantive view on what
the category purchases to procurement's category managers, and
runs the vendor-P&L discipline sibling chapters
[03](../03-grc-for-ai-vendor-pnl.md) through
[06](../06-assurance-body-relationship-pnl.md) develop as the
head's own substantive workstream.

The third common failure is the compression pressure test the
head has not rehearsed. The CFO opens the cycle with a
compression posture — 10%, 15%, sometimes 25% at the aggregate
— and the head who has not rehearsed the specific per-line
compression cost defaults to the reflexive "the function
fails" answer on every line. The CFO discounts the reflexive
answer immediately and compresses on the lines the head has
not defended substantively — typically training, community
leadership, and the incident reserve, because those are the
lines the head has treated as discretionary in the model's
own authoring. Force the specific per-line compression cost.
At 10% compression on training, the specific level-35
evaluator's specific ISO Lead Implementer track slips this
year and the CB audit reads the qualification gap as a
finding; at 25% compression on the incident reserve, the DFIR
retainer cannot be maintained and the incident-response
window extends from hours to weeks. The specific answer is
what the CFO reads as substantive engagement with the trade-
off.

On the incident-response reserve — the temptation is to treat
the reserve as a single line and to author its defence
generically. The chapter is explicit that the reserve has two
shapes running together: the retainer that unlocks it (a
modest recurring cost that maintains DFIR, external-counsel,
and crisis-communications capacity ready to engage in hours)
and the contingent reserve capacity itself (the authorised
draw the CFO's finance team has budgeted against). A head who
budgets the reserve capacity but not the retainer will
discover in the incident that the retainer's absence turns the
reserve into an unusable balance-sheet entry; a head who
budgets the retainer but not the reserve capacity has to open
an emergency-spend authorisation on incident declaration the
CFO reads as absence-of-planning. Author both shapes explicitly,
compose with [[mod-110-incident-leadership]] as the substantive
incident-preparedness posture the reserve funds, and equip the
CFO with the retainer-versus-reserve distinction ahead of the
hostile-audit-committee question the module's chapter warns
about.

The model is a live artefact, not a cycle document. Version
it, date it, refresh it at each substantive-change cadence —
a material vendor renegotiation, a material regulatory change,
a material incident that has drawn the reserve, a material
change in the AI portfolio's shape — and carry a running
narrative of what has changed and why. The CFO can and will
ask the on-demand question at an audit-committee or board
cycle three weeks after a material change, and the head who
has to scramble to update the model is the head who has
authored it as a paperwork exercise. The head who runs the
model as a live P&L is the head the CFO reads as running the
function as a business rather than as a queue of asks.
