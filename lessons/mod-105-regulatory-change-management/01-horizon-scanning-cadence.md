# The Horizon-Scanning Cadence at Leadership Scope

## Motivation

Regulatory change is the load-bearing input to the head of AI
governance's job that the head cannot commission, cannot delay, and
cannot negotiate. Everything else on the head's operating calendar —
the ISO/IEC 42001 AIMS management-review cadence
([[mod-102-running-the-program]] chapter 02), the board pack cadence
([[mod-103-board-and-audit-committee-reporting]] chapter 05), the
regulator engagement portfolio
([[mod-104-regulator-engagement]] chapters 01 to 05) — can be
sequenced by the head. The regulatory-change stream cannot. When the
EU AI Office publishes a General-Purpose AI Code of Practice, when a
national competent authority publishes new supervisory guidance, when
a US state attorney general finalises rulemaking, when OSFI issues an
E-23 revision, the head does not decide whether to respond. The head
decides only how fast and with what discipline.

That decision is only defensible if the head has *seen the change
coming*. Horizon scanning is the discipline that makes seeing it
possible.

The failure mode this module opens with is not a regulator surprising
the enterprise. The failure mode is the head being surprised by their
own program. A junior analyst on the level-15 tracking desk (see
[[mod-108-leading-the-governance-function]] chapter 01) knows about
a landing obligation three weeks before the head does. A product
leader gets a customer question about a new state AI act before the
head has even opened the interpretation memo. GC has been quietly
tracking a delegated act for months and the head learns about it in a
board pre-read. Each of these is a failure of the head's *scanning
cadence*, not of the analyst's tracking or the tracker's diligence.
The cadence is what turns raw tracking into the head's operational
awareness at the moment the head needs to make a decision.

This chapter builds the scanning cadence. Chapter 02 turns the
outputs of the cadence into the interpretation-and-prioritisation
workflow that decides what the enterprise does about them. Chapter 03
turns interpreted priorities into the enterprise change-management
plan. Chapters 04 to 07 rehearse the tension, the coordination, and
the concrete pending changes as of the research window.

## Core concept — scanning is a system, not an activity

Every enterprise that has been embarrassed by a regulatory-change
miss can point to somebody, somewhere, who saw it coming. Nobody
missed it in the sense of *nobody looking at the source*. The failure
is always downstream: the person who saw it did not know it mattered,
or the person who knew it mattered did not have the standing to make
the enterprise act, or the standing existed but the calendar did not
carry the item to the moment where a decision was possible.

The head who understands this stops trying to fix scanning by
"reading more". Scanning is a system with four components, and any
component that fails causes the whole system to look like the head
was not paying attention.

- **Sources.** The universe of monitored bodies, publications,
  registers, dockets, and channels, with an owner per source and a
  frequency per source. If a source is not on the list, the
  enterprise does not read it.
- **Cadence.** The rhythm at which sources are read, items are
  triaged, and the head is briefed. Different sources sit on
  different frequencies (daily wire, weekly desk review, monthly
  portfolio review, quarterly deep scan). The cadence is written
  down and it is the same in the calendar and in reality.
- **Escalation.** The rules that move a scanned item off the tracker
  and into the interpretation workflow (chapter 02). An item that
  merits escalation but never crosses the boundary is invisible;
  an item that gets escalated when it should not have been buries
  the head's attention.
- **Memory.** The register that holds the scanned universe over
  time, so items that were dismissed early can be revisited when
  facts change, and so the enterprise can defend, under audit, why
  it moved when it did.

The rest of this chapter walks each component. The head who
internalises the four-component structure stops asking "am I reading
enough?" and starts asking "which component of my scanning system is
degrading right now?" — which is the question that actually gets
fixed.

## Sources — the monitored universe

The head does not maintain the source list personally. The level-15
analyst tracking desk does. But the head *owns the shape* of the
list: which categories exist, what the minimum bar for inclusion is,
who owns each category, how new sources are added, how retired
sources are archived. A source list that grew by accretion over three
years, with nobody accountable for any category, is unusable.

The categories that matter for a head of AI governance operating a
program at enterprise scale, as of the research window, are the
following. Each source below is a public entry point; each has an
owner on the analyst desk and a frequency.

### Union-level and international bodies

- **EU AI Office** — publications and consultations on
  digital-strategy.ec.europa.eu, including GPAI Code of Practice
  work, guidance, and Commission implementing / delegated acts. The
  Office publishes a landing page for consultations and templates
  that shape how NCAs enforce.
