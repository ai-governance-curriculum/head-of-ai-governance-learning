# exercise-06: Critical Infrastructure Leadership Drill

**Estimated effort:** 4 hours

## Objective

Instantiate the critical-infrastructure leadership shape from
chapter 07 against a specific operator scenario. The deliverable
is the head's operating package for an operator: a sector-specific
regulator map, a CISA / NCSC / ENISA cross-sector cyber-and-AI
guidance mapping, an IT / OT AI inventory split, a three-function
operating protocol with the CISO / COO / Chief Engineering
Officer, a cyber-incident notification readiness map across CIRCIA
/ NIS2 / sectoral directives / SEC Item 1.05, and a board-and-
Safety-Committee three-beat story.

The deliverable is not a survey of critical-infrastructure AI
regulation. It is the operating record the head signs into so
that the enterprise's AI use extends the operator's existing
safety-and-reliability framework rather than sitting beside it as
a parallel governance stack.

## Prerequisites

- Chapter [07-critical-infrastructure-cisa-ncsc-enisa-leadership](../07-critical-infrastructure-cisa-ncsc-enisa-leadership.md)
  — read and internalised.
- Chapter 04 of [[mod-104-regulator-engagement]] — the sector-
  regulator engagement pattern the sectoral-regulator maps extend.
- [[mod-109-cross-enterprise-leadership]] cluster on CISO, COO,
  and Chief Engineering Officer interfaces — the peer-CxO
  coordination pattern the three-function operating protocol
  instantiates.
- [[mod-110-incident-leadership]] chapter 04 (US serious-incident
  disclosure map) and chapter 03 (Article 73 filing) — the
  incident-notification discipline the CIRCIA / NIS2 / sectoral /
  Item-1.05 map instantiates.
- [[mod-103-board-and-audit-committee-reporting]] cluster 4 and
  any Safety-Committee-adjacent cluster.
- A specific operator scenario. Options:
  - **Electricity — investor-owned utility.** A US bulk-electric
    operator under FERC and NERC CIP, with a state-PUC-regulated
    distribution business and DOE-CESER coordination for cyber-
    incident reporting.
  - **Telecom — national carrier.** A US carrier under FCC
    authority, with Ofcom / ARCEP / BNetzA / ACMA exposure
    depending on international footprint, and ITU standards
    engagement.
  - **Water — regional utility.** A US drinking-water utility
    under EPA and state environmental authority, with America's
    Water Infrastructure Act risk-and-resilience-assessment
    obligations.
  - **Transportation — modal operator.** A transportation
    operator under FAA (aviation), NHTSA (surface vehicles),
    FRA (rail), PHMSA (pipeline), or FMCSA (motor carrier)
    authority, with state DOT overlays.
  - **Financial-market infrastructure.** A designated FMU
    (financial market utility) under Title VIII of Dodd-Frank
    with SEC / CFTC / ESMA / FCA exposure and CPMI-IOSCO
    principle alignment.
  - **Multi-sector operator.** An operator that straddles two
    or more of the above (a utility with a telecom subsidiary;
    a transportation operator with pipeline and hazardous-
    materials exposures).

## Steps

1. **Operator profile one-pager.** Half-page scoping: sector,
   geographic footprint (US federal regulators the operator
   answers to; EU member states if NIS2 exposure applies;
   Canadian / Australian / Singaporean footprint if
   equivalent-body exposure applies), IT / OT boundary shape
   (a rough sizing of the enterprise's IT environment versus
   its OT environment), current AI portfolio scale split
   between IT AI and OT AI (order-of-magnitude counts), and
   existing three-function operating structure (CISO, COO,
   Chief Engineering Officer or sector equivalent).

2. **Sector-specific regulator inventory.** For the operator's
   sector, enumerate every applicable sectoral regulator per
   chapter 07:
   - Electricity — FERC, NERC (with named CIP standards in
     scope), state PUCs (per state), DOE / CESER.
   - Telecom — FCC (with named orders or notices on AI), state
     PUCs where applicable, international counterparts per
     footprint, ITU.
   - Water — EPA, state environmental agencies (per state),
     CISA (as sector-risk-management agency for water/
     wastewater).
   - Transportation — FAA / NHTSA / FRA / PHMSA / FMCSA per
     modal footprint, state DOTs, DOT departmental oversight,
     ICAO / IMO where international.
   - Financial-market infrastructure — SEC / CFTC (and any
     FMU designation), ESMA / FCA per footprint, ECB /
     Eurosystem for euro-area payments, CPMI-IOSCO for
     principle alignment.
   Per regulator, apply the regulator-inventory discipline
   from chapter 04 of [[mod-104-regulator-engagement]]: named
   counterpart, formal channel, informal channel, peer-fronting
   decision, cadence, escalation stance. Cite the specific
   instrument the regulator enforces (or a
   `<!-- needs-research: -->` flag where the current instrument
   set is uncertain).

