# exercise-04: Public Sector / Federal Contractor Leadership Drill

**Estimated effort:** 4 hours

## Objective

Instantiate the public-sector leadership shape from chapter 05
against either a federal-agency CAIO scenario or a federal-
contractor scenario. The deliverable is the head's operating
package: for a Federal CAIO, the M-25-21 minimum-practice
implementation, the AI Governance Board operating cadence, the
FedRAMP + NIST SP 800-53 + NIST AI RMF integration, the IG-
relations stance, and the congressional-oversight readiness; for
a federal contractor, the AI-product characterisation for CAIO
consumption, the M-25-22 contract-terms alignment, the FedRAMP
posture, and the CAIO relationship map.

## Prerequisites

- Chapter [05-public-sector-federal-contractor-caio](../05-public-sector-federal-contractor-caio.md)
  — read and internalised.
- Chapter 04 of [[mod-104-regulator-engagement]] — the regulator
  inventory discipline the agency-side or contractor-side maps
  extend.
- [[mod-103-board-and-audit-committee-reporting]] cluster 4 —
  adapted for the AI Governance Board (agency) or the audit
  committee (contractor).
- A specific scenario. Options:
  - **Federal agency.** A CFO Act agency of chosen size (small,
    mid-size, or large) with a specified mission area (national
    security, health, financial, regulatory, benefits) and a
    specified AI use-case portfolio scale.
  - **Federal contractor.** A specified contractor scenario —
    IT services prime; specialised AI product vendor; cloud-
    services provider with FedRAMP High authorisation; or
    system integrator with multi-agency book of business.

## Steps

### Federal-agency track

1. **Agency profile one-pager.** Half-page scoping: agency mission
   area, size (personnel and budget bands), current CAIO
   designation and reporting line, existing AI Governance Board
   composition, AI use-case inventory scale.

2. **AI Use Case Inventory review.** For each AI use case in
   scope, record: mission function, use-case description, model
   type, data inputs, output usage, human-oversight design, and
   the high-impact determination with reasoning. Where the
   determination is close, name the members of the AI Governance
   Board who agreed with it and any dissents.

3. **High-impact minimum-practice compliance.** For each high-
   impact AI use case, map to the M-25-21 minimum practices —
   pre-deployment testing, ongoing monitoring, human oversight,
   notice, remedy, opt-out — with concrete implementation
   evidence per practice.

4. **AI Governance Board operating cadence.** Author the Board
   charter or standing operating procedure: chair (Deputy
   Secretary or designee), required members, meeting cadence,
   agenda ownership (CAIO), decision-recording, and OMB
   reporting integration.

5. **FedRAMP + NIST SP 800-53 + NIST AI RMF integration.** Per
   AI use case, name the FedRAMP authorisation status of the
   underlying cloud service (or the agency-native ATO status),
   the applicable 800-53 controls, and the AI RMF profile or
   Generative AI Profile applied. Coordinate signatures with the
   Authorising Official.

6. **IG relations stance.** Author the operating relationship
   with the agency's IG: standard IG-work notification protocol,
   document-response practice, participation in exit interviews,
   and the CAIO's response to any AI-related IG findings.

7. **Congressional-oversight readiness.** For the committees
   most likely to hold hearings or issue letters, prepare the
   CAIO's baseline briefing materials: agency AI mission
   context, high-impact AI use-case summary, compliance status,
   and open questions. Include the legislative-affairs
   coordination protocol.

8. **AI Governance Board narrative.** Author the Board's
   standing pack sections in the three-beat structure from
   chapter 05: inventory and minimum-practice status; AI
   acquisition and technical-framework posture; IG and
   congressional posture.

### Federal-contractor track

1. **Contractor profile one-pager.** Half-page scoping: business
   size, federal book of business (agencies and dollar bands),
   product portfolio in the federal market, existing FedRAMP
   authorisations, and current AI product portfolio.

2. **AI product characterisation for CAIO consumption.** Per
   product, author the characterisation document in language
   that maps directly to an agency CAIO's AI Use Case Inventory
   entry: mission function, use case description, model type,
   data inputs, output usage, human-oversight design, monitoring,
   notice and remedy design if high-impact.

3. **Contract-terms alignment with M-25-22.** For each active or
   in-negotiation federal contract, map to M-25-22 acquisition-
   framework expectations: performance-based structure, AI-
   specific rights (data rights, IP, model reuse,
   transparency), and vendor accountability provisions. Where
   contract terms are under-aligned, name the change proposal
   the enterprise would present at renewal.

4. **FedRAMP posture per product.** For each cloud-delivered AI
   product, name the FedRAMP impact level authorised, the ATO
   scope, and the AI-specific dimensions of the SSP (System
   Security Plan). Where authorisation is pending or planned,
   name the milestone.