- **European Artificial Intelligence Board** — the coordination
  forum for NCAs established under Article 65 of Regulation (EU)
  2024/1689. Board opinions and recommendations arrive via the AI
  Office channel.
  <!-- needs-research: verify current publication venue for European
       AI Board opinions and any operational cadence stated on the
       AI Office pages -->
- **EU Official Journal (OJEU)** — the citation channel for
  harmonised standards (once cited, harmonised standards create a
  presumption of conformity under the AI Act). Standards from
  CEN-CENELEC JTC 21 land here.
- **US AI Safety Institute (US AISI) and the AI Safety Institute
  Consortium (AISIC)** — evaluation-methodology publications and
  consortium work products, hosted by NIST. Also NIST's own
  publications — updates to the AI RMF, AI RMF Generative AI
  Profile, and public-comment dockets.
- **UK AI Safety Institute (UK AISI)** — Inspect framework updates,
  systemic-safety evaluation reports, and publications on the
  aisi.gov.uk channel.
- **G7 Hiroshima Process** — Code of Conduct updates, monitoring
  reports, and joint communiqués via the OECD.AI observatory and
  G7 presidency channels.
- **OECD.AI** — policy observatory, national AI policy inventory,
  and expert-group outputs.
- **ISO/IEC JTC 1/SC 42** — standards work programme (ISO/IEC
  42001, 42005, 42006, 23894, 5259 series, TR 24028, TR 24368,
  and adjacent work items). New parts and revisions arrive via the
  ISO catalogue and the SC 42 secretariat.
- **CEN-CENELEC JTC 21** — European AI standards work in support
  of the AI Act (the harmonised standards mandate). Publications
  arrive via the CEN-CENELEC catalogue and Commission citation in
  the OJEU.
- **IEEE Standards Association 7000-series** — ethically aligned
  design standards. Publications arrive via the IEEE catalogue.

### National competent authorities and horizontal regulators

- **EU Member-State NCAs** — Article 70 designations. The head
  tracks each Member State where the enterprise operates high-risk
  systems, with the lead NCA's publication channel as an owned
  source. NCAs vary in publication discipline; some publish
  supervisory statements, some publish only in national gazettes,
  some publish only via press release.
- **UK ICO** — ICO25 strategy carry-over, AI and data-protection
  guidance, ADM (automated decision-making) publications, and
  enforcement notices on ico.org.uk.
- **US Federal Trade Commission (FTC)** — Section 5 enforcement,
  AI-focused blog posts on the Business Blog, workshop transcripts,
  and consent orders.
- **US Consumer Financial Protection Bureau (CFPB)** — AI-related
  guidance on adverse-action notices, ECOA / Regulation B updates,
  and enforcement actions.
- **US Equal Employment Opportunity Commission (EEOC)** — AI-in-HR
  guidance (technical assistance documents), section 1607 discussion
  under the Uniform Guidelines on Employee Selection Procedures.
- **US Department of Labor (DOL)** — OFCCP-related guidance, AI-in-
  employment materials.
- **US HHS Office for Civil Rights** — Section 1557 rulemaking and
  HIPAA guidance touching AI.
- **US Federal Communications Commission (FCC)** — AI-generated
  voice / robocall guidance under the TCPA.

### US state attorneys general and state agencies

- **Colorado AG and Colorado Division of Insurance** — Colorado AI
  Act (SB 24-205) rulemaking and enforcement, Colorado Insurance
  Regulation 10-1-1.
- **Texas Office of the Attorney General** — Texas Responsible AI
  Governance Act (TRAIGA) and any related sub-regulatory guidance
  as it develops.
  <!-- needs-research: verify the enacted status and citation of the
       Texas Responsible AI Governance Act as of the research window
       against the Texas Legislature bill tracker and Texas Register -->
- **California Privacy Protection Agency (CPPA)** — CCPA / CPRA
  rulemaking, ADMT (automated decision-making technology)
  rulemaking, risk-assessment regulations.
- **California AGO** — rulemaking under state AI bills and consumer
  protection enforcement.
- **New York AGO and NYC Department of Consumer and Worker
  Protection** — NYC Local Law 144 enforcement (AEDT for employment
  decisions) and adjacent city / state rulemaking.
- **Illinois AGO and Illinois Department of Labor** — Illinois HB
  3773 amendments and enforcement, BIPA-adjacent AI matters.