3. **CISA / NCSC / ENISA cross-sector guidance mapping.** For
   every AI system in the enterprise's inventory, map to:
   - The four areas of the CISA / NCSC Guidelines for Secure AI
     System Development (28 November 2023) — secure design,
     secure development, secure deployment, secure operation
     and maintenance.
   - The practices in CISA's Deploying AI Systems Securely
     (April 2024).
   - For EU-footprint operators, the ENISA Framework for AI
     Cybersecurity Practices and any AI-relevant ENISA reports
     (with `<!-- needs-research: -->` where current guidance is
     uncertain).
   - For jurisdictional footprints beyond the US and EU, the
     co-signatory national bodies' equivalent guidance
     (Canada's CSE / CCCS; Australia's ASD / ACSC; Singapore's
     CSA; others per footprint).
   Per practice per AI system, name the counterpart function
   (CISO, OT security lead, sectoral security lead) and the
   implementation status.

4. **IT / OT AI inventory split.** Author the enterprise's AI
   inventory in two clearly separated sections:
   - IT AI — enterprise business systems (email, HR, corporate
     finance, CRM). Standard enterprise IT controls apply.
     Change-management follows enterprise IT change-management.
   - OT AI — operational-technology systems (SCADA and ICS for
     electricity and water; network-management systems for
     telecom; air-traffic-management systems for aviation;
     dispatch systems for financial-market infrastructure).
     Safety-and-reliability requirements apply. Change-
     management follows OT change-management, which is typically
     cadenced, tested extensively, and often subject to
     regulator-approved planning.
   Per OT AI entry, name the sectoral-regulator instrument the
   entry attaches to (NERC CIP standard for electricity; TSA
   Security Directive for pipeline; safety-case for aviation;
   equivalent for other sectors) and the safety-case
   integration status.

5. **Three-function operating protocol.** Author the written
   protocol between the head, the CISO, the COO, and the Chief
   Engineering Officer, per chapter 07:
   - CISO — AI-specific cybersecurity (adversarial AI, prompt
     injection, model theft, training-data poisoning).
   - COO — AI systems in operational use across IT and OT.
   - Chief Engineering Officer — engineering discipline
     including OT engineering and safety-case integration.
   Name the specific decisions each function owns; name the
   specific decisions the head owns; name the joint decisions;
   name the escalation path where the three functions disagree.
   Ratify the protocol at the enterprise's operating-committee
   tier.

6. **Cyber-incident notification readiness map.** For every
   applicable notification regime, author the readiness map:
   - CIRCIA — covered-entity determination, 72-hour incident
     notification, 24-hour ransomware-payment notification,
     CISA reporting channel, coordination with sectoral
     directives.
   - Sectoral directives — TSA Security Directives for
     pipelines and rail; DOE / DHS coordination for electricity;
     sector-specific cyber directives for water and
     transportation. Per applicable directive, name the trigger
     and the operator's notification channel.
   - NIS2 for EU-footprint operators — member-state
     transposition applicable to the enterprise's footprint,
     with the notification timeline per member state.
   - SEC Form 8-K Item 1.05 — for public-company operators or
     public-company-parent operators, the materiality
     determination process and the four-business-day disclosure
     discipline.
   - State breach-notification statutes — per state where
     AI-related PII breach obligations apply.
   Per regime, name the trigger, the timeline, the decision-
   maker, the coordination with [[mod-110-incident-leadership]]
   chapter 04, and the standing-preparedness discipline.

7. **Board-and-Safety-Committee three-beat story.** Author the
   standing narrative in the three-beat structure from chapter
   07: AI inside the safety-and-reliability framework; cyber-
   and-AI and sectoral-regulator posture coherent and current;
   incident-notification readiness complete. The narrative is
   drop-in ready for the Safety Committee (or the Risk
   Committee) and reconciles with the Audit Committee's
   compliance-substance cluster.

## Deliverables

- `operator-profile.md` — the one-page scenario scoping.
- `sectoral-regulator-inventory.md` — the sectoral regulator
  inventory using the chapter-04 regulator-engagement
  discipline.
- `cisa-ncsc-enisa-mapping.md` (or `.csv`) — the AI-inventory-to-
  cross-sector-guidance mapping with counterpart and status per
  practice per AI system.
