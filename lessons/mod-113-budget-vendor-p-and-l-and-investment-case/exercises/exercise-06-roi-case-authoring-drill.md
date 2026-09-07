# exercise-06: ROI Case Authoring Drill

**Estimated effort:** 2 hours

## Objective

Author the enterprise's **four-axis AI-governance ROI model** —
avoided-loss, deal-enablement, trust-margin, and transformation
— with the defensible-modelling discipline that lets the number
survive the audit-committee's scrutiny. Every axis carries
cited inputs, named-range probabilities rather than point
estimates, sensitivity analysis at low / central / high bands,
an explicit counter-factual (the no-function scenario), and
honest attribution (deal-enablement attributed to sales-function
ratification, transformation FTE-recovery attributed to a
specific redirection of the recovered hours). The deliverable
is the ROI pack the head takes into the CFO annual budget
cycle ([01-governance-function-budget-line](../01-governance-function-budget-line.md))
and the artefact the audit committee reads in the annual
governance-function assurance discussion
([[mod-103-board-and-audit-committee-reporting]]).

The pack has to survive three stress tests. First, the CFO
challenges the avoided-loss axis — the model cannot lead with
a headline fine-avoidance number without a named-range
probability, a cited regulator base-rate source, and an
explicit sensitivity band. Second, the audit committee reads
the deal-enablement claims — the sales function has to have
ratified the "deals we won because AI governance let us
answer the questionnaire" claim in writing, not the head's
narrative. Third, the CFO challenges the transformation
FTE-recovery — the recovered hours have to redirect to a
named higher-value activity (control library authorship, red-
team programme, evidence-quality uplift, third-line audit
support), not vanish into "we saved effort".

The pack is the head's negotiating instrument in the budget
cycle and the discipline artefact the audit committee reads
to conclude the governance function is an investment rather
than a cost centre. The pack has to survive the audit-
committee scrutiny — discipline over number.

## Prerequisites

- Chapter [07-roi-case-modelling](../07-roi-case-modelling.md)
  — the four-axis model, the defensible-modelling discipline
  (cited inputs, named-range probabilities, sensitivity
  analysis, explicit counter-factual, honest attribution),
  and the six anti-patterns — read and internalised.
- Chapter [01-governance-function-budget-line](../01-governance-function-budget-line.md)
  because the ROI pack is the argument the head takes into
  the budget-cycle conversation about the function's line.
- Chapter [02-multi-year-investment-case](../02-multi-year-investment-case.md)
  because the multi-year investment case embeds the ROI model
  and the two artefacts have to reconcile.
- Chapters [03-grc-for-ai-vendor-pnl](../03-grc-for-ai-vendor-pnl.md),
  [04-ai-observability-vendor-pnl](../04-ai-observability-vendor-pnl.md),
  [05-ai-runtime-security-vendor-pnl](../05-ai-runtime-security-vendor-pnl.md),
  and [06-assurance-body-relationship-pnl](../06-assurance-body-relationship-pnl.md)
  because each vendor P&L reports back into the ROI model on
  one or more axes (GRC into avoided-loss and transformation;
  observability into avoided-loss and trust-margin; runtime
  security into avoided-loss and deal-enablement; assurance
  body into trust-margin and deal-enablement).
- [[mod-102-running-the-program]] because the evidence surface
  the program produces (AIA turnaround, evidence-completeness,
  control-effectiveness, MTTR) is the substrate underneath
  the avoided-loss axis.
- [[mod-103-board-and-audit-committee-reporting]] because the
  audit committee is the primary reader of the ROI pack and
  the pack has to fit the audit-committee narrative shape.
- [[mod-107-program-measurement-and-maturity]] because the
  maturity baseline is the counter-factual the ROI model
  compares against and the maturity progression is one of the
  transformation-axis inputs.
- [[mod-108-leading-the-governance-function]] because the
  FTE-recovery baseline (analyst hours spent on spreadsheet
  reconciliation, engineer hours spent on ad-hoc questionnaire
  responses) comes from the function's own load metrics.
- [[mod-110-incident-leadership]] because the incident-cost
  avoidance line under the avoided-loss axis draws on the
  incident-cost dataset the incident-leadership function
  maintains.

## Steps

