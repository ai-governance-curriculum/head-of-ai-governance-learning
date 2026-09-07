# US Serious-Incident Disclosure Map

## Motivation

Chapter 03 governed the Article 73 filing. In the EU, the
regime is a single named surface: one statutory definition
of "serious incident" in Article 3(49), one filing article
(Article 73), one recipient family (the market-surveillance
authorities of the affected Member States), one set of
timelines that runs from awareness. The head knows the
regime cold, the classification meeting resolves against a
bounded question set, and the filing signature is the
head's. The regime is heavy, but its shape is legible.

The US regime is not that. There is no single federal AI
serious-incident statute, no single recipient, no single
timeline, no single "AI Act" that names the obligation.
What exists is a patchwork — a sector-specific statute
here, a state-specific statute there, an agency guidance
letter that reads as an obligation in practice, a breach-
notification regime that catches AI-driven personal-data
exposures without naming AI, a securities-disclosure item
that catches cybersecurity incidents that materially affect
the listed enterprise. Each obligation has its own trigger,
its own recipient, its own timeline, its own filing content
shape, and its own political weather. A single serious AI
incident inside a US-exposed enterprise plausibly touches
three or four of them at once, and the enterprise's
Article 73 filing does not discharge any of them.

The failure mode this chapter defends against is the head
who runs the Article 73 filing with credit-worthy
discipline — classification meeting inside two hours,
filing signed and transmitted inside the Article 73(3)
window, follow-up sequence held to date — and misses the US
sector-specific disclosure because no one at the enterprise
owned the US map. The Colorado Attorney General's office
learns about the incident from a Reuters piece rather than
from the enterprise's own notification. HHS OCR opens a
HIPAA breach-notification enforcement matter because the AI
system's PHI exposure was reported to the EU market-
surveillance authority but not to OCR under 45 CFR 164.400
et seq. The SEC issues a comment letter on the enterprise's
next 10-Q asking why the Item 1.05 Form 8-K disclosure was
not filed inside the four-business-day window when the
Article 73 filing plainly acknowledged materiality. In each
case, the head who signed the Article 73 filing is on the
phone with the CEO explaining why the US-side disclosure
was missed. "We did not know we had a US obligation" is not
survivable at the audit-committee table.

This chapter is not a legal treatise on any of the US
regimes — the General Counsel does the statutory
interpretation at incident time. It is the head's
discipline of owning the *map* of US disclosure surfaces
the enterprise plausibly triggers, so that "is there a US
filing" is answered inside minutes against a live artefact,
not answered inside days against a scramble.

## Core concept — the head owns the US disclosure map as an artefact

The load-bearing move in this chapter is that the US
disclosure map is an artefact the head personally owns,
maintains, and consults. GC does the statutory-
interpretation work at incident time — GC characterises
whether the specific event triggers a specific obligation —
but GC cannot productively answer "is there a US filing" as
an open question at 2am on a Sunday. The head has to bring
the bounded question set to GC. The map is the question
set.

The distinction mirrors the one chapter 03 drew between the
general Article 73 regime (known before the incident) and
the incident-time execution of it. The general regime for
the US side is the map. Under the running clock, the head
opens the map, GC opens the specific statutory text for
each surface the map flags as plausibly in play, and the
classification meeting runs against a bounded surface set
rather than an unbounded discovery exercise.

Ownership is deliberate. The map is not the compliance
function's artefact, not GC's, not the CISO's, not the
Chief Privacy Officer's. Each of those functions owns one
or more surfaces on the map — the privacy office owns the
HIPAA row, securities counsel owns the SEC row, the CISO's
function owns the parent cybersecurity-breach-notification
surfaces — but none of them owns the head's cross-surface
view. The head's map says: given the current AI portfolio
per the AIMS inventory
([[mod-102-running-the-program]] chapter 06
<!-- needs-research: verify mod-102 chapter number for the
AIMS inventory -->), given the enterprise's jurisdictional
footprint, and given the current state of each regime,
*these are the disclosure surfaces a serious AI incident
plausibly triggers, and this is who signs each one*.

The map is a living artefact. It is refreshed against the
regulatory-change-management discipline from
[[mod-105-regulatory-change-management]] on a standing
cadence — quarterly at minimum, more frequently when a
named regime moves — and ratified in the CxO-adjacency map
from [[mod-101-role-scope-and-leadership-shape]] chapter 06
<!-- needs-research: verify mod-101 chapter number for the
CxO-adjacency map --> so that GC, the Chief Privacy
Officer, securities counsel, the CISO, and the head all
read the same artefact. It is exercised in the disclosure-
map rehearsal alongside the Article 73 rehearsal so that
the map is not consulted for the first time under real
incident pressure. The rest of this chapter walks the
surfaces the map covers, the columns each row carries, the
parallel-filing coordination challenge, and the lead-
jurisdiction discipline that keeps the sequence coherent.

## Colorado AI Act (SB24-205)

