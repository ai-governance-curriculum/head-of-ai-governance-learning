# Designing the Sector-Regulator Engagement Pattern

## Motivation

The EU AI Act and the national competent authorities that will
enforce it are, for most enterprises, the smallest fraction of the
regulator surface the head of AI governance actually has to manage.
Chapters 01-03 of this module focused on that AI-specific surface
because it is new, because it is where the head's engagement pattern
is most visible externally, and because it is the surface a board
will ask about first. It is not the surface where the enterprise
spends the most regulator hours.

Those hours are spent with sector regulators. A bank's model-risk
examiners from the Federal Reserve or the OCC arrive on a rhythm
that has nothing to do with the EU AI Act. An insurer's state
department-of-insurance examiners arrive under the NAIC AI Model
Bulletin adopted 14 December 2023, and increasingly under the
market-conduct examination cycle that state DOIs have run for
decades. A medical-device manufacturer's FDA reviewers arrive under
premarket submission timelines that predate any dedicated AI
statute. An employer's EEOC investigators arrive under Title VII
and the ADA. A consumer-finance firm's CFPB examiners arrive under
UDAAP authority. The head of AI governance is accountable to every
one of these regulators for the AI-specific dimension of what they
supervise, even where the regulator has issued no AI-specific rule
and the head is not the primary enterprise counterpart.

This is the widest-scope chapter in the module because the head
cannot memorise every sector regulator's rulebook, and cannot
delegate the engagement stance to whichever peer already fronts
that regulator. The head needs a *pattern* — a way to design an
engagement stance for any sector regulator in the enterprise's
footprint — and then apply it, sector by sector, across the
regulator portfolio the enterprise actually faces. The rest of this
chapter is that pattern and a walk-through of the major sector
clusters as concrete examples. Depth on any specific regulator is
carried by [[mod-111-sector-program-leadership]]. Horizon-scanning
that keeps the portfolio current is carried by
[[mod-105-regulatory-change-management]]. Examination mechanics
themselves are carried by chapter 05 of this module.

## Core concept: the four-part engagement pattern

For any sector regulator in the enterprise's footprint, the head
designs an engagement stance along four axes. The axes are the
same whether the regulator is the Federal Reserve, the FDA, the
UK ICO, or a state attorney general. What varies is the content
at each axis, not the axis itself.

### Obligation surface

The first axis is the specific legal instrument the enterprise is
supervised under, and what that instrument obligates the enterprise
to do about AI. This is not "what does the regulator care about in
general." It is the citable rule, guidance, letter, bulletin, model
law, examination handbook, or consent-order term that the regulator
would open a conversation with.

For banking model risk, the citable instruments are Federal Reserve
SR 11-7 (2011), OCC Bulletin 2011-12 (2011, parallel to SR 11-7),
the interagency third-party risk management guidance SR 23-4
(2023), and the OCC Comptroller's Handbook chapter on model risk
management. For Canadian federally-regulated banks it is OSFI
Guideline E-23 on model risk management and Guideline B-10 on
third-party risk. For UK banks it is PRA Supervisory Statement
SS1/23 on model risk management principles for banks (2023). None
of these instruments is an "AI regulation" in the sense the EU AI
Act is. All of them govern the enterprise's AI systems when those
systems meet the instrument's definition of a model.

The obligation surface at the AI-specific layer is often *layered
on top of* a non-AI-specific instrument. The NAIC AI Model
Bulletin explicitly rides on top of unfair-trade-practice and
market-conduct statutes that already existed. EEOC Title VII
technical assistance on algorithmic assessments (May 2023) rides
on top of Title VII disparate-impact doctrine that has existed for
decades. The head names both layers — the underlying instrument
and the AI-specific overlay — because the enforcement action, if
it comes, will cite both.

### Engagement channel

The second axis is *who at the enterprise talks to this regulator*,
through what formal and informal channels, at what seniority. The
head is almost never the front-line counterpart. The line-of-
business chief compliance officer, the in-house lawyer assigned to
that regulator, government affairs, or the CISO typically owns the
day-to-day channel. The head owns the AI-specific technical
positioning that flows through that channel.

Formal channels are the letter, the examination cycle, the
reporting form, the docket submission, the MOU. Informal channels
are the industry-body working group, the trade-association meeting,
the regulator's advisory committee, the public speech circuit, the
academic conference where a regulator staffer presents. Both
matter. Enterprises that only appear in the formal channel are
strangers when the formal channel opens. Enterprises that appear
in both are known quantities, and known quantities get the benefit
of the doubt at ambiguity — which is where most AI-specific
questions live.