1. **Inherit the enterprise context.** Confirm the context
   one-pager from earlier exercises (sector, jurisdictional
   footprint, AI portfolio scope, maturity stage, regulator
   posture) is current and reference it. The ROI model's
   inputs are sector-specific — the regulator base rates the
   avoided-loss axis draws on, the questionnaire volume the
   deal-enablement axis draws on, the retention benchmarks
   the trust-margin axis draws on, and the process-inventory
   the transformation axis draws on all depend on the
   enterprise's specific footprint.

2. **Author the counter-factual baseline.** Author the
   explicit no-function scenario. The counter-factual is not
   "governance never existed" — it is "the enterprise
   operates its AI portfolio at the maturity level that
   preceded the function, with the incident posture, the
   evidence surface, the deal-response capacity, and the
   process footprint that maturity implies". Name:
   - The specific maturity level the counter-factual anchors
     to (referenced against the maturity model authored in
     `[[mod-107-program-measurement-and-maturity]]`).
   - The specific incident-posture the counter-factual
     implies (incident-detection latency, MTTR, third-party
     defence capacity).
   - The specific deal-response posture (questionnaire
     turnaround, RFI/RFP response quality, assurance-body
     conformity claims available).
   - The specific process footprint (analyst hours on
     spreadsheet reconciliation, engineer hours on
     questionnaire responses, ad-hoc regulator engagement).
   The counter-factual is the denominator every axis
   compares against. A model without an explicit counter-
   factual fails the discipline; the number is measuring
   against an unnamed baseline and the audit committee
   cannot audit it.

3. **Author the avoided-loss modelling.** For each avoided-
   loss line, author the specific model with:
   - **Per regulator.** For each regulator in the
     enterprise's footprint, the regulator's fine base rate
     (cited to the regulator's published enforcement record
     or a named benchmark source, not to trade press), the
     probability the enterprise faces enforcement absent the
     function (named range — for example "low: 5–10%, central:
     15–20%, high: 25–35%" — not a point estimate), the
     probability the function reduces the enforcement outcome
     to a lower band or to no-action, and the resulting
     expected-loss delta.
     <!-- needs-research: verify regulator enforcement base
     rates for each in-scope regulator against the regulator's
     most recent published enforcement summary. -->
   - **Per incident class.** For each incident class from the
     incident-leadership taxonomy, the enterprise's own
     historical incident-cost dataset (drawn from
     `[[mod-110-incident-leadership]]`), the counter-factual
     incident-cost the maturity-level implies (cited to the
     enterprise's own pre-function record where available; to
     a named industry-benchmark source otherwise), and the
     function's incident-cost reduction.
     <!-- needs-research: verify industry-benchmark incident-
     cost source (Ponemon, IBM Cost of a Data Breach, sector-
     specific benchmark) is current and represents the
     enterprise's sector. -->
   - **Per third-party defence.** The third-party defence
     posture the function enables (the assurance-body
     conformity claim, the SOC-report AI extensions, the
     vendor-review discipline) and the specific loss the
     defence avoids (contract-penalty exposure, customer-
     indemnity exposure, litigation-defence cost).
   Each line reports at low / central / high sensitivity and
   names the assumption that moves it between bands.

4. **Author the deal-enablement modelling with sales-function
   ratification.** Deal-enablement is the axis most vulnerable
   to over-claiming; force the discipline. For each deal-
   enablement line, author:
   - The specific claim (enterprise deals in which the AI-
     governance evidence surface was material to closing —
     questionnaire responses, assurance-body claims, RFI/RFP
     posture answers, prospect audit visits).
   - The specific sales-function ratification — the sales
     leader (named role, not name) has signed off in writing
     that the deals attributed to governance would not have
     closed without the governance evidence surface, or would
     have closed at a discounted price / longer sales cycle /
     narrower scope. Attribution without sales-function
     ratification is the head's narrative, not a defensible
     ROI input.
   - The specific attribution shape (percentage of deal value
     attributed to governance where governance was one of
     several factors, or full attribution where governance was
     the deciding factor).
   - The counter-factual (what happens to the deal without the
     function: lost, discounted, delayed).
   - The named-range probability of the attribution being
     correct (not every deal claim survives audit; force the
     range).
   The line reports at low / central / high sensitivity.
   <!-- needs-research: verify the enterprise's own deal-
   registry for the specific deals cited; do not cite deals
   the sales function has not ratified in writing. -->

5. **Author the trust-margin modelling with HR / CRM
   sourcing.** Trust-margin is the axis measuring retention
   delta and employee-attraction delta the function generates.
   Author:
   - **Customer-retention delta.** The specific retention
     delta the function enables — customer-renewal rate delta,
     net-revenue-retention delta, customer-churn-reason
     analysis where "AI trust" or "AI governance posture" is
     a cited reason (drawn from the CRM's own churn-reason
     coding). Sensitivity band at low / central / high.
     <!-- needs-research: verify the CRM churn-reason coding
     includes an AI-trust / AI-governance category and that
     the coding has been in place long enough to produce a
     credible delta. -->
   - **Employee-attraction and retention delta.** The
     specific delta the function enables in AI-adjacent hiring
     — offer-acceptance rate for AI / ML engineering roles,
     regretted-attrition rate in AI-adjacent teams, employee-
     survey signal on "the enterprise takes AI responsibility
     seriously" (drawn from HR's own engagement-survey
     dataset). Sensitivity band at low / central / high.
     <!-- needs-research: verify HR engagement-survey items
     include the specific AI-responsibility signal and that
     the survey has multi-year history to support a delta
     claim. -->
   - **Third-party trust posture.** The specific delta in
     assurance-body-mediated trust surface (the ISO/IEC 42001
     conformity claim, the third-party audit reports the
     enterprise makes available to customers) and its
     traceable link to retention.
   The trust-margin axis is prone to storytelling; force the
   HR / CRM sourcing so every number has a data owner outside
   the governance function.

