# CPO / DPO Coordination Pattern — The Contested AIA / DPIA Boundary

## Motivation

The privacy adjacency is the single most contested boundary in
the field, and it is the one the head is most likely to have
to renegotiate every year if the interface is not written down.
The Chief Privacy Officer / Data Protection Officer owns the
enterprise privacy program at parent scope — the Article 30
record of processing activities (ROPA) under GDPR, the DPIA
methodology, GDPR / UK GDPR / CCPA / CPRA / PIPEDA / DPDPA /
LGPD / PIPL compliance at enterprise scope, subject-request
handling, and the privacy report line to the audit committee
(and, in GDPR jurisdictions, to the supervisory authority).
The head owns AI-scoped privacy — the AI system impact
assessment (AIA) under ISO/IEC 42005, the automated-decision-
making (ADM) obligations under GDPR Article 22 and the CPPA
ADMT regulations, and the AI-specific privacy risks in the AI
risk register.

The failure mode is two functions producing overlapping
documents on the same AI system that disagree in substance —
the DPIA reads one way about the risk to data subjects; the
AIA reads another way about the risk to affected persons. When
the enterprise is later examined by a data-protection
authority or an EU AI Act market-surveillance authority, the
disagreement between the two documents is the finding. The
enterprise cannot say "we produced both" as a defence when the
two documents contradict each other on the same facts.

The coordination pattern in this chapter is what prevents the
contradiction. It rests on a clear ownership split (DPO owns
DPIA; head owns AIA), an explicit *interface* between the two
documents (they share input assumptions, they cross-reference
each other, they are co-signed for AI systems that process
personal data), and joint discipline on the ROPA extension and
the shared regulatory obligations.

The pattern draws on GDPR Articles 22, 25, 30, and 35;
CCPA / CPRA and the CPPA's Automated Decisionmaking Technology
(ADMT) regulations; India's Digital Personal Data Protection
Act 2023 (DPDPA); Brazil's LGPD; the EU AI Act's Article 27
fundamental rights impact assessment (FRIA); the ICO's AI and
data-protection guidance; the CNIL's AI guidance; and the
IAPP AIGP body of knowledge on the AIA / DPIA interface. It
is executed against the specific interface document the head
and the DPO co-author and ratify.

## Core concept — the ownership split, and the interface

The load-bearing move is a single-sentence ownership split
that both officers agree to and can defend at the audit
committee.

**The DPO is the accountable executive for the DPIA. The head
is the accountable executive for the AIA. For any AI system
that processes personal data, both documents exist and both
are co-signed. Neither substitutes for the other.**

Two-sentence corollary: the DPIA answers "what is the risk to
data subjects arising from the processing of their personal
data by this system, and how is that risk mitigated to the
level GDPR and equivalent statutes require". The AIA answers
"what is the risk to affected persons arising from this AI
system's design, deployment, and operation across all its
outcomes, and how is that risk mitigated to the level ISO/IEC
42005, the EU AI Act, and the enterprise's own AI risk
framework require". These are overlapping but not identical
questions. The overlap is the interface.

The interface is not a merged document. The interface is a
*specification of shared inputs and cross-references*, so that
when the DPIA and the AIA are read together they describe the
same system, the same data, the same processing, and the same
population — with each document answering its own question.

## The three coordination surfaces

### Surface 1 — the AIA / DPIA interface

The interface specifies, for any AI system that processes
personal data, the shared elements the two documents must
agree on and the cross-references each must carry to the
other.

Shared elements:

- **The system definition.** Both documents describe the same
  system, at the same scope of processing, using the same
  identifiers (typically the AIMS inventory ID from
  [[mod-102-running-the-program]] chapter 06 and the ROPA
  processing-activity reference). If the DPIA says the system
  is a "customer-service assistant" and the AIA says it is a
  "customer-service chat interface with agent-tool access",
  they are describing different systems. The interface
  specifies that the definition is authored jointly and
  referenced identically.
- **The population and personal-data categories.** Who the
  data subjects are, what personal-data categories are
  processed (including special-category data under GDPR
  Article 9 or sensitive data under equivalent statutes), and
  what the data volumes are. Both documents pull from the
  ROPA record; the ROPA is the source of truth.
- **The processing purposes.** What the AI system is doing
  with the personal data — training, inference, monitoring,
  logging — and for what purpose in the ROPA sense.
- **The lawful basis.** Under GDPR Article 6 (and Article 9
  for special-category data), the lawful basis for the
  processing. The DPO is the accountable executive for the
  lawful-basis determination; the AIA cites the determination.