Colorado's Consumer Protections for Artificial Intelligence
Act — SB24-205, enacted in 2024, with effective provisions
that begin operating in 2026 — is the first US state
statute that names an AI-specific serious-incident-adjacent
notification obligation. <!-- needs-research: verify
SB24-205 effective date, the specific notification provision
text, and the current state of any 2025-2026 amendments,
including implementing regulations promulgated by the
Colorado Attorney General under the act --> The act applies
to developers and deployers of "high-risk artificial
intelligence systems" — systems that make, or are a
substantial factor in making, consequential decisions in
categories including employment, education, financial
services, essential government services, health care,
housing, insurance, and legal services. <!-- needs-research:
verify the SB24-205 definition of "high-risk artificial
intelligence system" and the enumerated consequential-
decision categories -->

The notification-adjacent obligation on the map is the
deployer's duty, on discovery that the deployment has caused
or is reasonably likely to have caused algorithmic
discrimination, to notify the Colorado Attorney General
within a specified window. <!-- needs-research: verify the
specific text of the Colorado AG notification obligation —
the trigger phrase ("algorithmic discrimination" as defined
in the act), the timing from discovery, the content
required in the notification, and whether the notification
runs to the AG directly or through another channel --> The
head's map carries the trigger (algorithmic discrimination
as the act defines it, not the general term of art), the
timeline (from discovery, not from the incident event), the
recipient (the Colorado Attorney General's office), the
signature holder (the head, through GC's Colorado-admitted
channel), and the composition point with the state's
general breach-notification regime where PHI or other
regulated data is also implicated.

The head does not treat the Colorado obligation as a
novelty because it is the first of its kind. The head
treats it as a template for the state-level AI-notification
regimes under active legislative development in a growing
number of state capitals. <!-- needs-research: verify the
current state-legislative landscape for AI-specific serious-
incident notification statutes as of the current authoring
window; identify which additional states have enacted or
introduced comparable bills --> The map is designed to
accept additional state-level rows as those regimes move,
picked up by the refresh cadence. The coordination
touchpoint is GC's Colorado-admitted counsel, the head, and
the operational function whose deployment triggered the
notification (typically HR for employment, the lending
function for consumer finance, the underwriting function
for insurance).

## NAIC AI Model Bulletin

The National Association of Insurance Commissioners (NAIC)
adopted the Model Bulletin on the Use of Artificial
Intelligence Systems by Insurers in 2023, and the bulletin
has been adopted or adapted by a growing set of state
insurance commissioners since. <!-- needs-research: verify
the 2023 NAIC Model Bulletin publication date, the exact
title, and the current state-by-state adoption status -->
The bulletin is not a statute; it is a guidance instrument
the commissioners use to communicate supervisory
expectations to authorised insurers. In adopting states, the
bulletin's expectations carry supervisory weight equivalent
to a formal communication — an insurer that ignores them
exposes itself to the commissioner's supervisory posture at
the next examination cycle.

The map has to carry the NAIC surface for an enterprise
that operates as an authorised insurer in any state that
has adopted the bulletin. <!-- needs-research: verify the
specific notification-adjacent expectations in the NAIC
Model Bulletin — whether the bulletin expects an insurer to
notify the state commissioner of AI-system incidents that
materially affect the insurer's compliance with the state
insurance code, and if so under what trigger and timing -->
The trigger, recipient, and timing vary state-by-state
because each state's adoption is a state-specific act. The
head's map carries one row per adopting state where the
enterprise is authorised.

For a multi-state insurer, the NAIC surface is the map
surface most exposed to patchwork risk. A single AI-
underwriting incident affecting policyholders across a
dozen NAIC-bulletin-adopting states plausibly triggers a
dozen separate commissioner notifications on twelve
separate timelines with twelve separate content
expectations. The head does not resolve that patchwork
under incident-time pressure by improvising; the map has
already resolved it into a matrix the enterprise files
against. The coordination touchpoint is the state-insurance-
compliance function, outside insurance-regulatory counsel
where used, the head, and the CCO's insurance desk for
industry-facing composition.

## HHS OCR — HIPAA breach notification

Where the enterprise operates as a HIPAA-covered entity or
as a business associate to one, and an AI system triggers
an unauthorised acquisition, access, use, or disclosure of
protected health information (PHI), the HIPAA Breach
Notification Rule at 45 CFR 164.400 through 164.414
governs. <!-- needs-research: verify the current text and
effective status of 45 CFR 164.400-164.414, and any AI-
specific interpretive guidance HHS has issued on the rule
in the current authoring window --> The rule is not AI-
specific — it applies to any breach of unsecured PHI — but
it catches AI-driven exposures without needing to. An AI-
enabled clinical-decision-support tool that surfaces one
patient's PHI in another patient's session is a HIPAA
breach as squarely as any other breach.

The rule's obligations run in three directions: individual
notification (to affected individuals, generally within 60
days of discovery), Secretary notification (to the
Secretary of HHS, timing depending on the number of
affected individuals — annual aggregate for smaller
breaches, without unreasonable delay and no later than 60
days for larger breaches), and media notification (for
breaches affecting more than 500 residents of a state or
jurisdiction, notice to prominent media outlets serving the
state or jurisdiction). <!-- needs-research: verify the
current individual-notification timeline, the 500-
individual media-notification threshold, and the Secretary-
notification timing bands under 45 CFR 164.404, 164.406, and
164.408 -->

The head's role on the HIPAA surface is coordination, not
signature. The signature and the operational filing sit
with the covered entity's Privacy Officer. The head's map
carries the surface so that at incident time the head knows
to convene the Privacy Officer into the classification
meeting, so that the head's AI-substantive account is
composed into the Privacy Officer's HIPAA-facing account,
and so that the head's Article 73 filing (where the
incident also implicates the EU regime) does not contradict
the Privacy Officer's OCR notification. The seven-pens
discipline from chapter 02 applies — the HIPAA notification
is one pen, the Article 73 filing is another, and the head
does not let them say different things about the same
event. The coordination touchpoint is the Chief Privacy
Officer, GC's health-law counsel, the head, and the CCO's
customer-comms desk for the individual-notification and
media-notification streams.

