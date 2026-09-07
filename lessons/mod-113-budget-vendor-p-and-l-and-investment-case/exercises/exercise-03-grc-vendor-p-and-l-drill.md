# exercise-03: GRC-for-AI Vendor P&L Drill

**Estimated effort:** 2 hours

## Objective

Author the enterprise's **GRC-for-AI vendor P&L portfolio** —
either (a) the per-vendor P&L for the enterprise's current
GRC-for-AI incumbent, or (b) a per-vendor P&L shortlist across
three candidates drawn from the category population where no
incumbent is yet in place. The category population the head
positions against for this drill is Credo AI, Holistic AI,
ModelOp, Monitaur, ServiceNow AI Control Tower, IBM
watsonx.governance, Fairly AI, Enzai, Trustible, and Verify AI,
plus any adjacent-category vendor (model-risk-management,
AI-observability, AI-runtime-security) the head reads as
credible pressure on the AI-governance category over the
contract horizon.

The deliverable is the artefact the head takes into three
distinct calendar events. First, the **quarterly account
review** with the incumbent (or the shortlist briefing cycle
where no incumbent is in place) — the P&L is the evidence base
against which the head reads value against contracted spend.
Second, the **annual budget cycle** — the P&L is what the head
consolidates into the vendor line in [chapter 01](../01-governance-function-budget-line.md)
and defends to the CFO. Third, and in renewal year the load-
bearing one, the **contract renewal negotiation** — the P&L is
what the head, procurement, and finance run against the
vendor's paper.

The P&L has to survive three stress tests. First, the CFO
challenges the total-cost-of-ownership number — the P&L has to
carry integration cost, admin cost, and workaround labour, not
just the contracted licence. Second, the CIO asks how the
consolidation-or-expansion decision was taken — the P&L has to
name the specific choice, the specific trade-offs, and the
specific framework inputs (current-state overlap map, cost-of-
consolidation model, cost-of-run-parallel model, migration-
risk model, roadmap-alignment view over the 3-year horizon).
Third, the audit committee asks what happens if the vendor
misses SLA at scale — the escalation ladder has to name the
P&L consequence at each level, not just the relational move.

The portfolio is the head's commercial instrument on the
category — the artefact that turns "we have a vendor" into
"we run this vendor as a portfolio position."

## Prerequisites

- Chapter [03-grc-for-ai-vendor-pnl](../03-grc-for-ai-vendor-pnl.md)
  — the category map discipline, the consolidation-or-expansion
  decision framework (single-vendor consolidation, best-of-
  breed expansion, hybrid core-plus-specialty), the six per-
  vendor P&L sections (contracted spend, actual spend, total
  cost of ownership, value delivered, SLA position, renewal
  disposition), the 12-to-18-month renewal-negotiation timing
  discipline, the four-stage SLA-slip escalation ladder, the
  multi-year commercial disciplines, and the six anti-patterns
  — read and internalised.
- Chapter [01-governance-function-budget-line](../01-governance-function-budget-line.md)
  because the vendor P&L rolls up into the budget line the
  head defends annually, and because the workaround-labour
  signal that appears in the P&L's total-cost-of-ownership
  section is defined there.
- Chapter [02-multi-year-investment-case](../02-multi-year-investment-case.md)
  because a consolidation-away disposition (or a shortlist-
  selection decision where no incumbent yet exists) triggers
  the transformation-case shape authored in that chapter, and
  the P&L is one of the inputs.
- Chapter [07-roi-case-modelling](../07-roi-case-modelling.md)
  because the value-delivered column in the per-vendor P&L
  bridges into the ROI case; the P&L is the source of the
  spend-side numbers the ROI case runs against.
- [[mod-108-leading-the-governance-function]] chapter 06 —
  the CxO-scope vendor relationship discipline (the account
  cadence, the satisfaction pulse, the continuity planning,
  the relationship-framed escalation ladder). The current
  chapter recasts the same disciplines in commercial framing;
  the two are the same shape read from two sides and cannot be
  authored in isolation.