- **Other state AGs** — the head tracks state AI bills across the
  states where the enterprise has material operations, via the
  National Conference of State Legislatures (NCSL) AI Legislation
  tracker and via state-legislature bill trackers.

### Sector regulators

- **Federal Reserve, OCC, FDIC (US banking)** — SR 11-7, OCC
  2011-12, SR 23-4 revisions or interpretive letters, plus the
  Federal Register for proposed rules touching model risk or AI.
- **OSFI (Canadian federal financial institutions)** — Guideline
  E-23 and successor / revision guidance.
- **NAIC (US state insurance)** — NAIC AI Model Bulletin adoption
  cadence across states, plus state Departments of Insurance for
  each state where the enterprise writes.
- **FDA (US medical devices, drugs, biologics)** — SaMD (software
  as a medical device) guidance, GMLP (Good Machine Learning
  Practice) publications, PCCP (predetermined change control plan)
  guidance, and CDER / CBER guidances touching AI. MDR (medical
  device reporting) obligations under 21 CFR Part 803.
- **MHRA (UK medicines and devices)** — Software and AI as a
  Medical Device Change Programme publications.
- **EMA and Health Canada** — analogous publications channels.
- **PMDA (Japan)** — pharmaceutical and device guidance.
- **CFPB and OCC on fair lending** — Regulation B and Fair Housing
  Act adjacencies.
- **FDIC and NCUA** — parallel financial-institution supervision
  publications.

### Cybersecurity and infrastructure agencies

- **CISA (US)** — Secure AI System Development Guidelines, JCDC
  publications, and secure-by-design guidance.
- **NCSC (UK)** — AI-related guidance and the CDEI's carried-over
  outputs.
- **ENISA (EU)** — AI-related threat landscape and good-practice
  publications.

### Voluntary codes, industry bodies, and standards-adjacent forums

- **Frontier Model Forum** — publications and working-group
  outputs.
- **Partnership on AI** — publications and consultations.
- **MLCommons AI Safety Working Group** — evaluation-suite
  publications and criteria.
- **Business Europe / DIGITALEUROPE** — EU-level industry positions.
- **Sector industry associations** — the enterprise's own sector
  bodies (SIFMA and ISDA for finance, PhRMA for pharma, AHIP for
  health payers, etc.), which mediate to Member-State ministries
  and to sector regulators.

### National regulators outside the US and EU

- **Korean AI Basic Act** — implementing decrees, ministry
  guidance, and enforcement communications.
  <!-- needs-research: verify the enacted status of Korea's AI Basic
       Act and any published implementing regulations as of the
       research window -->
- **Singapore IMDA and Model AI Governance Framework** — updates,
  AI Verify Foundation publications, and MAS publications for
  finance.
- **Japan METI and personal information regulator (PPC)** —
  publications and enforcement.
- **Canada** — federal AIDA (Artificial Intelligence and Data Act)
  status, Innovation, Science and Economic Development Canada
  guidance, and provincial regulators.
  <!-- needs-research: verify the current status of Canada's AIDA
       and any successor legislation as of the research window
       against the Parliament of Canada bill tracker -->
- **Brazil ANPD** — data-protection and AI publications.
- **India MeitY** — Digital India Act status, IT rules, and AI
  advisories.
- **Australia (Voluntary AI Safety Standard, DISR)** — publications
  and any move from voluntary to mandatory guidance.

The list above is not the final word. It is the shape of a list, the
categories that a head would defend to a certification body or a
third-line auditor asking "is your regulatory-change scanning
complete?" A head who cannot walk this shape from memory has a
scanning system that will fail under regulator inspection before it
fails under audit.

## Cadence — the rhythm that carries the source list to the head

The cadence layers three loops: a fast loop for signal detection, a
slow loop for portfolio review, and a longitudinal loop for maturity.

### The daily / weekly fast loop

Analyst desk activity happens on a daily wire and a weekly digest.
The head does not read the daily wire. The head reads the weekly
digest — a five- to ten-item summary produced by the analyst desk,
routed to the head every Monday morning, containing every new item
that crossed a triage threshold in the prior week.

The weekly digest has a rigid shape:

- **New obligations landed** — final rules, regulations, bulletins,
  or codes that are now binding or will be within twelve months.
- **New drafts published** — proposed rules or consultations open
  for comment.
- **New guidance / interpretive material** — supervisory statements,
  Q&As, blog posts from enforcement staff, workshop transcripts.