## FDA — Medical Device Reporting for AI/ML SaMD

Where the enterprise develops, manufactures, or holds
marketing authorisation for an AI/ML-enabled medical device
— Software as a Medical Device (SaMD) or software in a
regulated medical device — the FDA's Medical Device
Reporting (MDR) regime at 21 CFR Part 803 governs adverse-
event and malfunction reporting. <!-- needs-research: verify
the current scope of 21 CFR Part 803, the reporting
timelines (typically 30-day for adverse events and
malfunctions, 5-day for reportable events requiring
remedial action to prevent an unreasonable risk of
substantial harm), and any FDA-issued AI/ML-specific
interpretive guidance in the current authoring window --> An
AI/ML-enabled device triggers the same MDR obligations as
any other regulated device when a malfunction contributes
or could contribute to death or serious injury.

The AI-specific nuance the map has to carry is the
interaction with the Predetermined Change Control Plan
(PCCP) framework. FDA's evolving posture on AI/ML SaMD
allows manufacturers to specify, at the time of initial
device authorisation, a set of pre-authorised modifications
the manufacturer can implement without a new submission —
the PCCP. <!-- needs-research: verify the current state of
the FDA's PCCP framework, including the January 2025
guidance on Marketing Submission Recommendations for a
Predetermined Change Control Plan for Artificial
Intelligence-Enabled Device Software Functions, and any
2025-2026 updates --> Where a device malfunction is
traceable to a modification made under the PCCP, the MDR
obligation is unchanged, but the enterprise's account has
to reference the PCCP authorisation — what was pre-
authorised, what was implemented, and whether the
implementation stayed inside the PCCP envelope. If the
implementation exited the envelope, the enterprise is
disclosing both a device malfunction and a compliance
failure against the PCCP, which is a materially different
filing conversation.

The head's map carries the MDR reporting timelines (per
tier), the recipient (FDA through the manufacturer's
authorised reporter channel), the signature holder (the
manufacturer's designated MDR reporter — a role the
enterprise has assigned in advance; the head does not fill
it personally), and the PCCP composition point. The
coordination touchpoint is Regulatory Affairs (the FDA-
facing function for the device portfolio), the quality-
management function under whose QMS the malfunction
investigation runs, the head, and outside FDA-regulatory
counsel where used. Where the enterprise is a downstream
deployer of an AI/ML-enabled device manufactured by a third
party, the head's role is coordination with the
manufacturer's regulatory function so that the enterprise's
own incident account composes with the manufacturer's MDR
filing.

## EEOC and DOL — AI-in-HR incidents

Where the enterprise uses AI systems in employment-related
decisions — hiring, promotion, discipline, termination,
compensation, benefits — an incident that produces or is
likely to have produced discrimination against a protected
class implicates the equal-employment enforcement apparatus
of the EEOC and, for federal contractors, the DOL (including
OFCCP). Neither agency operates a serious-incident
notification regime in the shape of Article 73 —
enforcement runs through charge filings by affected
individuals, commissioner charges, and compliance
evaluations. But the map has to carry the surface because
the enterprise's response posture to a discovered AI-driven
employment-discrimination incident is a filing-adjacent
decision the head co-owns.

