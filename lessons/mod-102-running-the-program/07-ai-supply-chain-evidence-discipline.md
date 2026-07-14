# The AI Supply-Chain Evidence Discipline at Program Scope

## Motivation

Most AI systems the enterprise operates are not entirely of the
enterprise's own making. Foundation models come from third-party
providers. Training data flows in from data marketplaces, open
datasets, and licensed sources. Fine-tuning artefacts are produced by
research teams and later promoted to production. Inference stacks run
on third-party GPU clouds under third-party frameworks. Retrieval
pipelines call vector stores and embedding services. Model-orchestration
platforms sit between all of it. Any single production AI system may
have twenty upstream components across a dozen suppliers.

A regulator's inspection under EU AI Act Chapter III, a sector
examiner's supply-chain review under SR 23-4, or an ISO/IEC 42001
certification body's Annex A control sampling around third-party
management, will all ask the same set of questions: for each
component, where did it come from? What is inside it? What is its
provenance? What license terms govern its use? What model, system,
or dataset card documents its behaviour and limitations? What was
the integrity of the build pipeline that produced it? What
attestations back the claims?

Supply-chain evidence is how the enterprise answers those questions.
The level-50 architect designed the evidence architecture (see
[[mod-101-role-scope-and-leadership-shape]] chapter 01) — the schema,
the tooling, the integration pattern. The head owns the *operating
discipline* at program scope: that the evidence is complete for
every in-scope system, current with every material change, and
defensible under regulator inspection.

This chapter is that discipline.

## Core concept: five artefact classes, one composition

The evidence architecture is built around five artefact classes,
each addressing a different question. The head reads them as a
composition, not as a menu.

- **CycloneDX ML-BOM.** The machine-learning software-bill-of-
  materials extension to CycloneDX. Enumerates every component of
  the AI system: model, training data, hyperparameters, framework
  versions, inference-runtime dependencies. Answers *what is
  inside*. Consumed by regulators, supply-chain risk teams, and
  ISO/IEC 42001 third-party control auditors.
- **SPDX 3.0 AI profile.** The Software Package Data Exchange
  standard's AI profile extension. A complementary specification
  emphasising license, provenance, and metadata. Answers *what is
  its provenance and license*. Consumed by procurement, legal, and
  open-source-license compliance teams; widely required in public-
  sector procurement.
- **SLSA attestations.** Supply-chain Levels for Software Artifacts
  framework attestations. Signed statements about how the artefact
  was built and what tampering-resistance the build pipeline
  provides (SLSA levels 1 through 4 in the current framework).
  Answers *what is the integrity of the build pipeline*. Consumed
  by security teams and regulators concerned with training-data
  provenance and build-time tampering.
- **Sigstore.** The infrastructure — cosign, Fulcio, Rekor — that
  makes SLSA and other attestations verifiable. Provides
  cryptographic signing of artefacts, a transparency log for
  attestations, and a keyless-signing workflow that integrates with
  enterprise identity providers. Answers *how are the attestations
  verifiable and non-repudiable*. Consumed by build systems, model
  registries, and post-deployment integrity monitors.
- **Model cards, system cards, dataset cards.** Human-readable
  documentation of a model's, system's, or dataset's intended use,
  limitations, evaluation results, and ethical considerations.
  Model Cards trace to Mitchell et al. 2019; System Cards emerged
  from Meta and OpenAI practice; Dataset Cards to the Datasheets
  for Datasets and Data Cards work at Google. Answers *what are
  the AI-specific behaviours, limits, and evaluation results*.
  Consumed by end-users, deployers, downstream governance
  functions, and regulators reviewing intended use.

The five compose. A defensible AI-system evidence bundle contains
ML-BOM (contents), SPDX AI (provenance and license), SLSA
attestations (build integrity), Sigstore-verifiable signatures, and
model / system / dataset cards (behavioural documentation). Missing
any class is a specific missing question; the head does not permit
sampling to expose it.

## Reading the architect's design

The level-50 architect specified: which tool produces each artefact
class in the enterprise, how it is published to the evidence store,
how it is keyed to the inventory (chapter 06) and the control library,
and what completeness bar applies per system tier.

The head must be able to answer, on any Tuesday morning, for each of
the five classes:

- Which tool the enterprise uses to produce the artefact.
- How the artefact is published (typically to an OSCAL-shaped
  evidence store or the GRC-for-AI platform).
- How the artefact is signed and verified (via Sigstore).
- How the artefact is refreshed on material change to the underlying
  system (via CI/CD triggers, retraining pipelines, or manual gates).
- What the completeness bar is per system tier (tier-1 systems
  require all five in full; tier-3 systems may accept lighter
  documentation on some classes with justification).

