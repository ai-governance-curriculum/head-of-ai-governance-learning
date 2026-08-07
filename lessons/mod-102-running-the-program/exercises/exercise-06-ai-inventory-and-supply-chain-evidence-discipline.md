# exercise-06: AI Inventory and Supply-Chain Evidence Discipline

**Estimated effort:** 3 hours

## Objective

Produce a paired **AI system inventory operating handbook** and
**AI supply-chain evidence completeness bar** that together stand
up to an ISO/IEC 42001 certification body's Annex A control sampling
under ISO/IEC 42006, an EU AI Act inspection of Article 60
registration data and Article 72 post-market monitoring, and a
sector examiner's supply-chain review. The deliverables are not the
inventory schema or the evidence architecture — the level-50
architect designed both. The deliverables are the *operating
discipline* the head runs on top of the schema and the completeness
bar the head defends: intake gates, refresh cadences, quality-bar
enforcement per system tier, cross-reference integrity checks, and
a shadow-discovery non-conformity worked example.

## Prerequisites

- Chapter [06-ai-system-inventory-quality-bar](../06-ai-system-inventory-quality-bar.md)
  read and internalised.
- Chapter [07-ai-supply-chain-evidence-discipline](../07-ai-supply-chain-evidence-discipline.md)
  read and internalised.
- Chapter [02-aims-operating-calendar](../02-aims-operating-calendar.md)
  — the annual inventory walk-through and the coverage-metric
  review land on the AIMS calendar.
- Chapter [03-portfolio-risk-register-cadence](../03-portfolio-risk-register-cadence.md)
  — the inventory and register cross-reference each other; the
  reconciliation cadence composes with the register cadence.
- Familiarity with the CycloneDX ML-BOM specification, the SPDX
  3.0 AI profile, the SLSA framework's build-integrity levels, the
  Sigstore signing-and-transparency-log stack, and the Model Cards
  / System Cards / Dataset Cards literature, at the vocabulary
  depth chapter 07 assumes.
- Assumed enterprise from the prior exercises with an assumed
  sector and an assumed EU-provider posture (the enterprise
  provides high-risk AI systems in the EU under Article 16 / places
  systems in the EU as a deployer under Article 26 / neither).

## Steps

1. **In-scope definition and exclusion register.** Author the
   inventory's in-scope definition specialised to your assumed
   enterprise. Include the four inclusion bullets from chapter 06
   (learned parameters / procured AI services / research past the
   research boundary / AI-adjacent trusted decisioning) and the
   three exclusion patterns (classical MRM per SR 11-7 scope
   carve-out, rule-based systems, personal-productivity usage
   under acceptable-use). Include an exclusion register recording
   at least three specific systems the head has excluded, with the
   documented reasoning a regulator can read.
2. **Intake-gate discipline.** Author the operating discipline for
   the three intake channels (engineering, procurement, research)
   plus the shadow-discovery channel. Per channel: the gate event,
   the first-line owner enforcing it, the second-line owner
   verifying it, the minimum fields populated at intake, and the
   fields populated over the lifecycle. For shadow discovery,
   name the non-conformity classification (chapter 02), the root-
   cause analysis required, and the escalation to the council
   (chapter 01) if the same business unit produces repeat shadow
   discoveries.
3. **Refresh-cadence matrix.** Author the refresh-cadence matrix
   with four rows (event-driven, quarterly attestation, annual
   walk-through, regulator-triggered) and, per row: what
   triggers a refresh, what the refresh covers, who owns
   execution, who verifies completion, and what the retained
   evidence looks like. Cross-reference to the AIMS calendar
   (chapter 02) so annual walk-through lands on a named anchor.
4. **Tier-and-completeness-bar table.** Author the tier-and-
   completeness-bar table combining chapter 06's inventory
   tiering with chapter 07's supply-chain evidence tiering.
   Rows are system tiers (tier-1 production customer-facing or
   regulatory-high-risk / tier-2 production internal or
   non-high-risk / tier-3 development or limited-use). Columns
   are: required inventory fields at schema depth, required
   evidence artefacts (ML-BOM, SPDX AI, SLSA level, Sigstore
   signature scope, model card, system card, dataset card),
   card-refresh cadence, and third-party evidence expectations.
   The bar is what the head defends at the audit committee.