The EEOC's May 2022 technical assistance document on the
Americans with Disabilities Act and the use of software,
algorithms, and AI to assess job applicants and employees,
and the May 2023 technical assistance document on Title VII
and AI-driven employment decisions, together establish the
current EEOC interpretive posture. <!-- needs-research:
verify the publication dates and current status of the EEOC
2022 ADA guidance and the EEOC 2023 Title VII guidance on
AI-driven employment decisions, and any 2024-2026 updates or
superseding documents; verify current DOL / OFCCP guidance
on AI in federal-contractor employment decisions --> Neither
document establishes a notification obligation, but both
establish the interpretive lens the EEOC applies when a
charge is filed. The head's map carries the interpretive
lens so that at incident time the head knows what evidence
the enterprise has to preserve (adverse-impact analysis,
validation studies, four-fifths-rule analysis where
applicable, individual-decision records) and knows the
internal escalation path (the CHRO, the head of the
affected talent function, GC's labour-and-employment
counsel).

For federal contractors, the OFCCP's affirmative-action
compliance framework adds a proactive-monitoring obligation
that composes with the AI-in-HR incident response. Where an
AI system's operation has produced an adverse-impact
pattern, the contractor's affirmative-action plan has to
acknowledge the pattern and describe the corrective action,
and the OFCCP may open a compliance evaluation on that
basis. <!-- needs-research: verify the current OFCCP
compliance-evaluation framework and any AI-specific
enforcement priorities or guidance issued in the 2024-2026
window --> The map carries the OFCCP surface as a distinct
row. The coordination touchpoint is the CHRO per the CHRO
coordination chapter in
[[mod-109-cross-enterprise-leadership]] <!-- needs-research:
verify the mod-109 chapter for CHRO coordination on HR-in-
AI incidents -->, GC's labour-and-employment counsel, the
head, and (where an adverse-impact pattern requires public-
facing acknowledgement) the CCO. The head signs the AI-
substantive attachment to any EEOC position statement or
DOL compliance-evaluation response that references the AI
system's operation.

## State AG data-breach adjacencies — CPPA and the 50-state patchwork

Where an AI incident produces an exposure of personal data
— through a prompt-injection compromise that surfaced one
customer's data in another customer's session, a model-
extraction event that reconstructed personal data from the
training set, a RAG-corpus poisoning that caused the system
to disclose data that should have been access-controlled,
or a jailbreak that induced the model to output training-
set data — the parent state data-breach-notification regime
triggers independent of any AI-specific obligation. The map
has to carry this surface even when no AI-specific statute
is in play, because a serious AI incident with a personal-
data-exposure dimension is nearly always also a state-
breach-notification event.

The California Privacy Protection Agency (CPPA) is the
enforcement authority for the California Consumer Privacy
Act as amended by the California Privacy Rights Act
(CCPA/CPRA). <!-- needs-research: verify the current CPPA
enforcement authority under CCPA/CPRA, the current text of
the California data-breach notification statute at Civil
Code Section 1798.82, and any CPPA-issued guidance on AI-
adjacent breach notification --> The California regime
establishes a private-right-of-action dimension for breaches
of unencrypted or unredacted personal information,
notification obligations to affected California residents,
and — for breaches affecting more than 500 California
residents — notification to the California Attorney General
with a public breach report.

California is one row. Every other state has its own
breach-notification statute with its own trigger, timing,
recipient (typically the state AG, sometimes the state's
consumer-protection authority, sometimes a state-specific
data-protection commissioner), and content requirements.
<!-- needs-research: verify the current 50-state plus DC
and territories breach-notification statutory landscape,
the states that have amended their statutes in the 2023-2026
window to address AI-driven exposures explicitly, and any
interstate coordination frameworks --> The map carries one
row per state where the enterprise has sufficient user
footprint to be plausibly in scope. For a consumer-facing
enterprise, that is typically all fifty states plus DC plus
territories.

The state-AG surface is the map surface most exposed to
timing patchwork. Timelines vary from as short as thirty
days from discovery in some states to "without unreasonable
delay" framing in others, and the what-counts-as-discovery
threshold varies. <!-- needs-research: verify the current
spread of state breach-notification timelines and discovery-
trigger definitions across US states --> The map does not
attempt to resolve the specific timing against every state
at incident time — that is the Chief Privacy Officer's
operational work. The map's role at leadership scope is to
carry the surface so the head knows the CPPA / 50-state pen
has to be actively coordinated, that the Chief Privacy
Officer is in the classification meeting, and that the
head's Article 73 filing (where applicable) is consistent
with the factual account the state-breach notifications
carry. The coordination touchpoint is the Chief Privacy
Officer, GC's privacy counsel, the state-AG-relations
function where the enterprise has one, the head, and the
CCO's customer-comms desk for individual notification.

## SEC Form 8-K Item 1.05