- **The automated-decision-making analysis.** Whether the
  system's outputs meet the GDPR Article 22 threshold ("solely
  based on automated processing", "produces legal effects" or
  "similarly significantly affects"), and if so, what the
  Article 22 handling is. The DPO owns the Article 22
  determination; the AIA cites the determination and adds the
  AI-specific human-oversight design that supports the
  determination.

Cross-references:

- The AIA cites the DPIA reference and version.
- The DPIA cites the AIA reference and version.
- Where a mitigation in one document depends on a control
  described in the other, the reference is explicit
  ("adherence to the AIA-mandated evaluation cadence supports
  the DPIA's mitigation of accuracy risk").
- Both documents are co-signed for AI systems processing
  personal data — DPO signs the DPIA and endorses the AIA;
  head signs the AIA and endorses the DPIA.

Cadence: interface applied at every DPIA-triggering event
(new processing, material change to existing processing) and
at every AIA-triggering event (new AI system at qualifying
tier, material change to existing AI system). Joint owner: the
DPO's DPIA lead and the head's level-50 architect, with the
level-15 analyst maintaining the cross-reference registry.

### Surface 2 — the ROPA extension

The ROPA is the DPO's artefact under GDPR Article 30 (or its
equivalent in other regimes — e.g., CCPA does not have a
formal ROPA analogue, but the record-keeping obligations under
the CPPA regulations produce a functional equivalent). Where
personal data is processed for AI training, inference,
evaluation, monitoring, or any downstream AI-related purpose,
the ROPA record picks up specific AI-relevant fields.

The interface specifies the additional fields the ROPA carries
for AI-processing entries:

- **AI system reference.** Link back to the AIMS inventory ID
  for the AI system the processing is for.
- **AI-specific purpose classification.** Is the processing
  for training, inference, evaluation, monitoring, or a
  downstream administrative purpose. This is not a substitute
  for the ROPA's own purpose specification; it is an AI-
  specific tag that supports the AIA reference.
- **Data-minimisation posture.** For training data
  specifically, whether the personal data is used in raw
  form, pseudonymised, anonymised, or replaced with
  synthetic data. Because AI training and inference commonly
  create tensions with data-minimisation, the ROPA reflects
  the specific posture and the AIA elaborates on the
  trade-off.
- **Retention posture.** For training data, model weights
  potentially memorising training-data content, and inference
  logs, the retention posture and its lawful-basis
  justification.
- **Third-country transfers.** Where the AI system involves
  third-country processing (e.g., a third-party foundation-
  model API in a jurisdiction requiring Article 46 safeguards),
  the transfer basis is recorded.
- **DPIA and AIA cross-reference.** The ROPA entry cites both
  the DPIA and the AIA it belongs to.

The DPO's ROPA discipline owns the record. The head's function
provides the AI-specific inputs on the specified schedule and
verifies the ROPA reflects the AI system's processing
faithfully.

Cadence: ROPA reviewed at each material change (per the DPO's
ROPA discipline) and at the annual AI system inventory review.
Joint owner: DPO's ROPA lead and head's level-15 analyst, with
the level-50 architect as the interface owner.

### Surface 3 — shared regulatory obligations

Beyond GDPR, several AI-adjacent regimes divide obligations
between the DPO and the head. The interface specifies who is
the accountable executive on each.

- **GDPR Article 22 (ADM).** DPO is the accountable executive
  for the Article 22 determination. Head is the accountable
  executive for the AI-specific supporting evidence — the
  human-oversight design, the accuracy testing, the
  contestation mechanism, the explanation surface.
- **CPPA ADMT regulations (California).** Where the CPPA's
  Automated Decisionmaking Technology regulations apply, the
  head and the DPO share the notice, opt-out, and access
  obligations. DPO is the accountable executive for the
  privacy-notice surface; head is the accountable executive
  for the specific AI-system disclosures, the risk
  assessment, and the opt-out implementation. See the
  needs-research note on CPPA ADMT current status.
- **DPDPA (India), LGPD (Brazil), PIPEDA (Canada), PIPL
  (China), UK GDPR / DPA 2018 (UK).** In each jurisdiction,
  the DPO or equivalent statutory role is the primary
  accountable executive; the head's function supports on the
  AI-specific dimensions and maintains a jurisdiction map
  (which regime applies to which AI system based on
  data-subject residency and processing location).
