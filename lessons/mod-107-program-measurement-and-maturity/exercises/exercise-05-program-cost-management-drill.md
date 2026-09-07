# exercise-05: Program-Cost Management Drill

**Estimated effort:** 2 hours

## Objective

Author the enterprise's **AI-governance program-cost pack** and
the operating cadences that sit under it — the seven-category
cost breakdown, the monthly cost-review cadence with the
finance business partner, the quarterly variance review with
the CFO, and the annual-budget-cycle handoff. The deliverable is
the pack the head co-authors with the finance business partner,
the artefact the CFO's team consumes at monthly and quarterly
cadences, and the artefact that pairs with the ROI pack from
exercise 04 at the annual budget cycle.

The pack has to survive three stress tests. First, the finance
business partner picks up the pack and can reconcile every
line to the enterprise's general ledger. A line the finance
business partner cannot reconcile is a line the head has
authored outside the enterprise's system of record, and the
CFO's team learns not to trust the pack from that point
forward. Second, the CFO opens the quarterly variance review
and can read the composite spend against plan, the seven
categories, and the two or three variance stories in ten
minutes. A pack that requires the CFO to compute anything is a
pack that fails the credibility test. Third, the pack survives
a material incident that drives incident-response cost several
hundred percent over baseline in a single quarter — the
contingency discipline is authored so the head requests the
draw with the incident context and the projected total cost,
not with a general "please add more budget" ask.

The drill is not a study of chapter 05. It is the operating
artefact that turns chapter 05's seven-category discipline into
a living, ledger-anchored management pack the head runs the
program against.

## Prerequisites

- Chapter [05-program-cost-management](../05-program-cost-management.md)
  — the seven cost categories (headcount, vendor spend,
  tooling depreciation, external-audit cost, training cost,
  certification cost, incident-response cost), the finance-
  business-partner working interface (what the partner does,
  what the head does, what the head does not do), the monthly
  cost review shape, the quarterly variance review with the
  CFO, the annual budget cycle handoff, and the five anti-
  patterns (un-instrumented program, vacancy-as-savings,
  contingency-as-baseline, vendor-lock-in surprise, over-run
  by acquisition) — read and internalised.
- Chapter [04-roi-reporting-to-cfo](../04-roi-reporting-to-cfo.md)
  — the ROI pack pairs with this cost pack at the CFO
  conversation; the ROI-to-cost ratio requires the cost side.
- Chapter [01-kri-kpi-portfolio](../01-kri-kpi-portfolio.md)
  — metric 10 (cost-per-AI-system-governed) is the running-
  cadence signal the pack feeds; the pack's total-cost figure
  is the numerator.
- [[mod-102-running-the-program]] chapter 02 (AIMS operating
  calendar) — the monthly and quarterly cadences ride the
  operating calendar. Chapter 04 (regulatory crosswalk) —
  the certification-body relationship drives the external-
  audit cost line.
- [[mod-104-regulator-engagement]] chapter 04 (regulator-
  engagement inventory) — drives the external-audit cost line
  for regulatory examinations.
- [[mod-106-external-positioning-and-voluntary-codes]] chapter
  01 (voluntary-code register) — drives voluntary-code-
  signatory audit costs.
- [[mod-108-leading-the-governance-function]] — the source of
  the headcount category composition (levels, fully-loaded
  cost per FTE, structure).
- [[mod-110-incident-leadership]] — the incident register that
  drives the incident-response cost line.
- [[mod-112-certifications-career-path-community-leadership]]
  — the certification pathway that drives the certification
  cost line.
- [[mod-113-budget-vendor-p-and-l-and-investment-case]] — the
  full budget-authoring discipline and the vendor-P&L
  discipline the pack references.
- Exercise 01 (KRI/KPI portfolio design) already completed —
  metric 10 (cost-per-AI-system-governed) feeds from the pack.
  Exercise 04 (ROI modelling drill) already completed — the
  ROI pack pairs with this pack at the annual budget cycle.
- The concrete enterprise from exercises 01, 02, and 04 —
  sector, jurisdictional footprint, AI system portfolio scope,
  team structure, existing GRC-for-AI stack, existing
  certification-body relationship. If the enterprise has a
  named finance business partner, name them (as a role, not a
  person); if not, name the role the head is asking the CFO
  to designate.

## Steps

