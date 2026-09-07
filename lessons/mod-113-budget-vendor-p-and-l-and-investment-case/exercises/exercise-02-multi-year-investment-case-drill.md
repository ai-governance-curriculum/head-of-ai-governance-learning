# exercise-02: Multi-Year Investment Case Drill

**Estimated effort:** 3 hours

## Objective

Author the enterprise's **multi-year AI-governance investment
case pack** — the three-audience, three-case-type artefact the
head takes into the annual budget cycle. The pack composes
three distinct case types authored in parallel (the programme
case, the transformation case, and the incident-preparedness
case), rendered into three audience-specific deliveries (the
CFO-facing pack for value-for-cost, the CEO-facing two-pager
for strategic imperative, and the audit-committee-facing pack
for assurance adequacy against the ratified risk appetite).
The deliverable is the case-pack artefact the head carries
through the CFO one-on-one, the finance-team analysis window,
the joint CFO/CEO conversation, the audit-committee pre-read,
and the audit-committee meeting — the sequence that turns a
budget model into an approved multi-year investment.

The pack has to survive the five stress tests from chapter 02
before it leaves the head's desk. The first is "why now, not
next year" — every case has to name the specific reason a year
of delay is not free, in terms the CFO will re-run against the
finance team's own read. The second is "what breaks if
compressed" — each case has to carry its compression graph
(linear, step-function, or commit-or-abandon) rather than the
posture "the line cannot be compressed at all." The third is
"how do we know it worked" — each case is anchored to specific
KRIs or KPIs from [[mod-107-program-measurement-and-maturity]]
chapter 01 that the head is prepared to be held to. The fourth
is "who else pays" — the case is honest about which lines are
governance-function-owned, which are shared with security,
privacy, product, or engineering, and which are owned elsewhere
but co-governed. The fifth is the "what if we did nothing"
counter-factual — the case describes the no-investment scenario
honestly, and if the honest description is "not much," the head
compresses the case before the CFO does.

The pack is the head's decision instrument in the annual
budget cycle and the discipline that turns a spreadsheet the
CFO's finance team can carve line-by-line into a strategic
narrative the CFO can only compress at the level of the case
itself.

## Prerequisites

- Chapter [02-multi-year-investment-case](../02-multi-year-investment-case.md)
  — the three-audience shape (CFO / CEO / audit committee), the
  three case types (programme / transformation / incident-
  preparedness), the case-document structure (title / executive
  summary / strategic context / ask / case / risks and
  mitigations / ROI hooks / appendix), the four framing
  disciplines (regulatory-obligation, board-adopted-risk-
  appetite, peer-benchmarking, incident-precedent), the five
  stress tests, the five-step delivery sequence, and the six
  anti-patterns — read and internalised.
- Chapter [01-governance-function-budget-line](../01-governance-function-budget-line.md)
  because the multi-year budget model is the substrate the
  investment case is authored on top of. The case renders the
  numbers from the budget model; it does not re-invent them.
- Chapters [03-grc-for-ai-vendor-pnl](../03-grc-for-ai-vendor-pnl.md),
  [04-ai-observability-vendor-pnl](../04-ai-observability-vendor-pnl.md),
  [05-ai-runtime-security-vendor-pnl](../05-ai-runtime-security-vendor-pnl.md),
  and (where authored) the assurance-body relationship P&L
  because the vendor P&L files supply the line items into the
  programme case's tooling and external-audit categories and
  into the transformation case's platform and migration cost
  categories. The head does not re-author the vendor P&L
  content inside the investment case; the case carries the
  totals and points at the P&L files for substance.
- Chapter [07-roi-case-modelling](../07-roi-case-modelling.md)
  because the ROI hooks in the case are the modelled ROI
  numbers rather than aspirational ones; the head does not
  overclaim relative to what the model will defend under
  internal audit or finance-team challenge.
- [[mod-102-running-the-program]] because the AIMS runtime
  target — off spreadsheets, off point tools, on a certifiable
  runtime — is the anchor for the transformation case's
  substantive scope and sequencing.
- [[mod-103-board-and-audit-committee-reporting]] because the
  audit-committee-audience rendering is authored against the
  cadence and framing this module carries; the ratified AI risk
  appetite the case maps to sits here.
