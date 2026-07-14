# exercise-04: Sector-Regulator Engagement Pattern Authoring

**Estimated effort:** 5 hours

## Objective

Instantiate the four-part sector-regulator engagement pattern
from chapter 04 — obligation surface, engagement channel, cadence,
escalation and evidence — for a specific sector footprint, and
produce the **sector-regulator inventory** that feeds cluster 4
(regulator engagement) of the quarterly board pack in
[[mod-103-board-and-audit-committee-reporting]].

The deliverable is not a survey of what a sector's regulators
care about. It is the operating inventory the head would drop
into the next board cycle and hand to a successor, with every
regulator named, every obligation cited, every enterprise
counterpart identified, and every escalation stance pre-decided.

## Prerequisites

- Chapter [04-sector-regulator-engagement-pattern](../04-sector-regulator-engagement-pattern.md)
  — Designing the Sector-Regulator Engagement Pattern — read and
  internalised. The four axes and the inventory field list are
  the scaffolding the exercise fills in.
- [[mod-101-role-scope-and-leadership-shape]], chapter 06 on the
  CxO adjacency map, so the enterprise counterparts named in the
  inventory reflect the actual peer geography, not an idealised
  one.
- [[mod-105-regulatory-change-management]] for the horizon-scanning
  cadence that will keep the inventory current after it is authored.
- [[mod-111-sector-program-leadership]] for depth on any sector
  the enterprise operates in, where the inventory needs more than
  chapter 04's illustrative treatment.
- Chapter [05-regulator-exam-runbook](../05-regulator-exam-runbook.md)
  — the exam runbook that governs examinations for the regulators
  in the inventory once the inventory is in force.
- A concrete enterprise in mind, with an assumed sector footprint
  (banking, insurance, medical devices / pharma, employment
  technology, consumer technology, or a chosen combination) and a
  jurisdictional footprint. Where any element is hypothetical,
  hold a working assumption and note it.

## Steps

1. **Sector selection and scope one-pager.** Pick the sector or
   sector combination the exercise will be authored against.
   Options: banking (US federal and state, or with UK/Canada/EU
   overlay); insurance (US state and NAIC, or with UK/EU overlay);
   medical devices or pharma (FDA, MHRA, EMA, Health Canada);
   employment technology (EEOC, DOL, NYC Local Law 144, state
   ADS statutes); consumer technology (FTC, CFPB where consumer
   finance applies, state AGs, state privacy agencies); or a
   chosen combination the enterprise straddles. Write a half-page
   scoping the exercise: sector, jurisdictional footprint,
   approximate AI portfolio scale, dominant regulator regimes,
   and any material sub-sector nuance (retail banking vs
   investment banking; life vs P&C insurance; Class II vs Class
   III device). This scoping is the scenario every subsequent
   artefact refers back to.
2. **Obligation surface catalog.** For every regulator in the
   selected footprint, list the specific citable instruments —
   rules, guidance, letters, bulletins, model laws, examination
   handbooks, consent-order templates — that attach to the
   enterprise. Each entry has a specific citation with title,
   number, and date. "Banking regulators" is not an entry; "SR
   11-7 (2011), OCC Bulletin 2011-12 (2011), SR 23-4 (2023)" is.
   Where the AI-specific instrument sits on top of a non-AI
   base instrument (NAIC AI Model Bulletin on top of state
   unfair-trade-practice statutes; EEOC May 2023 guidance on top
   of Title VII), both layers are named. Where an instrument's
   current status is uncertain (draft vs final; adopted vs
   pending), flag it as needs-research rather than guessing.
3. **Engagement channel map.** For each regulator, identify
   the head-side counterpart (named individual and function,
   not a generic role), the routine channel (letter, examination
   cycle, reporting form, docket submission, MOU), and the
   informal channel (industry-body working group, trade
   association, regulator advisory committee, speech circuit,
   academic conference). Then record the peer-fronting decision:
   who fronts the routine channel (line-of-business, general
   counsel, government affairs, CISO, DPO, or the head), and
   what event moves the front seat to a different peer.
