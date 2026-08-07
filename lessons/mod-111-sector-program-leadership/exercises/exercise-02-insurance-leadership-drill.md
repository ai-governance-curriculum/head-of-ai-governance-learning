# exercise-02: Insurance Leadership Drill

**Estimated effort:** 4 hours

## Objective

Instantiate the insurance-sector leadership shape from chapter 02
against a specific US insurer (property and casualty, life, health,
or a mixed carrier). The deliverable is the head's operating
package for an insurer: a state-by-state regulatory map, an AI
Systems Program mapped to the NAIC AI Model Bulletin, a Colorado
Regulation 10-1-1 fit-check, an actuarial coordination protocol,
consumer-facing AI evidence packs across pricing, underwriting,
claims, and marketing, and a board-level three-beat story.

The deliverable is not a survey of insurance AI regulation. It is
the operating record the head defends state-by-state at the next
DOI examination.

## Prerequisites

- Chapter [02-insurance-doi-and-naic-leadership](../02-insurance-doi-and-naic-leadership.md)
  — read and internalised.
- Chapter 04 of [[mod-104-regulator-engagement]] — the sector-
  regulator engagement pattern the state-by-state map extends.
- [[mod-103-board-and-audit-committee-reporting]] cluster 4
  shape.
- A specific insurer scenario. Options: US-only regional P&C
  writer; multi-state life writer; national health insurer
  operating under state DOIs plus HHS OCR for HIPAA overlaps;
  or a mixed carrier. Include a specific state footprint list.

## Steps

1. **Insurer profile one-pager.** Half-page scoping: line-of-
   business mix, state footprint by count and by-name, direct
   written premium band, AI portfolio scale, and existing
   actuarial function structure (in-house Chief Actuary, external
   consulting actuary, or hybrid). Every state written in is a
   separate entry in the regulator inventory.

2. **State-by-state two-axis regulatory map.** For each state in
   the footprint, record three instrument layers per chapter 02:
   the underlying unfair-trade-practice and market-conduct
   statutes; the state's adopted version of the NAIC AI Model
   Bulletin (or a `<!-- needs-research: -->` flag if adoption
   status is uncertain); any state-specific AI or algorithmic
   decisioning instrument. Where the enterprise's footprint
   exceeds a manageable state-by-state view, adopt an explicit
   aggregation rule and name the states each aggregated entry
   covers.

3. **AI Systems Program mapped to NAIC bulletin expectations.**
   Author the enterprise AI Systems Program document mapped to
   the five substantive expectations of the NAIC AI Model
   Bulletin: written AIS Program, governance structure, risk-
   management controls, internal audit or independent evaluation,
   and documentation. Every material AI system in the inventory
   is inside the AIS Program's scope; the document names the
   inclusion criteria and the treatment of the exclusion set.

4. **Colorado Regulation 10-1-1 fit-check.** For every AI or
   external-consumer-data-driven system in scope of Colorado
   Regulation 10-1-1 (if the enterprise writes life in Colorado
   — or the broader lines if the regulation has been extended,
   verified against current status), map to Regulation 10-1-1's
   governance-and-risk-management framework. Where the
   enterprise does not write in Colorado, the fit-check runs as
   a maturity benchmark: does the AIS Program meet Regulation
   10-1-1's expectations even where they are not enforceable?

5. **NYDFS Circular Letter No. 7 (2024) fit-check.** For any
   underwriting or pricing AI used on New York risks, map to
   NYDFS's expectations: governance and risk management, fairness
   and disparate-impact testing, third-party AI oversight,
   disclosure.

6. **Joint operating protocol — head, Chief Actuary, Chief
   Underwriting Officer.** Author the written protocol per
   chapter 02: who owns what at each stage of AI-in-pricing
   lifecycle (development, actuarial calibration, underwriting
   deployment, rate filing, ongoing monitoring, retirement),
   with named signatures. The protocol names the Actuarial
   Standards of Practice the Chief Actuary operates against
   (ASOP 12, ASOP 56, and any AI-specific ASOP in force) and the
   evidence the AI Systems Program produces for the Chief
   Actuary's certifications.

7. **Consumer-facing AI evidence packs.** Author the AI-specific
   evidence packs for the four consumer-facing surfaces:
   pricing, underwriting, claims handling (Unfair Claims
   Settlement Practices Act), and marketing / distribution
   (state unfair-trade-practice authority).

