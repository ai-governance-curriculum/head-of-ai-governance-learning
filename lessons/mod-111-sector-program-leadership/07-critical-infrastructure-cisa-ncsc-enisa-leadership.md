# Critical Infrastructure — Leading AI Governance for an Operator Under CISA, NCSC, ENISA, and Sector-Specific Regulators

## Motivation

A critical-infrastructure operator — an electricity utility, a
telecommunications carrier, a water utility, a transportation
operator, a financial-market-infrastructure operator, a healthcare-
sector operator to the extent that operator is designated
critical — supervises AI systems inside a regulatory frame that is
distinct from every other sector's. The systems the enterprise
operates are, by public policy, essential to national security and
public safety. That designation drives four supervisory surfaces
the head of AI governance leads against.

1. The cross-sector cyber-and-AI guidance published by government
   cyber authorities — CISA and NCSC in particular, ENISA in the
   EU, and equivalents in Canada, Australia, Singapore, and other
   jurisdictions the enterprise operates in.
2. The sector-specific safety and reliability regulator — FERC and
   NERC for US bulk electric power, the FCC and state PUCs for US
   telecom, EPA and state environmental agencies for US water,
   the FAA and DOT and state transportation authorities for US
   transportation, ENISA and national regulators under NIS2 in the
   EU, ICO for UK privacy overlays, sectoral agencies in each
   jurisdiction.
3. The privacy and data-protection regulator — the same regulators
   any enterprise faces, but with elevated attention where the
   operator's operational-technology (OT) data or customer-usage
   data flows into AI-driven decisioning.
4. Cyber-incident notification regimes — CIRCIA in the US, NIS2 in
   the EU, TSA Security Directives for pipelines, DOE incident
   reporting, sectoral cyber directives, plus state breach-
   notification statutes — all of which apply to AI-relevant
   incidents.

This chapter maps the leadership shape across the four surfaces
and against the recurring critical-infrastructure specifics: the
IT / OT boundary, the safety-case discipline that predates AI, and
the operator-safety-culture norms the head's AI program has to fit
inside.

## Core concept — AI as a modality inside the operator's existing safety and reliability framework

Critical-infrastructure operators run safety-and-reliability
frameworks that predate AI by decades. The North American Electric
Reliability Corporation (NERC) has enforceable reliability
standards for US bulk electric power. NERC Critical Infrastructure
Protection (CIP) standards for cybersecurity of the bulk electric
system have been operating since 2008 and are enforceable through
FERC-approved reliability standards. Rail-safety and aviation-
safety frameworks under DOT and FAA operate against enforceable
safety-case discipline. Water-system safety operates under EPA and
state safety-plan requirements.

The head of AI governance does not import an AI framework onto the
operator. The head extends the operator's existing safety-and-
reliability framework to cover AI as a modality within it. The
enterprise's OT engineering function, safety function, and
reliability function are the primary operating counterparts. The
CIO / CISO organisation is the cyber counterpart. The head's
program is an AI-specific overlay across those functions, not a
separate AI-governance stack.

## Cross-sector cyber-and-AI guidance

### CISA and NCSC — Secure AI System Development Guidelines and Deploying AI Systems Securely

CISA and NCSC published the Guidelines for Secure AI System
Development (28 November 2023) with agencies from more than a dozen
countries co-signing. The guidelines cover four areas: secure
design, secure development, secure deployment, and secure operation
and maintenance. They are the reference standard for what
"reasonable AI security" looks like across governments; they are not
enforceable by themselves but are cited by sectoral regulators as
the interpretive baseline.

CISA and partner agencies published Deploying AI Systems Securely
(April 2024) as a follow-on covering deployment and operational
practice.

The head of AI governance at a critical-infrastructure operator
runs the enterprise's mapping against both documents. Every AI
system in the enterprise's inventory is cross-walked to the four
Secure AI System Development areas and the deployment guidance's
practices, with the CISO / OT security lead / sectoral security
lead named as counterpart per practice. The mapping is on file for
sectoral-regulator inspection and for CISA engagement.