### Cadence

The third axis is the operating rhythm — reporting, examinations,
requests for information, MOUs, consent orders. For a large bank
under the Federal Reserve's continuous-supervision framework, the
cadence is effectively daily. For a state insurance department in a
smaller state, the cadence may be a market-conduct examination
every three to five years plus periodic RFIs. For the FDA on a
premarket submission, the cadence is the submission review clock
plus post-market surveillance. For an FTC UDAP inquiry, the cadence
is set by the FTC.

The head reads the cadence and builds the enterprise's response
capacity to match. A regulator on a continuous rhythm needs a
standing evidence pipeline. A regulator on a five-year rhythm needs
an evidence pipeline that can be *reconstituted* on notice, without
requiring anyone in the current organisation to remember what
happened four years ago. Program design differs at each rhythm.

### Escalation and evidence discipline

The fourth axis is what happens when routine engagement stops
being routine — a matter requiring attention (MRA), a matter
requiring immediate attention (MRIA), a formal enforcement action,
a consent order, a settlement. Each tier has its own posture, and
the head has a defined role at each tier.

<!-- needs-research: verify precise definitions of MRA and MRIA
against the current Federal Reserve SR letters and the OCC
Comptroller's Handbook; the terms are used across US banking
regulators but exact definitional language and process differs by
agency. -->

At the routine tier, the head is the AI-specific evidence author.
At the MRA tier, the head is the remediation designer — the MRA
becomes a tracked programme with a named owner, a milestone plan,
and a closing-evidence package. At the MRIA tier, the head briefs
the audit committee (see [[mod-103-board-and-audit-committee-reporting]])
and the general counsel escalates alongside. At the enforcement or
consent-order tier, the general counsel and external counsel front
the relationship; the head is the technical author of the
enterprise's factual record and the designer of the compliance
programme that the settlement will require. At every tier, the
evidence discipline is the same: contemporaneous, primary, dated,
attributable, and reconcilable to the underlying system state at
the time the fact was true. Post-hoc reconstruction is a red flag
that examiners are trained to identify.

## Sector-by-sector walk-through

The rest of this chapter walks the four-axis pattern through the
major sector clusters an enterprise head of AI governance is
likely to face. Coverage is illustrative rather than complete —
[[mod-111-sector-program-leadership]] carries depth on the sectors
the enterprise operates in.

### Banking — federal, state, and cross-border prudential

The core US federal banking model-risk instruments are Federal
Reserve SR 11-7 (2011) and OCC Bulletin 2011-12 (2011). The two
are near-parallel and are treated as the interagency baseline for
model risk management. FDIC-supervised institutions apply the same
substance under FDIC's own examination approach. Third-party risk
management, including third-party AI providers, is governed by the
interagency guidance issued as SR 23-4 in 2023, which superseded
each agency's prior separate guidance.

In Canada, OSFI Guideline E-23 on model risk management applies
across federally-regulated financial institutions, and OSFI
Guideline B-10 governs third-party arrangements. In the UK, PRA
Supervisory Statement SS1/23 on model risk management principles
for banks was issued in 2023. At the EU level, the EBA Guidelines
on Internal Governance and the ECB Guide to Internal Models set
the model-governance baseline for banks under the SSM.

None of these is an "AI regulation." All of them apply to AI
systems that meet the definition of a model — which, under SR 11-7,
is very broad. The head's obligation-surface reading is that
model-risk-management guidance is the primary AI supervisory
instrument for a bank, and any AI-specific bulletin from a
prudential regulator sits on top of it, not beside it.

The enterprise counterpart is typically the Chief Model Risk
Officer or the head of model-risk management, working through the
Chief Risk Officer to the Federal Reserve or OCC examination-in-
charge. The head of AI governance coordinates with the CMRO to
ensure the AI-specific dimensions — foundation model dependencies,
generative-AI use cases that were not contemplated by SR 11-7's
2011 drafting, third-party model providers — are within the MRM
framework rather than beside it. In many banks the two functions
are being consolidated; the head's stance is designed for
consolidation even where the reporting lines remain separate.

Cadence is continuous supervision at large institutions, punctuated
by targeted examinations and horizontal reviews. The head's
evidence discipline is the model inventory, the model-validation
record, the model-monitoring log, the change-management record for
each model, and the third-party attestation trail. Escalation runs
through MRA and MRIA to formal enforcement; the head's role at
each tier is the technical author, not the front-line responder.