8. **State-DOI examination-readiness pipeline.** Name the
   reconstitutable evidence pipeline that will answer a market-
   conduct examination in any state on demand. Per element,
   name the capture cadence and the owner.

9. **Board-level three-beat story.** Author the audit-committee
   quarterly narrative in the three-beat structure from chapter 02:
   AIS Program defensible against NAIC baseline plus state
   overlays; pricing and underwriting coordination protocol
   ratified; state-DOI regulatory posture coherent per state and
   in aggregate.

## Deliverables

- `insurer-profile.md` — the one-page scenario scoping.
- `state-by-state-map.md` (or `.csv`) — the two-axis regulatory
  map covering every state in the footprint.
- `ais-program.md` — the AI Systems Program document mapped to
  the NAIC bulletin's five expectations.
- `colorado-regulation-10-1-1-fit-check.md` — the fit-check
  against Regulation 10-1-1.
- `nydfs-circular-letter-7-fit-check.md` — the fit-check against
  NYDFS Circular Letter No. 7 (2024).
- `pricing-underwriting-joint-protocol.md` — the head / Chief
  Actuary / CUO joint operating protocol.
- `consumer-facing-evidence-packs.md` — the four evidence packs.
- `dois-examination-readiness-pipeline.md` — the reconstitutable
  evidence pipeline.
- `board-three-beat-story.md` — the audit-committee narrative.

## Acceptance criteria

- Every state the enterprise writes in is a separate entry, or
  covered by an explicit aggregation rule. "State DOIs" as a
  category label is not acceptable.
- The state-by-state map cites the specific NAIC Model Bulletin
  adopted version per state (or a `<!-- needs-research: -->`
  flag), the specific state statute, and the specific state
  AI-adjacent instrument.
- The AIS Program document maps every one of the NAIC bulletin's
  five substantive expectations to a concrete implementation.
- The Colorado fit-check and the NYDFS fit-check cite the
  specific instrument text (or a `<!-- needs-research: -->`
  flag) and map every expectation to enterprise implementation.
- The joint operating protocol names the head, Chief Actuary,
  and CUO signatures; cites the specific ASOPs the Chief
  Actuary operates against; and names ratification at the
  audit-committee tier.
- Consumer-facing AI evidence packs are separated by surface
  (pricing, underwriting, claims, marketing) with the
  applicable state statute per surface named.
- The examination-readiness pipeline is reconstitutable — for
  every element the exercise says the enterprise captures, the
  capture cadence and owner are named.
- The board-level three-beat story is drop-in ready to cluster 4
  of the board pack.
- Uncertain state-DOI adoption status, uncertain Colorado
  Regulation 10-1-1 scope, and uncertain ASB ASOP status carry
  `<!-- needs-research: -->` flags rather than guesses.

## Stretch goals

- Author the multi-state coordinated examination stance: the
  NAIC's Market Actions Working Group has designated the
  enterprise for a coordinated examination. What is the head's
  operating stance across the participating states, and how
  does the enterprise avoid delivering divergent responses to
  different state-DOI participating teams?
- Rate-filing walk-through: pick one hypothetical AI-augmented
  pricing model and author the AI-specific documentation the
  Chief Actuary needs from the head to produce a filable
  rate structure in a specified state.
- Author a stance for the state-AG channel — attorneys general
  are increasingly active on AI-driven unfair-trade-practice
  matters. Where does the head's regulator inventory place the
  state AG relative to the state DOI, and who fronts what?

## Notes and starter guidance

- The state-by-state discipline is the single hardest element of
  the exercise. Resist the urge to reduce fifty entries to
  "adopting states / non-adopting states / New York." If the
  enterprise writes in fifty states, a defensible aggregation
  rule names each state per aggregation.
- The Chief Actuary is a first-class counterpart in insurance
  AI governance in a way the CFO or the Chief Compliance
  Officer is not the same in other sectors. If the joint
  operating protocol relegates the Chief Actuary to a receiver
  of AI evidence, redesign it.
- Consumer-facing AI in insurance is not the same as consumer-
  finance AI in banking. The evidence pack for insurance
  pricing is different from the ECOA/Reg B pack for credit
  decisioning. The exercise is testing sector-specific
  discipline, not generic consumer AI evidence.
- The board-level narrative reads coherently across the state
  footprint if the state-by-state discipline was executed
  before the narrative was drafted. Practise the state
  discipline first; the narrative follows.
