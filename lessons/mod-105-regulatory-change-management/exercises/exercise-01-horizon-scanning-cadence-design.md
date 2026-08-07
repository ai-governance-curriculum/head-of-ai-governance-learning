# exercise-01: Horizon Scanning Cadence Design

**Estimated effort:** 2 hours

## Objective

Author the enterprise **horizon-scanning system design** the head
would defend under a certification-body audit (ISO/IEC 42006) and
under an NCA information-request on why the enterprise did — or did
not — act on a specific obligation. The design has the four
components chapter 01 names — sources, cadence, escalation, memory —
each with an owner, a specific rule set, and an artefact.

The deliverable is not a study note about chapter 01. It is the
document the head hands to the level-15 analyst desk on day one, the
document the annual scanning-system audit tests against, and the
document a delegate reads to cover the head during a two-week
absence. If the design cannot be executed by an analyst who has
never met the head, the design is under-authored.

The design has to survive two stress tests. First, an NCA arrives on
day one of an enforcement enquiry and asks why the enterprise did
not act on an obligation the desk had visibility on for six months.
The register memory has to answer. Second, a new head walks in on
day zero and has to run scanning from week one. The written system
has to onboard them.

## Prerequisites

- Chapter [01](../01-horizon-scanning-cadence.md) —
  the four-component scanning system and the three-tier triage
  vocabulary (watch / active / priority) — read and internalised.
- [[mod-102-running-the-program]] — the AIMS operating calendar
  (chapter 02), the risk register cadence (chapter 03), and the AI
  system inventory (chapter 06). Scanning outputs feed all three.
- [[mod-108-leading-the-governance-function]] — chapters 01 and 02
  cover the level-15 analyst hire and the tracking desk
  responsibilities the design assumes. If the enterprise has not
  yet hired the analyst, note this in the design as a staffing
  precondition, not as a design compromise.
- [[mod-104-regulator-engagement]] chapter 07 — the engagement-
  versus-legal-opinion boundary the scanning system respects (the
  system produces preparation, not legal opinions).
- A concrete enterprise in mind — sector (banking, insurance,
  health / medical device, pharma, public sector, frontier lab,
  tech platform, industrial), jurisdictional footprint across at
  least three regulatory geographies (EU, US federal, at least two
  US states, and at least one non-US non-EU jurisdiction), and an
  in-scope AI system count large enough that scanning matters (a
  five-system portfolio does not need this system; a fifty-system
  portfolio does).

## Steps

1. **Enterprise context one-pager.** Author the half-page context
   the design will operate against: sector, jurisdictional
   footprint, in-scope AI system portfolio size and shape (Annex
   III categories where relevant, GPAI exposure, high-risk sector
   overlays), the current level-15 analyst headcount and the
   current architect (level 50) capacity. Every subsequent
   artefact refers back to this one-pager.
2. **Source list — category shape and per-source ownership.**
   Author the source universe under the category shape chapter 01
   walks (Union / international, national horizontal, US state,
   sector, cyber, voluntary code / standards, non-US-non-EU
   national). For each source: URL or citation channel, owner on
   the level-15 desk, read frequency (daily wire, weekly digest,
   monthly, quarterly), and inclusion rationale. Where a source
   is on the list because chapter 01 names it (e.g. EU AI Office,
   OJEU, US AISI / NIST, CEN-CENELEC JTC 21) mark it as canonical.
   Where a source is on the list because the enterprise's sector
   or footprint drives it (e.g. a specific Member-State NCA, a
   state DOI where the enterprise writes insurance, PMDA because
   the enterprise sells devices into Japan), mark it as
   enterprise-specific and cite the enterprise-context rationale.
   Where a source's current status is uncertain, use
   `<!-- needs-research: verify [source] current publication
   channel / mandate / responsible authority against [official
   registry] -->` — do not guess and do not skip.
3. **Cadence — the four loops.** Author the four loops chapter 01
   names, each as a specific meeting or artefact:
   - **Daily wire.** Owner, format, delivery mechanism, retention.
     The head does not read the daily wire — the design specifies
     who does and what the desk owner does with items that meet
     the fast-loop-to-weekly-digest promotion rule.
   - **Weekly digest.** Owner, delivery day, delivery mechanism,
     the five-section rigid shape (new obligations, new drafts,
     new guidance, new enforcement, new standards), the three
     per-item fields (what / source / preliminary triage), and
     the head's 15-minute read discipline.
   - **Monthly portfolio review.** Attendees (head, desk lead,
     level-50 architect), agenda template, decision-record
     artefact, escalation to the AI governance council when
     needed.
   - **Quarterly deep scan.** Scope (source-drift detection, add
     / retire sources, forward-look brief for the CxO layer),
     agenda, decision-record artefact, feed into the annual audit
     scope.
   Include the **annual scanning-system audit** as a fifth
   discrete artefact: scope, owner (third-line audit under
   [[mod-108-leading-the-governance-function]] chapter 05),
   deliverable, feed into the annual maturity assessment
   ([[mod-107-program-measurement-and-maturity]] chapter 03).