- [[mod-102-running-the-program]] — the AIMS operating
  substrate the platform runs against (AI system inventory,
  control library, evidence store, AIA / DPIA / conformity-
  assessment workflow). The platform's fit to the substrate
  is what the P&L's value-delivered column is measured against.
- [[mod-107-program-measurement-and-maturity]] — the KRI/KPI
  portfolio the platform produces the pipelines for. The
  value-delivered column in each per-vendor P&L is anchored
  to specific KRI/KPI feeds authored there.
- The enterprise's own current vendor contract (licence,
  professional-services envelope, SLA schedule, portability
  language, escape-clause language) if an incumbent is in
  place; the enterprise's shortlist candidate briefing
  material and public product material if not.

## Steps

1. **Inherit the enterprise context.** Confirm the enterprise
   context one-pager is current and reference it (sector,
   jurisdictional footprint, AI portfolio scope and growth
   trajectory, maturity stage, AIMS operating shape,
   certification calendar). The per-vendor P&L specifics
   depend on this context — a sector with an in-cycle
   ISO/IEC 42001 surveillance audit runs the SLA position
   against different tolerance than a sector with no active
   certification. Decide, and state explicitly at the top of
   the portfolio, whether the drill is running the
   **incumbent path** (one vendor P&L, deep) or the
   **shortlist path** (three vendor P&Ls, comparative) — the
   downstream steps compose against that choice.

2. **Map the category population.** Author the category map
   as a one-page (or few-page) view against the ten
   category-population vendors named in the chapter — Credo
   AI, Holistic AI, ModelOp, Monitaur, ServiceNow AI Control
   Tower, IBM watsonx.governance, Fairly AI, Enzai, Trustible,
   Verify AI — plus any adjacent-category vendor (model-risk,
   observability, runtime-security) the head reads as
   credible pressure on the category over the contract
   horizon. For each vendor, name:
   - The grouping the head places the vendor in (enterprise-
     GRC-with-AI-overlay, AI-native governance-of-record,
     adjacent-category pushing in).
   - The head's current read on the vendor's positioning
     against the enterprise's AIMS operating shape (strong
     fit, partial fit, adjacent, not evaluated).
   - The "as of" date and the source basis for the read
     (public material, vendor briefing, peer-network read,
     analyst-house read with critical distance). Where the
     head's read is thin, mark it — the map does not fake
     depth it does not have.
   Attach `<!-- needs-research -->` markers on any specific
   claim about a vendor's product depth, pricing tier, or
   market position that is not independently verified.

3. **Build the per-vendor P&L file(s).** Author the per-vendor
   P&L to the six-section structure from the chapter, one
   file per vendor. For each vendor:
   - **Contracted spend.** The annual licence, the tier
     position, the growth escalators, the professional-
     services envelope. For a shortlist candidate where no
     contract yet exists, populate the section with the
     head's current best read from vendor briefing and public
     material and label the numbers as candidate rather than
     contracted.
   - **Actual spend.** The invoice-level running total, the
     over/under position against the contracted envelope,
     the reconciliation to the general-ledger vendor line.
     For a shortlist candidate, mark the section as
     not-applicable-until-contracted rather than fabricate
     it.
   - **Total cost of ownership.** Contracted spend plus
     implementation labour, integration cost, internal-admin
     cost, and workaround labour. The head models each
     component explicitly rather than folding them into a
     single number.
   - **Value delivered.** The per-vendor value delivered
     mapped to the KRI/KPI portfolio — evidence-completeness,
     AIA / DPIA / conformity-assessment turnaround time,
     MTTR on control-failure closure, control coverage,
     audit-cycle support. The head cites the specific KRI or
     KPI feed each value entry is anchored to.
   - **SLA position.** The contracted SLAs (uptime, support-
     response by severity, resolution-time by severity,
     roadmap-delivery commitments where the contract carries
     any, data-residency and security-and-privacy
     commitments), the measured attainment, and the credit
     position. Where the enterprise has independent
     monitoring, cross-check the vendor's own SLA reporting
     against it. Do not invent SLA percentages; where the
     specifics are not yet documented in the enterprise's
     contract, mark the entry with a `<!-- needs-research -->`
     against the specific commitment.
   - **Renewal disposition.** The head's advance disposition
     on the renewal — renew as-is, renew with re-negotiation,
     consolidate away, or expand to adjacent scope. For a
     shortlist candidate, the equivalent field is the head's
     selection disposition — lead candidate, viable
     alternative, not-fit-for-shape.