6. **Author the transformation modelling with redirection
   discipline.** Transformation is the axis measuring the
   spreadsheet-elimination FTE-recovery and the process-
   maturation gain the function produces. Author:
   - **FTE-recovery per process line.** For each process line
     the function has industrialised (AIA authorship,
     questionnaire response, evidence gathering, regulator-
     engagement preparation, control-effectiveness testing),
     the counter-factual hours spent on the line (analyst
     hours, engineer hours, cross-functional hours pulled
     into the process) and the current-state hours. The
     recovered hours are the delta.
     <!-- needs-research: verify counter-factual hours claim
     against the function's own load metrics from
     [[mod-107-program-measurement-and-maturity]] and against
     the pre-function process baseline. -->
   - **The specific redirection.** For each recovered-hours
     line, name the specific higher-value activity the hours
     redirect to (control-library authorship, red-team
     programme delivery, evidence-quality uplift, third-line
     audit engagement support, maturity-progression work).
     FTE-recovery without redirection is the "we saved
     effort" anti-pattern — the enterprise cannot bank the
     savings because the analysts are still on the roster;
     the recovery only counts if the redirection is named.
   - **Maturity-progression measurement.** The specific
     maturity progression the function has produced,
     referenced against the maturity model from
     `[[mod-107-program-measurement-and-maturity]]`, and the
     enterprise-value the progression enables (deal-
     eligibility bands the enterprise crosses, insurance-
     posture improvements, regulatory-relationship postures
     the maturity opens up).
   The transformation axis reports at low / central / high
   sensitivity like the other axes.

7. **Compose the four axes into a single ROI number with
   sensitivity band.** Compose the four axes into a single
   composite ROI (annual benefit, three-year cumulative
   benefit, benefit-to-cost ratio against the function's
   fully-loaded cost from
   [01-governance-function-budget-line](../01-governance-function-budget-line.md)).
   Report at low / central / high — the composite is the sum
   of the axis-level lows, centrals, and highs, with an
   explicit note on where the axes are correlated (an
   incident-heavy year raises avoided-loss and stresses
   deal-enablement simultaneously; the composite is not a
   pure sum). Name the specific assumption driving the
   central-band number and the specific assumption that
   moves the composite to the low band.

8. **Author the audit-committee-facing pack.** Compose the
   audit-committee pack. The pack has to contain the
   discipline (methodology) as prominently as the number.
   Include:
   - The counter-factual baseline on the first page.
   - The four-axis composite ROI with sensitivity band on
     the second page.
   - The per-axis one-pager (methodology, inputs, cited
     sources, named-range probabilities, sensitivity, honest
     attribution posture) for each of the four axes.
   - The specific caveats the head is prepared to defend
     under audit-committee questioning (the axes most
     vulnerable to over-claim, the inputs most vulnerable to
     revision, the counter-factual assumptions the head is
     least confident in).
   - The refresh cadence (next step).
   A pack that leads with the headline number and buries the
   methodology fails the audit-committee test; a pack that
   leads with the methodology and derives the number from it
   passes.

