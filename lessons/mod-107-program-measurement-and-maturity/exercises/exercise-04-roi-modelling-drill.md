# exercise-04: ROI Modelling Drill

**Estimated effort:** 3 hours

## Objective

Author the enterprise's **AI-governance ROI pack** to the CFO —
the three-component ROI model (avoided-loss, deal-enablement,
trust-margin), each claim tiered by defensibility (anchored,
modelled, illustrative), with the prior-year backtest, the
confidence caveats, and the source data laid out as the CFO's
finance business partner expects. The deliverable is the pack
the head co-authors with the finance business partner, the
artefact the head presents at the annual budget cycle and, in
condensed form, at each quarterly budget-status review, and
the artefact the audit committee reads at the annual programme-
effectiveness cadence.

The pack has to survive three stress tests. First, the finance
business partner picks up the pack and can re-derive every
figure from source data — no unsourced number, no
un-recomputable claim. A number the finance business partner
cannot re-derive is a number the CFO's team learns not to
trust, and the head's ROI story stops carrying weight from
that year forward. Second, the audit committee reads the pack
and can determine, from the defensibility-tier annotation,
which claims are facts, which are estimates, and which are
context — the tiering discipline is load-bearing, and a pack
that hides tier annotations behind headline numbers fails the
test. Third, next year's backtest is honest — the model's
prior-year prediction is tested against the year's actuals,
variances are named, and the model is revised transparently. A
pack that consistently overshoots and never backtests is a
pack the CFO's team will stop reading.

The drill is not a study of chapter 04. It is the ROI model
laid out as a financial artefact, with the discipline that
every claim carries its source, its computation, its
assumption set, and its defensibility tier.

## Prerequisites

- Chapter [04-roi-reporting-to-cfo](../04-roi-reporting-to-cfo.md)
  — the three ROI shapes (avoided-loss, deal-enablement,
  trust-margin), the defensibility hierarchy (anchored,
  modelled, illustrative), the avoided-loss sub-components
  (regulator-fine avoidance, incident-cost avoidance,
  third-party-defence cost avoidance), the deal-enablement
  sub-components (trust-margin uplift on customer wins,
  regulator-approval-speed premium, tender-eligibility uplift),
  the trust-margin sub-components (customer-retention delta,
  employee-attraction delta), the ROI pack shape, the finance-
  business-partner co-authorship discipline, the backtest
  discipline, and the five anti-patterns (unbacktested model,
  peer-fine transposition, unspecified attribution, trust-
  margin-as-headline, composite-without-tiers) — read and
  internalised.
- Chapter [05-program-cost-management](../05-program-cost-management.md)
  — the ROI-to-cost ratio requires the cost side; the pack
  presents them together.
- Chapter [01-kri-kpi-portfolio](../01-kri-kpi-portfolio.md)
  — metric 10 (cost-per-AI-system-governed) is one input to
  the ROI-to-cost ratio.
- [[mod-104-regulator-engagement]] chapter 04 (regulator
  inventory) — source of regulator-fine-avoidance anchored
  evidence (specific findings closed without penalty on the
  basis of documented evidence).
- [[mod-106-external-positioning-and-voluntary-codes]] chapter
  04 (RFI / RFP intake register) — source of deal-enablement
  anchored evidence (specific customer contracts signed
  subject to specific AI-governance conditions).
- [[mod-110-incident-leadership]] — source of incident-cost-
  avoidance backtest data (the enterprise's own incident
  register, incident frequency, cost per incident, MTTR
  trend).
- [[mod-113-budget-vendor-p-and-l-and-investment-case]] — the
  budget cycle the pack lands at.
- Exercise 01 (KRI/KPI portfolio design) and exercise 02
  (maturity model authoring) already completed — the
  portfolio and the model provide the operating signals the
  ROI story is anchored on. Exercise 03 (annual maturity
  assessment runbook) already completed if authored in order
  — the trajectory the assessment ratifies is the anchor of
  the ROI story's forward projection.
- The concrete enterprise from exercises 01 and 02 — sector,
  jurisdictional footprint, AI system portfolio scope, and,
  importantly, at least one prior year of program operation
  to backtest against. If the enterprise is authoring the
  pack in year one (no prior year to backtest), name that
  explicitly in the pack and design the pack for the year-two
  backtest.

## Steps