### ENISA and NIS2

The EU Agency for Cybersecurity (ENISA) publishes AI-relevant
guidance and reports, including the Framework for AI Cybersecurity
Practices and reports on AI supply chain and threat landscape.

The NIS2 Directive (Directive (EU) 2022/2555) applies to essential
and important entities in specified sectors — energy, transport,
banking, financial market infrastructure, health, drinking water,
waste water, digital infrastructure, ICT service management, public
administration, space, postal and courier services, waste
management, manufacture of critical products, food, digital
providers, and research. Member State transposition applies to the
enterprise where operating; the head of AI governance coordinates
with the enterprise's NIS2-compliance function on how AI-related
cyber incidents are handled under NIS2's incident-notification
regime.

<!-- needs-research: verify current member-state NIS2 transposition
status by member state relevant to the enterprise's footprint and
any AI-specific ENISA guidance issued since the entry-into-force
date (October 2024). Confirm against enisa.europa.eu and national
transposition-tracking publications. -->

### Equivalent bodies in other jurisdictions

- Canada — Communications Security Establishment (CSE) and the
  Canadian Centre for Cyber Security. Co-signed the CISA/NCSC 2023
  Secure AI System Development Guidelines.
- Australia — Australian Signals Directorate and Australian Cyber
  Security Centre. Co-signed the 2023 guidelines.
- Singapore — Cyber Security Agency of Singapore. Co-signed the
  2023 guidelines.
- Others per co-signatory list.

The head maintains a per-jurisdiction map for each government cyber
authority the enterprise engages, using the same regulator-
inventory discipline chapter 04 of [[mod-104-regulator-engagement]]
introduced.

## Sector-specific regulator coordination

The specific sector determines the primary sectoral regulator.

### Electricity — FERC, NERC, and state PUCs

- FERC (Federal Energy Regulatory Commission) approves reliability
  standards for the US bulk electric system.
- NERC (North American Electric Reliability Corporation) develops
  and enforces reliability standards, including the CIP standards
  for cybersecurity. AI systems used in bulk-electric-system
  operations (load forecasting driving dispatch, outage prediction,
  generation optimisation, transmission control assistance) sit
  inside the CIP perimeter.
- State PUCs (Public Utilities Commissions) regulate distribution
  utilities, retail service, and rate-setting. AI systems used in
  distribution-system operation, in rate-making analytics, or in
  customer-facing decisioning attach to PUC authority.
- DOE (Department of Energy) issues guidance and, through CESER
  (Office of Cybersecurity, Energy Security, and Emergency
  Response), operates the sector's cyber-incident coordination.

The head coordinates with the enterprise's reliability compliance
function on NERC CIP standards' application to AI, with the OT
engineering function on operational integration, and with the state
regulatory function on state-PUC filings that reference AI use.

<!-- needs-research: verify current NERC CIP standard set (CIP-002
through CIP-014 baseline, with expansions), any AI-specific NERC
alert or Reliability Guideline, and the current DOE approach to
AI-specific cyber-incident reporting for the electric sector.
Confirm against nerc.com and energy.gov. -->

### Telecommunications — FCC and international counterparts

- FCC (Federal Communications Commission) regulates US
  telecommunications, including its own emerging positions on AI-
  driven network operations and consumer-facing AI (robocall AI-
  generated content under the Telephone Consumer Protection Act,
  for example).
- International — Ofcom in the UK, ARCEP in France, BNetzA in
  Germany, ACMA in Australia, and equivalent national telecom
  regulators.
- ITU (International Telecommunication Union) sets international
  standards and publishes AI-relevant reports.

<!-- needs-research: verify current FCC positions on AI in
telecommunications, including any 2024-2026 orders or notices on
AI-generated voice content, AI-driven network operations, and AI
transparency in consumer-facing telecommunications. Confirm against
fcc.gov. -->