- **New enforcement / adverse action** — consent orders, MRAs,
  penalties, or public criticism from a named regulator directed at
  a named counterparty.
- **New standards work** — JTC 1 SC 42, JTC 21, IEEE, or NIST
  publications and drafts.

Each item on the digest carries three fields the head needs to act:
what it is, what source, and the desk's *preliminary triage*
(watch / active / priority — the escalation categories developed in
the next section). The head reads the digest in fifteen minutes and
gives the desk a decision on any item where the head disagrees with
the preliminary triage.

### The monthly portfolio review

Once a month, the head sits with the analyst desk lead and the
level-50 architect to review the *portfolio* of active and priority
items. The portfolio review is not "read the digest more slowly". It
is a portfolio-management exercise: which items have progressed,
which have stalled, which have new interpretation, which are ready
for the interpretation-and-prioritisation workflow in chapter 02.

The monthly review is where the head catches the pathology of an
item sitting on the tracker for six months with no motion. Either
the item is genuinely dormant (in which case it should be moved
back to watch) or it is silently blocked (in which case the block
needs to break). The monthly review is the head's calibration point
for the desk.

### The quarterly deep scan

Once a quarter, the desk performs a deep scan across the source
universe — not for new items (those come through the fast loop) but
for *source drift*: which sources have changed their publication
patterns, which have added new channels, which have gone quiet
(potentially indicating restructuring), which sources should be
added or retired.

The quarterly deep scan is also when the head briefs the CxO layer
(chapters 04 and 05 of this module cover the coordination pattern)
on the regulatory-change landscape — a rolling forward look on
what is landing in the next twelve months, what the enterprise is
positioned for, and what the enterprise is not.

### The annual scanning-system audit

Once a year, the head commissions an audit of the scanning system
itself — not of individual items scanned, but of the four components
(sources, cadence, escalation, memory). The audit is scoped as a
third-line audit engagement under
[[mod-108-leading-the-governance-function]] chapter 05 (CAE and
third-line coordination). Findings feed the annual maturity
assessment ([[mod-107-program-measurement-and-maturity]] chapter 03).

## Escalation — the rules that move items into interpretation

The scanning system produces a stream of items. The interpretation-
and-prioritisation workflow (chapter 02) can absorb only a small
fraction of that stream at any moment. The escalation rules are what
decide which items cross the boundary.

Three tiers. Every item in the register is one of the three.

- **Watch.** The item is on the tracker but no work is scheduled.
  The enterprise reads it as it evolves. Most items live and die at
  watch. Examples: a foreign state's draft AI act that will not
  affect the enterprise's operating markets; a standards work item
  in an early consultative stage; an enforcement action against a
  counterparty whose facts do not resemble the enterprise's own.
- **Active.** The item is scheduled for interpretation within the
  quarter. The desk begins pre-work: a plain-English summary, an
  attachment sketch, an owner assigned. The interpretation workflow
  (chapter 02) processes active items in priority order.
- **Priority.** The item has attributes that require immediate
  interpretation — a compliance date in the current or next quarter,
  a materially high attachment breadth, a formal notice from an NCA
  addressed to the enterprise, or an enforcement action against a
  close peer whose facts resemble the enterprise's own. Priority
  items enter the interpretation workflow within two weeks.

The escalation rules — what promotes an item across tiers — are
written down and reviewed at the annual scanning-system audit. The
rules the head defends to a certification body as of the research
window include:

- Any final rule with a compliance date within twelve months.
- Any obligation with attachment breadth covering more than a named
  threshold of the enterprise's AI system inventory (the level-50
  architect's crosswalk supplies the attachment estimate).
- Any formal correspondence from an NCA, whether an information
  request, a supervisory letter, or a public statement citing the
  enterprise.
- Any enforcement action against a peer in the same sector with a
  facts pattern the level-50 architect judges close enough to
  matter.
- Any citation in the OJEU that creates a presumption of conformity
  (harmonised standards under the AI Act).
- Any Article 73 serious-incident precedent from an NCA that shifts
  the reasonable interpretation of what "serious" means.

The head does not memorise every rule. The head memorises the shape
of the rules and defends them collectively. The desk applies the
rules on the wire; the head adjudicates disagreement at the monthly
portfolio review.

## Memory — the register that holds the scan over time

The final component is the register itself. Every item ever entered
into the scanning system has a durable record: what it was, when it
landed, what triage tier it entered at, what tier changes it went
through, why, and what interpretation output (if any) it produced.