- [[mod-105-regulatory-change-management]] because the
  regulatory-change-readiness component of the programme case
  and the regulatory-obligation framing discipline are both
  anchored on the horizon-scanning and change-management
  cadence in this module.
- [[mod-107-program-measurement-and-maturity]] because the
  measurement backbone supplies the KRI / KPI anchors the "how
  do we know it worked" stress test names, and the annual
  maturity assessment is the anchor for the maturity-progression
  component of the programme case and for peer-benchmarking
  framing.
- [[mod-110-incident-leadership]] because the incident-
  preparedness case is anchored on the scenario library, the
  response cadence, the tabletop-exercise pattern, and the on-
  event authority this module authors.
- The exercise-01 artefacts (the multi-year budget model, the
  category taxonomy, the year-two and year-three trajectory
  assumptions) as the inputs the case pack builds on.

## Steps

1. **Inherit the enterprise context.** Confirm the exercise-01
   context one-pager is current and reference it. The case-
   pack specifics — the case-type scope, the transformation
   the enterprise is genuinely running, the incident-
   preparedness posture the sector warrants — depend on the
   sector, jurisdictional footprint, AI portfolio scope, and
   maturity stage on the one-pager. A head running the
   spreadsheet-to-AIMS transformation authors a different
   transformation case than a head running the point-tools-
   to-governance-of-record transformation; the case-pack
   scope is anchored to the enterprise's actual substrate
   position, not to a generic transformation shape.

2. **Author the programme case.** Produce the programme case
   document to the chapter-02 structure — title (case type
   and year), executive summary (two pages), strategic
   context (one to two pages), the ask (one page), the case
   (three to five pages), risks and mitigations (one page),
   ROI hooks (half a page pointing at chapter 07), and the
   appendix. Compose the case from the artefacts the chapter
   names: the headcount trajectory from
   [[mod-108-leading-the-governance-function]] chapter 02
   (summarised as cost implication, not re-authored), the
   tooling cost from the vendor P&L files, the external-audit
   cost from the assurance-body relationship P&L, the maturity-
   progression cost from [[mod-107-program-measurement-and-
   maturity]] chapter 03, and the regulatory-change-readiness
   cost from [[mod-105-regulatory-change-management]]. The
   programme case's commercial shape is stable and year-on-
   year incremental; its risk shape is under-investment risk
   with gradual capacity degradation over eighteen to twenty-
   four months if compressed. Name both explicitly.

3. **Author the transformation case.** Produce the
   transformation case document to the chapter-02 structure,
   sized for the additional phase-and-sequencing detail
   transformation cases carry (five to seven pages in the case
   body). Name the specific transformation the enterprise is
   running — off spreadsheets onto a certifiable AIMS runtime,
   off point tools onto a governance-of-record platform, or
   legacy privacy-tooling retirement (or the specific
   transformation the enterprise's actual substrate position
   warrants). For each year of the transformation window
   (typically two to three years), author:
   - The front-loaded capex profile — implementation labour,
     license purchase or annual commitment, integration
     engineering — with the specific year each cost lands.
   - The dual-run cost profile — the legacy substrate that has
     to continue running until the new substrate is proven —
     with the specific window the dual-run persists across.
   - The retirement savings on the far side — the specific
     hidden labour recovered when the legacy substrate is
     retired, cross-referenced to chapter 07 for the modelled
     recovery — and the specific year the recovery begins to
     land.
   - The commit-or-abandon risk shape — the explicit CFO
     framing that partial funding produces the stranded
     outcome (running dual-run cost indefinitely with no
     escape either forward or back), so the CFO understands
     that a proportional compression on the transformation
     case does not produce a proportional reduction in
     capability.
   - The sequencing dependencies — the AIMS scope readiness
     ([[mod-102-running-the-program]] chapter 02), the hiring
     plan's implementation capacity
     ([[mod-108-leading-the-governance-function]] chapter 02),
     and the CxO peer alignment on platform-integration work
     (chapter 08). Sequencing risk is real; the case names it
     and the mitigations.