4. **Author the consolidation-or-expansion decision.** Author
   the specific decision the enterprise takes on the category
   shape — single-vendor consolidation on the incumbent, best-
   of-breed expansion across a named vendor set, hybrid core-
   plus-specialty against a named combination, or (for the
   shortlist path) a selection-and-consolidation decision
   against a named lead candidate. The decision has to name:
   - The specific choice, in the chapter's taxonomy.
   - The specific trade-offs the head accepts as consequence
     of the choice, drawing on the chapter's per-shape trade-
     off enumeration (single-throat-to-choke versus category
     coverage, best-of-breed fit-per-scope versus integration
     cost, hybrid marginal-cost efficiency versus roadmap-
     coordination risk).
   - The specific framework inputs that produced the choice
     — the current-state overlap map (which vendors overlap
     in scope and where the duplication sits), the cost-of-
     consolidation model, the cost-of-run-parallel model, the
     migration-risk model (with the AIMS calendar overlay —
     migrations against in-flight certifications endanger the
     certification), and the roadmap-alignment view over the
     3-year horizon.
   - The CxO stakeholders the decision is coordinated with
     (CFO, CIO, CAIO where the enterprise has one; the
     chapter's reference to [chapter 08](../08-caio-and-cxo-budget-envelope-coordination.md)
     is where the CAIO envelope coordination sits).
   A decision that names a shape without naming trade-offs
   fails the discipline; a decision that lists trade-offs
   without picking a shape fails just as clearly.

5. **Author the renewal-negotiation posture.** Author the
   renewal-negotiation posture the head takes into the
   negotiation cycle, 12–18 months ahead of renewal (or, for
   the shortlist path, the head's opening negotiating posture
   for the initial contract). The posture has to name:
   - The head's read on the four leverage sources — credible
     alternative-vendor evaluation (which alternatives, at
     what depth, over what window), documented SLA
     underperformance (which SLAs, with which specifics),
     defensible growth trajectory (what growth story the
     enterprise carries into the negotiation), and reference-
     account value (whether the enterprise's name is
     materially valuable to the vendor and, if so, what the
     head is willing to trade for).
   - The specific contract-shape improvements the head is
     driving at renewal beyond price — SLA-definition
     sharpening, uptime and credit-schedule specificity,
     roadmap-commitment language, portability commitments
     (specific export format(s) — OSCAL, CycloneDX ML-BOM,
     SPDX AI profile, or vendor-native but documented),
     data-residency commitments, security-and-privacy
     attestation commitments, escape-clause specificity.
   - The **walkaway conditions** — the specific terms and
     price at which the head is not willing to renew (or, on
     the shortlist path, the specific terms below which the
     head does not sign a first contract), and the CIO and
     CFO alignment behind the walkaway. The walkaway is
     documented, not implied. A negotiation without a
     walkaway is a negotiation the vendor prices against.
   - The specific engagement shape with procurement and
     finance — procurement runs the transactional
     negotiation, the head runs the substantive contract-
     shape terms, and the boundary between the two is
     authored explicitly so neither runs into the other's
     scope mid-cycle.

