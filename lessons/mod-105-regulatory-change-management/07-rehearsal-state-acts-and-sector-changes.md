# Rehearsal — State AI Acts, OSFI E-23, and the Korea AI Basic Act

## Motivation

Chapter 06 rehearsed the discipline against Union-scale and
standards-scale items. This chapter rehearses against three
patterns that are commercially and operationally more disruptive
to many enterprises than the Union-scale items are: US state
AI-specific legislation (with Colorado's SB 24-205 as the
anchor and Texas's Responsible AI Governance Act as a peer),
Canadian financial-sector supervisory guidance (OSFI's E-23), and
the Korean AI Basic Act. Each of these has the property that
attachment is often narrower than the Union-scale items but
compliance-date pressure is often sharper, and each is the kind
of item where an enterprise operating across many jurisdictions
loses coordination first.

Each rehearsal follows the template from chapter 06: what the
item is at head level, triage tier, interpretation packaging
shape, plan shape, and coordination pattern. As before, the
purpose is not legal briefing (GC's work) but shaping the head's
discipline muscle-memory.

The three items are chosen to span the plausible landscape of
sub-Union scale change: a US state horizontal AI act (Colorado),
a peer US state act with a distinctive shape (Texas), a national
sector-supervisory guideline (OSFI E-23), and a national
horizontal AI framework outside the US and EU (Korea's Basic
Act). An enterprise that has run each pattern once has muscle-
memory for the shape of most sub-Union changes it will
encounter.

## Rehearsal 4 — the Colorado AI Act (SB 24-205)

### What the item is at head level

Colorado's SB 24-205, signed in May 2024, is a horizontal AI act
focused on consumer protection in high-risk AI systems. Its core
obligations attach to developers and deployers of high-risk AI
systems used for consequential decisions concerning Colorado
residents — decisions on education, employment, financial or
lending services, essential government services, health-care
services, housing, insurance, or legal services.
<!-- needs-research: verify the enacted text and the definition of
     "consequential decision" and "high-risk artificial
     intelligence system" under Colorado SB 24-205 against the
     Colorado General Assembly published text and any amending
     legislation (including subsequent-session bills that may have
     modified the enforcement date or the substantive obligations) -->

The Act's original effective date was February 1, 2026, but
subsequent legislative activity has modified the timing — a 2025
special-session bill delayed enforcement and refined provisions.
<!-- needs-research: verify the current effective date of Colorado
     SB 24-205 as amended by any subsequent legislation, including
     the 2025 special session and any 2026 legislative session
     changes, against Colorado General Assembly records; confirm
     whether enforcement is set for 2026, 2027, or a later date -->

Colorado's Division of Insurance operates a distinct AI regulation
(Regulation 10-1-1) that applies specifically to AI systems used
by insurers licensed in Colorado. That regulation predates SB
24-205 and applies independently of it.
<!-- needs-research: verify the current text and effective date of
     Colorado Insurance Regulation 10-1-1 against the Colorado
     Division of Insurance published rulemaking -->

The head's operating question: does the enterprise use, provide,
or deploy AI systems that make consequential decisions
concerning Colorado residents in one of the eight named domains,
and if so, at what depth do the developer and deployer
obligations attach.

### Triage tier at scanning

For most enterprises with any material customer base in
Colorado, this is a priority-tier item once the effective date
is confirmed. The attachment analysis is central to the priority
calibration: many enterprises are surprised to discover on
attachment analysis that they are in scope of one of the eight
domains even if AI-in-consequential-decisions is not their core
product.

For insurance-writing enterprises, Regulation 10-1-1 has been
an active-tier item since its 2023 issuance and merits ongoing
tracking regardless of SB 24-205.

### Interpretation packaging

The packaging memo captures three sub-packages.

- **Developer obligations under SB 24-205.** Reasonable care to
  protect consumers from algorithmic discrimination, disclosure
  obligations to deployers, statement of intended uses and
  known / foreseeable harms, and updated documentation when
  substantive modifications occur.
- **Deployer obligations under SB 24-205.** Risk-management
  policy and programme, impact assessment obligations, consumer
  notice obligations, and adverse-consequence disclosure and
  appeal-and-correction obligations.
- **Interaction with Colorado Insurance Regulation 10-1-1** for
  insurance-writing enterprises. Regulation 10-1-1 has its own
  governance-and-risk-management framework requirements that
  overlay SB 24-205 for the insurance domain.

Each sub-package is packaged against the enterprise's AI system
inventory using the level-50 architect's crosswalk. Attachment
analysis names which of the enterprise's AI systems are "high-
risk" under the Act's definition, which decisions those systems
make, which Colorado residents are affected, and where the
enterprise sits as developer versus deployer versus both.

The specific questions for GC include: how does the Colorado
Attorney General's rulemaking authority under the Act translate
into specific enforcement expectations; how do the exceptions
in the Act (small deployer threshold, industry-specific
carve-outs where applicable) apply to the enterprise's specific
facts; and what is the interaction with any pending or in-force
federal AI legislation the enterprise is planning against.

### Plan shape and compliance-date posture

Colorado is a full-seven-lane plan for in-scope enterprises. The
distinctive plan-shape features:

- **Lane 2 (communications)** carries a customer-facing notice
  obligation for adverse consequences. The head coordinates with
  the CCO and with the customer-facing operating teams on the
  notice content and delivery.
- **Lane 3 (training)** is heavy because the deployer risk-
  management programme requires trained staff to operate it.
- **Lane 4 (exceptions)** carries the specific interaction with
  any pending state-level exemption or delay: as the Act's
  effective date has shifted, the exception window planning has
  had to accommodate legislative changes mid-flight.
- **Lane 5 (board reporting)** for enterprises with material
  Colorado customer bases: the audit committee is briefed on
  the readiness posture ahead of the effective date.
- **Lane 6 (regulator notification)** is triggered by consumer
  complaints or adverse-consequence reports the Act creates
  channels for, not by proactive filings.
- **Lane 7 (supply chain)** is significant because the developer-
  to-deployer disclosure obligations propagate up the enterprise's
  supplier chain of AI models used in in-scope systems.

The compliance-date posture almost always involves a transition-
window component — the Act's obligations are structurally novel
enough that full readiness on the effective date across a broad
in-scope inventory is expensive and typically not what the
regulator is expecting for reasonable, well-governed enterprises.

### Coordination pattern

Lane A (architect + engineering) coordinates the AI system
inventory attachment analysis and the technical work for
impact-assessment production. Lane B (GC) handles the
interaction with prior federal fair-lending, employment, and
housing law where the Act's high-risk domains overlap those
regimes. Lane C (procurement) carries the developer-to-deployer
information exchange with model vendors. Lane E
(communications) carries the consumer-notice content. Lane F:
the CPO / DPO is a peer where the CPA (Colorado Privacy Act)
overlaps; the CHRO is a peer on employment-domain systems; the
GC is a peer where the AG's enforcement authority becomes
relevant.

## Rehearsal 5 — Texas Responsible AI Governance Act (TRAIGA)

### What the item is at head level

Texas has considered horizontal AI-governance legislation across
recent legislative sessions, culminating in the Texas Responsible
AI Governance Act (TRAIGA). Its provisions and its enacted
status have moved through iterations, and its final substantive
shape and effective date are subject to verification as of the
research window.
<!-- needs-research: verify the enacted status of TRAIGA as of the
     research window against the Texas Legislature bill tracker,
     confirm the final substantive text (including whether any
     final version differs materially from prior drafts), and
     confirm the effective date -->

TRAIGA is worth rehearsing separately from Colorado because
Texas takes a distinctive drafting posture on several
substantive questions — including prohibitions on specific
uses, enforcement authority allocation between the Attorney
General and the Department of Information Resources, and
interactions with federal law. An enterprise that has done
Colorado's plan does not automatically have a Texas plan.

### Triage tier at scanning

TRAIGA is an active-tier item during the interpretation window
between passage and effective date, promoting to priority as
the effective date closes. For enterprises with material Texas
customer bases or Texas-consumer-facing AI systems, the triage
tier is aggressive.

### Interpretation packaging

The packaging memo distinguishes TRAIGA obligations from
Colorado's SB 24-205 obligations along three axes: which uses
are addressed (Texas takes a distinct approach to certain
uses), which enforcement channel applies (state AG, state
department, or private right of action), and how federal-law
interaction is handled. Each axis is a specific question for
GC.

### Plan shape and compliance-date posture

Where the enterprise has run Colorado, the Texas plan reuses
Lanes A (architect / engineering) and C (procurement) heavily
— the technical inventory work is largely portable — but Lane
B (GC) is heavier because the interpretation of Texas-specific
provisions is standalone work. Lane 5 (board reporting) for
enterprises that have already briefed on Colorado can briefly
note Texas as a state-scale peer; for enterprises without
Colorado exposure, Texas may be the first state-scale item
briefed to the audit committee.

The compliance-date posture is usually a transition-window
posture for the enterprise's first state AI act; enterprises
that already run Colorado can often approach Texas from a
narrower delta-posture.

### Coordination pattern

Similar to Colorado, with the addition of state-Attorney-
General-relations posture. Government Affairs
(mod-104 chapter 07 covers the boundary) is a coordination peer
here because the enterprise's relationship with Texas state
government generally is broader than a single Act, and
Government Affairs carries the political-relationship layer.

## Rehearsal 6 — OSFI Guideline E-23

### What the item is at head level

OSFI (Office of the Superintendent of Financial Institutions) is
the Canadian federal financial-institution supervisor. Its
Guideline E-23 governs model risk management at federally
regulated financial institutions. OSFI issued a revised
Guideline E-23 in 2023 and has communicated an effective date
of July 1, 2027 for the revised guideline.
<!-- needs-research: verify the current effective date of OSFI's
     revised Guideline E-23 against the OSFI published guidance
     and any subsequent supervisory communications; verify the
     substantive scope of the revised guideline, particularly
     whether AI/ML models fall within its scope explicitly or
     implicitly through the definition of "model" -->

E-23 covers model risk broadly and is not AI-specific — it
applies to any model that meets its definitional threshold at a
federally-regulated financial institution. AI/ML models
generally fall in scope. The revision brings E-23 closer in
spirit to US SR 11-7 (Federal Reserve model-risk guidance),
though with Canadian regulatory-culture differences.

The head's operating question: for a Canadian federally-
regulated financial institution, does the enterprise's AI model
population fall in scope of E-23 as revised, and what is the
delta from the enterprise's current model-risk-management
programme (which is often owned by the Head of MRM, not by the
Head of AI Governance) to the E-23 revised expectations.

### Triage tier at scanning

Priority-tier for Canadian FRFIs. Active-tier for peer
enterprises tracking sector-supervision practice. Watch-tier for
enterprises outside Canadian federal financial-institution
scope.

### Interpretation packaging

The distinctive feature of E-23 packaging is the interaction
with the enterprise's existing model-risk-management programme.
For most Canadian FRFIs, MRM is a mature discipline owned by a
Head of MRM (typically reporting to CRO or to a Chief Risk
Officer for models). AI governance is a newer discipline. The
packaging question is not "how do we build E-23 compliance from
zero" but "how do the head of AI governance and the head of
MRM coordinate to close the enterprise's E-23 delta together".

The packaging memo captures: the scope overlap between AI
governance and MRM at the enterprise; the delta from current
MRM practice to E-23's revised expectations, focused on AI/ML
model risk; the governance-boundary question (which function
owns the AI/ML component of the E-23 filing to OSFI); and the
GC questions on OSFI examination practice.

### Plan shape and compliance-date posture

E-23 plans are heavily architect-and-MRM-coordinated. Lane A
carries the AI-governance overlay; MRM carries the parent
programme. Lane B (GC) handles OSFI supervisory-relationship
posture. Lane C (procurement) is affected only where the
enterprise uses third-party AI models in E-23 scope. Lane E
(communications) is minimal — E-23 is a supervisor-facing
matter, not a consumer-facing matter. Lane 6 (regulator
notification) is the OSFI supervisory dialogue itself, running
through the Chief Risk Officer for models and the Head of MRM
with the head of AI governance in the room for AI-specific
substance.

The compliance-date posture usually aligns to the July 2027
effective date with a phased readiness plan running from the
mid-window: full readiness by the effective date on the AI
overlay, dependent on MRM's overall readiness posture.

### Coordination pattern

Lane A: the level-50 architect and the Head of MRM's model-
inventory function are peers. Lane B: GC handles OSFI
relationship and Canadian federal-supervisory practice. Lane F:
the CRO is the primary CxO peer here (E-23 sits inside the
enterprise's risk framework); the CAE is a peer because third-
line audit of MRM programmes is dense; the CFO is a peer on
material model-population costs.

For enterprises operating in both the US and Canada,
coordination with the US model-risk-management programme (SR
11-7, OCC 2011-12, SR 23-4) is coordinated with the E-23 work
to avoid parallel programmes on the same model population.
Cross-reference: [[mod-111-sector-program-leadership]] chapter
01 (banking leadership drill).

## Rehearsal 7 — the Korea AI Basic Act

### What the item is at head level

South Korea passed a horizontal AI framework — commonly referred
to as the AI Basic Act — in late 2024, with implementing
regulations and effective-date arrangements developing in the
period following passage.
<!-- needs-research: verify the enacted status of the Korean AI
     Basic Act (the "Act on the Development of AI and
     Establishment of Trust Foundation" or equivalent title) as of
     the research window against the National Assembly of Korea
     records; verify the effective date, the promulgation of
     implementing decrees by the Ministry of Science and ICT
     (MSIT) or equivalent, and the current status of any related
     rulemaking -->

The Basic Act's provisions establish a horizontal framework for
AI development and use in Korea, including risk-classification
provisions for "high-impact AI" and transparency and
accountability requirements for AI providers. Enforcement is
allocated to Korean ministries with sector-specific overlays
from sector regulators.
<!-- needs-research: verify the specific substantive obligations
     of the Korean AI Basic Act (high-impact AI definitions,
     provider and deployer obligations, transparency requirements)
     and the enforcement allocation among ministries against the
     enacted text -->

The head's operating question: does the enterprise provide or
deploy AI systems that reach Korean users, and if so, what
attachment do the Basic Act's obligations create on the
enterprise's operating posture in Korea.

### Triage tier at scanning

Active-tier for enterprises with material Korean operations or
Korean user bases. Watch-tier for enterprises without direct
Korean exposure. Priority-tier for GPAI providers reaching
Korean users, because the interaction with the Basic Act's
transparency provisions can be material.

### Interpretation packaging

The packaging memo's distinctive features:

- **Multi-language interpretation.** The Basic Act's authoritative
  text is Korean, and interpretation for a non-Korean-speaking
  head requires either GC's engagement of Korean-speaking outside
  counsel or careful use of official English translations
  (which are working translations, not authoritative texts).
  The interpretation packaging identifies the source of the
  reading the head is relying on.
- **Ministry-implementing-decree tracking.** The Basic Act
  operates through implementing decrees from MSIT (Ministry of
  Science and ICT) and adjacent ministries. Individual decrees
  land after the Act itself; the interpretation packaging
  tracks the specific decrees as they publish and reads them
  as sub-obligations.
- **Interaction with Korean data protection.** The Personal
  Information Protection Act (PIPA) creates data-protection
  obligations that interact with the Basic Act's provisions on
  training data and AI transparency. The CPO / DPO is a
  substantive peer on any AI system in scope of both.

### Plan shape and compliance-date posture

For enterprises with a Korean presence, the plan is a full-
seven-lane plan with the distinctive addition of local-market
adjustments: Lane 2 (communications) has a Korean-language
external posture; Lane 3 (training) covers Korea-based
employees; Lane 6 (regulator notification) coordinates with
Korean ministries. Lane C (procurement) is affected where
Korean-based suppliers are in scope.

For enterprises without direct Korean presence but with
material Korean user bases (extraterritorial reach), the plan
is thinner and focuses on the transparency and disclosure
provisions the enterprise can meet without a local operating
footprint.

The compliance-date posture aligns to the Basic Act's phased
implementation schedule and the decree cadence. Because the
regime is new, the compliance-date posture typically involves
a transition-window arrangement that the enterprise coordinates
with Korean sector or ministry counterparts where possible.

### Coordination pattern

Lane A: architect works with the enterprise's Korean product /
engineering teams (where present) on Korea-specific evidence
production. Lane B: GC engages Korean-speaking outside counsel
for authoritative interpretation. Lane C: procurement handles
Korean-supplier contracts if any. Lane E: Communications runs
the Korean-language external posture and, where the enterprise
has a Korean government-affairs footprint, coordinates with
that function. Lane F: the CPO / DPO for PIPA interaction; the
CISO where the Basic Act's transparency provisions touch
security-relevant model information.

## What the four rehearsals have in common

Two patterns worth naming.

- **Sub-Union scale often produces sharper compliance-date
  pressure than Union scale.** Colorado's effective-date churn,
  Texas's rapid enactment, OSFI's fixed 2027 date, and Korea's
  post-passage decree cadence all create sharper timing
  pressure at the enterprise than the AI Act's phased schedule
  does — because they are less predictable and because the
  enterprise often has less time to organise. The head's
  scanning cadence (chapter 01) works harder on sub-Union
  items than on Union items, per unit of attachment.
- **Attachment analysis carries more weight than obligation
  reading at sub-Union scale.** For each of the four items,
  the enterprise's answer to "does this attach to us" is more
  variable and more consequential than the enterprise's
  answer to "what does the obligation require". Colorado's
  eight-domain scope, Texas's use-based provisions, E-23's
  model definition, and Korea's high-impact AI classification
  each create attachment-analysis judgement calls that the
  head owns. GC opines on interpretation; the head owns
  attachment.

## The one-sentence summary

The sub-Union rehearsals — Colorado, Texas, OSFI E-23, Korea
Basic Act — put the head's discipline against items where
compliance-date pressure is sharper, attachment analysis is
harder, and coordination with sector peers (MRM for OSFI,
Korean product for the Basic Act) is more distinctive; the
enterprise that has muscle-memory for these four shapes has
muscle-memory for most sub-Union changes.

## Summary

- Sub-Union scale regulatory change often produces sharper
  compliance-date pressure than Union scale, because it is
  less predictable and the enterprise has less time.
  Attachment analysis carries more weight than obligation
  reading at sub-Union scale.
- Colorado SB 24-205 is a priority-tier item for enterprises
  with material Colorado exposure in the eight high-risk
  domains. The plan is seven-lane with heavy communications
  (consumer notice), training, exception (legislative-timing
  interaction), and supply-chain lanes. Coordination with the
  CCO, CHRO, and Insurance Division as relevant.
- Texas TRAIGA is a companion state-scale item with a
  distinctive drafting posture. Where an enterprise has run
  Colorado, the Texas delta is smaller on Lanes A / C and
  larger on Lane B (GC).
- OSFI Guideline E-23 (effective 2027 per current supervisory
  communication) applies at Canadian federally-regulated
  financial institutions. The plan coordinates with the Head
  of MRM and the CRO closely, with the head of AI governance
  as the AI-specific overlay peer.
- The Korea AI Basic Act creates a horizontal framework with
  multi-language interpretation, ministry-decree tracking, and
  PIPA interaction as distinctive coordination features. The
  plan shape is full for enterprises with Korean presence,
  thinner for extraterritorial-reach-only enterprises.
- The muscle-memory across the four rehearsals: know the
  enterprise's attachment picture before the item lands; know
  which CxO peers are load-bearing per item; know which
  ministry, division, or supervisor is the counterparty; and
  do not overuse Union-scale plan-shape machinery on sub-Union-
  scale items.
- Rehearsal is what turns the general discipline (chapters 01
  to 05) into a defensible response the day the item lands.