4. **Author the incident-preparedness case.** Produce the
   incident-preparedness case document to the chapter-02
   structure (three to four pages in the case body). Compose
   the case from the five components the chapter names: the
   contingency reserve (sized honestly against plausible
   incident scope from [[mod-110-incident-leadership]]), the
   incident-response retainer (a standing engagement with a
   DFIR firm with AI-incident specialism), the tabletop
   exercise budget (the recurring annual budget for cross-
   functional tabletops with the CISO, CPO, DPO, CRO, GC, and
   CAE), the cross-functional rehearsal cadence cost
   (evaluation rehearsals, containment rehearsals, external-
   communications rehearsals), and the external-communications
   retainer (a standing engagement unlockable on incident
   event). The case's commercial shape is standing cost plus
   reserve plus on-event authority; make the asymmetric risk
   shape visible in the CFO framing — the standing cost is
   small, the on-event authority is what the case actually
   buys, and the on-event authority is worthless if the
   standing infrastructure is not in place when the incident
   lands. Cite public incident precedent for the sector where
   one exists (the pattern rather than the party — the head
   does not name specific enterprises), and use incident-
   precedent framing to defend tooling lines the sector's
   incident history has made materially prudent.

5. **Author the three-audience differentiation.** Produce
   three audience-shaped renderings of the case pack, one per
   audience. The three renderings share a single spine
   (assumptions, line items, trajectory, ROI hooks) but are
   substantively different documents:
   - **The CFO two-pager plus supporting pack.** Opens with
     the three-year cost envelope. Carries the capex/opex
     breakdown, the ROI hooks cross-referenced to chapter 07,
     the peer-benchmark comparators where the head has
     credible peer data, the specific finance-team-facing
     detail the CFO's staff will re-run against, and the
     head's specific ask (year-one authorisation, year-two
     and year-three trajectory ratification, the contingency-
     reserve authority shape, the transformation-case commit
     or the transformation-case decision). The appendix
     carries the vendor P&L details and the line-item substance.
   - **The CEO two-pager.** Two slides. The strategic
     imperative in one paragraph (composing regulatory-
     licence-to-operate, competitive-differentiator, and
     incident-non-repeatability threads as the enterprise's
     context warrants). The specific ask in a second
     paragraph — endorsement in the next board meeting, veto
     over a CFO compression proposal, or a specific CxO-peer
     instruction (e.g., the CEO instructing the CIO to allocate
     platform-integration engineering time to the
     transformation case). No capex/opex breakdown on page
     one; the CEO does not have the finance team's time to
     re-run the numbers, and a CEO document that opens with
     capex/opex is not a CEO document.
   - **The audit-committee two-pager plus supporting pack.**
     Opens with assurance adequacy against the ratified AI
     risk appetite from
     [[mod-103-board-and-audit-committee-reporting]]. Carries
     the assurance-adequacy narrative, the independence-and-
     rigour signal, the mapping to the audit plan the CAE has
     authored (see [[mod-108-leading-the-governance-function]]
     chapter 05), and — critically — the case *before* CFO
     compression has been applied, so the committee
     understands what the head is asking for. If the CFO has
     compressed by the time the committee reads, the
     compression and its assurance-adequacy implications are
     explicit. ROI is a secondary concern in the audit-
     committee rendering; the committee's question is not "is
     this investment worth the money" but "is this investment
     adequate to the assurance obligation the committee has
     ratified." An audit-committee rendering that opens with
     ROI or capex/opex is the audit-committee-lite anti-pattern
     the chapter warns against.