### Insurance — NAIC and state DOIs

The NAIC AI Model Bulletin on the Use of Artificial Intelligence
Systems by Insurers was adopted 14 December 2023. It is a model
bulletin, meaning it becomes enforceable in each state only as the
state department of insurance adopts it. Adoption is on a rolling
basis and the head tracks the current-adopter list as part of the
regulator inventory.

<!-- needs-research: maintain a current list of state DOIs that
have adopted or are actively considering the NAIC AI Model
Bulletin; the list is moving through 2025-2026 and the head's
inventory needs a dated source. Early adopters commonly cited
include Connecticut and Colorado; verify current status directly
against each state DOI's bulletin publications. -->

The New York Department of Financial Services has issued its own
circular letter on the use of AI systems and external consumer
data in insurance underwriting.

<!-- needs-research: verify the specific NYDFS circular letter
number, year, and current status; NYDFS has issued multiple
circular letters on insurance AI use and the head's inventory
needs the current citation, not a paraphrase. -->

The obligation surface for a US insurer is therefore layered: the
state's underlying unfair-trade-practice and market-conduct
statutes, the state's adopted version of the NAIC AI Model
Bulletin (which may vary from the model text), any state-specific
circular letters or bulletins, and, for insurers writing in
multiple states, the intersection of all of the above. The head
maintains a per-state view because the obligation surface differs
per state.

The enterprise counterpart is typically the insurance-regulatory
compliance function, working through the general counsel to the
state DOI. Government affairs plays a heavier role in insurance
than in banking because the model-bulletin adoption cycle is itself
a policy process the enterprise engages with. Cadence is the
market-conduct examination cycle plus data calls, RFIs, and rate-
filing review. Escalation runs through examination findings to
consent orders and, in serious cases, to enforcement.

### Health — medical devices, pharma, and clinical use

The FDA published the Artificial Intelligence/Machine Learning
Software as a Medical Device Action Plan in January 2021, then
issued Good Machine Learning Practice guiding principles in
October 2021 jointly with Health Canada and the UK MHRA. FDA
released draft guidance on Predetermined Change Control Plans
(PCCP) for AI/ML-enabled device software functions in April 2023.

<!-- needs-research: verify whether the FDA PCCP guidance for
AI/ML-enabled device software functions has moved from draft to
final since April 2023, and update the citation accordingly.
Guidance-document status changes are exactly the kind of
regulatory-change item that must be current in the head's
inventory. -->

The MHRA operates an AI as a Medical Device work programme. The
EMA published the Reflection Paper on the Use of Artificial
Intelligence in the Medicinal Product Lifecycle. Health Canada
participates in the joint GMLP work with FDA and MHRA and issues
its own guidance on machine-learning-enabled medical devices.

The obligation surface splits into a pre-market layer and a post-
market layer. Pre-market obligations govern the submission itself
— 510(k), De Novo, PMA in the US; MHRA marketing authorisation in
the UK; EMA centralised or national procedures in the EU. Post-
market obligations govern surveillance, adverse-event reporting,
change control, and — under PCCP — the pre-authorised space
within which a model may continue to learn without triggering a
new submission.

The enterprise counterpart at a medical-device manufacturer or
pharma company is regulatory affairs, working through the chief
medical officer or chief regulatory officer to the agency. The
head of AI governance coordinates with regulatory affairs on the
AI-specific technical content of submissions, the GMLP-aligned
lifecycle documentation, and the post-market monitoring pipeline
that produces evidence for both the agency and the AI risk
management system. Cadence is the submission review clock plus
post-market surveillance and periodic reporting. Escalation runs
through inspection findings and 483 observations to warning
letters, consent decrees, and — at the extreme — product recall.

### Employment — EEOC, DOL, and state-level ADS statutes

The EEOC issued Technical Assistance on the Americans with
Disabilities Act and the Use of Software, Algorithms, and
Artificial Intelligence to Assess Job Applicants and Employees in
May 2022, followed by a Technical Assistance document on Title VII
and algorithmic assessments in May 2023. The DOL Wage and Hour
Division has issued guidance touching on AI in wage-hour
enforcement contexts.

At the city and state level, New York City's Local Law 144 on
automated employment decision tools took effect in 2023, and
Illinois's Artificial Intelligence Video Interview Act imposes
notice and consent requirements on AI-based analysis of video
interviews. Multiple state legislatures have active AI-employment
bills.