Where the enterprise is a public company subject to SEC
reporting, and an AI incident meets the materiality
standard under Item 1.05 of Form 8-K — the cybersecurity-
incident disclosure item the SEC adopted in the 2023
Cybersecurity Risk Management, Strategy, Governance, and
Incident Disclosure rule — the four-business-day
disclosure obligation runs from the enterprise's
determination that the incident is material.
<!-- needs-research: verify the current text of Item 1.05 of
Form 8-K, the four-business-day timeline from materiality
determination (not from incident discovery), the delayed-
disclosure exception for national-security or public-safety
concerns, and any SEC-issued interpretive guidance in the
current authoring window on AI-specific applications of
Item 1.05 --> The rule catches AI incidents where the event
has a cybersecurity nexus — an AI system compromise that
constitutes unauthorised access to the enterprise's
information systems, or an AI-driven data exposure that
constitutes a cybersecurity incident under the rule's
definition — and where the enterprise determines the
incident is material to a reasonable investor.

The AI-specific interpretation of Item 1.05 is actively
evolving. <!-- needs-research: verify the current SEC posture
on whether an AI-specific incident with no traditional
security-perimeter breach dimension (for example, a
jailbreak that produced harmful downstream output without
any information-system compromise) triggers Item 1.05, and
whether the SEC has issued interpretive guidance or brought
enforcement matters that address AI-specific incidents -->
The head's map does not resolve the evolving interpretive
question; the head's securities counsel and disclosure
committee resolve it against the specific incident. The map
carries the SEC surface so that at incident time the head
convenes securities counsel and the disclosure committee
alongside GC and the CISO, and so that the head's AI-
substantive account of the incident is composed into the
materiality analysis the disclosure committee runs.

The materiality determination is not the head's decision;
it is the disclosure committee's, informed by securities
counsel. What the head brings is the AI-substantive account
— what happened, what the affected-population estimate is,
what the reversibility posture is, what the ongoing
exposure is, what the containment status is. The disclosure
committee reads the head's account alongside the CISO's
operational-security account, GC's legal account, and the
CFO's financial-impact account, and reaches the materiality
determination that starts the four-business-day clock. The
head signs the AI-substantive account; the disclosure
committee signs the materiality determination; the
enterprise's Chief Legal Officer (or an authorised Section
16 officer) signs the Form 8-K itself. The coordination
touchpoint is securities counsel, the disclosure committee,
the CFO, the CISO, GC, the head, the Head of Investor
Relations, and the CCO's external-communications desk.

## Federal Reserve SR 11-7 and sector model-risk expectations

Where the enterprise is a US-regulated bank — a national
bank, a state member bank, a bank holding company, or a
non-bank subsidiary subject to Federal Reserve or OCC
supervision — the parent Model Risk Management (MRM)
framework the enterprise operates under is anchored in the
Federal Reserve's SR 11-7 supervisory guidance and the
OCC's parallel OCC 2011-12 guidance. <!-- needs-research:
verify the current effective status of SR 11-7 and OCC
2011-12, whether either has been amended or superseded, and
any 2024-2026 supervisory letters or guidance the Federal
Reserve or OCC has issued on AI/ML model risk --> The MRM
framework is not a serious-incident notification regime in
the shape of Article 73 — supervision runs through the
ongoing examination cycle rather than through discrete
incident filings — but the framework establishes an
expectation that material model-risk incidents flow through
the enterprise's MRM governance to the supervising
examiner, and that the audit committee of the bank's board
is briefed on material incidents at the operating cadence.

The map carries the SR 11-7 surface for a regulated bank so
that at incident time the head knows the incident's AI-
substantive account has to be composed into the MRM
incident register, that the MRM function is convened into
the classification meeting, and that the audit committee's
Model Risk Committee (or equivalent) is briefed at the
earliest cycle if the incident is material under MRM
criteria. The examination-facing composition happens at the
next supervisory examination, not at incident time — but the
record the enterprise carries into that examination is
built at incident time, and the head's account is what the
record reads. For non-bank enterprises with sector-specific
model-risk supervisory frameworks — the insurance
industry's evolving NAIC-adopted model-risk expectations,
FINRA and SEC posture on algorithmic-trading model risk,
CMS posture on AI in payment and coverage decisions — the
map carries the sector's equivalent row. <!-- needs-research:
verify current sector-specific model-risk frameworks in
insurance (NAIC-adjacent), securities (FINRA / SEC on
algorithmic trading), and health-care (CMS on AI in payment
and coverage) --> The coordination touchpoint is the CRO,
the MRM function head, GC's bank-regulatory counsel, the
head, and the audit committee's Model Risk Committee chair.

## The map artefact

The map is a structured artefact, maintained in the same
discipline the AIMS inventory
([[mod-102-running-the-program]]) is maintained under —
living, versioned, refreshed on a bounded cadence,
consulted at incident time. Each row is one disclosure
surface. Each row carries seven columns.

- **Obligation.** The named statutory, regulatory, or
  supervisory instrument that establishes the obligation.
  The citation is precise enough that GC can open the text
  without ambiguity — the statutory section, the regulation
  citation, the guidance-document title and date. Where the
  obligation is composite (the state breach-notification
  patchwork), sub-rows carry the jurisdiction-specific
  citation.