- **EU AI Act Article 27 (FRIA).** For deployers of Annex III
  high-risk systems that are public bodies or private entities
  providing public services (or specifically bank-scoped
  systems under Annex III), the fundamental rights impact
  assessment is required. FRIA is the head's artefact (the
  EU AI Act positions it against the deployer); the DPO's
  DPIA feeds it where personal data is involved. The
  interface specifies which document is the accountable
  primary and how the two compose.
- **Subject-access-requests (SARs) that touch AI systems.**
  When a data subject requests access, deletion, correction,
  or restriction against personal data processed by an AI
  system, the DPO's SAR process is the parent process. The
  head's function provides the AI-specific response inputs —
  training-data lineage, inference-log records, model-
  memorisation testing, deletion feasibility analysis. The
  interface specifies the SLA the head's function meets to
  support the DPO's SAR SLA.

Cadence: annual joint review of the shared-obligation map;
per-jurisdiction review when a new regime enters force. Joint
owner: DPO's regulatory lead and the head's level-50 architect.

## The AIA / DPIA co-authoring pattern

For AI systems processing personal data, the practical
authoring pattern:

1. **AI system trigger.** A new AI system is proposed, or an
   existing AI system materially changes. The trigger fires the
   AIMS onboarding process ([[mod-102-running-the-program]]
   chapter 06) and, if personal data is involved, the DPO's
   DPIA process.
2. **Joint scoping session.** Head's level-50 architect and
   DPO's DPIA lead meet with the product owner to align on the
   system definition, the personal-data flows, the ROPA
   reference, and the Article 22 pre-analysis. Session is
   time-boxed (typically 60–90 minutes) and the output is a
   one-page scoping note both documents cite.
3. **Parallel authoring.** DPIA and AIA authored in parallel
   against the scoping note. Each references the other by
   reference identifier and version.
4. **Cross-review.** DPO reviews the AIA for consistency with
   the DPIA on shared elements; head reviews the DPIA for
   consistency with the AIA on shared elements. Cross-review
   is a joint working session, not an email exchange, on
   material AI systems.
5. **Co-sign.** For systems in scope, both officers co-sign
   (DPO on the DPIA, head on the AIA; each endorses the
   other).
6. **Registration.** Both documents registered in the
   respective document-control systems, with the ROPA record
   updated to cite both.

The pattern is version-controlled. When the DPIA is revised
in response to a supervisory-authority interaction, the AIA
is revised in parallel. When the AIA is revised in response
to an evaluation-suite finding, the DPIA is revised in
parallel.

## The interface document

Consolidated in a single interface document co-signed by the
head and the DPO, ratified in the CxO adjacency map. The
document has, at minimum:

1. **Ownership split.** The one-sentence split above, with the
   two-sentence corollary, and the co-sign requirement for AI
   systems processing personal data.
2. **The AIA / DPIA interface specification.** Shared
   elements, cross-references, co-signing convention.
3. **The ROPA extension specification.** AI-specific fields,
   maintenance protocol.
4. **The shared-obligation map.** Per regime (GDPR Article
   22, CPPA ADMT, DPDPA, LGPD, PIPEDA, PIPL, UK GDPR, EU AI
   Act Article 27, SAR handling), the accountable executive
   and the supporting-function boundary.
5. **The co-authoring pattern.** The six-step pattern above,
   with named session owners and named artefacts.