1. **Reuse the enterprise context one-pager from exercises 01,
   02, and 04.** Add a short cost-scope note naming the
   enterprise's team structure (levels, headcount by level),
   the current GRC-for-AI stack under contract, the current
   certification-body relationship (ISO/IEC 42001 status —
   pre-cert, in-cert, certified with surveillance year, re-
   certification year), the current voluntary-code signatory
   status ([[mod-106-external-positioning-and-voluntary-codes]]
   chapter 01), and the finance-business-partner assignment.
   The context is what determines the pack's category
   depth; a health-sector enterprise with an active FDA GMLP
   posture has a different external-audit surface than a
   fintech serving retail consumers.

2. **Author the model shell in the enterprise's financial
   convention.** As with exercise 04, adopt the enterprise's
   financial-modelling conventions from the start — variance
   thresholds (typically ±5% on a line or ±10% on a category
   triggers commentary; the enterprise's specific convention
   is set by the finance business partner), currency and
   rounding conventions, source-data linkage patterns (each
   line links to the general-ledger account it reconciles
   to), and the plan-versus-forecast-versus-actual discipline.

3. **Author each of the seven category templates.** For each
   of the seven categories, author the template the pack uses:
   - **Headcount.** Structure (levels the enterprise staffs —
     level 60, level 50, level 40, level 25–35, level 15 per
     [[mod-108-leading-the-governance-function]]), fully-
     loaded cost per FTE (salary + benefits + payroll tax +
     workspace allocation + equipment + training baseline —
     the finance business partner maintains the figures),
     utilisation reporting (fraction on program-critical work
     versus overhead), and the vacancy discipline (vacancy as
     a delivery risk, not a positive variance).
   - **Vendor spend.** The GRC-for-AI stack (policy
     management, control testing, evidence capture, incident
     tracking, audit management) as annual subscription with
     multi-year commitment; adjacent tooling (AI-evaluation
     platforms, data-lineage and model-provenance tools,
     third-party-risk-management tools with AI-specific
     configurations); professional-services engagements
     (external consultancy, external SME retainers, outside
     counsel on AI-specific matters). Every vendor line names
     the contract start date, the contract term, the renewal
     date, and the notice period — the vendor-lock-in
     surprise anti-pattern is defended against by the
     calendar visibility.
   - **Tooling depreciation.** Capitalised tooling investments
     amortised over useful life. The head does not author the
     capitalisation posture — the CFO's team does, per the
     enterprise's asset-accounting policy — but the head
     understands the multi-year cost impact before approving
     each capital investment. Name each depreciating asset
     with its capitalisation date, useful life, and annual
     depreciation.
   - **External-audit cost.** ISO/IEC 42001 certification cost
     (initial certification, annual surveillance, three-year
     re-certification), sector regulatory-examination cost,
     independent-audit cost under IAAIS or comparable
     programmes, voluntary-code signatory audit cost. Name
     each engagement with the audit date, the audit body,
     the expected cost, and the bundle opportunity (an ISO
     42001 surveillance audit run in parallel with an ISO
     27001 audit at the same certification body can reduce
     combined cost).
   - **Training cost.** Team training (per-FTE annual
     training baseline plus specific one-time expenses),
     enterprise-wide AI-governance training (workforce
     training, role-based deeper training, delivery mode
     costing), CxO peer and board-director training.
   - **Certification cost.** Individual certifications (IAPP
     AIGP for program managers and analysts, ISACA CDPSE for
     adjacent roles, security certifications for security-
     adjacent architects, cloud-provider AI certifications for
     engineering-adjacent staff) with exam fees, study
     material, retake budget, CPE maintenance; enterprise-
     level certifications (ISO/IEC 42001 maintenance under
     external-audit, sector certifications like HITRUST where
     applicable).
   - **Incident-response cost.** Baseline (prior-year incident
     volume and severity) plus contingency (drawable on
     specific incident escalation). Line components on a
     material incident: external counsel (often the largest
     line), external technical experts, regulator engagement
     cost, notification and disclosure cost, business-impact
     cost where booked to the AI-governance budget rather
     than the affected business line.
   Each category template names its plan line, its actual
   line, its variance-computation formula, and its variance-
   commentary trigger threshold.

4. **Author the finance-business-partner interface.** Author
   the joint operating shape — what the finance business
   partner does (owns actuals data, accounting posture,
   enterprise financial-modelling conventions, interface into
   the CFO's own tools), what the head does (owns substantive
   interpretation of variances, strategic-response decisions
   when reallocation is required, CFO-facing narrative), and
   what the head does not do (compute variances, format
   reports, produce actual figures). Chapter 05 is explicit
   that the head who runs their own finance function is the
   head who has not built the relationship the CFO expects.