6. **Run the five stress tests.** For each of the three cases
   (programme, transformation, incident-preparedness), run
   the five stress tests explicitly and document the answers:
   - **Why now, not next year.** Name the specific reason a
     year of delay is not free — the regulatory compliance
     date, the transformation sequencing window, the
     incident-readiness gap. A case that cannot answer this
     for a specific line item has authored a discretionary
     line the CFO will compress.
   - **What breaks if compressed.** Name the compression graph
     per line item. Some lines are linearly compressible (each
     dollar of compression removes a dollar of capability),
     some are step-function compressible (compression up to a
     threshold has modest impact, past the threshold breaks a
     capability), some are commit-or-abandon (partial funding
     produces the worst outcome). Name the shape for each
     line, not the posture "the line cannot be compressed at
     all."
   - **How do we know it worked.** Anchor each case to specific
     KRIs or KPIs from
     [[mod-107-program-measurement-and-maturity]] chapter 01,
     specific maturity-progression indicators, or specific
     audit-finding trajectories the head is prepared to be
     held to. A case without measurement is a case the audit
     committee cannot assure has worked.
   - **Who else pays.** Name, per line item, whether the cost
     is governance-function-owned entirely (the GRC-for-AI
     platform, the ISO/IEC 42001 CB engagement), shared (AI-
     runtime security tooling with the security function, AI-
     observability tooling with the evaluation team), or owned
     elsewhere but co-governed (product-team model cards,
     engineering-team model inventory contributions). Document
     the cross-CxO co-funding conversations the head has had.
   - **What if we did nothing.** Describe the no-investment
     counter-factual honestly per case — capacity degradation
     over eighteen to twenty-four months for the programme
     case, stranded substrate for the transformation case,
     unreadiness on days-to-weeks scale rather than hours-to-
     days scale for the incident-preparedness case. If the
     honest description is "not much," the case is padded and
     the head compresses it here rather than in front of the
     CFO.