6. **The escalation ladder.** When the interface breaks —
   disagreement on Article 22 determination, disagreement on
   lawful basis for training data, DPIA and AIA produce
   inconsistent facts — how the head and the DPO escalate.
   Typically: DPO-head peer conversation, then CEO or audit
   committee. Where the disagreement involves external
   authorities (a supervisory authority disagreeing with the
   DPO's determination), the DPO is the accountable
   executive for the external interaction and the head
   supports.
7. **The joint audit-committee appearance.** Once a year, the
   head and the DPO appear jointly on the AI-and-privacy
   review at the audit committee, presenting the interface's
   effectiveness against the ROPA / DPIA / AIA cross-reference
   discipline and any material incidents.
8. **The review cadence.** Annual review of the interface
   document; ad-hoc when a jurisdiction's privacy law changes
   materially.

## Anti-patterns the head does not permit

**The AIA-as-DPIA-plus.** The head authors an AIA that is a
DPIA with a section on "AI-specific risks" appended, and the
DPO's DPIA is never authored (or is a stub). This fails on the
first supervisory-authority review because the DPIA has to
answer specific statutory questions the AIA does not. The
remedy is: both documents exist, and each answers its own
question against its own methodology.

**The DPIA-as-AIA-substitute.** The DPO authors a DPIA that
covers AI-specific risks by reference to a generic "AI risk
statement" and the head's function has not produced a real
AIA. This fails on any material AI-specific incident where the
absence of an ISO/IEC 42005-shape AIA is visible. The remedy
is: the AIA is a first-class artefact, not a footnote to the
DPIA.

**The ROPA lag.** The ROPA does not reflect changes in AI
processing until the DPO's annual ROPA review, and by then
the AIMS inventory has moved. The DPO reads the ROPA as an
authoritative record; if it is stale, the SAR handling breaks
and the supervisory authority's next examination finds the
gap. The remedy is: the ROPA update is triggered on the AIMS
onboarding process, not on the DPO's ROPA review cycle.

**The unilateral Article 22 determination.** The head's
function decides a system is not "solely based on automated
processing" because a human reviews the output before it is
acted on, without the DPO's concurrence. The determination is
the DPO's. The head provides the AI-specific supporting
evidence; the DPO signs off. Unilateral determinations are
what the ICO and the EDPB have specifically flagged as failure
modes in guidance.

**The SAR-orphan record.** A data subject requests deletion
against personal data processed by an AI system; the DPO's
SAR process routes the request to the head's function; the
head's function does not respond inside the DPO's SLA; the
DPO's statutory-response deadline is missed. The remedy is:
the interface specifies the head's SAR-support SLA and the
head's function tracks it as a KPI.

## Composition with adjacent modules

- The **CxO adjacency map** in
  [[mod-101-role-scope-and-leadership-shape]] chapter 06 is
  the parent boundary document.
- The **AIMS inventory** in [[mod-102-running-the-program]]
  chapter 06 is the source of the AI-system identifier the
  ROPA and DPIA reference.
- The **AI risk register** in [[mod-102-running-the-program]]
  chapter 03 carries the AI-specific privacy risks; the
  DPO's privacy risk register carries the enterprise privacy
  risks; each references the other.
- The **regulatory change discipline** in
  [[mod-105-regulatory-change-management]] surfaces new
  privacy regimes and material amendments; the head and the
  DPO jointly assess the impact on the shared-obligation map.
- The **incident-leadership discipline** in
  [[mod-110-incident-leadership]] carries the AI-and-privacy
  incident response; the DPO's supervisory-authority
  notification duties (GDPR Article 33) run in parallel.
- The **CIO / CTO / CDO coordination** in chapter 02 governs
  the data platform's training-data provenance and
  minimisation controls the AIA cites.

## Summary

- The DPO owns the DPIA. The head owns the AIA. For AI
  systems processing personal data, both documents exist and
  both are co-signed. Neither substitutes for the other.
- The AIA / DPIA interface specifies shared elements (system
  definition, personal-data categories, purposes, lawful
  basis, Article 22 analysis) and required cross-references,
  so the two documents describe the same system consistently.
- The ROPA extension carries AI-specific fields (AI system
  reference, purpose classification, data-minimisation
  posture, retention posture, third-country transfers, DPIA
  and AIA cross-reference) and is updated on AIMS onboarding,
  not on the DPO's periodic review cycle.
- Shared regulatory obligations divide by regime: DPO
  primary on GDPR Article 22, CPPA ADMT privacy-notice
  surface, DPDPA / LGPD / PIPEDA / PIPL / UK GDPR statutory
  roles; head primary on EU AI Act Article 27 FRIA and on
  AI-specific supporting evidence. SAR handling is DPO-led
  with head-supported SLA.
- The AIA / DPIA co-authoring pattern is a six-step
  discipline — trigger, joint scoping, parallel authoring,
  cross-review, co-sign, registration — that produces
  consistent documents on the same system.
- Five anti-patterns to refuse: AIA-as-DPIA-plus, DPIA-as-
  AIA-substitute, ROPA lag, unilateral Article 22
  determination, SAR-orphan record.
- The interface document — co-signed by head and DPO — is
  ratified in the CxO adjacency map, reviewed annually at the
  audit committee, and defended jointly.
- Chapter [[04-cro-coordination]] turns to the risk
  adjacency — how the AI risk portfolio composes with the
  parent ERM framework and the head's reporting line into
  the CRO.

<!-- needs-research: verify the current effective status of
the CPPA ADMT (Automated Decisionmaking Technology)
regulations and any subsequent CPPA rulemakings on cyber-
security audits and risk assessments before citing specific
obligations. -->

<!-- needs-research: verify current implementation status of
India's DPDPA 2023, including whether the Data Protection
Rules have been notified and the Data Protection Board
constituted, before citing operational obligations. -->