6. **Author the SLA-slip escalation ladder.** Author the four-
   stage escalation ladder recast in P&L framing per the
   chapter — account-executive engagement, vendor CxO sponsor
   engagement, internal CFO / CIO engagement, contract
   termination and replacement. For each level:
   - The **triggering condition** — the specific SLA-slip
     pattern (not a one-off incident) that fires the level.
     A pattern is dates, incidents, measured SLA-attainment
     numbers, and the record of the prior-level engagement
     that failed to move the pattern.
   - The **specific ask** the head brings — for level 1, the
     specific remediation window and the SLA-credit
     invocation against the current period; for level 2, the
     CxO-scope commitment with named executive
     accountability and a restructuring-or-acceleration ask;
     for level 3, the authority to invoke contractual
     remedies and open replacement-vendor evaluation; for
     level 4, the termination-for-cause invocation and the
     transition-services execution.
   - The **P&L consequence modelled before triggering** —
     the specific number (SLA credit against the invoice,
     professional-services concession, restructure delta,
     migration cost minus recovered credit) the head brings
     into the level's engagement. A level triggered without
     a modelled P&L consequence is theatre; the vendor's
     account team reads the difference immediately.
   - The **decision to hold or advance** at the end of the
     level's remediation window — what the head reads to
     decide whether the pattern has moved substantively
     enough to hold, or whether the head advances to the
     next level.

7. **Author the continuity plan against platform lock-in.**
   Author the specific continuity plan the head runs
   underneath the P&L. The plan has to name:
   - The specific **data-portability format(s)** the vendor
     is contracted (or will be contracted, for the shortlist
     path) to export against — OSCAL for controls and
     assessment results, CycloneDX ML-BOM or SPDX AI profile
     for model bill-of-materials, or a specific vendor-
     native format that the head has verified is documented
     and consumable by an alternative platform.
   - The **alternative-vendor awareness posture** — which of
     the category-population vendors the head keeps
     intelligence on through the annual category refresh
     discipline, the specific briefing cadence per alternate,
     and the depth of the head's own current read on each.
     The chapter is explicit that a vendor whose contract
     does not carry portability is a vendor whose lock-in
     the head is underwriting; the continuity plan is the
     head's answer.
   - The **migration-cost model** — the current best
     estimate of what it costs to move off the incumbent
     onto the leading alternative (implementation,
     integration, data-migration, workflow-retraining,
     dual-run period), refreshed annually. The head does
     not fabricate a precise number where the estimate is
     rough; the head marks the roughness explicitly and
     names what would sharpen the estimate.
   - The **exit-services posture** — what the head expects
     from the vendor on exit (data return in the portable
     format, transition support through cutover, wind-down
     of vendor access), and whether the current contract
     carries the language or the head is driving it in at
     the next renewal.

8. **Author the failure-mode audit against the six anti-
   patterns.** Author a short section — one paragraph per
   anti-pattern — naming how the P&L portfolio detects and
   recovers from each of the chapter's six anti-patterns:
   - **RFP-and-forget.** The head has run a procurement,
     signed a multi-year contract, and not opened the P&L
     since. Detection: the per-vendor P&L file is not on a
     quarterly refresh cadence; the account review discipline
     from [[mod-108-leading-the-governance-function]] chapter
     06 is not running.
   - **Three-tool-drift.** The enterprise carries multiple
     overlapping platforms because each was procured for a
     point need. Detection: the category map shows scope
     overlap without a documented reason; the consolidation-
     or-expansion decision has never been taken explicitly.
   - **Single-vendor-lock-in.** The enterprise has
     consolidated on a single vendor without portability
     discipline. Detection: the continuity plan section is
     empty, the contract carries no export-format language,
     the migration-cost model has never been authored.
   - **Analyst-house-driven selection.** The enterprise has
     selected on the current Magic Quadrant / Wave without
     first-hand evaluation. Detection: the category map is
     a restatement of the analyst placement without the
     head's own peer-network or briefing-based read.
   - **"Renewal is procurement's job" abdication.** The head
     has never engaged renewal at business-owner scope.
     Detection: the renewal-negotiation posture section is
     empty on substantive terms; procurement's paper on the
     last renewal shows no head-driven contract-shape
     improvements.
   - **Escalation-avoidance.** The head sees the pattern
     but does not open the ladder. Detection: the SLA
     position in the P&L shows sustained under-attainment
     with no level-1 engagement record; the account review
     minutes read as satisfied where the SLA numbers do not
     support it.
   For each anti-pattern, name the specific detection signal
   and the specific recovery action.