5. **Cross-reference integrity check.** Author the monthly
   cross-reference integrity check the head runs between the
   inventory and the evidence bundles (chapter 07). Enumerate
   the four common integrity failures from chapter 07 (ML-BOM
   pointer resolves to prior model version; card evaluation
   results refer to retired version; SLSA attestation not
   re-verified after component upgrade; vendor evidence
   expired) and, for each, the automated check that surfaces
   it, the ageing threshold at which it becomes a
   non-conformity, and the escalation path.
6. **Third-party AI vendor tiering and evidence expectation.**
   Author the AI-specific vendor tiering (tier-1 foundation-model
   provider / model hosting / MLOps core; tier-2 adjunct
   services; tier-3 specialised) and, per tier, the evidence
   the vendor supplies, the contractual continuous-notification
   SLA, and the drift-to-non-conformity trigger. Reference the
   parent third-party framework (SR 23-4 or ISO/IEC 27036) the
   enterprise operates.
7. **Shadow-discovery worked example.** Author a minute-shaped
   worked example following the chapter 06 example structure:
   a specific shadow-discovery incident (invent a plausible one
   for your assumed enterprise — a procurement bypass on a
   customer-service chatbot, a research promotion without
   intake, a business-unit-scoped procurement of a vendor AI
   service, or similar), the incident triage that surfaces it,
   the retroactive inventory intake, the non-conformity opened
   against the failed gate, the council review (chapter 01),
   and the audit-committee brief that follows. The example is
   defensible under sampling six months later.
8. **Article 60 / Article 72 / Article 73 composition note.**
   Write a half-page note on how the inventory feeds EU AI Act
   Article 60 high-risk system registration, Article 72 post-
   market monitoring, and Article 73 serious-incident reporting.
   Name the specific inventory fields each obligation reads
   from, the state tracking for Article 60 registrations
   (submitted / live / updated / suspended), and the incident-
   classification cadence for Article 73. If your assumed
   enterprise has neither provider nor deployer status in the
   EU, write instead about the sector-equivalent registration
   or reporting regime (SR 11-7 model inventory expectations,
   NAIC AI Model Bulletin filings, FDA GMLP post-market
   surveillance, OMB M-25-21 use-case inventory, or others).
9. **Coordination-with-the-architect note.** Write a half-page
   note describing the discipline for coordinating schema
   changes and evidence-architecture changes back to the
   level-50 architect (chapter 07's coordination discipline
   section). Name: how change requests land on the council
   agenda (chapter 01), the migration plan the architect
   supplies, the backward-compatibility window, and how the
   head's operating experience feeds back to the architect for
   design revision.

## Deliverables

- `in-scope-definition-and-exclusion-register.md` — the definition
  and the three-item exclusion register with documented reasoning.
- `intake-gate-discipline.md` — the four-channel intake discipline
  with per-channel owners and shadow-discovery escalation.
- `refresh-cadence-matrix.md` — the four-row refresh matrix keyed
  to the AIMS calendar.
- `tier-and-completeness-bar-table.md` — the tier-by-artefact
  completeness bar defensible at the audit committee.
- `cross-reference-integrity-check.md` — the monthly integrity
  check with per-failure automated check, ageing threshold, and
  escalation.
- `third-party-ai-vendor-tiering.md` — the AI-vendor tiering with
  per-tier evidence and SLA expectations.
- `shadow-discovery-worked-example.md` — the minute-shaped worked
  example running through triage, retroactive intake, non-
  conformity, council, and audit-committee brief.
- `article-60-72-73-composition.md` (or sector-equivalent) — the
  half-page EU AI Act (or sector) composition note.
- `architect-coordination-note.md` — the half-page coordination
  discipline note.

## Acceptance criteria

- The in-scope definition names both what is included and what is
  explicitly excluded, with the exclusion register giving at
  least three specific systems the head has excluded and the
  documented reasoning.
- All four intake channels (engineering, procurement, research,
  shadow-discovery) are covered with a first-line owner and a
  second-line verifier per channel.