### Water — EPA and state environmental agencies

- EPA (Environmental Protection Agency) supervises drinking water
  and wastewater under the Safe Drinking Water Act and the Clean
  Water Act. AI systems used in water-quality prediction, treatment
  optimisation, or leak detection sit inside the safety-plan
  discipline.
- State environmental agencies enforce state safety-plan
  requirements, including the risk and resilience assessment
  requirements from America's Water Infrastructure Act.
- CISA operates the sector-specific coordination for water and
  wastewater as one of the 16 critical-infrastructure sectors.

### Transportation — FAA, DOT, and state authorities

- FAA (Federal Aviation Administration) regulates civil aviation.
  AI in aircraft systems, air-traffic-management systems, and
  airport operations attaches to FAA rulemaking and safety
  oversight.
- DOT (Department of Transportation) and its administrations
  regulate surface transportation. AI in autonomous vehicles, rail
  operations, pipeline operations, and hazardous materials
  transport each attaches to a modal administration (NHTSA, FRA,
  PHMSA, FMCSA).
- State DOTs regulate state-jurisdiction transportation
  operations.
- ICAO (International Civil Aviation Organization) and IMO
  (International Maritime Organization) frame international-level
  standards.

<!-- needs-research: identify current FAA, NHTSA, FRA, PHMSA, and
FMCSA rulemakings, orders, or safety letters specifically addressing
AI in each modal domain. AI-in-transportation rulemaking is
evolving; confirm current status against transportation.gov and
each administration's website. -->

### Financial-market infrastructure

- SEC and CFTC in the US, ESMA in the EU, FCA in the UK, and
  equivalents for capital-markets infrastructure. Financial-
  market-utility designations under Title VIII of Dodd-Frank
  attach elevated supervisory expectations.
- ECB and Eurosystem for payments in the euro area.
- CPMI-IOSCO principles for financial market infrastructures.

## The IT / OT boundary

Critical-infrastructure enterprises operate distinct information-
technology (IT) and operational-technology (OT) environments. IT
runs enterprise business systems — email, HR, corporate finance,
customer relationship management. OT runs the operational systems
that deliver the essential service — SCADA and industrial control
systems for electricity and water, network-management systems for
telecom, air-traffic-management systems for aviation.

The IT / OT boundary matters for AI governance because:

- OT systems have safety and reliability requirements that IT
  systems do not. An AI misbehaviour in an OT system can result
  in a physical-world event; an AI misbehaviour in an IT system
  usually cannot.
- OT systems have change-management discipline (typically
  cadenced, tested extensively, and often subject to regulator-
  approved planning) that IT systems do not. AI systems entering
  OT must fit that discipline.
- OT security architectures (network segmentation, whitelisted
  applications, air-gap or DMZ boundaries) constrain AI system
  design.