- **Recipient.** The specific regulator, agency, or
  authority that receives the notification. Where the
  recipient has a named point of contact the enterprise has
  previously worked with, the point of contact is on the row
  for continuity of relationship per
  [[mod-104-regulator-engagement]].
- **Triggering condition.** The specific event that starts
  the obligation, phrased as a testable question — "has the
  deployment caused or is it reasonably likely to have
  caused algorithmic discrimination" for the Colorado row,
  "has an unauthorised acquisition, access, use, or
  disclosure of unsecured PHI occurred" for the HIPAA row,
  "has the disclosure committee determined the incident is
  material" for the SEC row.
- **Timeline from awareness.** The specific window inside
  which the notification is due, measured from the specific
  event the regime treats as awareness (which varies —
  discovery in some regimes, materiality determination in
  others, occurrence in still others). Where the regime has
  tiered timelines, the row carries each tier.
- **Filing content template.** The pre-built template the
  enterprise files against for this surface. The template
  is authored outside incident time, rehearsed against the
  exercises in this module, and refreshed against
  regulatory-change-management cadence. Under running-clock
  pressure, filings are composed against the template, not
  from scratch.
- **Internal sign-off routing.** The named sign-off chain
  — who drafts, who reviews, who signs. The head signs some
  surfaces (the AI-substantive account, the Colorado AG
  notification); other roles sign others (the Chief Privacy
  Officer signs HIPAA notifications, the designated MDR
  reporter signs the FDA MDR, the disclosure committee
  signs the Item 1.05 materiality determination). The map
  does not leave the signature holder ambiguous.
- **Coordination touchpoint.** The GC-side counsel, the
  operational function, and the executive peer whose
  involvement the surface requires. This is the map's
  interface with the CxO-adjacency map from
  [[mod-101-role-scope-and-leadership-shape]] chapter 06.

The map is refreshed on the standing cadence from
[[mod-105-regulatory-change-management]]. Quarterly review
is the default; more frequent review is triggered when a
named regime moves — a new state enacts an AI-notification
statute, the FDA publishes new AI/ML SaMD guidance, the SEC
issues interpretive guidance on Item 1.05's AI application,
a state insurance commissioner adopts the NAIC bulletin,
HHS issues AI-specific interpretive guidance on the HIPAA
Breach Notification Rule. The refresh is not a compliance
activity run by a compliance analyst; it is a leadership
activity run by the head and reviewed by GC, the Chief
Privacy Officer, the CISO, the CRO, and the audit
committee. The audit committee sees the map's structure and
revision history at the standing cadence per
[[mod-103-board-and-audit-committee-reporting]]
<!-- needs-research: verify the mod-103 cluster that covers
the audit committee's line of sight on the disclosure-map
artefact -->. The audit committee does not review each
row's substantive content, but it reads the artefact's
existence, its currency, and the head's ownership of it as
an audit-committee-visible control.

## The parallel-filing coordination challenge

A single serious AI incident inside a US-and-EU-exposed
enterprise plausibly triggers filings across multiple
regimes at once. The Article 73 filing to the affected
Member States' market-surveillance authorities runs on the
timelines chapter 03 governs. The state-breach notifications
to the affected US states' attorneys general run on state-
specific timelines. The SEC Item 1.05 disclosure runs on the
four-business-day clock from materiality determination. The
HIPAA OCR notification runs on the 60-day-from-discovery
clock. The Colorado AG notification runs on the SB24-205
timeline. The NAIC-adopting states' commissioners each
expect the state's own timing. The head runs all of these
in parallel, keeps the filings consistent, and honours each
regime's timeline independently.

The load-bearing move is that the same substantive facts
get told the same way across every pen. The seven-pens
discipline from chapter 02 was authored for the single-
jurisdiction case; it extends to the multi-jurisdiction case
naturally, but the extension is where discipline slips. The
Article 73 filing to the Irish national CA cannot say the
incident affected 8,000 users while the SEC 8-K describes
the same event as affecting "fewer than 10,000 users" and
the CPPA notification to the California AG asserts
"approximately 12,000 affected California residents". A
reasonable regulator reading the three filings side-by-side
reads the enterprise as either sloppy or evasive. Either
reading is durable.