4. **Escalation rules — the promotion criteria.** Author the
   promotion rules that move an item across watch → active →
   priority. Start from the six rules chapter 01 defends (final
   rule with compliance date within twelve months; attachment
   breadth crossing a named portfolio threshold; formal NCA
   correspondence; peer enforcement with a matching facts
   pattern; OJEU citation of a harmonised standard creating a
   presumption of conformity; Article 73 precedent shifting the
   reasonable interpretation of "serious"). Extend where the
   enterprise's sector or footprint demands (e.g. a state DOI
   adopting the NAIC AI Model Bulletin for an insurer footprint;
   a CFPB circular changing adverse-action posture for a lender
   footprint). For each rule, name: the trigger, the promotion
   destination (active vs priority), the SLA that then applies
   (chapter 02 step 1 — 30 days active, 14 days priority), and
   the owner who executes the promotion at the weekly digest read.
5. **Memory register — schema and retention.** Author the
   register schema: item identifier, source citation, first-seen
   timestamp, triage history (with reason for each promotion or
   demotion), owner, disposition (interpretation output reference,
   change-management plan reference, or archived-at-watch
   rationale), and cross-reference to the level-50 architect's
   crosswalk. Name the storage location — the register lives in
   the GRC-for-AI stack, not on the head's laptop. Name the
   retention posture (retain for the enterprise's document-
   retention default plus any regulator-specific longer horizon,
   e.g. Article 18 AI Act ten-year technical-documentation
   retention where relevant). Name the access-control posture
   (read-only for the enterprise; write for the analyst desk and
   the head; audit-visible to the third line and to external
   auditors under NDA).
6. **Coordination interface — the analyst desk and GC.** Author
   the two coordination contracts:
   - **With the level-15 analyst desk.** Name the desk lead, the
     specific expectations (own the source list execution, run
     the daily wire, produce the weekly digest, maintain the
     register, run preliminary triage), the escalation SLA for
     items that cross the priority threshold between weekly
     digests, the review cadence for the desk lead's performance
     ([[mod-108-leading-the-governance-function]] chapter 02).
   - **With GC.** Name the boundary — the scanning system
     produces preparation, not legal opinion; the vocabulary
     stays on the program-management side (watch / active /
     priority; scheduled / in-progress / disposed) not the
     legal-conclusion side (compliant / non-compliant). Name the
     hand-off point — items that reach interpretation (chapter
     02) are packaged for GC, GC opines. Cite
     [[mod-104-regulator-engagement]] chapter 07 as the
     controlling boundary discipline.
7. **Failure-mode audit.** Author a short section — one paragraph
   per failure — naming how the design detects and recovers from
   each of the four component failures chapter 01 names:
   - A source category has no owner or has a stale owner.
   - The cadence's monthly review has stopped running for a
     quarter or more.
   - Escalation rules have not fired on an item that later turned
     out to warrant priority.
   - The register memory has gaps for a specific quarter.
   The section is the head's own operating checklist — how the
   head, at the annual scanning-system audit, tests each component
   for degradation.

## Deliverables

- `enterprise-context.md` — the half-page scenario one-pager.
- `source-list.md` — the categorised source universe with owner,
  frequency, inclusion rationale, and needs-research markers.
- `cadence.md` — the four loops (daily wire, weekly digest,
  monthly portfolio review, quarterly deep scan) plus the annual
  scanning-system audit, each with attendees / agenda / artefact /
  decision-record.
- `escalation-rules.md` — the promotion rules from watch → active
  → priority, each with trigger, destination, SLA, owner.
- `memory-register.md` — the register schema, storage location,
  retention posture, access control.
- `coordination-contracts.md` — the analyst-desk contract and the
  GC-boundary contract.
- `failure-mode-audit.md` — the detection-and-recovery paragraphs
  for each of the four component failures.

## Acceptance criteria

- Every source in the source list has a named owner (a role or
  named person, not "the desk") and a specific frequency, not
  "as needed" or "regularly".
