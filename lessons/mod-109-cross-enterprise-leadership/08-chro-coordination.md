# CHRO Coordination Pattern — AI-in-HR Is a Regulated Surface Now

## Motivation

The Chief Human Resources Officer runs the enterprise's human-
capital function: hiring, performance management, compensation,
workforce planning, learning and development, employee
relations, and the HR report line to the board's compensation
committee and, on material matters, to the audit committee. The
head of AI governance interfaces with the CHRO on a distinct
surface: *AI-in-HR governance*. This is the AI-specific
governance of AI systems used *by* HR (hiring tools,
performance-management systems, employee-monitoring systems,
compensation-analytics systems) and the AI-training strategy
for the workforce (which is the CHRO's operational domain but
which the head's function specifies the content of).

The failure mode is a head who treats AI-in-HR as an "HR
matter" that the CHRO handles independently. Under the current
regulatory environment — NYC Local Law 144 (bias audits for
automated employment decision tools, effective July 2023),
EEOC guidance on AI in employment (May 2022 ADA and May 2023
Title VII guidance), Illinois HB 3773 (amending the Illinois
Human Rights Act to address AI in employment, effective January
2026), Colorado SB 24-205 (AI Act) with its employment
applicability, EU AI Act Annex III item 4 (AI systems in
employment as high-risk), and the ever-expanding state and
international patchwork — AI-in-HR is one of the most heavily
regulated AI use surfaces in the enterprise. A CHRO handling it
independently without the head's function's governance discipline
is a CHRO exposing the enterprise to enforcement, class-action
litigation, and reputational risk.

The other failure mode is a head who tries to run AI-in-HR
governance without the CHRO. HR practices are the CHRO's
domain by charter and by statute in many jurisdictions
(specifically the DPO's or CHRO's role under GDPR for
employee-data processing). A head who bypasses the CHRO on
AI-in-HR controls will find the controls ignored by the HR
function they were supposed to govern.

The coordination pattern in this chapter is the middle path.
It rests on a joint AI-in-HR governance surface (AI systems
used by HR are inventoried, assessed, bias-audited, and
monitored jointly), performance-management AI governance (a
specific sub-surface with acute litigation exposure), and a
joint workforce AI-training strategy (the head specifies the
governance content; the CHRO's L&D function delivers it).

The pattern draws on NYC Department of Consumer and Worker
Protection (DCWP) guidance on Local Law 144, the EEOC's ADA
(May 2022) and Title VII (May 2023) guidance on AI in
employment, Illinois HB 3773 as codified in the Illinois Human
Rights Act, Colorado SB 24-205, the EU AI Act Annex III item
4, ISO 30414:2018 (human capital reporting) as a relevant
framework, GDPR Articles on employee-data processing (Article
88 empowers member-state law on employee data), and industry
practice on bias-auditing (with methodological references from
NIST SP 1270 and equivalent literature).

## Core concept — AI-in-HR is joint by design

The load-bearing move is a single-sentence discipline: AI
systems used by HR are jointly governed — the CHRO owns the
HR operational discipline, the head owns the AI-governance
discipline, and every AI-in-HR system falls under both.

Two consequences.

- **The AIMS inventory carries AI-in-HR systems as a
  distinct category** with the specific regulatory-obligation
  overlay applied to them: NYC LL 144 bias audit
  requirement, EEOC guidance-relevant testing, Illinois HB
  3773 applicability, Colorado AI Act applicability, EU AI
  Act Annex III item 4 applicability, and any other
  jurisdiction-specific overlays. The head's function
  maintains the inventory and the regulatory overlay; the
  CHRO's function operates the systems.
- **The AI Governance Council** (per chapter
  [[11-chairing-the-governance-council]]) has the CHRO or the
  CHRO's AI-in-HR delegate as a standing member for
  decisions touching AI-in-HR systems. Decisions on AI-in-HR
  systems are not made without CHRO endorsement.

## The three coordination surfaces

### Surface 1 — hiring-tool AI governance

Hiring tools that use AI — resume screening, video-interview
analysis, skills-assessment scoring, matching algorithms —
have been the first AI-in-HR category to face heavy
regulation. The interface between the head and the CHRO here
carries specific artefacts and specific cadences.

The interface specifies:

- **The hiring-tool AI inventory.** Every AI-driven hiring
  tool in production (whether built internally or procured)
  is in the AIMS inventory under the hiring-tool category.
  Vendors are named; contract references are named;
  jurisdictional applicability is named.
- **Regulatory-overlay mapping.** For each hiring tool, the
  jurisdictions the tool operates in (based on where
  candidates reside, where they are hired for, and where
  the enterprise operates) and the applicable regulations
  per jurisdiction. The mapping is co-authored by the head's
  level-50 architect and the CHRO's employment-law lead.
- **The bias-audit discipline.** For tools subject to NYC LL
  144 or equivalent bias-audit obligations, the audit is
  conducted by an independent auditor at the cadence the
  regulation requires (annual for NYC LL 144). The head's
  function is the accountable executive for the audit's
  procurement, methodology review, and result publication;
  the CHRO's function is the accountable executive for the
  operational use of the tool and for any post-audit
  operational changes.
- **The candidate-disclosure discipline.** For jurisdictions
  requiring pre-use candidate disclosure (NYC LL 144, EU AI
  Act Article 26 deployer transparency, and equivalent
  provisions), the CHRO's function operates the disclosure
  at the candidate-experience layer; the head's function
  specifies the content the disclosure must contain and
  reviews the disclosure for compliance.
- **The adverse-action discipline.** Where a hiring tool
  produces an adverse decision on a candidate (rejection,
  down-ranking, exclusion from further consideration) and
  the jurisdiction requires notification (Illinois HB 3773
  under specific conditions; EEOC ADA guidance on reasonable
  accommodation; state-specific credit-adjacent adverse-
  action regimes), the CHRO's function operates the
  notification; the head's function specifies the content and
  the underlying explanation logic.
- **The vendor-management overlay.** For third-party hiring
  tools, the third-party evidence discipline (per
  [[mod-102-running-the-program]] chapter 07) applies, with
  the CHRO's vendor-management lead as joint owner.

Cadence: hiring tools inventoried on onboarding and reviewed
annually; bias audits at the regulation-required cadence;
regulatory-overlay mapping reviewed at each jurisdiction's
regulatory change; vendor-evidence review on the third-party
cadence. Joint owner: the head's level-50 architect and the
CHRO's employment-law-and-hiring lead.

### Surface 2 — performance-management AI governance

Performance-management AI — AI systems that produce inputs
into promotion, compensation, discipline, or termination
decisions — is the AI-in-HR sub-surface with the highest
per-decision litigation exposure. A hiring tool that
misclassifies a candidate produces one adverse hiring
decision; a performance-management tool that misclassifies
an employee produces potentially years of career impact.

The interface specifies:

- **Performance-management AI inventory.** Every AI system
  that produces inputs into promotion, compensation,
  discipline, or termination decisions is in the AIMS
  inventory under the performance-management category, with
  the specific decision types the system's outputs feed
  into and the specific human-review or human-decision
  interlock.
- **The human-in-the-loop discipline.** For every
  performance-management AI system, the specific human
  decision-maker who ratifies the AI system's output before
  it is acted on is named. "The system flags; a manager
  reviews and decides" is a discipline; "the system's output
  is the decision" is a discipline break the head's function
  refuses.
- **The transparency discipline.** For employees subject to
  performance-management AI, the enterprise's disclosure
  posture — what the employee is told about the system's
  role in performance evaluation, what recourse the employee
  has to contest an AI-informed decision — is co-authored by
  the CHRO's employee-relations lead and the head. The
  disclosure is compliant with the jurisdictions the
  employees are subject to.
- **The audit discipline.** Performance-management AI is
  audited at a cadence matching the risk. For high-impact
  systems (compensation-decision AI, discipline-decision
  AI), the audit cadence is at least annual, with disparate-
  impact analysis by protected class per applicable
  jurisdiction. For lower-impact systems (feedback-summary
  AI, coaching-recommendation AI), the audit cadence may be
  less frequent but is documented.
- **The recourse discipline.** When an employee contests an
  AI-informed performance decision, the CHRO's employee-
  relations function handles the contestation; the head's
  function provides the AI-specific technical inputs (system
  logic explanation, output-generation trace, evidence of
  human review). The recourse discipline is documented as
  part of the AIMS onboarding for the system.

Cadence: inventory at onboarding and annually; audit at
system-specific cadence; recourse case-by-case. Joint owner:
the head's level-50 architect and the CHRO's performance-
management-and-employee-relations lead.

### Surface 3 — workforce AI-training strategy

The workforce needs to know how to work with AI — how to use
sanctioned AI capabilities effectively, how to recognise AI-
specific risks in their work, how to escalate AI-related
concerns. The training is the CHRO's operational domain (the
L&D function delivers it); the substantive content is jointly
authored by the head's function and the CHRO's L&D lead.

The interface specifies:

- **The AI-training curriculum framework.** A joint
  curriculum framework covering: AI foundations (what AI is,
  what the enterprise's AI systems do, what risks AI carries),
  role-specific training (specific training tracks for
  engineers, product managers, sales, customer support, HR
  itself, legal, and other functions), leadership training
  (a level-60-appropriate track for the enterprise's leaders
  on AI governance), and specialist training (for the head's
  own function's team members and for closely-adjacent
  functions like the CISO's team, the CDO's team, and GC's
  team).
- **The certification-support programme.** For roles where
  external AI-governance certifications add material value
  (IAPP AIGP for governance staff, ISO/IEC 42001 Lead
  Implementer / Lead Auditor for architect and audit-
  adjacent staff, sector-specific certifications where
  relevant), a jointly-authored sponsorship programme with
  the CHRO's L&D-and-certifications lead. See
  [[mod-112-certifications-career-path-community-leadership]].
- **The AI-literacy compliance.** Under EU AI Act Article 4
  (AI literacy), the enterprise as a deployer / provider must
  ensure sufficient AI literacy of staff involved in AI
  systems' use. The head's function specifies the literacy
  standard; the CHRO's L&D delivers the training and
  maintains the completion records; the head's function
  monitors completion rates and reports at the KRI/KPI
  cadence (evidence-completeness rate includes training
  completeness).
- **The AI-in-HR-specific training for HR staff.** HR staff
  using AI-driven hiring, performance-management, or
  employee-monitoring tools need training specific to those
  tools' correct use and specific to the regulatory
  obligations that attach to their use. This is delivered by
  the CHRO's L&D on content authored by the head's function.

Cadence: annual curriculum review; new-hire onboarding
delivery; role-transition delivery; ad-hoc for material AI
system changes. Joint owner: the head's level-50 architect
and the CHRO's L&D lead.

## The interface document

Consolidated in a single interface document co-signed by the
head and the CHRO, ratified in the CxO adjacency map. The
document has, at minimum:

1. **The joint-governance principle.** AI systems used by HR
   are jointly governed; the CHRO owns HR operational
   discipline; the head owns AI-governance discipline; every
   AI-in-HR system falls under both.
2. **The three coordination surfaces.** Hiring-tool AI
   governance, performance-management AI governance,
   workforce AI-training strategy — each with the artefacts,
   the cadence, and the joint owners.
3. **The regulatory-overlay register.** A specific register
   listing AI-in-HR systems, jurisdictions, and applicable
   regulations, maintained by the head's function and the
   CHRO's employment-law lead jointly.
4. **The AI Governance Council membership.** The CHRO or the
   CHRO's AI-in-HR delegate is a standing member on
   decisions touching AI-in-HR systems.
5. **The escalation ladder.** When the interface breaks — a
   hiring tool is procured without the head's function's
   inventory registration; a performance-management AI
   decision is made without the human-in-the-loop discipline;
   an AI-literacy training completion rate falls below the
   KRI threshold — how the head and the CHRO escalate.
   Typically: peer conversation, then CEO or audit committee.
6. **The joint audit-committee or compensation-committee
   appearance.** Once a year, the head and the CHRO appear
   jointly at the audit committee (on the AI-in-HR
   compliance dimension) and, where the enterprise's
   governance splits AI-in-HR into the compensation
   committee's remit for performance-management AI, at the
   compensation committee (on the performance-management
   AI dimension).
7. **The review cadence.** Annual review of the interface
   document; ad-hoc on material regulatory changes affecting
   AI-in-HR.

## Anti-patterns the head does not permit

**The AI-in-HR unilateral procurement.** The CHRO's function
(or a business-unit HR delegate) procures an AI hiring tool
or performance-management tool without informing the head's
function. The tool enters production, misses the AIMS
inventory, misses the bias audit, and surfaces at the next
regulatory examination or the next candidate complaint. The
remedy is: the AIMS onboarding process (per
[[mod-102-running-the-program]] chapter 06) treats AI-in-HR
tools as first-class inventory entries; procurement gates
require the head's function's registration; the CHRO's
function respects the gate.

**The performance-management AI without human-in-the-loop.**
A performance-management AI system's outputs are acted on
directly (compensation adjustment, discipline, termination)
without a named human decision-maker in the loop. When an
adverse decision is contested, the enterprise cannot defend
that the AI's output was the decision. The remedy is: no
performance-management AI system operates without a named
human-in-the-loop discipline; the head's function refuses to
inventory-register systems that do not meet this bar.

**The training-content overreach.** The head's function
authors AI-training content that is then delivered by L&D,
but the head's function then also tries to run the L&D
delivery discipline (attendance tracking, comprehension
testing, completion certification). The CHRO's L&D reads
this as encroachment. The remedy is: content-authoring is
joint; delivery is the CHRO's L&D; the head's function
consumes completion metrics through the interface, not
through parallel tracking.

**The bias-audit-as-vendor-fig-leaf.** The bias audit is
delegated to the vendor of the hiring tool and no
independent audit is procured. The vendor's audit is
predictably favourable; the audit fails when the
jurisdiction's regulator or a class-action plaintiff commissions
an independent audit that finds bias the vendor's audit did
not. The remedy is: bias audits under NYC LL 144 and
equivalent regimes are conducted by *independent* auditors;
the head's function is the accountable executive for
independence and for methodology review.

**The employee-monitoring drift.** AI-driven employee
monitoring (productivity monitoring, communication
monitoring, activity monitoring) enters production without
the joint governance discipline. Employee-relations
consequences follow. The remedy is: employee-monitoring AI
is in scope for the joint interface, treated with the same
inventory-and-audit discipline as hiring-tool AI, with the
CHRO's employee-relations lead as the joint owner.

## Composition with adjacent modules

- The **CxO adjacency map** in
  [[mod-101-role-scope-and-leadership-shape]] chapter 06 is
  the parent boundary document.
- The **AIMS inventory** in [[mod-102-running-the-program]]
  chapter 06 is where AI-in-HR systems are categorically
  registered.
- The **third-party evidence discipline** in
  [[mod-102-running-the-program]] chapter 07 is what the
  hiring-tool vendor-management overlay operates against.
- The **regulatory-change discipline** in
  [[mod-105-regulatory-change-management]] is what surfaces
  new AI-in-HR regulations; the regulatory-overlay register
  updates on the discipline's cadence.
- The **AI Governance Council** (chapter
  [[11-chairing-the-governance-council]]) is where AI-in-HR
  decisions are ratified with the CHRO present.
- The **CPO / DPO coordination** in chapter 03 is where the
  employee-data processing dimension (GDPR Article 88,
  equivalent regimes) coordinates.
- The **certification-and-career-path discipline** in
  [[mod-112-certifications-career-path-community-leadership]]
  is where the certification-support programme sits.

## Summary

- AI-in-HR is a heavily regulated surface (NYC LL 144, EEOC
  guidance, Illinois HB 3773, Colorado SB 24-205, EU AI Act
  Annex III item 4, and expanding). The CHRO cannot govern
  it alone; the head cannot govern it without the CHRO. The
  coordination pattern is joint by design.
- Three coordination surfaces carry the work: hiring-tool AI
  governance (inventory, regulatory-overlay mapping,
  independent bias audits, candidate disclosure, adverse-
  action notification, vendor evidence), performance-
  management AI governance (inventory, human-in-the-loop
  discipline, transparency, audit, recourse), workforce AI-
  training strategy (curriculum framework, certification-
  support programme, AI-literacy compliance under EU AI Act
  Article 4, AI-in-HR-specific training for HR staff).
- The joint-governance principle: AI systems used by HR
  fall under both the CHRO's HR discipline and the head's
  AI-governance discipline. The AI Governance Council
  ratifies AI-in-HR decisions with the CHRO present.
- Five anti-patterns to refuse: AI-in-HR unilateral
  procurement, performance-management AI without human-in-
  the-loop, training-content overreach, bias-audit-as-
  vendor-fig-leaf, employee-monitoring drift.
- The interface document — co-signed by head and CHRO — is
  ratified in the CxO adjacency map, reviewed annually, and
  the head and CHRO appear jointly at the audit committee
  (and, where relevant, the compensation committee) on the
  AI-in-HR compliance-and-effectiveness review.
- Chapter [[09-chief-compliance-officer-coordination]] turns
  to the Chief Compliance Officer adjacency — the parent
  compliance framework the AI-policy taxonomy plugs into.

<!-- needs-research: verify the current effective status and
scope of Illinois HB 3773 amending the Illinois Human Rights
Act to address AI in employment, given the January 2026
effective date and any pre-effective-date guidance from the
Illinois Department of Human Rights before citing specific
obligations. -->

<!-- needs-research: verify current state adoption of NYC-LL-
144-style bias-audit requirements in other jurisdictions
(New Jersey has proposed similar; California has separate
CPPA ADMT applicability; other states are considering
similar measures) before citing a specific jurisdictional
overlay list. -->