The head's discipline is that a single facts-of-the-incident
document — the AI-substantive account the head signs — is
the single source every pen composes against. The Article
73 filing quotes it. The SEC 8-K materiality analysis cites
it. The HIPAA OCR notification's cover letter references
it. The state-AG notifications' factual sections carry it.
Where a pen phrases the facts for a jurisdiction-specific
audience (the SEC's investor-facing frame differs from
OCR's covered-entity-compliance frame differs from the
market-surveillance authority's product-safety frame), the
phrasing differs but the underlying facts do not. The head
reads across before signing anything; the head does not
sign a filing whose facts diverge from the head's own
single source.

Timeline coordination is the second discipline. The
timelines do not align. The SEC's four-business-day clock
starts from materiality determination, which may be days
after Article 73 discovery-awareness. The HIPAA 60-day
clock starts from breach discovery. The Colorado AG
timeline starts from the deployer's discovery of
algorithmic discrimination, which may be later still. The
head's map carries each timeline; the head's incident-
response cadence tracks each clock independently. An
incident-filing register, operated by Regulator Relations
and refreshed at the standing operating cadence during the
acute window, shows every open filing surface, its clock,
its next milestone, its sign-off status, and its
transmission status. The head reads it before every
checkpoint on the bridge.

Where two filings' timing conflict — for example, the SEC's
four-business-day materiality-triggered clock lands before
the Article 73(3) two-day widespread-infringement clock,
and the SEC filing has to acknowledge the incident before
the Article 73 filing is complete — the head does not
resolve the conflict by delaying one for the other. Both
are statutory. Both file inside their windows. The head's
discipline is that they say consistent things about the
incident even if the SEC's public 8-K lands hours before
the Article 73 filing is transmitted. The head coordinates
with securities counsel, the disclosure committee, and
Regulator Relations to ensure the parallel filings do not
create the appearance that the enterprise disclosed to one
regulator and hid from another.

## The lead-jurisdiction discipline

Chapter 03 introduced the lead-NCA convention — where more
than one Member State's national CA is a recipient of the
Article 73 filing, the head names an internal lead-NCA
relationship for coordination discipline. The same shape
applies at the cross-jurisdictional level. Where the
enterprise has both US and EU exposure, the head names an
internal *lead-jurisdiction convention* so the follow-up
sequence across the two regimes does not fragment.

The lead-jurisdiction convention is not a legal choice — the
statutes each impose their own obligations independently,
and the enterprise cannot use a lead jurisdiction to
satisfy an obligation elsewhere. The convention is an
internal coordination discipline: the enterprise names, at
the outset of the incident, which jurisdictional side of
the filing map is holding the primary coordination role for
the enterprise's cross-jurisdictional posture, which side
is holding the secondary role, and what the interface
between them is.

Two practical patterns dominate. The first is the
enterprise-EU-seat-lead pattern, where the EU seat holds
the primary coordination role because the Article 73 filing
carries the most operationally demanding timeline and the
EU AI Act's serious-incident regime is the most-
substantively-shaped regime in play. The head's Article 73
filing decision-meeting (per chapter 03) becomes the primary
filing-decision meeting, and the US filings — SEC, HIPAA,
state AGs, sector regulators — are coordinated to compose
with the Article 73 filing's factual account. The second is
the US-materiality-lead pattern, where the SEC's four-
business-day Item 1.05 clock is the tightest timeline in
play and the disclosure committee's materiality
determination carries the primary coordination role. The
Article 73 filing is composed to be consistent with the
Item 1.05 disclosure that will publish inside the business
week; the state-AG notifications carry the same factual
account.

The head names the lead-jurisdiction convention at the
initial cross-jurisdiction coordination meeting — a meeting
distinct from either the Article 73 classification meeting
or the US-side classification meetings, convened by the
head inside the first day of the incident where the
incident is plausibly cross-jurisdictional. The convention
is recorded in the incident record, communicated to every
internal function participating in any of the parallel
filings, and does not shift once set except in response to
a materially new fact.

The lead-jurisdiction discipline is distinct from the
lead-NCA discipline in chapter 03. The lead-NCA discipline
operates inside the Article 73 regime — it names, among the
Member States' national CAs receiving the same Article 73
filing, which one the enterprise runs as its primary
relationship. The lead-jurisdiction discipline operates
across regimes — it names, among the US and EU regimes
both imposing obligations, which one the enterprise's
cross-regime coordination is anchored to. Both disciplines
run simultaneously in a fully cross-jurisdictional serious
incident. The head reads both in the incident record.

## Composition with adjacent modules

- The **CxO-adjacency map** in
  [[mod-101-role-scope-and-leadership-shape]] chapter 06
  <!-- needs-research: verify mod-101 chapter number for the
  CxO-adjacency map --> records the disclosure map's
  existence, its owner (the head), and the peer-function
  interfaces the map's rows depend on (Chief Privacy
  Officer, securities counsel, Regulatory Affairs for FDA-
  facing work, state-insurance-compliance, CHRO, CRO, MRM
  function).
- The **AIMS inventory** in
  [[mod-102-running-the-program]] chapter 06
  <!-- needs-research: verify mod-102 chapter number for the
  AIMS inventory --> is the reference the head reads to
  determine which disclosure-map surfaces the enterprise's
  actual AI portfolio plausibly triggers. Applicability is
  a function of the inventory; when the inventory changes,
  the map changes.
- The **board / audit-committee reporting cadence** in
  [[mod-103-board-and-audit-committee-reporting]] cluster 3
  <!-- needs-research: verify mod-103 cluster number for the
  incident-and-near-miss cluster --> is where the map's
  existence, its refresh status, and each acute-incident-
  time activation of it become board-visible artefacts.