7. **Author the response-to-challenge log template.** Author
   the template the head uses to log the challenges raised
   across the delivery sequence — by the CFO in the one-on-
   one, by the finance team in the analysis window, by the
   CEO in the joint conversation, by the audit-committee chair
   in the pre-read, by the audit committee in the meeting —
   and the response the head produced. For each log entry,
   the template captures:
   - The audience (CFO, finance team, CEO, audit-committee
     chair, audit committee).
   - The specific challenge raised (the line item, the
     assumption, the framing).
   - The response the head produced (the substantive answer,
     the artefact or appendix section cited, any commitment
     the head made).
   - The disposition (resolved in-cycle, deferred to next
     year's re-authoring, taken as a plan commitment).
   The log has three purposes the chapter names: the head
   does not have to re-author the same defence twice in a
   single cycle; the head has material for next year's re-
   authoring; and the head has a written trace of the case's
   evolution under scrutiny as a governance artefact.

8. **Author the delivery-sequence plan.** Author the specific
   sequence-and-timing plan for the enterprise's actual
   budget cycle — the CFO one-on-one date (before the
   finance-team pack lands), the finance-team analysis
   window (typically two to three weeks), the joint CFO/CEO
   meeting date, the audit-committee pre-read window with
   the committee chair, and the audit-committee meeting date.
   Name for each step:
   - The audience the head is preparing for.
   - The rendering of the pack the head brings (CFO pack, two-
     slide CEO deck, audit-committee pack) with the appendix
     scope for that audience.
   - The specific outcome the head is seeking from the step
     (CFO substantive alignment, finance-team credibility,
     CEO endorsement, audit-committee chair pre-read
     acknowledgment, audit-committee ratification).
   - The escalation path if the step does not produce the
     outcome (a second CFO one-on-one on a compression
     proposal, a written response to the finance-team read, a
     revised CEO conversation, an in-committee revision).
   The sequence matters — a case that lands with the audit
   committee before CFO alignment is a case that produces a
   difficult audit-committee conversation with no CFO backing,
   and a case that lands with the CEO before the finance-team
   analysis is a case the CEO cannot substantively endorse.

9. **Run the failure-mode audit.** Author a short section —
   one paragraph per failure mode — naming how the case pack
   detects and recovers from each of the six anti-patterns
   from chapter 02, plus the seventh (undiscussed-with-CxO-
   peers) the chapter also names:
   - **The everything-in-one-case pattern.** The three case
     types collapse into a single ask, the CFO carves
     proportionately, and the commit-or-abandon transformation
     case is damaged worst. Detection: the pack fails the
     three-case-type discipline. Recovery: separate the cases,
     each with its own commercial and risk shape.
   - **The narrative-only case.** Strategic language and
     regulatory-obligation framing with no line items the
     finance team can model. Detection: the appendix cannot
     be re-run by finance. Recovery: author the appendix
     substance the finance team needs.
   - **The overclaim-on-ROI case.** The case cites avoided-
     fine amounts, deal-enablement upside, or retention
     deltas the chapter-07 model will not defend. Detection:
     the ROI hooks exceed the modelled ROI numbers. Recovery:
     re-anchor to the modelled numbers.
   - **The pass-through-of-vendor-quotes case.** The pack is
     a stack of vendor quotes with a covering page rather
     than a business-owner position on the P&Ls. Detection:
     the head cannot answer a substantive question about a
     vendor line without opening the vendor quote. Recovery:
     author the business-owner substance on top of the
     vendor P&L inputs.
   - **The audit-committee-lite pattern.** The audit-
     committee rendering is a light re-brand of the CFO pack.
     Detection: the audit-committee two-pager opens with ROI
     or capex/opex. Recovery: author a genuine audit-
     committee rendering that opens with assurance adequacy.
   - **The single-year investment case.** The case has no
     year-two or year-three trajectory. Detection: the ask
     is for one year in isolation. Recovery: extend the case
     to the multi-year trajectory even if only year one is
     being ratified.
   - **The undiscussed-with-CxO-peers case.** The shared-cost
     lines have not been aligned with the CISO, CPO, DPO, or
     CIO before the CFO conversation. Detection: the "who
     else pays" stress test surfaces a shared line the head
     cannot say the peer has agreed to. Recovery: run the
     CxO-peer alignment ahead of the CFO conversation
     ([[mod-109-cross-enterprise-leadership]] and chapter 08).

## Deliverables

- `case-pack/programme-case.md` — the programme case document
  to the full chapter-02 structure (title, executive summary,
  strategic context, ask, case, risks and mitigations, ROI
  hooks, appendix) with the headcount, tooling, external-
  audit, maturity-progression, and regulatory-change-
  readiness components composed from the source artefacts.
- `case-pack/transformation-case.md` — the transformation case
  document, sized for the phase-and-sequencing detail, naming
  the specific transformation the enterprise is running, the
  front-loaded capex profile, the dual-run cost window, the
  retirement savings tail, the commit-or-abandon risk shape,
  and the sequencing dependencies.
- `case-pack/incident-preparedness-case.md` — the incident-
  preparedness case document, composing the contingency
  reserve, incident-response retainer, tabletop exercise
  budget, cross-functional rehearsal cadence cost, and
  external-communications retainer components, with the
  asymmetric risk shape made visible.
- `case-pack/cfo-two-pager.md` — the CFO-audience rendering,
  opening with the three-year cost envelope and the value-
  for-cost framing, with the supporting pack referenced.
- `case-pack/ceo-two-pager.md` — the CEO-audience rendering,
  two slides, opening with the strategic imperative and the
  specific ask, with no capex/opex breakdown on the first
  page.
- `case-pack/audit-committee-chair-two-pager.md` — the audit-
  committee-audience rendering, opening with assurance
  adequacy against the ratified AI risk appetite, mapped to
  the CAE's audit plan, with the case presented before CFO
  compression has been applied.
- `stress-tests.md` — the five stress tests run explicitly
  against each of the three cases (fifteen stress-test entries
  in total), with the specific answers documented per line
  where the case survives the test and per line where the
  head has compressed pre-CFO because the case did not
  survive.
- `delivery-sequence.md` — the specific sequence-and-timing
  plan for the enterprise's budget cycle, naming the CFO
  one-on-one date, the finance-team analysis window, the
  joint CFO/CEO meeting date, the audit-committee pre-read
  window, and the audit-committee meeting date, with the
  pack-rendering and outcome-sought per step.
- `response-to-challenge-log-template.md` — the running-log
  template the head uses across the delivery sequence, with
  the audience / challenge / response / disposition fields.
- `failure-mode-audit.md` — the seven failure-mode
  detection-and-recovery paragraphs (six chapter-02 anti-
  patterns plus the undiscussed-with-CxO-peers pattern), each
  naming the detection signal and the recovery action.

## Acceptance criteria

- Every one of the three cases (programme, transformation,
  incident-preparedness) has a specific ask populated with a
  specific cost envelope trajectory across the multi-year
  window. A case with a blank ask or a "TBD" cost envelope
  fails the criterion — the case pack is the budget-cycle
  instrument and cannot carry TBDs into the CFO one-on-one.
- Every one of the three cases survives all five stress tests
  or has been compressed pre-CFO on the specific test it did
  not survive, with the compression documented. A case that
  fails the "why now" test on a line item that has been kept
  in the ask fails the criterion; the head compresses before
  the CFO does.
- The audit-committee two-pager differs materially from the
  CFO two-pager. A light re-brand — the same substance with a
  re-titled cover — fails the criterion. The audit-committee
  rendering opens with assurance adequacy against the ratified
  risk appetite; the CFO rendering opens with the three-year
  cost envelope. A pack where the two documents can be
  produced by search-and-replace on the cover page is the
  audit-committee-lite anti-pattern.
- The "what if we did nothing" counter-factual is explicit and
  specific for each of the three cases. "Governance capability
  degrades" is not a counter-factual; "the intake queue depth
  KRI rises past the ratified threshold within [window], the
  regulatory-change absorption cadence extends past the
  compliance-date margin on the horizon-scanned register, and
  the AIMS scope cannot extend to the FY[X+1] system-inventory
  additions" is a counter-factual.
- The "who else pays" analysis exists for every shared or co-
  governed line item, naming the specific CxO peer whose
  function co-owns or co-governs the line and referencing the
  cross-CxO co-funding conversation the head has held. A
  shared line without the CxO-peer alignment fails the
  criterion, because it exposes the head to the CFO
  conversation the chapter warns against — the CFO asks
  whether the shared partner has agreed, the answer is no,
  the case fails in the CFO's presence.
- The three case types are kept structurally distinct in the
  pack. A single document that folds programme, transformation,
  and incident-preparedness spend together fails the
  criterion, because the CFO cannot carve compression cleanly
  when the three case types have different commercial and
  risk shapes.
- The CEO two-pager fits on two slides and opens with the
  strategic imperative rather than the cost envelope. A CEO
  rendering that opens with capex/opex, or that exceeds two
  slides, fails the criterion — it is not a CEO document.
- The response-to-challenge log template has the audience,
  challenge, response, and disposition fields populated with
  an example entry per audience, so the running log is
  operational from the first CFO one-on-one rather than
  authored on the fly under time pressure.
- The delivery-sequence plan places the audit-committee pre-
  read *after* CFO substantive alignment and *before* the
  audit-committee meeting. A sequence that lands the audit-
  committee rendering with unresolved CFO gaps fails the
  criterion; the committee reads unresolved CxO gaps as
  governance-function immaturity and discounts the substance
  accordingly.
- Any factual claim about peer-benchmark envelopes,
  contingency-reserve sizing bands, or public incident-
  precedent patterns carries a `<!-- needs-research: verify
  [specific fact] against [source] -->` marker where the fact
  is not independently verifiable. The chapter itself carries
  such markers on peer-benchmark sources and reserve-sizing
  bands; the exercise inherits the discipline. Specific budget
  figures are not invented for the case; the case-pack
  artefact carries the enterprise's actual numbers from the
  exercise-01 budget model, or, where the artefact is authored
  as a training deliverable rather than against a real budget
  model, the case carries the categories and structural shape
  without invented totals.

## Stretch goals

- Author the **compression-scenario pack** — the specific pack
  the head prepares for the case in which the CFO returns a
  compression proposal. For each of the three cases, name the
  compression levels the head is willing to accept (five
  percent, ten percent, fifteen percent, twenty percent), the
  specific capability lost at each level (per the compression
  graph in the stress-test artefact), and the specific
  compression the head will not accept without escalating to
  the CEO or the audit committee. The compression-scenario
  pack turns the reactive "how do you feel about the CFO's
  compression?" conversation into a pre-negotiated position.
- Author the **CxO-peer alignment memo** — the specific memo
  the head shares with the CISO, CPO, DPO, CIO, and CAIO
  before the CFO conversation, naming the shared-cost lines
  the head is carrying, the co-funding position the head is
  proposing, and the specific ratification each peer is being
  asked to provide. The memo is what enables the head to
  answer the "who else pays" stress test with the CxO peers'
  alignment already in hand rather than to promise the CFO
  the alignment will happen after the CFO conversation.
- Author the **transformation-case-abandonment decision
  template** — the specific template the head uses if the
  CFO compresses the transformation case below the commit
  threshold. The template walks the head through the decision
  to abandon the transformation case for the current year
  rather than accept the stranded-substrate outcome, the
  specific communication to the CEO and the audit committee
  on why the transformation is being deferred, and the re-
  authoring shape for the following year's cycle.
- Author the **incident-precedent citation library** for the
  enterprise's sector — a curated list of public incident
  patterns the head cites in the incident-preparedness case
  and in the programme case's tooling defence (prompt-
  injection patterns, training-data-provenance patterns,
  model-integrity patterns), with the specific line items
  each precedent supports. The library is the head's citation
  substrate across annual re-authorings; a citation library
  authored once serves multiple budget cycles.