1. **Reuse the enterprise context one-pager from exercises 01
   and 02.** Add a short ROI-scope note naming the enterprise's
   regulatory exposure surface (jurisdictions and sector-
   specific enforcement regimes the avoided-loss model touches),
   the enterprise's deal surface (customer segments and tender
   pools where AI-governance evidence enters procurement), and
   the enterprise's talent surface (roles where AI-governance
   posture affects recruitment and retention). The context is
   what determines which sub-components of each ROI shape are
   material for the enterprise; a fintech serving retail
   consumers has a different deal-enablement surface than a
   B2B SaaS platform selling to regulated enterprises.

2. **Author the model shell in the enterprise's financial-
   modelling convention.** The finance business partner will
   have specific conventions the enterprise uses across all
   financial models — variance thresholds, currency and
   rounding conventions, source-data linkage patterns,
   assumption-set discipline. Adopt those conventions from the
   start, not as an afterthought. A model authored in the head's
   preferred format that the finance business partner then has
   to reformat is a model that will not survive the first
   quarterly review.

3. **Author the avoided-loss component.** Author each of the
   three sub-components with the discipline chapter 04 names:
   - **Regulator-fine avoidance.** The expected-avoided-loss
     figure per fine class. Inputs: regulator-fine-quantum data
     from published enforcement actions in the enterprise's
     sector and jurisdictions (GDPR fine registers, FTC consent
     orders, state AG press releases, sector-regulator
     enforcement bulletins, EU AI Office enforcement disclosure
     as it appears); base-rate estimates for the probability
     of the enterprise facing a fine of that type; mitigation-
     efficacy estimates for the program's specific controls
     against each fine class. Attribution is conservative — a
     control chain to a specific fine class is one story; a
     generic reduction of risk is a much weaker story. Mark
     each fine-class claim with its defensibility tier
     (anchored, modelled, illustrative).
   - **Incident-cost avoidance.** The expected-avoided-cost
     figure per incident class. Inputs: the enterprise's own
     incident data (frequency, cost per incident, MTTR trend
     from [[mod-110-incident-leadership]]); peer disclosure
     from voluntary-code signatory reporting and sector
     enforcement disclosure; industry-body cost surveys
     where available (Ponemon / IBM Cost of a Data Breach or
     equivalent for the sector — mark with
     `<!-- needs-research -->` if extended to AI-specific
     incidents without independent verification). Attribution
     is against the program's demonstrable effect on incident
     frequency and MTTR, not against speculative "incidents
     that never happened".
   - **Third-party-defence cost avoidance.** The expected-
     avoided-defence-cost figure. Inputs: the enterprise's own
     external-counsel billing and internal-time-tracking
     systems, comparing defence-cost per event pre-program
     versus post-program maturity. Often better anchored than
     the other avoided-loss components because the enterprise's
     own defence-cost data is directly available.

4. **Author the deal-enablement component.** Author each of
   the three sub-components with the discipline chapter 04
   names:
   - **Trust-margin uplift on customer wins.** The enabled-
     revenue figure per deal class. Inputs: sales-pipeline
     data; specific deals where the enterprise's AI-governance
     posture was named in the procurement process (customer
     RFPs asking for ISO/IEC 42001 certification, for AI Bill
     of Rights alignment, for specific NIST RMF coverage —
     see [[mod-106-external-positioning-and-voluntary-codes]]
     chapter 04 for the RFI/RFP intake register). Anchor each
     claim to specific deals under access controls (not on the
     pack itself); the attribution logic is on the page.
   - **Regulator-approval-speed premium.** The revenue-timing-
     premium figure per approval. Inputs: the enterprise's
     own approval-time data (banking model approvals, health
     market-authorisation approvals, insurance product-launch
     approvals); industry benchmarks where available; the
     revenue attribution to the time-to-approval delta. Model
     conservatively — the counterfactual is inherently
     speculative.
   - **Tender-eligibility uplift.** The eligibility-uplift
     figure per tender class. Inputs: tender data; eligibility
     criteria; historical win-rate on eligible tenders; the
     AI-governance credentials that opened the eligibility.
     Often anchorable where the tender criteria explicitly
     name AI-governance credentials.

5. **Author the trust-margin component.** Author both sub-
   components with the discipline chapter 04 names, and with
   disciplined humility about the attribution:
   - **Customer-retention delta.** The renewal-value figure
     per customer segment. Inputs: customer-retention data;
     customer survey data on trust drivers where available;
     attribution logic that isolates the AI-governance
     contribution from other trust drivers (security posture,
     service reliability, pricing, relationship). Report as
     modelled, with an explicit confidence caveat.
   - **Employee-attraction delta.** The reduced-cost-of-hire
     or reduced-time-to-fill figure per talent class. Inputs:
     recruiting-funnel data; talent-market survey data;
     attribution logic that isolates AI-governance-specific
     contribution from other employer-brand drivers. Report
     as modelled, typically illustrative at the enterprise
     level.