- Shadow discovery is classified as a non-conformity with root-
  cause analysis and council escalation on repeat pattern.
- The refresh-cadence matrix cross-references at least one named
  AIMS calendar anchor from chapter 02 for the annual walk-through.
- The tier-and-completeness-bar table specifies all five evidence
  artefact classes (ML-BOM, SPDX AI, SLSA, Sigstore, cards) per
  tier at the depth chapter 07 defines.
- The cross-reference integrity check has an automated surfacing
  method per failure type — not a manual review.
- The vendor tiering names named foundation-model or MLOps
  provider archetypes at tier-1 and requires ML-BOM, SPDX AI,
  SLSA attestation, cards, and governance-posture certification
  from them; not a generic security questionnaire.
- The shadow-discovery worked example is defensible under sampling
  six months later — the retroactive inventory intake, the
  non-conformity plan, and the audit-committee brief are
  reconstructible from the artefact alone.
- The composition note names the specific inventory fields each
  obligation reads from — not a promise to determine them later.
- The coordination note preserves the architect's design
  ownership; the head does not redesign the schema locally.

## Stretch goals

- Author the inventory schema as a machine-readable JSON schema
  (or as an extension to the level-50 architect's schema in
  YAML) so the GRC-for-AI platform the architect selected can
  import it directly. Include controlled-vocabulary enumerations
  for lifecycle stage, regulatory classification, and tier.
- Author the OSCAL profile the inventory exports to for control-
  mapping evidence, keyed to at least one control area per
  ISO/IEC 42001 Annex A cluster.
- Draft the specific automated check the head runs across the
  inventory and evidence store to detect stale cross-references
  (ML-BOM pointer resolving to a deleted document, model card
  referencing a retired model version, SLSA attestation not
  refreshed after a dependency upgrade). Pseudocode or a
  runnable script is acceptable.
- Extend the third-party vendor section with a worked example of
  a vendor evidence drift — a foundation-model provider ships a
  new model version and does not refresh the model card within
  the contractual window — and the non-conformity, remediation,
  and re-tier decision that follows.
- Draft the EU AI Act Article 60 registration extract format
  (which inventory fields become which registration fields, in
  what shape) and the state-tracking dashboard the head runs
  against Article 60 status.
- Extend the shadow-discovery worked example into a corrective-
  action pattern library the enterprise adds to when repeat
  patterns emerge (procurement-bypass patterns, research-
  promotion patterns, business-unit-scoped patterns).

## Notes and starter guidance

- The single most damning finding an auditor can produce against
  the inventory is a shadow system surfaced during the audit
  itself. If your intake discipline does not include a real
  shadow-discovery channel with real teeth, revise. Chapter 06
  on the fourth channel is the discipline.
- Beware the temptation to treat the completeness bar as
  aspirational. The bar is what the head defends at the audit
  committee *today*, not what the head hopes to defend once
  tooling catches up. If the bar exceeds what the enterprise
  actually produces, either write in a specific tooling
  investment (feeding into the maturity trajectory from
  exercise 05) or lower the bar honestly.
- The cross-reference integrity check must be automated to be
  credible. Manual quarterly reviews miss drift the
  ageing-in-the-middle-of-a-quarter systems produce. Chapter 07
  on the four common integrity failures gives the exact checks
  to automate.
- The shadow-discovery worked example is where the pack becomes
  real. If the example does not include a council review and a
  non-conformity plan, the pack under-authors the head's own
  discipline. Chapter 06's worked example is the shape.
- Coordinate the tiering with the level-50 architect's risk
  taxonomy and the tiering in the register (chapter 03). If the
  inventory tier and the register tier and the evidence tier
  drift out of alignment, the operating discipline is silently
  incoherent. A single tier definition, cross-referenced from
  three places, is defensible.
- Sample-test the pack by asking: if an ISO/IEC 42006 auditor
  sampled five inventory records tomorrow and followed the
  cross-references from each, would every ML-BOM, SPDX AI
  profile, SLSA attestation, Sigstore signature, and card
  pointer resolve to a live current artefact? If not, the pack
  is under-authored — either the bar is too high, the intake is
  too loose, or the integrity check is too infrequent.