4. **Cadence table.** Per regulator, record the operating rhythm:
   continuous supervision, periodic examination cycle, event-
   driven inquiry, complaint-driven inspection, submission-clock,
   RFI cadence, reporting-form frequency, MOU touch-points,
   consent-order milestone dates where applicable. The cadence
   determines whether the enterprise's evidence pipeline is
   standing or reconstitutable-on-notice; both stances are
   legitimate but they are different program designs.
5. **Escalation and evidence discipline.** For each regulator,
   author the sector-specific escalation ladder using the
   regulator's own vocabulary — MRA, MRIA, cease-and-desist,
   civil money penalty, and consent order for US banking; 483
   observation, warning letter, consent decree, and recall for
   FDA; enforcement notice, assessment notice, information
   notice, and monetary penalty notice for the UK ICO;
   resolution agreement and civil monetary penalty for HHS OCR;
   civil investigation demand and assurance of discontinuance
   for state AGs; cause finding, conciliation, and litigation
   for EEOC. Per tier, pre-decide the head's role (technical
   author, remediation designer, audit-committee briefer,
   factual-record author), the peer who takes the front seat,
   and the evidence discipline that governs the enterprise's
   response.
6. **Inventory artefact.** Assemble the entries from steps 2-5
   into a single running inventory — table form is fine, well-
   structured prose is fine, spreadsheet is fine — with the
   fields the board pack requires:
   - Regulator name and jurisdiction.
   - Obligation surface (specific citations with dates and
     current status).
   - AI-specific overlay on top of underlying base instrument
     where both apply.
   - Enterprise counterpart (named individual and function).
   - Routine engagement channel (formal and informal).
   - Peer-fronting decision.
   - Cadence.
   - Current status (routine, examination, MRA remediation,
     consent-order compliance, litigation, no active engagement).
   - Next-action-by-date with named owner.
   - Escalation stance pre-decided at each tier of the
     sector-specific ladder.
7. **Board-pack drop-in check.** Read the inventory back as if
   dropping it into cluster 4 of the next quarterly board pack
   from [[mod-103-board-and-audit-committee-reporting]]. Any
   entry that a board reader could not follow without asking a
   clarifying question is rewritten. Any entry that reduces to
   a category name is expanded to a specific citation.

## Deliverables

- `scope-one-pager.md` — sector, jurisdictional footprint,
  portfolio scale, and dominant regulator regimes.
- `obligation-surface.md` — catalog of citable instruments per
  regulator, with dates, status, and needs-research flags where
  status is uncertain.
- `engagement-channels.md` — head-side counterparts, formal and
  informal channels, and peer-fronting decisions per regulator.
- `cadence-table.md` — operating rhythm per regulator with the
  evidence-pipeline stance it implies.
- `escalation-ladder.md` — sector-specific escalation vocabulary
  per regulator with the head's role, front-seat peer, and
  evidence discipline at each tier.
- `sector-regulator-inventory.md` (or `.csv` / `.xlsx`) — the
  assembled inventory in the field structure chapter 04 specifies,
  in a form directly droppable into cluster 4 of the quarterly
  board pack.
- `board-pack-drop-in-check.md` — the read-back against the board
  pack, with any rewritten entries flagged and the rationale for
  the rewrite.

## Acceptance criteria

- Every listed regulator has at least one specific citation with
  a title, number where applicable, and date. Category references
  ("banking regulators," "state DOIs," "the FDA") without a
  specific instrument attached are not acceptable.
- Where an AI-specific instrument sits on top of a non-AI base
  instrument, both layers are named. NAIC AI Model Bulletin
  (adopted 14 December 2023) plus the state's unfair-trade-
  practice statute. EEOC May 2023 Title VII technical assistance
  plus Title VII itself. CFPB Circular 2022-03 plus ECOA and
  Regulation B.
- Every engagement channel has a named counterpart on the
  enterprise side (named individual and function; where the
  individual is hypothetical, flagged as such) and a named
  counterpart on the regulator side (examination-in-charge,
  supervisory team lead, or the specific office within the
  agency).
- Every peer-fronting decision is written down, per regulator,
  with the specific event that moves the front seat.