6. **Tier every claim explicitly.** For every figure on the
   pack, label its defensibility tier: **anchored** (mapped to
   a specific transaction, incident, or contract in the
   enterprise's systems of record — presentable as fact);
   **modelled** (derived from an explicit model with named
   assumptions — presentable as estimate with assumptions on
   the page); **illustrative** (directional signal without a
   defensible model — presentable as context, never as a
   number on the ROI slide). Chapter 04 is explicit that the
   tier annotation is the load-bearing discipline. A single
   ROI number without the tier breakdown is the composite-
   without-tiers anti-pattern.

7. **Author the prior-year backtest.** Take the prior year's
   ROI pack (or, if year one, design the year-two backtest
   shape now so the model has a defined backtest). For each
   prior-year prediction, name the actual outcome:
   - Regulator-fine-avoidance prediction versus actual
     enforcement outcome — did a fine occur, did an
     investigation open, was a finding closed without penalty.
   - Incident-cost-avoidance prediction versus actual
     incidents — where an incident occurred that the model
     had counted as avoided, name the incident, the modelled
     cost, the actual cost, and the variance.
   - Third-party-defence-cost prediction versus actual
     defence spend.
   - Deal-enablement prediction versus actual deals — where
     deals materialised, confirm with the deal identifiers;
     where deals did not materialise, name the shortfall.
   - Trust-margin prediction versus the measurable proxy
     (retention, attraction) — where the proxy moved, report
     the actual movement.
   Where the model materially overshot, name the overshoot
   and revise the model. Where the model materially
   undershot, name the undershoot and revise. A model that
   tracks actuals within a reasonable band is what the CFO
   trusts.

8. **Author the ROI-to-cost ratio.** Combine the ROI figure
   with the cost side from [[05-program-cost-management]] and
   exercise 05. The ratio is on the pack so the CFO does not
   have to compute it. Compute the ratio at the composite
   level and at the per-component level (avoided-loss
   ratio, deal-enablement ratio, trust-margin ratio). A
   composite ratio that hides a strong avoided-loss ratio
   averaging with a weak trust-margin ratio is legible only
   at the composite; the per-component ratios are what the
   finance business partner reads.

9. **Author the confidence caveats.** Author the explicit
   statement of what the ROI figures do not measure, where
   the modelling is weakest, and what would change the CFO's
   read of the figure. Boards and audit committees trust
   models that acknowledge limits; models that present as
   omniscient invite scrutiny of every number. The caveats
   are the humility that makes the confidence claim credible
   in the rest of the pack.

10. **Author the finance-business-partner co-authorship
    discipline.** Author the joint-authorship shape in the
    pack: the substantive input the head brings (mitigation
    efficacy attributable to which control, deal-linked
    evidence, incident-cost delta); the financial modelling
    craft the finance business partner brings (model
    structure, composite computation, defensibility in the
    enterprise's financial-modelling conventions, backtest
    craft); the co-authorship signature discipline (both
    sign off on the pack, not one). The discipline is chapter
    04's central point: a model authored solely by the head
    is a model the CFO's team has not signed onto.

11. **Author the failure-mode audit.** Author a short section
    — one paragraph per failure mode — naming how the pack
    detects and recovers from each of these failure modes:
    - The unbacktested model (chapter 04's headline anti-
      pattern): a large ROI figure in year one, a similarly
      large figure in year two, without ever showing what
      happened to year one's prediction.
    - The peer-fine transposition: a peer's specific fine
      reported as the enterprise's avoided-loss, rather than
      as base-rate evidence for the model's inputs.
    - The unspecified attribution: a figure for enabled deal
      value without deal-level attribution, that the finance
      business partner cannot verify and will not defend.
    - The trust-margin-as-headline anti-pattern: the largest
      figure (trust-margin) reported as the headline number
      because it flatters, inviting the CFO to challenge the
      hardest-to-defend component first.
    - The composite-without-tiers report: a single ROI
      number without the anchored / modelled / illustrative
      breakdown, laundering weaker components into the
      composite's weight.

## Deliverables

- `roi-pack/README.md` — the pack overview: version, joint-
  authorship record, the three-component structure, the
  defensibility-tier discipline, the pack's specific asks of
  the CFO.
- `roi-pack/enterprise-context.md` — the ROI-scope note (the
  enterprise's regulatory exposure surface, deal surface,
  talent surface) appended to the exercise-01 / exercise-02
  context one-pager.
- `roi-pack/model-shell.md` — the shell in the enterprise's
  financial-modelling convention (variance thresholds,
  currency and rounding conventions, source-data linkage
  patterns, assumption-set discipline).
- `roi-pack/01-avoided-loss.md` — the avoided-loss component
  with the three sub-components (regulator-fine avoidance,
  incident-cost avoidance, third-party-defence cost
  avoidance), tier-annotated per fine or incident or defence
  class.
- `roi-pack/02-deal-enablement.md` — the deal-enablement
  component with the three sub-components (trust-margin
  uplift on customer wins, regulator-approval-speed premium,
  tender-eligibility uplift), tier-annotated per deal or
  approval or tender class.
- `roi-pack/03-trust-margin.md` — the trust-margin component
  with the two sub-components (customer-retention delta,
  employee-attraction delta), tier-annotated with explicit
  confidence caveats.
- `roi-pack/04-backtest.md` — the prior-year backtest with
  the variance analysis and the model revisions applied.
- `roi-pack/05-roi-to-cost-ratio.md` — the ratio at
  composite and per-component depth, combined with the cost
  side from exercise 05.
- `roi-pack/06-confidence-caveats.md` — the explicit statement
  of what the ROI figures do not measure, where the modelling
  is weakest, and what would change the CFO's read.
- `roi-pack/07-finance-partner-co-authorship.md` — the joint-
  authorship shape and the signature discipline.
- `roi-pack/failure-mode-audit.md` — the five failure-mode
  detection-and-recovery paragraphs.

## Acceptance criteria

- Every figure on the pack has a defensibility tier
  (anchored, modelled, illustrative). A figure without a
  tier annotation fails the criterion — the tiering is the
  load-bearing discipline chapter 04 names.
- Every modelled figure has its computation on the page —
  the inputs, the formula, the assumption set. A modelled
  figure presented as a bare number the finance business
  partner cannot re-derive fails the criterion.
- Every anchored figure names the specific transaction,
  contract, incident, or finding it is anchored to — under
  access controls (specific deal identifiers, specific
  incident references) held off the pack itself, with the
  attribution logic on the page. An "anchored" claim without
  a specific anchor fails the criterion — that is a modelled
  claim mis-labelled.
- The pack contains a prior-year backtest. Where the
  enterprise is authoring in year one and there is no prior
  year to backtest, the pack states this explicitly and
  designs the year-two backtest shape. A year-two pack with
  no backtest of year one fails the criterion — chapter 04
  names the unbacktested model as the headline anti-pattern.
- The pack presents the ROI-to-cost ratio at composite and
  per-component depth. A pack that presents only the
  composite ratio, hiding weaker per-component ratios in the
  average, fails the criterion.
- The pack contains explicit confidence caveats naming what
  the model does not measure and where the modelling is
  weakest. A pack that presents as omniscient fails the
  criterion — chapter 04 is explicit that boards and audit
  committees trust models that acknowledge limits.
- The pack is co-authored with the finance business partner
  and carries a joint signature. A pack authored solely by
  the head fails the criterion — the finance business partner
  is the CFO's own function's counterpart, and joint
  authorship is the defensibility posture chapter 04 names.
- The pack orders the components in the CFO-facing shape
  (avoided-loss first, deal-enablement second, trust-margin
  last). A pack that leads with the trust-margin figure
  because it is the largest fails the criterion — chapter 04
  names trust-margin-as-headline as an anti-pattern.
- The failure-mode audit names, for each of the five failure
  modes, at least one specific detection signal and one
  specific recovery action.
- Any factual claim about a specific regulator's enforcement
  history, a specific peer institution's fine, a specific
  industry-body cost survey, or a specific customer's
  procurement condition carries a
  `<!-- needs-research: verify [specific fact] against
  [official source] -->` marker where the fact is not
  independently verifiable. Chapter 04 carries several such
  markers by design; the pack does not silently drop them.

## Stretch goals

- Author the **anchored-evidence register** — the closed-
  ledger register the head keeps of specific transactions,
  contracts, incidents, and findings that support anchored
  claims in the pack. The register is held under access
  controls (not on the pack) but is what the finance business
  partner tests against when the CFO challenges an anchored
  claim. Include the specific evidence per entry (the deal
  contract clause, the regulator finding closure letter, the
  incident register entry) so the register is auditable.
- Draft the **CFO briefing memo** — the short memo (one page)
  that fronts the ROI pack for the CFO's read. The memo names
  the composite figure, the trajectory versus prior year, the
  two or three material claims (the largest anchored
  claim, the largest modelled claim with the largest
  variance from prior year, the largest illustrative signal),
  and the head's specific ask (budget approval, contingency
  authorisation, mid-year investment). Use the memo shape
  convention from
  [[mod-103-board-and-audit-committee-reporting]] chapter 04
  (CxO sign-off flow).