The obligation surface is layered on top of Title VII, the ADA,
the ADEA, and state civil-rights and employment statutes.
Algorithmic assessment is a modality question; the underlying
prohibition on disparate impact and disparate treatment is the
substance. The head's stance is that AI-specific bulletins from
EEOC extend, but do not replace, the underlying anti-discrimination
regime.

The enterprise counterpart is typically the chief human resources
officer and employment counsel, working with the general counsel
on any enforcement matter. The head of AI governance coordinates
on the fairness evaluation evidence, the vendor attestation trail
for AI-based hiring or performance tools, and — for NYC Local Law
144 — the annual independent bias audit and the public-facing
summary. Cadence is charge-driven at EEOC (a charge triggers an
investigation cycle) and audit-driven at NYC (annual bias audit
plus notice obligations). Escalation runs through cause findings
and conciliation to litigation.

### Consumer — FTC and CFPB

The FTC has issued a series of business-guidance blog posts and
enforcement statements applying Section 5 of the FTC Act (unfair
or deceptive acts or practices) to AI, and has finalised the
Government and Business Impersonation Rule. Its enforcement
posture treats AI-specific claims as commercial claims subject to
substantiation, and treats AI-enabled deceptive conduct as
actionable under existing authorities.

The CFPB issued Circular 2022-03 on adverse action notification
requirements under the Equal Credit Opportunity Act and Regulation
B in the context of algorithmic credit decisioning, and Circular
2023-03 on the use of chatbots in consumer finance. The circulars
are advisory as to CFPB's supervisory and enforcement posture; the
underlying obligation surface is ECOA/Reg B and the Consumer
Financial Protection Act's UDAAP authority.

The enterprise counterpart is the chief compliance officer at a
consumer-finance firm, working with general counsel; at a non-
finance consumer-facing firm, it is the general counsel and the
marketing-compliance function. The head coordinates on the AI-
specific dimensions of adverse-action explanation, chatbot design
and disclosure, and substantiation of AI-related product claims.
Cadence at CFPB is examination plus supervisory highlights; at
FTC, it is inquiry-driven or rulemaking-driven. Escalation runs
through consent orders, and in the FTC's case, through Section 13(b)
and Section 19 proceedings.

### Health privacy — HHS OCR

HHS Office for Civil Rights enforces HIPAA and the HITECH Act.
AI systems that process protected health information are covered
entities' or business associates' systems under HIPAA and fall
within the same Privacy Rule, Security Rule, and Breach
Notification Rule obligations as any other PHI-processing system.
OCR has issued guidance touching on AI in healthcare in recent
years.

<!-- needs-research: identify current HHS OCR guidance specifically
addressing AI systems processing PHI, including any bulletins on
online tracking technologies as they apply to AI-driven analytics
in healthcare. OCR's guidance in this space is being updated and
the head's inventory needs current citations. -->

The obligation surface is HIPAA and its implementing regulations.
The AI-specific overlay is thinner than at other sector regulators
because OCR's enforcement posture treats AI as a technology that
processes PHI, not as a distinct regulated modality. The head's
stance is to apply HIPAA to AI systems the same way HIPAA applies
to any PHI-processing system, and to add AI-specific evidence
where AI increases the surface area (training-data governance,
inference logging, prompt handling of PHI).

The enterprise counterpart is the HIPAA privacy officer and
security officer, working with the general counsel. Cadence is
complaint-driven and breach-driven. Escalation runs through
resolution agreements and civil monetary penalties.

### US state privacy and AI regulators

The California Privacy Protection Agency is engaged in rulemaking
on Automated Decisionmaking Technology under the CCPA/CPRA. The
Colorado Attorney General enforces the Colorado AI Act (SB 24-205),
which was signed in May 2024.

<!-- needs-research: verify the current effective date of the
Colorado AI Act (SB 24-205); the statute as signed set an effective
date but has been subject to potential amendment and delay through
the 2025 legislative cycle. Confirm current status against the
Colorado General Assembly and Colorado AG publications. -->

The Texas Attorney General has authority under Texas consumer-
protection and privacy statutes, and Texas has considered a
Responsible AI Governance Act (TRAIGA).

<!-- needs-research: verify current status of TRAIGA and any Texas
AG guidance on AI-specific enforcement priorities; state-level AI
statutory activity is moving quickly and the head's inventory needs
current citations. -->