The register serves four purposes.

- **Audit defence.** A certification body under ISO/IEC 42006, or a
  third-line internal auditor under IIA IPPF, or an NCA under
  market-surveillance information-request powers, may ask *why the
  enterprise did or did not act* on a specific obligation. The
  register is the answer. If the register cannot show that the item
  was seen, triaged, and disposed with reasoning, the head cannot
  defend the decision.
- **Later revival.** Items dismissed at watch sometimes need
  revisiting when facts change — a state passes a bill that had
  looked dead, a foreign regulator publishes enforcement material
  that reframes an earlier reading, a peer enforcement action
  changes the risk calculus. The register makes revival possible.
  Without the register, revival requires the desk to re-scan the
  universe, which is expensive and error-prone.
- **Cross-crosswalk into the level-50 architect's control library.**
  Items that reach interpretation and produce operating changes
  should trace back into the crosswalk that
  [[mod-102-running-the-program]] chapter 04 covers. The register
  is the trace point.
- **Program-measurement input.** Metrics like *median time from
  landing to interpretation start* and *fraction of items with an
  interpretation output within their tier's SLA* live in
  [[mod-107-program-measurement-and-maturity]] chapter 01. The
  register is the data source.

The register is not a spreadsheet on the head's laptop. It lives in
the GRC-for-AI stack that
[[mod-113-budget-vendor-p-and-l-and-investment-case]] covers, with
the same access controls, retention discipline, and integrity
requirements as the risk register itself
([[mod-102-running-the-program]] chapter 03).

## Coordination with the level-15 analyst and with legal

The four components above are the *shape* of the scanning system.
Its execution depends on two coordination interfaces the head owns.

The **analyst desk (level 15)** does the source-reading, the daily
wire, the weekly digest, the preliminary triage, and the register
maintenance. The head does not do these things and does not
second-guess them item-by-item. The head sets the shape (which
categories, which sources within each category, what the digest
must contain, what the triage tiers mean), reviews the shape at
the annual audit, and adjudicates at the monthly portfolio review.
[[mod-108-leading-the-governance-function]] chapter 02 covers the
level-15 analyst hire and career-pathing.

The **legal-opinion interpretation interface** — General Counsel and
the enterprise's outside counsel — is where interpretation with legal
force lives. The head's scanning system produces *preparation*, not
opinion. When an item enters interpretation (chapter 02), the head
packages the obligation and takes a technical position; GC delivers
the opinion. The scanning system does not deliver legal opinions and
does not label items as "compliant" or "non-compliant" — that
vocabulary belongs to GC. The scanning system labels items on the
program-management vocabulary: watch, active, priority; scheduled,
in-progress, disposed. This distinction is directly imported from
[[mod-104-regulator-engagement]] chapter 07 (the engagement-versus-
legal-opinion boundary).

## The one-sentence summary

Horizon scanning is the head's operational awareness system for a
domain the head cannot control. The head owns the *shape* of the
system (sources, cadence, escalation, memory); the analyst desk owns
the execution; GC owns the legal opinions the system produces
inputs for. When the head is surprised by a regulatory change, one
of the four components has failed — and the head can name which.

## Summary

- Regulatory change is the load-bearing input the head cannot
  commission or delay. The scanning cadence is what makes it
  possible to see change coming and act with discipline.
- Scanning is a system with four components: sources, cadence,
  escalation, memory. Any component failure looks like inattention
  from the outside.
- Sources span the Union, national, sector, cybersecurity, voluntary
  code, standards, and international bodies. The head owns the
  category shape; the level-15 analyst desk owns the source-by-
  source execution.
- Cadence layers a weekly digest, a monthly portfolio review, a
  quarterly deep scan of source drift and forward look, and an
  annual scanning-system audit sourced from the third line.
- Escalation moves items across watch → active → priority using
  written rules — compliance-date proximity, attachment breadth,
  formal NCA correspondence, peer enforcement, harmonised-standard
  citations, and Article 73 precedents.
- Memory lives in the register — every item ever scanned, its
  triage journey, and its disposition — serving audit defence,
  later revival, crosswalk trace, and program-measurement.
- The scanning system produces preparation, not legal opinion. The
  level-15 analyst desk executes; GC opines; the head sets the
  shape and adjudicates disagreement. Chapter 02 turns the outputs
  of the scanning system into the interpretation-and-prioritisation
  workflow.