- Author the **regulator-fine-avoidance sensitivity analysis**
  — the specific sensitivity table showing how the avoided-
  loss figure moves with reasonable variation in the base-
  rate probability, the fine-quantum estimate, and the
  mitigation-efficacy attribution. The sensitivity is what
  the CFO's team runs first when the pack lands; producing it
  proactively surfaces the model's dependencies.
- Extend the pack with a **three-year forward ROI
  projection** — where the head expects the ROI figure to
  move over the next three years as regulations mature, deal-
  surface expands (particularly EU AI Act enforcement
  cadence, sector-body AI standards adoption, and voluntary-
  code signatory expansion), and program maturity trajectory
  ratified in exercise 03 delivers. Each year of the
  projection carries its own defensibility tier per component.
- Draft the **audit-committee ROI briefing pack** — the
  version of the pack tailored for the audit committee's
  annual programme-effectiveness cadence
  ([[mod-103-board-and-audit-committee-reporting]] chapter
  02). The audit committee reads the pack differently from
  the CFO — the committee is concerned with the defensibility
  of the model and the trajectory of the maturity plot,
  where the CFO is concerned with the composite and the
  variance to prior year. Author the pack for the committee's
  read.
- Author the **incoming-head handover on the ROI pack** — the
  short note an outgoing head hands to an incoming head
  explaining the pack's model, the finance-business-partner
  relationship, the backtest history, the known modelling
  weaknesses, and the pending model revisions.