5. **Author the monthly cost-review cadence.** Author the
   shape of the working meeting the head and the finance
   business partner run monthly:
   - Actuals against plan for each of the seven categories,
     at the line-item depth the enterprise's ledger supports.
   - Variance commentary for each category with a non-
     trivial variance.
   - Reforecast where a variance is material and expected to
     persist.
   - Reallocation requests where a variance requires moving
     budget between lines (small reallocations within the
     head's authority; larger require finance-business-
     partner concurrence; largest require CFO sign-off).
   - Contingency status (draw to date, remaining, forecast
     need).
   The monthly review is a working meeting, not a
   presentation. The output is a monthly cost note on a
   standing cadence to the CFO — read in most months
   passively, read closely in months where a variance
   warrants attention.

6. **Author the quarterly CFO variance review.** Author the
   shape of the quarterly presentation to the CFO:
   - Composite spend against plan for the quarter and year-
     to-date, in one line.
   - Seven categories in a table, with actual, plan,
     variance, and forecast for the year.
   - The two or three variance stories that matter — where
     the variance is material and the CFO needs to hold the
     story.
   - Reforecast for the balance of the year if applicable.
   - Specific asks — contingency draws, mid-year budget
     requests, mid-year vendor-contract renegotiations —
     phrased so the CFO can approve or challenge in the
     room.
   The presentation is short. The CFO's time is finite. A
   quarterly pack that reads as an activity summary rather
   than as a cost pack is the pack the CFO discounts.

7. **Author the annual budget cycle handoff.** Author how the
   cost pack feeds the annual budget cycle
   ([[mod-113-budget-vendor-p-and-l-and-investment-case]]):
   - Prior-year actuals as the baseline (a budget authored
     without the finance business partner's actuals is a
     budget authored against fiction).
   - Trajectory moves from the annual maturity assessment
     ([[03-annual-maturity-assessment]] and exercise 03)
     feed the incremental spend requests — a specific level-4
     target on a specific axis requires a specific investment,
     and the investment is a line item.
   - Multi-year commitments already in place (depreciation
     schedules, multi-year vendor contracts, external-audit
     cadences) baked into the base spend and not presented
     as discretionary.
   - The ROI pack (exercise 04) presented alongside — the
     CFO reads the two together.

8. **Author the incident-driven contingency-draw discipline.**
   Author the specific discipline for what happens when a
   material incident drives incident-response cost several
   hundred percent over baseline in a single quarter. Name the
   trigger threshold (a specific-value or a specific-percentage
   overrun), the notification path (the head to the finance
   business partner within a fixed window; the head to the
   CFO within a longer window; the head to the audit committee
   at the next scheduled cadence or an unscheduled interim
   note if the overrun is material), the contingency-draw
   request shape (incident context, projected total cost,
   remaining contingency, specific ask — draw, reallocation,
   or mid-year budget addition), and the reset discipline (how
   the baseline is re-negotiated the following year if the
   incident reveals a chronic under-budgeting of the
   contingency).

9. **Author the vendor-renewal calendar.** Author the specific
   calendar the head keeps of vendor-renewal dates — every
   vendor contract with a renewal date, a notice period, and a
   review-decision date that falls before the notice period
   expires. The calendar is what defeats the vendor-lock-in
   surprise anti-pattern. The full vendor-P&L discipline lives
   in [[mod-113-budget-vendor-p-and-l-and-investment-case]];
   the calendar is the operating artefact that surfaces
   renewal decisions to the head in time to make them.

10. **Author the failure-mode audit.** Author a short section
    — one paragraph per failure mode — naming how the pack
    detects and recovers from each of these failure modes:
    - The un-instrumented program (chapter 05's headline
      anti-pattern): the head cannot say what has been spent
      because the finance business partner relationship was
      never built or the head runs shadow numbers in personal
      spreadsheets.
    - The vacancy-as-savings claim: vacancy reported as a
      positive budget variance without acknowledging the
      work-not-done cost, while the maturity plot's
      trajectory slips.
    - The contingency-treated-as-baseline pattern: the
      contingency is gradually reforecast into predictable
      spend, and when a material incident hits the contingency
      is depleted.
    - The vendor-lock-in surprise: a vendor contract renews on
      a multi-year commitment without the head's active
      engagement.
    - The over-run explanation by acquisition: variance
      explained by external drivers (peer institution
      incident, regulatory announcement, industry trend) only,
      without the enterprise's own decision path that
      produced the variance.

## Deliverables

- `cost-pack/README.md` — the pack overview: version,
  joint-authorship record, the seven-category discipline, the
  finance-business-partner interface, the monthly and
  quarterly cadences, the annual budget cycle handoff.
