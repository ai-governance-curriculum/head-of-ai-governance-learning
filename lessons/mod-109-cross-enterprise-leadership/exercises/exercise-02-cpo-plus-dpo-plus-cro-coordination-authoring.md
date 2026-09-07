# exercise-02: CPO + DPO + CRO Coordination Authoring

**Estimated effort:** 4 hours

## Objective

Author the **privacy-and-risk-adjacency interface set** — one
document co-signed by the head and each of the Chief Privacy
Officer / DPO and the Chief Risk Officer — that operationalises
chapters [03-cpo-dpo-coordination](../03-cpo-dpo-coordination.md)
and [04-cro-coordination](../04-cro-coordination.md).
Deliverables are the two written interface documents plus the
composed AIA-into-DPIA template, the ROPA-integration mapping,
the jurisdictional-obligation split (GDPR, CPPA, DPDPA, and any
sector-specific rules the enterprise carries), the AI-risk-
appetite-tolerance-limit statement composed with the enterprise
risk register (ISO 31000, ISO/IEC 27005, COSO ERM), and the
reporting-line specification where the head reports into the
CRO.

The interface set has to survive three stress tests. First, a
regulator's data-protection examiner reads the composed
AIA-into-DPIA template and confirms it satisfies GDPR Article
35 DPIA requirements at the required scope — a composed
template that omits GDPR Article 35(7) required content fails
the test. Second, the CRO's second-line coordinator reads the
appetite-tolerance-limit statement and confirms it composes
with the enterprise's parent risk register at the CRO's
convention — an appetite statement in AI-only language that
does not translate to the enterprise register fails the test.
Third, the audit committee reads the reporting-line
specification and understands, without a briefing, how the
head's function reports up through the CRO and where the
head's independent audit-committee access is preserved — a
reporting-line spec that reads ambiguously on that invariant
fails the audit-committee readability standard.

## Prerequisites

- Chapter [03-cpo-dpo-coordination](../03-cpo-dpo-coordination.md)
  — the three coordination surfaces with the CPO / DPO
  (AIA / DPIA composition, ROPA interface, jurisdictional-
  obligation split), the interface-document structure, and
  the named anti-patterns.
- Chapter [04-cro-coordination](../04-cro-coordination.md)
  — the ERM composition, the appetite-tolerance-limit
  language, the reporting-line discipline, and the named
  anti-patterns.
- [[mod-101-role-scope-and-leadership-shape]] chapter 06
  (CxO adjacency map) and chapter 07 (engagement-contract
  discipline — where the audit-committee-access invariant
  is negotiated at hiring).
- [[mod-102-running-the-program]] chapter 03 (AI risk
  register), chapter 06 (AIMS inventory), chapter 07 (AIA
  discipline).
- Primary sources cited in `resources.md` — GDPR Articles
  25 and 35, EDPB Guidelines on DPIAs (WP248 rev.01), CPPA
  regulations, DPDPA notifications, ISO 31000:2018,
  ISO/IEC 27005, COSO ERM 2017, ISO/IEC 42001 clauses 6.1
  and 8.
- A concrete enterprise in mind — sector, jurisdictional
  footprint (EU / EEA scope, UK scope, US state-privacy-law
  scope including CCPA / CPRA and analogues, Indian DPDPA
  scope, other jurisdictions in operation), whether the
  enterprise has a distinct CPO and DPO or a combined role,
  whether the head reports solid-line to the CRO or under a
  matrixed arrangement, and the AI system portfolio's
  privacy sensitivity.

## Steps

1. **Enterprise context one-pager.** Author the half-page
   context: sector, jurisdictional footprint, whether the
   CPO and DPO roles are distinct or combined, current
   privacy governance framework (ISO 27701 alignment, the
   ROPA platform), current enterprise risk framework the
   CRO runs (COSO / ISO 31000 posture), current reporting-
   line the head has with the CRO (solid, matrixed, peer).
   Every subsequent artefact references this one-pager.

2. **The CPO / DPO interface document.** Author the co-
   signed interface document (8 to 12 pages) with the
   sections required by chapter 03:
   - Scope statement.
   - The three surfaces (AIA / DPIA composition, ROPA
     interface, jurisdictional-obligation split) each with
     artefacts, cadence, and joint owner.
   - The named jurisdictional-obligation table — for each
     jurisdiction in the enterprise's footprint, which
     obligations divide to the CPO / DPO's function, which
     divide to the head's function, and which are jointly
     owned.
   - Data-subject-rights interface for AI-in-scope systems
     (Article 22 automated decision-making, right to
     explanation, opt-out, and adjacent).
   - Personal-data-breach coordination (where the incident
     under [[mod-110-incident-leadership]] has a personal-
     data dimension).
   - Escalation ladder.
   - Joint annual audit-committee appearance.
   - Review cadence.