- `it-ot-ai-inventory.md` — the split inventory with OT-side
  sectoral instrument attachment.
- `three-function-protocol.md` — the head / CISO / COO / Chief
  Engineering Officer written protocol.
- `cyber-incident-notification-readiness.md` — the CIRCIA / NIS2 /
  sectoral / Item-1.05 / state-breach map with triggers and
  timelines.
- `board-safety-three-beat-story.md` — the standing Safety-
  Committee narrative.

## Acceptance criteria

- Every sectoral regulator applicable to the operator is a
  separate entry, with a named counterpart and a cadence.
  Aggregation labels ("state PUCs" for a multi-state operator)
  are acceptable only with an explicit aggregation rule.
- Every AI system in the inventory has a CISA / NCSC guidance
  mapping across all four areas, plus deployment-practice
  mapping and ENISA mapping where EU footprint applies. Missing
  areas are called out as gaps, not omitted.
- The IT / OT AI split is explicit and complete. Every AI
  system is in one category or the other; category "both" is
  not accepted (systems that touch both are decomposed into
  their IT and OT components).
- OT AI entries name the sectoral-regulator instrument the
  entry attaches to. "Enterprise cyber standards apply" is not
  sufficient for an OT AI in a NERC CIP or a TSA Directive
  scope.
- The three-function protocol names specific decisions per
  function. Functional-scope descriptions without decision-typing
  fail on accountability at incident.
- The incident-notification readiness map covers every
  applicable regime with a specific trigger, timeline,
  decision-maker, and standing-preparedness discipline.
- The three-beat story is drop-in ready to the Safety Committee
  or Risk Committee and reconciles with the Audit Committee's
  compliance-substance cluster.
- Uncertain instrument status (CIRCIA final rule; NIS2 member-
  state transposition; current FCC / FAA / EPA AI-specific
  guidance; current DOE-CESER AI reporting practice; sectoral-
  ISAC AI-incident-sharing state) carries a
  `<!-- needs-research: -->` flag rather than a guess.

## Stretch goals

- Rehearse a specific OT AI incident: a load-forecasting AI at
  an electricity operator produces an anomalous dispatch signal
  during a summer peak-load event. Author the incident-response
  walk-through against the three-function protocol, the NERC
  CIP incident-reporting obligation, the CIRCIA obligation, the
  state-PUC notification, and the internal safety-case-owner
  briefing.
- Rehearse a multi-jurisdiction cyber-incident: a compromise of
  a shared foundation-model provider affects operators in the
  US, the EU, and the UK. Author the coordination map for
  CIRCIA, NIS2 (per member-state transposition), and the ICO
  overlay, and the operator's coordination with the sectoral
  ISAC and CISA.
- Circulate the sectoral-regulator inventory and the incident-
  notification readiness map to a peer at another operator in
  the same sector (through the sector's ISAC channel or
  through direct executive contact) and incorporate one round
  of critique.
- Author the operator's stance for a scenario where a
  government body (CISA in the US; ENISA in the EU) requests
  voluntary AI-incident-sharing information beyond the mandatory
  notification obligation — the head's engagement posture, the
  legal counsel's confidentiality posture, and the sectoral-
  regulator coordination.

## Notes and starter guidance

- The single most common failure mode is importing a private-
  sector AI-governance framework onto a critical-infrastructure
  operator without extending the operator's existing safety-and-
  reliability framework. Designs that produce an AI stack beside
  the safety framework rather than inside it fail the exercise.
- The IT / OT split is not an optional distinction. OT AI has
  different regulatory attachment, different change-management
  discipline, and different consequence profile. Designs that
  treat OT AI as "IT AI with reliability requirements" miss the
  sector's shape.
- The three-function protocol prevents split answers at
  regulator or incident. If the operator's CISO, COO, and Chief
  Engineering Officer produce inconsistent responses to a NERC
  CIP audit or a CIRCIA notification, the protocol has failed.
- Sectoral-regulator engagement is per regulator. The CISA
  channel is not a substitute for the FERC / NERC channel; the
  ENISA channel is not a substitute for the national
  regulator's channel under NIS2 transposition; the SEC
  Item-1.05 channel is not a substitute for the sectoral
  directive channel. Designs that consolidate channels fail on
  regulator-facing coherence.
- Uncertain sectoral-regulator instrument status is a live-
  issue item. CIRCIA is in final rulemaking; NIS2 member-state
  transposition is uneven; FCC / FAA / EPA AI-specific guidance
  is moving; sectoral-ISAC AI-incident-sharing practice is
  evolving. The exercise expects `<!-- needs-research: -->`
  flags on any item where current effective status is
  uncertain.