- Every escalation ladder uses the sector's own vocabulary.
  Banking uses MRA, MRIA, cease-and-desist, civil money penalty,
  consent order. FDA uses 483, warning letter, consent decree,
  recall. UK ICO uses information notice, assessment notice,
  enforcement notice, monetary penalty notice. State AGs use
  civil investigation demand and assurance of discontinuance.
  A generic "escalate to enforcement" is not sector-specific.
- Every inventory entry has a next-action-by-date with a named
  owner, or an explicit "no scheduled action; status is monitor"
  where that is the accurate posture.
- The inventory is droppable directly into cluster 4 of the
  regulator-engagement cluster of the board pack (see
  [[mod-103-board-and-audit-committee-reporting]]) without a
  separate translation pass.
- Where a citation's current status is uncertain (draft vs
  final; adopted by which states; effective date after
  legislative amendment), the entry carries a needs-research
  flag rather than a guess.

## Stretch goals

- Author a one-page written narrative for the audit committee
  summarising the aggregate regulatory posture across the sector
  footprint — where the enterprise is over-exposed, where under-
  engaged, where the posture is defensible and where it needs
  investment. Chapter 04's peer-fronting discipline and the
  inventory's current-status column are the raw material.
- Where the enterprise straddles two sectors (banking plus
  insurance is the most common combination; medical devices plus
  employment technology if the enterprise operates a device with
  employer-facing analytics; consumer technology plus health if
  the enterprise operates a wellness product with a device
  claim), produce a side-by-side rendering of the inventory
  covering both sectors, with the intersection points — regulators
  that supervise both, obligation surfaces that overlap, peer-
  fronting decisions that must reconcile — called out explicitly.
- Author the horizon-scanning intake shape that keeps the
  inventory current, per the hand-off in
  [[mod-105-regulatory-change-management]] — the specific format
  in which a new instrument, a status change on an existing one,
  or an amendment to a state adoption enters the inventory
  without requiring the head to re-author from scratch.
- Circulate the inventory to a peer at head-of-role level, or to
  a sector regulatory-affairs lead within the enterprise, and
  incorporate one round of critique before the inventory is put
  in force.

## Notes and starter guidance

- The single most common failure mode is category-level entries.
  "Banking regulators" is not a regulator. "State insurance
  departments" is not a regulator. If the enterprise writes in
  fifteen states, the inventory has fifteen state DOI entries
  or a defensible aggregation rule that names the states each
  aggregated entry covers. The board pack reader needs to be
  able to ask "which state" and get an answer.
- The peer-fronting decision is a design artefact, not a
  personal relationship. Write it so that when the CMRO, DPO,
  regulatory-affairs VP, or general counsel leaves, the
  successor inherits the front seat without renegotiation.
- Escalation stance is pre-decided precisely because the head
  should not be designing posture under time pressure when an
  MRA lands or a warning letter arrives. Put the stance in
  writing while the pressure is off; the audit committee will
  read it and either endorse it or ask for a revision, and
  either outcome is preferable to improvising in the moment.
- Evidence discipline at every tier is contemporaneous, primary,
  dated, attributable, and reconcilable to the underlying system
  state at the time the fact was true. Post-hoc reconstruction
  is a pattern examiners are trained to identify. The inventory
  entry for each regulator names the evidence pipeline that
  produces the primary record.
- Where chapter 04 flagged an instrument as needs-research
  (Colorado AI Act SB 24-205 effective date; TRAIGA current
  status; specific NYDFS circular-letter number; current HHS
  OCR AI guidance; state adoption list for the NAIC AI Model
  Bulletin), carry the flag forward rather than substituting a
  guess. An inventory with three needs-research flags and
  eighty confirmed citations is more useful than an inventory
  with eighty-three citations of unknown reliability.
- Resist the urge to make the inventory comprehensive at the
  expense of currency. An inventory that lists every regulator
  ever mentioned in any AI context, but is not updated when
  status changes, is a positioning artefact rather than an
  operating one. Chapter 04 is explicit on this point.
- The inventory is the head's operating record and the artefact
  by which the head's successor will be onboarded. Author it
  for a successor reader as well as for the board.