- Author the **response-to-challenge log for a prior cycle**
  as a retrospective artefact — the head takes the log from
  the prior year's investment-case cycle and populates the
  disposition column with what actually happened (which
  challenges landed as planned changes, which challenges were
  deferred and are re-surfacing this cycle, which challenges
  the head under-estimated at the time). The retrospective is
  the discipline that makes the next cycle materially better
  than the current one.

## Notes and starter guidance

The most common first-cut failure is the case pack that folds
the three case types into a single ask. The head produces one
document with a headline number that composes headcount,
tooling, transformation labour, and incident-preparedness
reserve, and hands it to the CFO. The CFO carves compression
proportionately across the aggregate, because the CFO has no
signal on which components carry which commercial and risk
shapes. The programme case survives the compression at modest
capability loss; the transformation case, which is commit-or-
abandon, is stranded; the incident-preparedness case is
compressed on the standing infrastructure that is precisely
what the on-event authority depends on. Force the three-case-
type separation. Each case is authored as its own document,
with its own commercial shape, its own risk shape, its own
counter-factual, and its own compression graph. The CFO can
compress each on its own merits; the head defends each on its
own merits.

The second common failure is the three-audience differentiation
that is not genuine. The head authors the CFO pack substantively
and then produces the audit-committee version by re-titling the
cover and lightly editing the executive summary. The audit
committee reads the wrong-audience framing — ROI opening,
capex/opex detail early, assurance-adequacy framing muted — and
discounts the substance. The head is judged as one who does not
understand the audit committee's mandate, and the case suffers
across every subsequent year in front of that committee. Force
the audit-committee rendering to open with assurance adequacy
against the ratified risk appetite and to treat ROI as
secondary. The audit-committee document is a different document
from the CFO document; if the two can be produced by search-
and-replace, one of them is wrong.