5. **NIST AI RMF and profile alignment.** For each product,
   name the AI RMF alignment and any applicable profile
   (Generative AI Profile AI 600-1; sector-specific profiles).
   Evidence supporting the alignment is captured.

6. **CAIO relationship map.** For each agency the enterprise
   sells to, name: the agency CAIO (function; individual if
   publicly known); the account manager or business-development
   lead who fronts the commercial channel; the head-of-AI-
   governance's engagement cadence; the peer-fronting decision.

7. **Audit-committee narrative.** Author the audit-committee
   quarterly narrative in the three-beat structure from chapter 05:
   product characterisation status; contract terms across the
   book; CAIO relationship map current.

## Deliverables

### Federal-agency track

- `agency-profile.md`
- `ai-use-case-inventory.md` (or `.csv`)
- `high-impact-minimum-practice.md`
- `ai-governance-board-charter.md`
- `fedramp-800-53-ai-rmf-integration.md`
- `ig-relations-stance.md`
- `congressional-oversight-briefing.md`
- `ai-governance-board-narrative.md`

### Federal-contractor track

- `contractor-profile.md`
- `product-characterisation.md` (one entry per product)
- `contract-terms-alignment.md`
- `fedramp-posture.md`
- `nist-ai-rmf-alignment.md`
- `caio-relationship-map.md`
- `audit-committee-narrative.md`

## Acceptance criteria

### Common

- Every entry cites the specific memorandum or framework it
  attaches to (M-25-21, M-25-22, NIST AI 100-1, NIST AI 600-1,
  FedRAMP baselines).
- Uncertain memorandum status (M-25-21 / M-25-22 as current or
  subject to amending guidance) carries a `<!-- needs-research: -->`
  flag rather than a guess.

### Federal-agency track

- Every AI use case has a high-impact determination with
  documented reasoning.
- Every high-impact AI use case has minimum-practice compliance
  evidence per practice — not a category note.
- The AI Governance Board charter names the chair, members,
  cadence, and OMB reporting integration.
- FedRAMP + 800-53 + AI RMF integration is per use case, not a
  single blanket statement.
- IG relations and congressional-oversight readiness are
  operating practices, not one-time preparations.

### Federal-contractor track

- Every product has a CAIO-consumable characterisation entry.
- Contract-terms alignment is per contract or per master
  agreement, not per product family.
- FedRAMP posture is per product with impact level named.
- CAIO relationship map has a named individual (or function if
  hypothetical) and a peer-fronting decision per agency.

## Stretch goals

- **Federal agency.** Rehearse an IG audit walk-through: the IG
  has opened an audit of the agency's high-impact AI compliance.
  Author the response plan across the CAIO office, the AI
  Governance Board, general counsel, and OMB coordination.
- **Federal agency.** Author the response to a congressional
  letter asking pointed questions about a specific high-impact
  AI use case. Include the coordination flow through legislative
  affairs, general counsel, and OMB.
- **Federal contractor.** Rehearse an agency CAIO's rejection
  of a product's characterisation as insufficient for their
  inventory. Author the head's re-characterisation response
  plus the internal-product-management coordination that
  reshapes the product artefacts.
- **Federal contractor.** Author the enterprise's stance for a
  situation where two agencies interpret the same M-25-21
  practice differently, and both are customers. How does the
  head reconcile without appearing partisan?

## Notes and starter guidance

- The public-facing nature of the AI Use Case Inventory is the
  most distinctive feature of the federal-agency track. Every
  entry is a public commitment. The exercise's inventory
  discipline reflects that — no entry that would embarrass a
  reader at a congressional hearing.
- The Federal CAIO's authority is set by memorandum, not by
  charter. Designs that treat the CAIO as a charter-negotiated
  role and understate the memorandum's specifics fail the
  exercise.
- The federal contractor's job is not to replicate the agency
  CAIO's role internally; it is to supply AI product
  characterisations the agency CAIO can drop into their
  inventory. Contractor designs that build a private-sector-
  style AI governance program without adapting to the CAIO
  workflow miss the sector's shape.
- IG relations are not adversarial. Designs that posture the
  CAIO defensively toward the IG fail on tone and on
  substantive fit with M-25-21's cooperative frame.
- Congressional oversight preparation is a discipline, not a
  one-time hearing prep. Standing baseline briefing materials
  are the exercise's expectation.
- Memorandum status is a live-issue item. Federal AI policy has
  moved and continues to move; the exercise expects
  `<!-- needs-research: -->` flags on any item where current
  effective status is uncertain.