9. **Reconcile against the budget line and the ROI case.**
   Confirm the total-cost-of-ownership numbers in the
   per-vendor P&L reconcile to the vendor cost-category line
   in the [chapter 01](../01-governance-function-budget-line.md)
   budget artefact. Confirm the value-delivered column feeds
   the ROI axes in [chapter 07](../07-roi-case-modelling.md)
   coherently. Where a workaround-labour signal is material,
   confirm it is flagged for the transformation-case shape
   in [chapter 02](../02-multi-year-investment-case.md).
   Cross-artefact reconciliation is what turns the P&L from
   a standalone document into a portfolio position.

## Deliverables

- `vendor-p-and-l/<vendor>.md` — the per-vendor P&L file, one
  per vendor in scope. For the incumbent path, a single file.
  For the shortlist path, three files against three named
  candidates from the category population. Each file carries
  the six required sections (contracted spend or candidate
  spend read, actual spend or not-applicable marker, total
  cost of ownership, value delivered, SLA position, renewal
  or selection disposition).
- `category-map.md` — the head's category map against the
  category-population vendors with grouping, positioning read,
  "as of" date, source basis per read, and `<!-- needs-research
  -->` markers where the head's read is thinner than citation
  depth requires.
- `consolidation-or-expansion-decision.md` — the specific
  consolidation-or-expansion decision the enterprise takes,
  with named trade-offs and the specific framework inputs
  (current-state overlap map, cost-of-consolidation model,
  cost-of-run-parallel model, migration-risk model, roadmap-
  alignment view). Names the CxO stakeholders the decision is
  coordinated with.
- `renewal-negotiation-posture.md` — the renewal-negotiation
  posture (or, for the shortlist path, the opening initial-
  contract posture) with the four-source leverage read, the
  substantive contract-shape improvements the head is driving,
  the walkaway conditions, and the head-plus-procurement
  engagement-boundary shape.
- `escalation-ladder.md` — the four-stage SLA-slip escalation
  ladder with, at each level, the triggering condition, the
  specific ask, the modelled P&L consequence, and the
  advance-or-hold decision at the level's remediation window.
- `continuity-plan.md` — the continuity plan with the
  specific data-portability format(s) the vendor is (or will
  be) contracted against, the alternative-vendor awareness
  posture, the migration-cost model, and the exit-services
  posture.