The architect's design is not the head's daily concern. Its
*operation* is.

## The completeness bar the head enforces

At program scope, the head enforces a specific completeness bar per
system tier. A typical bar the head defends at the council and the
audit committee:

- **Tier-1 (production customer-facing or regulatory-scope
  high-risk systems).** All five artefact classes at full depth.
  ML-BOM enumerates every component. SPDX AI profile carries
  license and provenance for every component. SLSA attestation at
  level 3 minimum with signed metadata. Sigstore signatures on all
  attestations, verifiable through the transparency log. Model,
  system, and dataset cards at the enterprise's most detailed
  template. Cards reviewed and re-attested annually or on material
  change.
- **Tier-2 (production internal-facing or non-high-risk external
  systems).** ML-BOM at full depth. SPDX AI profile at license-and-
  provenance depth. SLSA at level 2 minimum. Sigstore signatures on
  key attestations. Model card and system card at standard depth;
  dataset card at standard depth for training data owned by the
  enterprise, at inherited depth for third-party training data
  where the provider supplies a card.
- **Tier-3 (development, evaluation, or limited-use systems).**
  ML-BOM at core-components depth. SPDX AI profile at license-only
  depth. SLSA at level 1. Sigstore signatures where the tooling
  supports it. Model card at lightweight depth; system and dataset
  cards where materially relevant.

The head does not personally set the tiers; the level-50 architect
did, keyed to the risk taxonomy. The head enforces that every system
in the inventory (chapter 06) carries the tier tag, that the tag is
current, and that the evidence bundle meets or exceeds the tier's
completeness bar.

## The head's operating cadence for supply-chain evidence

Three cadences the head runs.

- **Continuous (per-change).** Every material change to an in-scope
  system — retraining, model version upgrade, dependency upgrade,
  data-source change, deployment configuration change — triggers a
  refresh of the affected artefact classes. Automated through CI/CD
  where possible; enforced through the AIMS operating discipline
  where automation is not yet complete.
- **Monthly (council).** The AI governance council (chapter 01)
  reviews evidence-bundle completeness metrics: which systems'
  bundles fell below the tier bar in the period, why, and the
  corrective actions. The council does not review individual
  systems' bundles at this cadence; it reviews the coverage
  dashboard.
- **Annual (walk-through).** As part of the annual AIMS calendar
  (chapter 02) and inventory walk-through (chapter 06), every
  in-scope system's bundle is sampled and any drift from the
  tier's completeness bar is remediated. The walk-through is the
  final catch for drift the continuous and monthly cadences
  missed.

## Third-party AI vendor discipline

The single largest supply-chain risk in AI is third-party dependence
on foundation-model providers, training-data licensors, and MLOps
platforms. The head runs a tiered third-party program specifically
for AI vendors, keyed to the enterprise's SR 23-4 or ISO/IEC 27036
third-party framework and specialised for AI-specific evidence.

The AI-vendor tiering and evidence expectation:

- **Tier-1 AI vendors (foundation model providers, model
  hosting, MLOps platforms where the enterprise's core AI
  capability depends on the vendor).** The vendor supplies:
  ML-BOM for the model version the enterprise consumes; the
  vendor's own SPDX AI profile carrying training-data provenance
  and licensing at the depth the vendor can share; SLSA
  attestation for the model's build pipeline (some frontier
  labs publish this under Responsible Scaling Policy / Preparedness
  Framework / Frontier Safety Framework disclosures); the vendor's
  model card, system card, and (where available) dataset card;
  ongoing evidence of the vendor's own governance posture
  (typically the vendor's ISO/IEC 42001 certification or NIST AI
  RMF adoption disclosure). The vendor's continuous-monitoring
  evidence — model behaviour changes, incident notifications,
  regulatory posture changes — is a contractual obligation with an
  SLA.
- **Tier-2 AI vendors (adjunct services — vector stores,
  embedding services, orchestration tooling, evaluation
  services).** Standard SBOM, security certifications (SOC 2, ISO
  27001), plus any AI-specific evidence the vendor supplies.
  Continuous monitoring at contractual notification cadence.
- **Tier-3 AI vendors (specialised or peripheral).** Standard
  vendor management under the enterprise procurement policy;
  AI-specific evidence where materially relevant.

The head owns the tiering discipline — which vendor is in which
tier, the criteria for reclassification, and the review cadence.
The evidence the vendor supplies is stored in the enterprise
evidence architecture keyed to the systems that consume the vendor
(chapter 06). When a vendor's evidence drifts from contractual
expectation — a model card that is not refreshed after a version
change, an ISO certification that expires without a plan for
renewal, an incident notification that arrives late — the drift is
opened as a non-conformity against the third-party program.