Other state attorneys general are increasingly active on AI-
specific enforcement matters under general consumer-protection
authority, and the multistate AG coordination on tech issues that
has developed over the past decade extends to AI.

The obligation surface at the state level is the specific state
statute plus the state's general UDAP authority. The head's stance
is to treat each state AG office and each state privacy agency as
a distinct regulator in the inventory, with distinct obligation
surfaces, distinct counterparts (typically state-specific outside
counsel plus in-house), and distinct cadences.

### UK data protection — ICO

The UK Information Commissioner's Office updated its Guidance on
AI and Data Protection in 2023 and operates a regulatory sandbox
that admits AI-focused applicants. The ICO's enforcement posture on
automated decision-making draws on Article 22 of the UK GDPR and
on the underlying fairness, lawfulness, and transparency
principles.

The obligation surface is the UK GDPR and the Data Protection Act
2018, with the ICO's AI-specific guidance sitting on top as the
regulator's articulation of how those instruments apply to AI. The
head coordinates with the data protection officer, who typically
owns the ICO relationship. The head's role is the AI-specific
technical content — the DPIA methodology for AI systems, the
Article 22 analysis for automated decisions, the sandbox
application if the enterprise chooses to engage.

Cadence is a mix of complaint-driven, audit-driven, and voluntary-
engagement (sandbox, prior consultation). Escalation runs through
information notices, assessment notices, and enforcement notices
to monetary penalty notices.

### Cyber — CISA and NCSC

The US Cybersecurity and Infrastructure Security Agency and the
UK National Cyber Security Centre jointly issued the Guidelines
for Secure AI System Development in November 2023 and the Joint
Guidance on Deploying AI Systems Securely in April 2024. The
guidance is not enforceable by itself; it establishes the
expectation baseline that both agencies apply in their supervisory
and advisory roles, and that other regulators cite as a reference
for what "reasonable" AI security looks like.

The obligation surface, strictly speaking, is elsewhere — sector-
specific cybersecurity statutes, the FTC's data-security cases,
state data-security statutes, HIPAA Security Rule, GLBA
Safeguards Rule, PCI DSS as a contractual overlay — with CISA/NCSC
guidance operating as the interpretive reference. The enterprise
counterpart is the CISO. The head of AI governance owns the AI-
specific application of secure-development and secure-deployment
practices, and coordinates with the CISO on the boundary between
enterprise cybersecurity and AI-specific security.

Cadence for CISA is advisory and incident-driven; for NCSC,
advisory and incident-driven within the UK's cyber-incident
regime. Neither is a traditional supervisor. The value of the
engagement is at the informal channel — the working groups, the
consortium meetings, the pre-publication comment cycles on joint
guidance — and at the incident-response channel when the
enterprise experiences an AI-relevant cyber incident.

## The peer-fronting discipline

Across every sector regulator, the head decides in advance who
fronts the relationship, and holds that decision until a specific
event changes it. The head is accountable to the board and the
audit committee for the AI-specific dimensions of every
engagement, but the head does not always speak first. The design
discipline is:

- **Line-of-business fronts the routine channel.** The CMRO fronts
  banking model-risk examinations. Regulatory affairs fronts FDA
  submissions. HR fronts EEOC charge responses. The head is in
  the room, or on the paper, but is not the primary voice.
- **General counsel fronts anything that has become a legal
  matter.** MRA, MRIA, formal enforcement, consent order,
  litigation, subpoena, investigation. The head remains the
  technical author of the record but the GC controls the posture.
- **Government affairs fronts the policy channel.** Rulemaking
  comments, model-bulletin engagement, industry-body positioning,
  legislative testimony. The head contributes the technical
  substance; government affairs owns the political and reputational
  positioning.
- **CISO fronts cyber-incident notification and the CISA/NCSC
  channel.** The head owns AI-specific incident content within
  that channel.
- **DPO fronts the ICO and equivalent DPA channels.** The head
  owns the AI-specific DPIA and Article 22 analysis.
- **The head fronts only where the regulator has been designed
  around AI as its subject matter.** The EU AI Office and the AI
  Safety Institutes are the clearest examples. Even there, the
  general counsel is copied on every material communication.

The discipline is written down, per regulator, in the enterprise's
regulator-engagement RACI. It survives personnel change because
it is a design artefact, not a personal relationship. When a peer
who owns the front seat leaves, the successor inherits the seat;
when the head leaves, the head's successor inherits the
accountability. The board can read the RACI and see who to call
in a crisis.

## The head's sector-regulator inventory