- `cost-pack/enterprise-context.md` — the cost-scope note
  (team structure, GRC-for-AI stack, certification-body
  status, voluntary-code signatory status, finance-business-
  partner assignment).
- `cost-pack/model-shell.md` — the enterprise's financial-
  modelling conventions applied (variance thresholds,
  currency and rounding, source-data linkage, plan-forecast-
  actual discipline).
- `cost-pack/01-headcount.md` — the headcount category
  template with structure, fully-loaded cost per FTE by
  level, utilisation reporting, vacancy discipline.
- `cost-pack/02-vendor-spend.md` — the vendor-spend category
  template with the GRC-for-AI stack, adjacent tooling,
  professional-services engagements, and the vendor-renewal
  calendar cross-reference.
- `cost-pack/03-tooling-depreciation.md` — the depreciation
  category template with each capitalised asset named,
  useful life, and annual depreciation.
- `cost-pack/04-external-audit.md` — the external-audit
  category template with ISO/IEC 42001 certification,
  sector regulatory examinations, IAAIS, and voluntary-code
  signatory audits, with the bundle opportunities named.
- `cost-pack/05-training.md` — the training category template
  with team training, enterprise-wide training, and CxO /
  board-director training.
- `cost-pack/06-certification.md` — the certification category
  template with individual and enterprise-level
  certifications.
- `cost-pack/07-incident-response.md` — the incident-response
  category template with baseline and contingency, and the
  incident-driven contingency-draw discipline.
- `cost-pack/finance-partner-interface.md` — the joint
  operating shape naming what each side owns.
- `cost-pack/monthly-review-cadence.md` — the monthly review
  shape and the monthly cost note that goes to the CFO.
- `cost-pack/quarterly-cfo-review.md` — the quarterly review
  shape with the specific-asks discipline.
- `cost-pack/annual-budget-cycle-handoff.md` — the handoff
  into the annual budget cycle.
- `cost-pack/vendor-renewal-calendar.md` — the standing
  calendar of vendor-renewal decisions.
- `cost-pack/failure-mode-audit.md` — the five failure-mode
  detection-and-recovery paragraphs.

## Acceptance criteria

- Every line on the pack reconciles to a specific general-
  ledger account. A line the finance business partner cannot
  reconcile fails the criterion — the un-instrumented program
  is chapter 05's headline anti-pattern.
- The seven categories are all populated and named
  separately, even where a category is small for the specific
  enterprise. A pack that hides small categories inside
  larger ones fails the criterion — chapter 05 is explicit
  that the composite hides signal.
- The vacancy line reports vacancy as a delivery risk, not
  as a positive variance. A pack that reports vacancy as a
  saving without the trajectory-slippage annotation fails
  the criterion.
- The vendor-renewal calendar names every vendor contract
  with the renewal date, notice period, and review-decision
  date. A calendar that misses a contract with a multi-year
  auto-renewal fails the criterion — chapter 05 names the
  vendor-lock-in surprise as an anti-pattern.
- The incident-response contingency discipline is written
  down: baseline plus contingency, drawn on incident, not
  reforecast into predictable spend. A pack that treats the
  contingency as baseline fails the criterion.
- The monthly cost note is a working artefact the finance
  business partner co-signs, not a note the head authors
  unilaterally. A note without joint sign-off fails the
  criterion — the joint interface is what the CFO reads.
- The quarterly CFO review is structured for a short read
  (composite in one line, seven categories in a table, two-
  or-three variance stories, specific asks). A review that
  reads as an activity summary fails the criterion.
- The failure-mode audit names, for each of the five failure
  modes, at least one specific detection signal and one
  specific recovery action.
- Any factual claim about a specific vendor's pricing model,
  a specific certification-body fee structure, a specific
  regulator-examination cost pattern, or a specific peer
  program's cost benchmark carries a
  `<!-- needs-research: verify [specific fact] against
  [official source] -->` marker where the fact is not
  independently verifiable.

## Stretch goals

- Author the **fully-loaded-cost-per-FTE reference sheet** —
  the specific figures the finance business partner and the
  head agree on for each level the head staffs, with the
  breakdown (salary band, benefits, payroll tax, workspace
  allocation, equipment, training baseline). The reference
  sheet is what the head takes to the annual budget cycle
  when a headcount request has to be defended against a CFO
  challenge. See
  [[mod-113-budget-vendor-p-and-l-and-investment-case]] for
  the underlying budget-authoring discipline.