- `failure-mode-audit.md` — one paragraph per anti-pattern
  (RFP-and-forget, three-tool-drift, single-vendor-lock-in,
  analyst-house-driven selection, "renewal is procurement's
  job" abdication, escalation-avoidance) with a specific
  detection signal and a specific recovery action for each.

## Acceptance criteria

- Every per-vendor P&L file carries **all six required
  sections** (contracted spend, actual spend, total cost of
  ownership, value delivered, SLA position, renewal
  disposition). A file that omits total cost of ownership or
  value delivered fails the criterion — the licence-only P&L
  is the pattern the chapter opens against.
- The total-cost-of-ownership section names, at minimum,
  implementation labour, integration cost, internal-admin
  cost, and workaround labour explicitly rather than folding
  them into a single number. A TCO section that carries only
  the contracted licence figure fails the criterion.
- The value-delivered section anchors each entry to a
  specific KRI or KPI feed from
  [[mod-107-program-measurement-and-maturity]]. Value
  entries in narrative form ("the platform makes assessments
  faster") without a named KRI/KPI feed fail the criterion.
- The **consolidation-or-expansion decision** names one
  specific choice in the chapter's taxonomy (single-vendor,
  best-of-breed, hybrid, or — for the shortlist path — the
  selection-and-consolidation shape) with the specific trade-
  offs the head accepts as consequence. A decision that lists
  the shapes without picking one, or picks a shape without
  naming trade-offs, fails the criterion.
- The **renewal-negotiation posture** names specific
  **walkaway conditions** — the specific terms and price the
  head is not willing to renew below (or the specific terms
  below which the head does not sign an initial contract on
  the shortlist path) — and names the CIO and CFO alignment
  behind the walkaway. A posture without a documented
  walkaway fails the criterion.
- The **escalation ladder** names a specific **P&L
  consequence at each level** — SLA credit against invoice at
  level 1, restructure-or-acceleration delta at level 2,
  contractual-remedy-and-replacement-evaluation modelled cost
  at level 3, full migration cost minus recovered credit at
  level 4. A level authored without a P&L number (or a
  labelled placeholder where the number is not yet estimable)
  fails the criterion.
- The **continuity plan** names one or more specific
  **data-portability format(s)** the vendor is (or will be)
  contracted against — OSCAL, CycloneDX ML-BOM, SPDX AI
  profile, or a specific documented vendor-native format the
  head has verified is consumable by an alternative platform.
  A continuity plan that references portability without
  naming a format fails the criterion.
- The **failure-mode audit** names, for each of the six
  anti-patterns, at least one specific detection signal and
  one specific recovery action. A paragraph that restates the
  anti-pattern without a detection signal fails the criterion.
- Any specific claim about a vendor's pricing tier, market
  share, product depth in a named sub-category, contract-
  language norm, uptime commitment norm, or SLA-credit norm
  carries a `<!-- needs-research: verify [specific fact]
  against [source or vendor briefing basis] -->` marker where
  the fact is not independently verified. The chapter itself
  carries such markers around category positioning and
  contract-norm claims; the exercise inherits the discipline.

## Stretch goals

- Author the **CFO-facing account-review pack** — the specific
  two-page pack the head takes to the CFO alongside the
  budget-cycle preparation, compressing the vendor P&L
  portfolio into contracted-spend-versus-TCO delta by vendor,
  value-delivered-per-dollar read against the KRI/KPI
  portfolio, SLA-position summary with credit position, and
  the head's renewal-disposition read on each vendor in
  scope. The pack is what enables the CFO to hold the vendor
  line coherently against enterprise cost pressure.
- Draft the **alternative-vendor briefing brief** — the
  specific brief the head hands to the two-to-three
  alternative vendors the head runs at head-to-head scope in
  the 12 months leading to renewal (or, for the shortlist
  path, at final-selection scope). The brief carries the
  enterprise's AIMS operating shape, the specific integration-
  surface requirements, the specific portability commitments
  the head requires, and the specific SLA-shape asks. A well-
  authored brief is what turns a vendor briefing into a
  substantive competitive read rather than a marketing
  session.
- Draft the **migration playbook shape** for the leading
  alternative to the incumbent, or for the specific
  consolidation-away disposition the P&L points to. The
  playbook is authored fully as a transformation case in
  [chapter 02](../02-multi-year-investment-case.md); this
  stretch sketches the shape so the migration-cost model in
  the continuity plan is anchored to a specific execution
  path rather than a hand-waved estimate.
- Author the **peer-institution reference-network map** the
  head runs against the incumbent (or the shortlist
  candidates). Two-to-three peer heads-of-role, the specific
  conversation cadence, the specific topics the peer network
  is asked about (roadmap-slippage signals, executive-team
  turnover, contract-shape improvements the peer has
  extracted, category-consolidation reads). The map is the
  head's earliest signal on category shifts and the source
  of the reference-check leverage the head brings into
  renewal.
- Author the **quarterly-refresh calendar** — the specific
  quarterly cadence the head runs on the P&L portfolio
  (which weeks, which reviewers, which upstream inputs
  feed the refresh, which downstream artefacts consume the
  refresh output). A calendar that lands on real dates in
  the enterprise's own quarterly cycle is what turns the
  quarterly-refresh discipline from an aspiration into a
  standing practice.

## Notes and starter guidance

The most common first-cut failure is a per-vendor P&L that
carries the contracted licence line and nothing else. The
licence is the smallest of the numbers that matter; the
integration cost is often materially larger in the first two
years of the contract, the workaround-labour cost is often the
signal that a transformation case wants authoring, and the
value-delivered column is what turns a spend line into a
portfolio position. Force the six-section discipline —
contracted spend, actual spend, total cost of ownership, value
delivered, SLA position, renewal disposition — and force the
workaround-labour line specifically. A P&L that hides
workaround labour is a P&L the CFO will discover in a cost
cycle when the discovery is least useful.

The second common failure is the consolidation-or-expansion
decision that names all three shapes and picks none. The
chapter is explicit — the decision is the load-bearing
commercial move on the category, taken on roughly a three-year
cycle. A head who runs the P&L without ever taking the
decision explicitly is a head who has drifted into whatever
shape the current vendors procured historically. Force a
choice, force the named trade-offs, and force the framework
inputs (overlap map, cost-of-consolidation, cost-of-run-
parallel, migration-risk, roadmap-alignment). The choice is
revisited on the next three-year cycle; it is not permanent,
but it is not optional either.

The third common failure is a renewal-negotiation posture that
signals displeasure without a walkaway. The chapter is precise
on why this fails — the vendor's account team reads the
difference between real walkaway posture and theatre
immediately, prices against the pattern over successive
renewals, and the enterprise's contract worsens on each
renewal cycle. Force the documented walkaway, force the CIO
and CFO alignment behind it, and force the migration path and
migration-cost model that make the walkaway credible. A
walkaway the head cannot execute is not a walkaway; it is a
concession the vendor will discover.

On the escalation ladder — the temptation is to author the
ladder as relationship moves rather than commercial moves. The
chapter is explicit that the current chapter recasts the
[[mod-108-leading-the-governance-function]] chapter 06 ladder
in P&L framing. The recast is the discipline. Each level
carries a modelled P&L consequence the head brings into the
conversation. Level 1 is not "we called the account executive";
level 1 is "we invoked $X of SLA credit against the current
period's invoice and asked for the specific remediation
pattern by the specific date." The vendor's account team
knows which of the two conversations they are in.

On the continuity plan — the temptation is to treat
portability as language the contract carries in the abstract.
The chapter's discipline is specific: name the format. OSCAL
for controls and assessment results, CycloneDX ML-BOM or SPDX
AI profile for the model bill-of-materials, or a specific
documented vendor-native format that the head has verified an
alternative platform can consume. A portability commitment
without a named format is a portability commitment the vendor
will meet with an unstructured data dump the alternative
platform cannot ingest without months of engineering. Name the
format, verify the format is consumable elsewhere, and drive
the format language into the contract at the next renewal.

The portfolio is a living artefact. Refresh the per-vendor
P&L files quarterly at the account-review cadence, refresh
the category map annually as a standing calendar item, revisit
the consolidation-or-expansion decision on the three-year
cycle (usually aligned to the incumbent's major renewal
window), open the renewal file 12 to 18 months ahead of
expiry, and update the continuity plan when a category event
warrants it (a large acquisition, a category consolidation, a
material vendor struggle, a peer-network signal on executive-
team turnover). A portfolio that has not been touched since it
was authored is a portfolio the category has already outrun.