## Model-card and system-card authorship discipline

Model cards and system cards are the AI-specific artefact classes.
Their authorship discipline determines whether they are useful
governance artefacts or decorative documents.

The head enforces:

- **Templates the architect defined.** The enterprise's model-card
  and system-card templates are documented; every card follows the
  template; deviations require exception approval through the
  council. Templates typically include: intended use and out-of-
  scope use; training data description and characteristics;
  evaluation methodology and results per demographic slice where
  applicable; known limitations; ethical considerations; contact
  and versioning.
- **Authorship by named engineering roles.** The AI evaluation
  engineer (level 35) or the AI risk engineer (level 25) authors;
  the AI governance analyst (level 15) reviews for completeness;
  the head samples for depth. The card is not authored by product
  marketing.
- **Under document control.** Every card is versioned, timestamped,
  and retained under the AIMS document-control policy. Every
  material change to the underlying system produces a card
  revision.
- **Cross-referenced from the inventory (chapter 06).** Every
  inventory record's model-card pointer resolves to the current
  card version; historical versions remain accessible.

A model card that has not been refreshed since first authorship,
that is not aligned to the enterprise template, or that is authored
by a role without technical accountability for the model is exactly
the artefact a regulator will surface as evidence of decorative
governance.

## Composition with the AI system inventory (chapter 06)

The inventory (chapter 06) and the evidence bundle are
cross-referenced. Every inventory record lists pointers to its
ML-BOM, SPDX AI, SLSA attestation, Sigstore signature reference, and
its cards. Every artefact carries a back-pointer to the system(s) it
documents.

The head runs a monthly integrity check across the cross-references.
Common integrity failures:

- Inventory records whose ML-BOM pointer resolves to an ML-BOM for
  a prior model version (drift-from-current).
- Cards whose evaluation-results section refers to a model version
  no longer in production (retirement-not-tracked).
- SLSA attestations that were signed but never re-verified after
  a component upgrade (integrity-not-refreshed).
- Vendor-supplied evidence that has expired (contract-clock-drift).

Each is a non-conformity against the operating discipline. Ageing
failures escalate through the standard council mechanism (chapter
01).

## Coordination with the level-50 architect on schema changes

The evidence architecture is the architect's design (chapter 01,
mod-101). Schema changes — a new field on the ML-BOM, a new
attestation format, a change to the model-card template — are
proposed by the architect and executed by the head's operating
function.

The head's coordination discipline:

- **Change intake.** Architect-proposed schema changes are
  intake items on the AI governance council agenda. Impact on
  currently-populated evidence bundles is assessed before ratification.
- **Migration plan.** Approved changes carry a migration plan —
  which existing bundles must be refreshed, in what order, over
  what window. Materiality thresholds constrain the plan (tier-1
  bundles migrate first; tier-3 may migrate at next natural
  refresh).
- **Backward-compatibility window.** Bundles authored under the
  prior schema remain readable during a transition window; the
  evidence architecture is not brittle to change.
- **Feedback loop to the architect.** Where the operating
  discipline surfaces schema deficiencies — fields the tooling
  cannot populate, cross-references that consistently fail — the
  head feeds this back to the architect for design revision.

Under-coordination produces evidence-architecture drift that later
audits will surface. The head does not attempt to redesign the
schema locally.

## Composition with regulatory obligations

Supply-chain evidence obligations are pointed at by several
regulatory regimes the head must be able to name and defend against:

- **EU AI Act Chapter III (Articles 8–15).** High-risk system
  documentation, technical documentation (Annex IV), record-
  keeping (Article 12), transparency (Article 13). The supply-
  chain evidence bundle supplies the substance of the Annex IV
  technical documentation for high-risk systems the enterprise
  provides.
- **EU AI Act Chapter V — general-purpose AI models.** Article 53
  imposes obligations on GPAI-model providers including the
  technical documentation (Annex XI) and the copyright / training
  content summary (Article 53(1)(d)) — even providers not
  established in the EU whose models are placed on the EU market.
  The head coordinates with the level-50 architect on how the
  enterprise's own GPAI activity (if any) meets these; for
  procured GPAI, the head expects the provider to have discharged
  them.
- **NIST AI RMF MEASURE and MANAGE functions.** Supply-chain
  provenance is called out under MEASURE 2.10 and MANAGE 3.1; the
  ML-BOM and SPDX AI profile are how the enterprise evidences
  these.