9. **Author the refresh cadence.** Author the annual refresh
   discipline. When the pack is revisited (the CFO budget-
   cycle preparation window is the anchor; the audit-
   committee annual assurance discussion is the delivery
   point), who convenes the refresh (the head, with sales-
   function, HR, CRM, and incident-leadership partners
   named), what triggers a mid-year re-baselining (a material
   enforcement event moving base rates, a material incident
   moving the incident-cost dataset, a material deal loss
   attributed to governance gaps), and how the refresh is
   ratified.

10. **Failure-mode audit against the six anti-patterns.**
    Author a short section — one paragraph per anti-pattern —
    naming how the pack detects and recovers from each of the
    chapter-07 anti-patterns:
    - Headline-number-only: the pack presents a single ROI
      figure with no sensitivity, no counter-factual, no
      cited inputs.
    - Point-estimate probabilities: probabilities of
      enforcement, of attribution, of retention delta are
      stated as single numbers, not named ranges.
    - Trade-press citation: avoided-fine base rates are cited
      to sector news rather than to the regulator's own
      enforcement record.
    - Sales-function-unratified deal claims: deal-enablement
      attribution is the head's narrative rather than the
      sales function's written ratification.
    - Trust-margin storytelling: retention and attraction
      claims are asserted without HR or CRM data sourcing.
    - FTE-recovery without redirection: recovered hours are
      claimed as savings without naming the higher-value
      activity the hours have redirected to.

## Deliverables

- `counter-factual-baseline.md` — the explicit no-function
  scenario with maturity anchor, incident posture, deal-
  response posture, and process footprint.
- `avoided-loss-model.md` — the per-regulator, per-incident-
  class, per-third-party-defence avoided-loss modelling with
  cited inputs, named-range probabilities, and low / central
  / high sensitivity.
- `deal-enablement-model.md` — the deal-enablement modelling
  with per-deal attribution, sales-function ratification,
  counter-factual, and sensitivity.
- `trust-margin-model.md` — the retention-delta and
  employee-attraction-delta modelling with HR / CRM sourcing
  and sensitivity.
- `transformation-model.md` — the FTE-recovery-per-process-
  line modelling with named redirection per line, maturity-
  progression measurement, and sensitivity.
- `composite-roi.md` — the four-axis composite with
  sensitivity band, correlation notes, and the specific
  central-band and low-band assumptions.
- `audit-committee-pack.md` — the audit-committee-facing
  pack with counter-factual, composite, per-axis one-pagers,
  and the caveats the head is prepared to defend.
- `refresh-cadence.md` — the annual refresh cadence and the
  mid-year re-baselining triggers.
- `failure-mode-audit.md` — the six failure-mode detection-
  and-recovery paragraphs against the chapter-07 anti-
  patterns.

## Acceptance criteria

- The counter-factual baseline is explicit. A pack that
  reports ROI without a named no-function scenario fails
  the criterion — the number has no denominator.
- Every axis's inputs are cited to a primary source (the
  regulator's own enforcement record, the enterprise's own
  incident-cost dataset, the CRM's own churn-reason coding,
  the HR system's own engagement-survey dataset) or to a
  named enterprise data source. A pack that cites avoided-
  fine benchmarks to trade press or "industry consensus"
  fails the criterion.
- Probabilities are named ranges, not point estimates. A
  pack that reports "there is a 20% probability of
  enforcement absent the function" without a low / high
  band fails the criterion; the probability has to be
  reported as a range and the range has to be defensible.
- Every headline number is reported at low / central / high
  sensitivity. A pack that reports a single ROI figure
  without a sensitivity band fails the criterion.
- Deal-enablement claims are attributed to the sales
  function's written ratification. A pack that claims deals
  won because of governance without a sales-leader sign-off
  fails the criterion; deal-enablement is the axis most
  vulnerable to over-claim and the discipline is the head's
  own protection under audit-committee scrutiny.
- Transformation FTE-recovery names the specific
  redirection of recovered hours. A pack that claims analyst
  hours saved without naming the higher-value activity the
  hours redirect to fails the criterion — the recovery is
  not banked unless the redirection is named.
- The audit-committee-facing pack contains the discipline
  (methodology) as prominently as the number. A pack that
  leads with a headline ROI figure and treats the
  methodology as an appendix fails the criterion; the
  audit committee reads the discipline, not the number.
- Any factual claim about a specific regulator's enforcement
  base rate, a specific industry-benchmark incident cost, or
  a specific credential-cohort or assurance-body attach rate
  carries a `<!-- needs-research: verify [specific fact]
  against [named source] -->` marker where the fact requires
  benchmark verification. The chapter itself carries such
  markers; the exercise inherits the discipline.