3. **The composed AIA-into-DPIA template.** Author the
   template every AI system with personal-data scope uses.
   The template composes:
   - The AIA content the head's function requires (impact
     assessment for the AI system across fairness, safety,
     security, and operational-suitability dimensions).
   - The DPIA content GDPR Article 35(7) requires
     (systematic description of processing operations and
     purposes; necessity and proportionality assessment;
     risks to rights and freedoms; measures to address
     risks).
   - The CPPA / CCPA / CPRA equivalent content where
     applicable.
   - The DPDPA equivalent content where applicable.
   The template is one document with sections cross-
   referenced to each source obligation, not two documents
   stapled together. The DPO's substantive approval and the
   head's substantive approval are named as separate sign-
   offs on the composed document.

4. **The ROPA-integration mapping.** Author the mapping
   between the AIMS inventory ([[mod-102-running-the-
   program]] chapter 06) and the enterprise ROPA (Record
   of Processing Activities). The mapping names:
   - For each AI system in scope for personal-data
     processing, the ROPA record it maps to (or the ROPA
     record that must be created if the AI system's
     processing is not yet ROPA-registered).
   - The AI-specific rows the ROPA carries (categories of
     data subjects, categories of personal data, purposes
     of processing, categories of recipients, transfer
     mechanisms) with the AI-specific detail (model
     training, evaluation-set usage, synthetic-data
     derivation, inference-time processing).
   - The freshness discipline — when the AIMS inventory
     changes for a personal-data-in-scope system, the ROPA
     updates within a named window (typically 30 days per
     the enterprise's ROPA-maintenance discipline).

5. **The jurisdictional-obligation split.** Author the
   named table — one row per jurisdiction in the
   enterprise's footprint — with the following columns:
   - Jurisdiction (EU / EEA, UK, California, other US
     states in scope, India, other jurisdictions).
   - Primary obligation source (GDPR, UK GDPR + DPA 2018,
     CCPA / CPRA / CPPA regulations, DPDPA and forthcoming
     regulations, other).
   - Head-owned obligations (AI-specific requirements,
     evaluation and fairness testing where the obligation
     names AI systems).
   - CPO / DPO-owned obligations (data-protection
     principles at parent scope, DSAR handling, breach
     notification, ROPA maintenance).
   - Jointly-owned obligations (AIA / DPIA when personal
     data is in scope, cross-border transfer mechanisms
     for AI training data, algorithmic decision-making
     disclosures under Article 22 or CPRA equivalent).

6. **The CRO interface document.** Author the co-signed
   interface document (6 to 10 pages) with the sections
   required by chapter 04:
   - Scope statement.
   - The AI risk register's composition into the enterprise
     risk register (ISO 31000 / ISO/IEC 27005 / COSO ERM
     vocabulary).
   - The appetite-tolerance-limit statement (see step 7).
   - The reporting-line specification (see step 8).
   - Material-event escalation.
   - Preserved audit-committee-access invariant
     ([[mod-101-role-scope-and-leadership-shape]] chapter
     07).
   - Joint annual audit-committee appearance.
   - Review cadence.

7. **The AI-risk-appetite-tolerance-limit statement.**
   Author the statement in the CRO's vocabulary — appetite
   (the level of AI risk the enterprise is willing to
   accept in pursuit of its strategy), tolerance (the
   boundary at which management action is triggered), limit
   (the boundary at which board escalation is required).
   For each named AI-risk dimension (safety, fairness,
   security, privacy, operational, regulatory, reputational),
   the statement names:
   - The appetite qualitatively and, where quantifiable,
     quantitatively.
   - The tolerance threshold (in KRI terms — see
     [[mod-107-program-measurement-and-maturity]] chapter
     01 for the KRI portfolio).
   - The limit threshold and the board-escalation trigger.
   - The current position of the AI portfolio against each
     threshold, as of the interface-set publication date.

8. **The reporting-line specification.** Author the specific
   reporting-line arrangement — solid-line, matrixed, or peer
   — between the head and the CRO. The specification names:
   - Whether solid-line to CRO or matrixed (with the primary
     solid-line specified).
   - The material-event escalation path from the head to the
     audit committee via the CRO's line.
   - The preserved independent audit-committee access on
     second-line-material events (independence-impairment
     attempts, retaliation concerns, material dissent on
     risk matters the CRO does not escalate).
   - The performance-review arrangement (who authors the
     head's performance review; who inputs).
   - The engagement-contract cross-reference to
     [[mod-101-role-scope-and-leadership-shape]] chapter 07.

9. **The failure-mode audit.** Author a short section — one
   paragraph per failure mode — naming how the interface set
   detects and recovers from each of the named anti-
   patterns across chapters 03 and 04 (typically five to
   seven modes total: parallel AIA / DPIA, ROPA drift,
   jurisdictional-obligation gap, AI-risk register outside
   the enterprise register, appetite-tolerance-limit
   language mismatch, reporting-line bypass, and the
   invariant misused as a routine lever).

## Deliverables

- `enterprise-context.md` — the half-page context one-pager.
- `interface-cpo-dpo.md` — the co-signed CPO / DPO interface
  document.
- `aia-dpia-template.md` — the composed AIA-into-DPIA template.
- `ropa-integration-mapping.md` — the AIMS-to-ROPA mapping.
- `jurisdictional-obligation-table.md` — the per-jurisdiction
  obligation split.
- `interface-cro.md` — the co-signed CRO interface document.
- `appetite-tolerance-limit.md` — the AI-risk appetite,
  tolerance, and limit statement in the CRO's vocabulary.
- `reporting-line-specification.md` — the reporting-line
  arrangement with the audit-committee-access invariant.
- `failure-mode-audit.md` — the failure-mode detection-and-
  recovery paragraphs.

## Acceptance criteria

- The composed AIA-into-DPIA template covers every element
  GDPR Article 35(7) requires, every element the CPPA / CPRA
  equivalent requires (where in scope), every element the
  DPDPA equivalent requires (where in scope), and every
  element the AIA requires. A missing element fails the
  criterion.
- The ROPA-integration mapping has an entry for every AIMS-
  inventoried AI system with personal-data scope; systems
  without a mapped ROPA record are flagged with a scheduled
  registration action. A missing entry fails the criterion.
- The jurisdictional-obligation table has a row for every
  jurisdiction in the enterprise's footprint and every row
  has all four columns (jurisdiction, obligation source,
  head-owned, CPO / DPO-owned, jointly-owned) populated. A
  jurisdiction missing or a row with unpopulated columns
  fails the criterion.
- The appetite-tolerance-limit statement covers every
  named AI-risk dimension (safety, fairness, security,
  privacy, operational, regulatory, reputational) and every
  dimension has appetite, tolerance, and limit specified. A
  dimension with an unspecified threshold fails the
  criterion.
- The reporting-line specification names the arrangement
  (solid-line, matrixed, peer), names the material-event
  escalation path, and names the preserved audit-committee-
  access invariant explicitly. Ambiguous language on the
  invariant fails the criterion.
- Any factual claim about a specific jurisdiction's
  obligation, a specific regulator's interpretation, or a
  specific standard's requirement carries a
  `<!-- needs-research: verify [specific fact] against
  [official source] -->` marker where not verifiable from
  the cited primary sources.

## Stretch goals

- Extend the deliverable with a **cross-border-transfer
  addendum** — where the enterprise's AI systems involve
  training data or inference-time processing crossing
  jurisdictional boundaries, the specific transfer
  mechanism (SCCs under the EU Commission's 2021 decision,
  UK IDTA, other jurisdictional equivalents) and the
  transfer-impact assessment posture the enterprise has
  adopted, co-authored with GC (chapter [[06-general-
  counsel-coordination]]).
- Author the **jurisdictional-obligation delta tracker** —
  where the horizon-scanning discipline from
  [[mod-105-regulatory-change-management]] surfaces a
  material change (a new US state law, an EU
  implementing act, a DPDPA rule publication), how the
  interface set updates.
- Draft the **rehearsed Article-22 request scenario** — a
  data subject exercises the Article 22 right to human
  review of an AI-driven decision. Walk the interface's
  data-subject-rights coordination from inbound to
  resolution.
- Draft the **appetite-breach rehearsal** — the KRI
  portfolio shows an AI-risk dimension crossing the
  tolerance threshold on a specific system. Walk the
  interface's material-event escalation to the CRO and,
  where required, to the audit committee.
- Author the **onboarding brief** the head hands to a newly-
  appointed DPO or CRO at their first working session,
  summarising the interface set and where the head's
  function's current program lands against it.

## Notes and starter guidance

The most common first-cut failure on this exercise is the
composed AIA-into-DPIA template that reads as two documents
stapled together. The composition works when the AI-scope
sections and the personal-data-scope sections cross-
reference each other and the reader can follow a single
narrative through the assessment; it fails when the AIA and
the DPIA sit adjacent without composition. Force the
composition — some sections will map one-to-one, others will
compose, and some will be AI-specific extensions to the DPIA
skeleton. Name the composition explicitly.

The second common failure is the appetite-tolerance-limit
statement written in AI-governance-only vocabulary. The CRO
reads the statement against the enterprise's parent risk
register; if the AI statement uses "fairness KPI at threshold
X" without translating to appetite / tolerance / limit
vocabulary, the composition breaks. Force the translation
into the CRO's language even where the underlying metric is
AI-specific.

The third common failure is the reporting-line specification
that is ambiguous on the audit-committee-access invariant.
The invariant is load-bearing: it is the escape valve that
lets the head raise a material second-line concern the CRO
does not escalate. A specification that says "the head
reports up through the CRO on all matters" and does not name
the invariant fails the head's own engagement-contract
discipline. Force the invariant into the spec explicitly,
even where the CRO reads it as an implicit constraint on
the reporting line.

On the jurisdictional-obligation table — the temptation is
to assign every AI-adjacent obligation to the head. Do not.
Many privacy obligations (breach notification, DSAR handling,
ROPA maintenance) sit with the CPO / DPO at parent scope and
the head extends only where the AI system's specifics
require. Force the split honestly; head-owned means "head is
accountable executive", not "head participates".

The interface set is a governance artefact. Version it, date
it, refresh it annually, and distribute the current version
to the CPO, DPO, CRO, CAE, GC, and audit-committee
secretariat.