The third common failure is the "what if we did nothing"
counter-factual that is soft. "Governance capability would
degrade" is not a counter-factual — it is a hedge. The credible
counter-factual is specific: which KRI moves past which
threshold, which regulatory obligation misses which compliance
window, which system-inventory scope goes uncovered, which
incident scenario the enterprise is not ready for. The head
who cannot author the specific counter-factual is the head who
has padded the case, and the CFO's finance team will find the
padding faster than the head expects. Author the counter-factual
first, before authoring the ask; the counter-factual is the
discipline that keeps the ask honest.

On the delivery sequence — the temptation is to compress the
sequence when the budget cycle is under time pressure. Skip the
CFO one-on-one, land the pack with the finance team directly,
push the joint CFO/CEO conversation and the audit-committee pre-
read into the same week. The compressed sequence produces the
CFO who first hears the substance in a joint conversation with
the CEO, the audit committee that first sees the case with
unresolved CxO gaps, and the finance team that has not had time
to re-run the numbers. Every one of those outcomes damages the
case's credibility. Run the sequence as authored — the CFO one-
on-one before the finance-team analysis window, the joint
CFO/CEO conversation after finance-team alignment, the audit-
committee pre-read before the meeting.

The case pack is a living artefact. Version it, date it, refresh
it at the annual CFO budget-cycle preparation window, extend
the year-two and year-three trajectory when year one closes and
the plan rolls forward, update the transformation case as the
transformation progresses through its phases, and re-anchor the
incident-preparedness case when a new sector incident pattern
warrants a specific tooling or retainer line. The response-to-
challenge log from each cycle is the substrate for the next
cycle's re-authoring; a case pack that is re-authored from
scratch each year is a case pack that never accumulates the
enterprise's specific defensive substance, and that loses to
the CFO's finance-team accumulation of institutional memory.