The artefact the head maintains, and that feeds the regulator-
engagement cluster of the quarterly board pack (cluster 4 in
[[mod-103-board-and-audit-committee-reporting]]), is the sector-
regulator inventory. Per regulator, the fields:

- **Regulator name and jurisdiction.** Federal Reserve System —
  US federal. NYDFS — New York State. UK ICO — UK.
- **Obligation surface.** Specific rules, guidance, letters,
  bulletins, model laws cited, with dates and current status.
  SR 11-7 (2011). OCC Bulletin 2011-12 (2011). SR 23-4 (2023).
  NAIC AI Model Bulletin (adopted 14 December 2023). Colorado AI
  Act SB 24-205 (signed May 2024).
- **AI-specific overlay.** Where the AI-specific instrument sits
  on top of a non-AI-specific base instrument, both are named.
  Title VII plus EEOC May 2023 technical assistance. ECOA/Reg B
  plus CFPB Circular 2022-03.
- **Enterprise counterpart.** Named individual and function.
  CMRO for Federal Reserve model-risk examinations. Regulatory
  affairs VP for FDA. DPO for ICO. Named individual, not just a
  function, because the regulator will remember the name.
- **Current status.** In routine engagement. In examination. In
  MRA remediation. In consent-order compliance. In litigation.
  In no active engagement (which is itself a status the board
  reads).
- **Next-action-by-date.** Concrete milestone with owner.
- **Escalation stance.** Pre-decided posture at MRA, MRIA, and
  enforcement tiers, so that the head is not designing posture
  under time pressure when escalation happens.
- **Peer-fronting decision.** Who fronts the routine channel; who
  fronts on escalation; when the head steps forward.

The inventory is kept current on a rolling basis. Horizon-scanning
from [[mod-105-regulatory-change-management]] adds new instruments
and updates the status of existing ones. Exam runbook execution
from chapter 05 of this module updates status through examination
cycles. The board pack draws on the inventory quarterly. External
counsel and government affairs advise on entries in their
respective columns. The inventory is the head's operating record
of the regulator portfolio, and the artefact by which the head's
successor will be onboarded.

An inventory that lists only the AI-specific regulators is
incomplete. The point of this chapter is that most of the
regulator hours are spent under instruments that are not AI-
specific, applied to AI systems. The inventory reflects that
reality or it is a positioning artefact rather than an operating
one.

## Summary

- The head designs the engagement stance for every sector
  regulator along four axes: obligation surface (citable
  instruments, AI-specific overlays on non-AI-specific bases),
  engagement channel (who fronts, formal and informal), cadence
  (continuous vs periodic vs event-driven), and escalation and
  evidence discipline (routine, MRA, MRIA, enforcement, consent).
- Banking, insurance, health, employment, consumer, health-
  privacy, US state privacy and AI, UK data protection, and cyber
  are the main sector clusters; each has named instruments —
  SR 11-7 and OCC 2011-12 and SR 23-4; NAIC AI Model Bulletin
  (December 2023); FDA GMLP (October 2021, joint with Health
  Canada and MHRA) and PCCP guidance (draft April 2023); EEOC
  May 2022 ADA and May 2023 Title VII guidance and NYC Local Law
  144 (2023); CFPB Circulars 2022-03 and 2023-03; HHS OCR under
  HIPAA; CPPA ADMT rulemaking and Colorado AI Act SB 24-205
  (signed May 2024); UK ICO AI and Data Protection guidance
  (updated 2023); CISA/NCSC Guidelines for Secure AI System
  Development (November 2023) and Joint Guidance on Deploying AI
  Systems Securely (April 2024).
- The peer-fronting discipline names, per regulator, who speaks
  first: line-of-business at the routine channel, general counsel
  at anything that has become a legal matter, government affairs
  at the policy channel, CISO at cyber, DPO at DPAs, and the head
  only where the regulator's subject matter is AI itself.
- The sector-regulator inventory is the head's operating artefact:
  regulator, jurisdiction, obligation surface with AI-specific
  overlay, enterprise counterpart named, current status, next-
  action-by-date, escalation stance, peer-fronting decision.
- The inventory feeds cluster 4 of the quarterly board pack in
  [[mod-103-board-and-audit-committee-reporting]], is kept current
  by [[mod-105-regulatory-change-management]] horizon-scanning,
  and drives examination readiness through chapter 05 of this
  module; depth on any given sector is carried by
  [[mod-111-sector-program-leadership]].