The head's program treats OT AI and IT AI as separate inventory
categories with separate controls. The head coordinates with the
Chief Operations Officer and the Chief Engineering Officer (or the
sector's equivalent) on the OT AI portfolio. The OT AI portfolio
is often small in count but disproportionately high in
consequence.

## Cyber-incident notification regimes

Critical-infrastructure operators face multiple cyber-incident
notification obligations, and the head owns AI-specific
dimensions of each.

- CIRCIA (Cyber Incident Reporting for Critical Infrastructure Act
  of 2022) requires covered entities to report substantial cyber
  incidents to CISA within 72 hours and ransomware payments within
  24 hours. CISA's implementing rulemaking is finalising the
  covered-entity definition and reporting-requirement detail.
- Sectoral cyber directives — TSA Security Directives for
  pipelines and rail; DOE and DHS coordination for electricity;
  sector-specific cyber directives for water and transportation.
- NIS2 for EU-footprint operators — incident-notification within
  the NIS2 framework's timeline.
- State breach notification for AI-related PII breaches.
- Where the operator is a public company or has public-company
  parent — SEC cyber incident disclosure under 17 CFR § 229.106
  and Form 8-K Item 1.05.

<!-- needs-research: verify CIRCIA final rulemaking status (proposed
rule published April 2024, final rule projected for late 2025 /
2026) and confirm effective compliance timing. Confirm against
cisa.gov. -->

The head's incident-leadership coordination with [[mod-110-incident-leadership]]
addresses the AI-specific incident-response discipline. The critical-
infrastructure overlay adds sector-regulator notification and the
operator's own emergency-response coordination requirements.

## The head's operating protocol with the CISO, COO, and Chief Engineering Officer

At a critical-infrastructure operator, the head of AI governance
operates through a three-function protocol with the CISO, the COO,
and the Chief Engineering Officer.

- The CISO owns cybersecurity. The head coordinates AI-specific
  cybersecurity (adversarial AI, prompt injection, model theft,
  training-data poisoning) with the CISO.
- The COO owns operations. AI systems in operational use — in
  IT or OT — sit inside the COO's operating cadence. The head
  contributes AI-specific technical characterisation.
- The Chief Engineering Officer (or Chief Technology Officer, in
  enterprises without a distinct CEO in the executive-officer
  sense) owns engineering discipline including OT engineering.
  The head coordinates AI in OT with the CEO.

The three-function protocol is written down, ratified, and
governed by the same enterprise-level operating architecture the
COO's incident-response and reliability-management framework
runs on.

## The head's board-level story at a critical-infrastructure operator

At the board — often with a Risk Committee or a Safety Committee
in addition to an Audit Committee — the AI governance story has
three beats.

1. The AI portfolio is inside the enterprise's safety-and-
   reliability framework, not beside it. The OT AI inventory is
   named, sized, and controlled to OT discipline. The IT AI
   inventory is named and controlled to enterprise IT discipline.
2. Cyber-and-AI guidance from CISA / NCSC / ENISA / national
   equivalents is mapped to the enterprise's program, with the
   CISO's implementation of each practice named. Sectoral-
   regulator posture (NERC CIP, FERC, PUCs, FCC, EPA, FAA, etc.,
   per sector) is coherent and current.
3. Incident-notification readiness is complete across CIRCIA,
   sectoral directives, NIS2 for EU-footprint operators, and
   SEC cyber-incident disclosure for public-company operators.

## Summary

- Critical-infrastructure AI sits inside the operator's existing
  safety-and-reliability framework. The head extends that
  framework to cover AI as a modality, not to replace it.
- Cross-sector cyber-and-AI guidance from CISA / NCSC (Secure AI
  System Development Guidelines, November 2023; Deploying AI
  Systems Securely, April 2024), ENISA for EU operators, and
  co-signatory national bodies (Canada CSE, Australia ACSC,
  Singapore CSA, and others) is the reference baseline.
- Sector-specific regulators — FERC and NERC for electricity, FCC
  and state PUCs for telecom, EPA for water, FAA and DOT for
  transportation, SEC and CFTC and ESMA and FCA for financial
  market infrastructure — each supervise AI use within their
  jurisdiction, and each attaches AI to existing safety-and-
  reliability discipline.
- The IT / OT boundary matters: OT AI has safety-and-reliability
  requirements IT AI does not, has stricter change-management
  discipline, and has architectural constraints. The head's
  inventory keeps OT AI and IT AI as separate categories with
  separate controls.
- Cyber-incident notification regimes — CIRCIA (US, in
  implementation), sectoral directives, NIS2 for EU footprint,
  state breach-notification statutes, SEC cyber-incident
  disclosure for public companies — apply to AI-relevant incidents.
- The head operates through a three-function protocol with the
  CISO, COO, and Chief Engineering Officer, ratified enterprise-
  wide.
- The board-level story has three beats: AI inside safety-and-
  reliability framework, cyber-and-AI and sectoral-regulator
  posture coherent and current, incident-notification readiness
  complete.