- The **regulator-engagement discipline** in
  [[mod-104-regulator-engagement]] provides the durable
  relationship posture with each recipient on the map — the
  Colorado AG, the state insurance commissioners, HHS OCR,
  the FDA, the EEOC / DOL, the state AGs, the SEC, and the
  Federal Reserve / OCC.
- **Regulatory change management** in
  [[mod-105-regulatory-change-management]] is where the map
  is refreshed on the standing cadence and where new state-
  level AI-notification statutes, new federal-agency
  guidance, and new supervisory expectations are picked up
  into the map.
- The **GC coordination chapter** in
  [[mod-109-cross-enterprise-leadership]] chapter 06
  <!-- needs-research: verify mod-109 chapter number for GC
  coordination --> is the parent for the head-GC interface
  the disclosure map operationalises. The head does not
  interpret statutes; GC does. The map is the head's
  artefact that lets GC's incident-time interpretation work
  be bounded and fast.
- Chapter [[03-article-73-filing-at-incident-time]] is the
  EU counterpart to this chapter. Where an incident has both
  EU and US exposure, the two chapters run in parallel under
  this chapter's lead-jurisdiction discipline.
- Chapter [[06-difficult-incident-conversations]] rehearses
  the conversations that follow when a US-side filing is
  late or when a filed disclosure produces a difficult
  regulator follow-up. A missed Colorado AG notification, an
  SEC comment letter on a delayed Item 1.05, an OCR
  investigation opening on a HIPAA breach — each generates a
  difficult conversation the head steps into.
- Chapter [[05-post-incident-learning-cycle-sponsorship]]
  picks up the disclosure-map artefact as an input to the
  learning cycle. A serious incident that surfaced a
  disclosure-map gap — a surface the map did not carry, a
  timing the map got wrong, a sign-off routing that did not
  hold under pressure — produces a map-update finding the
  head sponsors alongside the RCA's other findings.

## Summary

- There is no single US AI serious-incident regime the head
  files against at incident time. The US surface is a
  patchwork of federal, state, and sector obligations, each
  with its own trigger, recipient, timeline, and sign-off
  routing. The head's discipline is to maintain a live map
  of the surfaces the enterprise plausibly triggers.
- The map is the head's artefact. GC does the incident-time
  statutory interpretation, but GC cannot productively
  answer "is there a US filing" as an open question. The
  head brings the bounded question set; the map is the
  question set.
- The named surfaces the map carries include: the Colorado
  AI Act (SB24-205) AG-notification obligation for
  algorithmic discrimination, the NAIC AI Model Bulletin's
  state-by-state commissioner-notification expectations, the
  HHS OCR HIPAA Breach Notification Rule (45 CFR 164.400-
  414) where AI triggers PHI exposure, the FDA MDR regime
  (21 CFR Part 803) for AI/ML-enabled medical devices
  including the PCCP composition, the EEOC / DOL / OFCCP
  surfaces for AI-in-HR incidents, the CPPA / 50-state
  state-AG breach-notification patchwork, the SEC Form 8-K
  Item 1.05 cybersecurity-incident disclosure obligation
  for listed enterprises, and the Federal Reserve SR 11-7 /
  sector model-risk surfaces for regulated banks and their
  sector equivalents.
- The map has seven columns: obligation, recipient,
  triggering condition, timeline from awareness, filing
  content template, internal sign-off routing, and
  coordination touchpoint. Each row is fully populated so
  that at incident time the head reads across rather than
  interprets afresh.
- The map is refreshed on the standing regulatory-change-
  management cadence from
  [[mod-105-regulatory-change-management]] — quarterly at
  minimum, more frequently on named-regime moves — and
  ratified in the CxO-adjacency map. It is audit-committee-
  visible.
- A single serious AI incident with cross-jurisdictional
  exposure plausibly triggers Article 73 filings, SEC 8-K
  disclosure, HIPAA OCR notification, state-AG
  notifications, the Colorado AG notification, and NAIC-
  adopting-state commissioner notifications in parallel.
  The head's discipline is that a single AI-substantive
  account of the incident is the single source every filing
  composes against; the filings say the same things about
  the same facts.
- Timelines across regimes do not align. The head does not
  delay one filing for another; the head runs each on its
  statutory clock and ensures the parallel filings do not
  create the appearance of selective disclosure. An
  incident-filing register tracks every open filing surface,
  its clock, and its sign-off status.
- The lead-jurisdiction convention names, at the outset of
  a cross-jurisdictional incident, which side of the map
  holds the primary coordination role for the enterprise's
  cross-regime posture. The convention is distinct from
  the lead-NCA convention from chapter 03; both run
  simultaneously in a fully cross-jurisdictional incident.
- The failure mode this chapter defends against is the head
  who filed the Article 73 filing on time and missed the
  US sector-specific disclosure because the map did not
  exist or was stale. The map is what makes that failure
  mode preventable.