## Stretch goals

- Author the **CFO-facing budget-cycle pack** — the specific
  two-page pack the head takes to the CFO in the budget-cycle
  conversation, compressing the four-axis composite into the
  benefit-to-cost narrative the CFO needs, with the specific
  budget-line justification per vendor P&L and the specific
  ask for the function's authorised cost envelope.
- Author the **audit-committee narrative script** — the
  specific script the head runs at the audit-committee
  annual assurance discussion, walking the committee through
  the counter-factual, the four axes, the sensitivity band,
  the caveats, and the specific questions the head expects
  the committee to ask (and the discipline-forward answers
  the head is prepared to give).
- Draft the **ROI-refresh retrospective template** — the
  short template the head runs at the end of the ROI year
  to assess which axis moved most, which inputs revised
  materially, which probabilities need re-ranging, and how
  the counter-factual has itself shifted (the maturity level
  the counter-factual anchors to is not static).
- Author the **honest-attribution audit** — a short
  self-audit the head runs before presenting to the audit
  committee, testing every deal-enablement claim against
  sales-function ratification, every retention-delta claim
  against CRM/HR data, every FTE-recovery claim against
  named redirection, and every avoided-loss claim against
  a primary-source citation. The audit is what stops the
  head from over-claiming in the committee room.
- Draft the **cross-axis correlation note** — a short
  written explanation of the specific correlations between
  the four axes (an incident-heavy year raises avoided-loss
  realisation and stresses deal-enablement; a maturity-
  progression year raises trust-margin and transformation
  simultaneously) so the composite ROI is read correctly
  rather than summed naively.

## Notes and starter guidance

The most common first-cut failure is the headline-number-
only pack. A pack that leads with "the AI governance
function generates a benefit-to-cost ratio of X" and buries
the methodology in an appendix fails the audit-committee
test on the first read. The audit committee's job is to
audit the discipline, not to accept the number; a pack that
does not surface the discipline gives the committee nothing
to audit and reads as advocacy rather than assurance. Lead
with the counter-factual, lead with the methodology, and
let the number derive from it. The number the audit
committee trusts is the number they can trace back to
inputs they can question.

The second common failure is the temptation to over-claim
on avoided fines. Fine avoidance is the most emotionally
compelling axis (large regulator penalties in the news
create a natural target for the model) and the axis most
vulnerable to over-claim. The regulator's own enforcement
record is the primary source — not the trade press
headline about a competitor's fine, and not the head's
sense that "we would have been fined". Cite the regulator
directly; range the enforcement probability honestly (a
first-time actor's enforcement probability differs from a
repeat actor's); and report the low band prominently so
the committee sees the head has not led with the tail.

The third common failure is the pack that skips the
counter-factual. A ROI figure without an explicit no-
function scenario is a figure measuring against an unnamed
baseline; the committee has no way to audit it because
they cannot see what the number is compared to. Force the
counter-factual authorship early in the drill and let
every axis compare against it explicitly. The counter-
factual is itself a defensible-modelling artefact — it
has to be plausible (the maturity level it anchors to
should be the maturity level the enterprise credibly
occupied before the function stood up), it has to be
sourced (the incident posture it implies should be
citable), and it has to be revisited annually (the
counter-factual shifts as the maturity progresses).

The fourth common failure is the transformation axis
claiming FTE-recovery without redirection. "The function
recovered 4,000 analyst hours" is a claim; "the function
recovered 4,000 analyst hours and redirected them to
red-team programme delivery and control-library authorship"
is a defensible claim; the difference is the redirection.
Analyst hours the enterprise cannot see redirected are
analyst hours the CFO will read as slack in the roster and
target in the next headcount review. Name the redirection
every time. If the head cannot name a redirection for a
recovered-hours line, the line is not on the ROI model.

The pack is a living artefact. Version it, date it,
refresh it at the annual CFO budget-cycle preparation
window, revise the inputs against the primary sources at
the refresh, re-range the probabilities when the
enforcement record moves or the incident dataset grows,
re-baseline the counter-factual when the maturity
progresses past the anchor level, and re-ratify the
deal-enablement claims with the sales function every
year. A ROI pack that has not been touched since the
prior budget cycle is a pack the enterprise's own
progress has already outrun — and the audit committee
will read the staleness as a discipline failure long
before they question the number.