## Notes and starter guidance

The most common first-cut failure of the pack is the head who
authors it alone, without the finance business partner in the
room. A pack the finance business partner has not seen before
the CFO reads it is a pack the finance business partner will
either defend under duress (badly) or quietly distance from
(fatal). Start the pack with a joint working session, not with
a draft the head hands over for review. Chapter 04 is explicit:
joint authorship is the defensibility posture.

The second common failure is the head who over-claims on the
avoided-loss component because it is the largest. A large
avoided-loss claim without conservative attribution is the
number the finance business partner will contest most
sharply, and losing the argument on the largest component is
losing the argument on the pack. Attribution is where the
head earns the defensibility — a control chain that specific
regulator-fine class is a strong story; a generic risk
reduction that is claimed as fine avoidance is a weak story.

On the peer-fine transposition — this is the most tempting
error. A peer's public fine ("Peer X was fined €1B") is
readable, salient, and easy to appropriate. It is not the
enterprise's avoided outcome. The peer's fine is *base-rate
evidence* for the model's probability and quantum inputs, and
that is all. The distinction is chapter 04's headline
discipline, and the pack has to hold the line.

On the tier discipline — resist the temptation to promote a
modelled claim to anchored because the number would be more
salient. The finance business partner will notice; the
audit committee will notice on the second cycle; the CAE will
notice on the first assurance engagement. A modelled claim
labelled as such and defended with its assumption set on the
page is the credible claim; an anchored claim without an
anchor is the fatal one.

On the backtest — the backtest is the single strongest
defensibility signal on the pack. A pack with a candid
backtest that names variances honestly (both overshoots and
undershoots) is the pack the finance business partner will
carry into the CFO's own review. A pack that omits the
backtest, or that presents the backtest as universally
favourable, is the pack the CFO's team will stop trusting.

On the trust-margin component — the head runs it because the
board reads it with interest, not because it is defensible.
Run it with disciplined humility. Report it modelled with
explicit confidence caveats; report it illustrative at the
enterprise level where the enterprise-specific attribution
cannot be isolated from other trust drivers. Do not lead with
it; do not inflate its weight in the composite. Chapter 04's
trust-margin-as-headline anti-pattern names the failure
mode.

The pack is a living artefact. Version it, date it, backtest
annually, revise the model transparently when the backtest
requires revision, and carry the model version and the
revision reason forward across years. A pack that has been
carried year over year without ever being revised is a pack
whose model has drifted from the enterprise's actual
operation; a pack that has been revised opportunistically to
preserve favourable numbers is a pack whose credibility has
been quietly eroded. The revision discipline is the difference
between the two.