- **NIST Cybersecurity Framework 2.0 GV.SC (Supply Chain Risk
  Management).** The CSF 2.0 GOVERN function added a supply-chain
  category in February 2024; AI supply-chain evidence composes
  under it for AI-security-adjacent controls.
- **CISA / NCSC Guidelines for Secure AI System Development.**
  The 2023 joint guidance emphasises supply-chain security for AI
  systems as a first-class concern.
- **Sector regimes.** SR 23-4 in banking, HIPAA covered-entity
  vendor management in health, NAIC AI Model Bulletin third-party
  expectations in insurance, GMLP predetermined-change-control-plan
  supply-chain expectations in medical devices, OMB M-25-21
  vendor-evidence expectations in the US federal government.

The head does not derive the composition; the level-50 architect's
crosswalk (chapter 01, mod-101) does that. The head defends the
composition at the audit committee.

## Example — an audit sample against the evidence bundle

A worked example of the operating discipline in action.

An ISO/IEC 42001 surveillance auditor requests a sample of five
in-scope AI systems' evidence bundles for review. The head's
audit-liaison (chapter 04) generates the sample from the inventory
(chapter 06) using a documented sampling method (stratified by
tier, biased toward tier-1 systems with recent material changes).

For each sampled system the auditor receives, from the evidence
architecture:

- The system's inventory record, at a fixed timestamp, exported to
  the auditor-preferred format.
- The current CycloneDX ML-BOM, Sigstore-signed and verifiable
  against the transparency log.
- The SPDX 3.0 AI profile, matching the ML-BOM's component list
  and adding license and provenance.
- The SLSA attestation for the current build, verifiable via
  Sigstore.
- The model card, system card, and (where applicable) dataset
  card at the current version, cross-referenced from the inventory
  record.
- The impact assessment reference and, if requested, the impact
  assessment itself.
- The relevant risk-register rows (chapter 03).

The auditor samples deeper on one of the five systems: verifies the
Sigstore signature on the ML-BOM independently, resolves the
ML-BOM's foundation-model component against the tier-1 AI vendor's
disclosed model card, and traces one training-data component to its
license under the SPDX AI profile.

No finding is generated because the bundle is complete, current,
signed, and cross-references resolve. The auditor's sample succeeds
on the surface. That is the goal.

## Common failure modes

- **Cards without cross-references.** Model cards that exist but are
  not linked from the inventory record and are not versioned under
  document control. The auditor cannot find them; effectively, they
  do not exist for evidence purposes.
- **Signed once, not re-verified.** Sigstore signatures generated at
  first build and never verified after subsequent component
  upgrades. The signature is stale; the integrity claim is not
  current.
- **Vendor evidence never refreshed.** Foundation-model vendor
  supplies a model card at contract signing; the model updates every
  few months; the enterprise never refreshes the card. The card is
  wrong within a quarter.
- **SLSA level claimed without evidence.** The enterprise's build
  pipeline is claimed at SLSA level 3, but the specific attestations
  are not present or not verifiable. The claim is a compliance
  liability.
- **ML-BOM as a list of names.** The ML-BOM lists component names
  but no versions, hashes, or dependencies. It does not
  reconstruct the actual build.

## Summary

- Supply-chain evidence composes five artefact classes — CycloneDX
  ML-BOM, SPDX 3.0 AI profile, SLSA attestations, Sigstore
  signatures, model / system / dataset cards — into a single
  audit-defensible bundle per in-scope AI system.
- The level-50 architect designed the evidence architecture,
  including the tools per class, the schema, and the tiered
  completeness bar. The head enforces the operating discipline
  that every in-scope system's bundle meets the tier bar and stays
  current.
- Three cadences run: per-change refresh triggered by CI/CD or
  manual gates; monthly council review of coverage metrics;
  annual walk-through as part of the AIMS calendar (chapter 02).
- Third-party AI vendors are tiered separately from software
  vendors; tier-1 AI vendors' evidence expectations include
  ML-BOM, SPDX AI, SLSA, cards, governance-posture certification,
  and contractual continuous notification.
- Model-card and system-card authorship follows the architect's
  template, is authored by named engineering roles, is under
  document control, and cross-references the inventory.
- Cross-reference integrity between the inventory (chapter 06)
  and the evidence bundle is checked monthly; drift is a
  non-conformity.
- Schema changes are initiated by the architect and executed by
  the head's operating function under a documented change-intake,
  migration-plan, and backward-compatibility discipline; the head
  does not redesign the schema locally.
- Regulatory composition (EU AI Act Chapters III and V, NIST AI
  RMF, NIST CSF 2.0 GV.SC, CISA / NCSC guidance, sector regimes)
  is defended at the audit committee; the architect owns the
  crosswalk.