- Sources from outside the head's knowledge cutoff, or where the
  publication channel or mandate is uncertain, carry a
  `<!-- needs-research: ... -->` marker naming the specific fact
  and the official registry to verify against. No source is
  guessed.
- The weekly digest section of `cadence.md` names the five rigid
  sections (new obligations, new drafts, new guidance, new
  enforcement, new standards) and the three per-item fields
  (what / source / preliminary triage). A digest produced against
  this design is testable against the shape.
- Every escalation rule has a trigger, a destination tier, an
  SLA that then applies, and a named owner who executes the
  promotion. No rule is left as "the desk decides."
- The register schema includes fields for triage history (with
  reasons), disposition, and crosswalk cross-reference. A
  register produced against this schema can answer "why did the
  enterprise not act on obligation X" for any archived-at-watch
  item.
- The coordination contracts explicitly cite
  [[mod-104-regulator-engagement]] chapter 07 for the GC
  boundary and use program-management vocabulary (watch / active
  / priority; scheduled / in-progress / disposed) for scanning
  outputs. No output is labelled "compliant" or "non-compliant".
- The failure-mode audit names, for each of the four components,
  at least one specific signal the head monitors and at least
  one recovery action the head takes when the signal fires.

## Stretch goals

- Author the **first month of weekly digests** for the scenario,
  populated from actual current-window items (EU AI Office
  publications, JTC 21 progress, US AISI / NIST publications, one
  US state AG action, one sector-regulator publication in the
  enterprise's sector). Mark each item with the preliminary
  triage the desk would produce. The stretch goal is calibration
  — does the head's discipline against the design produce triage
  that matches what the head would expect on hindsight review?
- Draft the **onboarding brief** for a new level-15 analyst
  starting on the desk. The brief is the design document plus a
  scenario-specific first-90-days plan (weeks 1–4 shadow, weeks
  5–8 own the weekly digest under review, weeks 9–12 present at
  the monthly portfolio review). The scanning system is only as
  strong as the desk's onboarding.
- Author the **third-line audit programme** for the annual
  scanning-system audit — the specific evidence samples the
  auditor pulls, the acceptance criteria for each component, the
  reporting format. Coordinated with the CAE
  ([[mod-108-leading-the-governance-function]] chapter 05).
- Extend the design with the **cross-crosswalk trace** — how a
  register entry links to the level-50 architect's control-
  library update ([[mod-102-running-the-program]] chapter 04). A
  register that cannot trace to the crosswalk cannot answer the
  "did this obligation land in operating controls" question at
  audit.

## Notes and starter guidance

The most common first-cut failure is a source list that reads as
"we monitor the EU AI Office, NIST, state AGs, and sector
regulators" — a list of categories, not a list of sources with
owners and frequencies. Force the design to be executable by an
analyst who has never met the enterprise. If a category entry does
not name a URL or a citation channel, the desk cannot execute it.

The second common failure is over-designing the daily wire and
under-designing the weekly digest. The daily wire is the desk's
own tool; the head does not read it. The weekly digest is the
head's operational awareness. The digest's five-section shape is
what makes the head's 15-minute read possible; the design has to
enforce the shape or the digest becomes prose the head does not
finish.

On the memory register — resist the pull to design a rich
taxonomy the desk cannot maintain. A register with fifteen fields
per item is a register the desk will keep in seven of them. A
register with six fields that are always filled is a register
that answers the audit question. The chapter 01 schema (item,
source, first-seen, triage history, owner, disposition,
crosswalk cross-reference) is the working floor.

On coordination — the analyst desk contract is the artefact that
turns a role description into an operating contract. Without it,
the desk drifts, the head backfills, and the design silently
fails. Write the contract as the head would defend it to the CHRO
if the desk lead pushed back on the workload — specific,
bounded, matched to the level-15 job description
([[mod-108-leading-the-governance-function]] chapter 02).

On the GC boundary — every scanning system that has failed at
audit has failed the same way: the desk started drafting
compliance conclusions in weekly digest language, GC never saw
them, and a regulator later cited the desk's language as the
enterprise's position. The vocabulary discipline is not
pedantic. Keep the scanning system in program-management
vocabulary. Handoff to interpretation (chapter 02) is where the
enterprise starts talking about attachment; hand-off to GC is
where the enterprise starts talking about legal position.

The design is a living artefact. Version it, date it, review it
at the annual scanning-system audit, and update it when the
source universe shifts materially (a new NCA is designated, a
new sector regulator publishes AI-specific supervision, a new
US state passes an AI act). A design that has not been touched
in eighteen months is a design that no longer reflects the
system it claims to describe.