- Draft the **contingency-reset case** — the specific case
  the head makes to the CFO when a prior year's incident
  reveals that the baseline contingency was chronically
  under-budgeted and the next-year baseline needs to be
  re-negotiated. The case is anchored on the specific
  incident, the specific spend, the specific pattern the
  incident reveals, and the specific ask. Chapter 05 names
  the contingency-as-baseline anti-pattern; this stretch is
  the case for a *deliberate*, ratified baseline reset
  rather than a silent drift.
- Extend the pack with a **cost-per-AI-system-governed
  trend** — the running-cadence signal from
  [[01-kri-kpi-portfolio]] metric 10, computed from the
  pack's total-cost figure and the inventory count from
  [[mod-102-running-the-program]] chapter 06. The trend is
  what the CFO reads to compare program-cost efficiency
  year-over-year and against sector benchmarks where
  available.
- Draft the **audit-committee cost briefing pack** — the
  version of the pack tailored for the audit committee's
  annual programme-effectiveness cadence. The committee
  reads for adequacy of investment against the maturity
  trajectory ratified in exercise 03, not for tactical
  variance. Author the pack for the committee's read.
- Author the **vendor-consolidation analysis** — the specific
  analysis of whether the enterprise's GRC-for-AI stack could
  be consolidated (fewer vendors, longer commitments, better
  total cost) or should be diversified (more vendors, avoid
  lock-in, higher unit cost). The analysis is on cadence
  every two-to-three years, tied to the largest vendor's
  renewal cycle. Feeds
  [[mod-113-budget-vendor-p-and-l-and-investment-case]].
- Draft the **outgoing-head handover on the cost pack** —
  the short note an outgoing head hands to an incoming head
  explaining the seven categories' current state, the
  finance-business-partner relationship, the standing
  variance stories, the multi-year commitments in force, and
  the pending vendor renewals.

## Notes and starter guidance

The most common first-cut failure of the pack is the head who
tries to run the finance function themselves — computing
variances in a personal spreadsheet, formatting the pack in
their own convention, presenting the numbers without the
finance business partner having seen them first. The CFO's
team is a professional finance function; the head who tries
to substitute for it produces numbers that look wrong to the
finance function and takes the credibility hit. Chapter 05 is
explicit: the head owns substance; the finance business
partner owns actuals, formatting, accounting posture, and the
enterprise's financial-modelling conventions. Build the
interface early and use it.

The second common failure is the head who reports vacancy as a
saving. Vacancy is a delivery risk. When the maturity plot's
trajectory slips because a critical hire has been open for six
months, the CFO looks at the budget under-run on headcount and
the trajectory slippage on the plot and reads them as
inconsistent — the head is under-spent because the head is
under-delivering. The remedy is to report vacancy as a risk
throughout the year, not as a saving at year-end. The finance
business partner will support this framing because it is what
allows the finance function to defend the head's headcount ask
in the next budget cycle.

On the contingency — resist the temptation to reforecast the
contingency into predictable spend when the year is quiet. A
quiet year is when the contingency should stay in the
contingency line, not migrate to headcount or vendor spend.
The migration is easy and small on any single occasion, but
after a few quiet years the head has silently absorbed the
contingency into baseline and, when a material incident hits,
the contingency is not there. Chapter 05 names the pattern.

On the vendor calendar — the most damaging vendor-renewal
surprise is not a contract the head chose to renew badly; it
is a contract the head did not know was auto-renewing. Every
contract with a multi-year auto-renewal has a review-decision
date on the calendar that falls before the notice period
expires, and the review is on the head's own calendar as an
active decision. This is chapter 05's vendor-lock-in surprise
anti-pattern, and it is the anti-pattern that most easily
sneaks up on a head who inherited a vendor stack from a
predecessor.

On the over-run explanation — resist the temptation to explain
a variance by naming external drivers only (a peer
institution's incident, a regulatory announcement, an industry
trend). The CFO expects internal ownership of internal
variances. Every variance has an enterprise decision path that
produced it; naming the decision path is what carries the
head's credibility. The head accepted an accelerated scope;
the level-50 architect approved a scope expansion; the AI
Governance Council directed an incremental control. The
external context is the frame, but the decision is what the
CFO wants named.

The pack is a living artefact. Update it monthly, review it
quarterly with the CFO, reset the baseline annually at the
budget cycle, and treat every material variance as an
opportunity to strengthen the pack's discipline rather than to
work around it. A pack that has been carried without revision
for a year is a pack whose baseline no longer reflects the
program's actual operation; a pack whose baseline has been
opportunistically revised each time a variance emerged is a
pack whose baseline has been laundered. The discipline is the
difference between the two.
