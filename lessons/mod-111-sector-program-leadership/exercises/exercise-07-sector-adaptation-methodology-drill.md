# exercise-07: Sector Adaptation Methodology Drill

**Estimated effort:** 3 hours

## Objective

Instantiate the sector-adaptation methodology from chapter 08
against either a single-sector or a multi-sector enterprise
scenario. The deliverable is the head's methodology-in-use: the
architect-blueprint gap-and-fit read, the sector-specific
regulator-engagement pattern per regulator, the board-reporting
cadence and content adapted to the sector's board conventions,
and the external-positioning posture adapted to the sector's
expected surfaces — plus, for a multi-sector enterprise, the
reconciliation logic that keeps the head running one program
rather than multiple parallel programs.

The deliverable is not a survey of the methodology. It is the
operating record that shows the methodology executed against a
specific enterprise, at leadership scope, in a form the audit
committee (or the equivalent primary body) can ratify.

## Prerequisites

- Chapter [08-sector-adaptation-methodology](../08-sector-adaptation-methodology.md)
  — read and internalised.
- At least two of chapters 01-07 (the sector chapters) — one
  chapter for a single-sector scenario, two or more for a multi-
  sector scenario. The methodology only lands if there is
  sector content to methodologise about.
- Chapter 04 of [[mod-104-regulator-engagement]] — the generic
  regulator-engagement pattern the sector-specific patterns
  instantiate.
- [[mod-103-board-and-audit-committee-reporting]] cluster 4 —
  the generic board-reporting shape the sector adaptations
  reshape.
- [[mod-106-external-positioning-and-voluntary-codes]] chapters
  02 and 03 — the generic external-positioning portfolio the
  sector adaptations populate.
- [[mod-101-role-scope-and-leadership-shape]] chapter 04 — the
  level-40 / level-50 / level-60 scope stack the methodology
  keeps explicit.
- A specific enterprise scenario. Options:
  - **Single-sector.** Pick one of the seven sectors from
    chapters 01-07 and instantiate against a specific
    enterprise scoping (bank / insurer / health system / pharma
    / federal agency or contractor / frontier lab / critical-
    infrastructure operator).
  - **Two-sector.** A bank with an insurance subsidiary; a
    hospital that markets an in-house-developed diagnostic AI;
    a telecom that owns a media property; a defense contractor
    that sells to civilian agencies; a health system with a
    device-development spinout that reaches FDA regulation.
  - **Three-plus-sector conglomerate.** A financial services
    conglomerate spanning banking, insurance, and asset
    management; a healthcare-and-life-sciences group spanning
    hospital operations, pharma manufacturing, and health
    plan administration; a diversified industrial spanning
    manufacturing, energy operation, and equipment sales.

## Steps

1. **Enterprise profile one-pager.** Half-page scoping: sectors
   in scope (each named against a chapter 01-07), business-unit
   or entity structure (group parent, subsidiary boards, legal-
   entity separation), current head-of-AI-governance placement
   in the org (peer of CxO; specialist under a CxO; enterprise-
   wide role), current architect-level counterpart (the level-50
   senior-ai-governance-architect on the paired track), and
   current sector blueprint state per sector (blueprint exists;
   blueprint exists but under refresh; blueprint pending).

2. **Architect-blueprint gap-and-fit read.** For each sector in
   scope, read the current architect-authored sector blueprint
   against three lenses from chapter 08:
   - Instrument coverage — does every material sector instrument
     the sector's chapter identifies have a corresponding control
     or evidence element in the blueprint? Name gaps concretely
     (Colorado Regulation 10-1-1 was signed after the last
     insurance blueprint refresh; NYDFS Circular Letter No. 7
     is not yet integrated; the FDA CDER January 2025 draft
     guidance has moved and the blueprint has not caught up).
   - Jurisdictional coverage — does the blueprint's evidence
     pipeline serve every jurisdiction the enterprise operates
     in? Name new footprint (the UK subsidiary that brings PRA
     SS1/23 into scope; the Colorado line of business that
     brings Regulation 10-1-1 into scope; the new EU footprint
     that brings NIS2 into scope).
   - Workflow fit — does the blueprint's workflow structure
     align with the enterprise's actual org design and existing
     operating cadences? Name friction points (the blueprint
     assumes an MRM function co-located with AI governance but
     the enterprise runs them separately; the blueprint assumes
     a Quality Committee that the enterprise does not have).
   Per gap, open a concrete change request to the architect
   (or record that the architect has already opened one). Per
   fit issue, name the workflow adaptation the head has
   negotiated with the architect and the affected workflow
   chapter in [[mod-102-running-the-program]].

3. **Sector-specific regulator-engagement pattern instantiation.**
   For each sector in scope, take the generic regulator-
   engagement pattern from chapter 04 of
   [[mod-104-regulator-engagement]] and instantiate against each
   regulator the sector chapter identifies. Per regulator:
   - Named enterprise counterpart (individual and function).
   - Formal channel (letter, examination, submission, MOU).
   - Informal channel (industry-body, trade association,
     advisory committee, speech circuit).
   - Peer-fronting decision (who fronts routine; who fronts on
     escalation).
   - Cadence.
   - Escalation stance pre-decided at each tier of the sector's
     escalation ladder (MRA / MRIA for banking; market-conduct
     examination findings for insurance; FDA-483 observations
     for FDA-regulated sectors; IG audit findings for federal
     agencies; sectoral-regulator directives for critical
     infrastructure).
   The instantiation is the head's work, not the architect's;
   the architect's blueprint may name the regulator as in-scope
   but does not name how the enterprise engages the regulator.

4. **Board-reporting cadence and content adaptation.** For each
   sector in scope, adapt the generic board-reporting cluster
   shape from [[mod-103-board-and-audit-committee-reporting]]
   to the sector's actual board conventions. Per sector, name:
   - The primary committee for AI-substantive content (Quality
     Committee for a health system; Risk Committee for a bank;
     R&D or Science and Technology Committee for a pharma;
     AI Governance Board for a federal agency under M-25-21;
     Safety and Security Committee for a frontier lab; Safety
     Committee or Risk Committee for a critical-infrastructure
     operator).
   - The audit-committee slice — where compliance and internal-
     control substance lands.
   - The cluster mapping — which AI-substantive content flows
     to which committee, and how the two committees'
     narratives reconcile.
   - The refresh cadence — quarterly (default), or another
     cadence justified by the sector's cadence conventions.
   Adaptations are stable across quarters (regenerating the
   reporting structure quarterly is a governance failure), but
   are refreshed materially when the enterprise's board
   structure changes or the sector's board conventions shift.

5. **External-positioning posture adaptation.** For each sector
   in scope, populate the generic external-positioning portfolio
   inventory from [[mod-106-external-positioning-and-voluntary-codes]]
   chapter 02 with the sector's expected industry-body surfaces.
   Per body:
   - Body name and sector attachment.
   - Signed / considered-and-declined / under-consideration /
     watched status.
   - Owner (typically the head, the head's delegate, or a
     ratified individual on the head's team).
   - Chair or officer role status, with external-positioning-
     committee ratification cite.
   - Cross-portfolio consistency notes (where a public position
     in one body needs to reconcile with a public position in
     another body).

6. **Multi-sector reconciliation (if applicable).** If the
   enterprise operates in more than one sector, apply the
   chapter 08 reconciliation logic:
   - Every applicable sector's adaptation is executed. No
     sector is skipped because "the primary sector is X."
   - Where adaptations overlap on the same instrument or the
     same counterpart, the more stringent adaptation prevails
     and is applied enterprise-wide, unless the enterprise's
     group structure isolates the entity.
   - The board-reporting adaptation reflects the multi-sector
     reality — a group Audit Committee reads the aggregate
     posture; entity-level boards (a bank subsidiary board;
     an insurance subsidiary board) read the entity-specific
     slice.
   - The external-positioning portfolio inventory includes each
     sector's industry-association surface, and cross-portfolio
     consistency is a live consideration.
   Document each reconciliation decision so a successor can
   read it without re-litigation.

7. **Level-40 / level-50 / level-60 scope-stack record.** For
   the sector-adaptation work in scope, name — per sector, per
   artefact — the level at which each element sits:
   - Level 40 (individual-contributor architect under the
     senior architect) authors the technical implementation of
     a sector control (an SR 11-7-aligned validation package
     for a specific banking AI model; a GMLP-aligned lifecycle
     documentation for a specific FDA submission; the OT AI
     safety-case update for a specific NERC CIP-scope asset).
   - Level 50 (senior architect) authors the sector blueprint
     (how SR 11-7 alignment is achieved enterprise-wide; how
     GMLP-aligned documentation is produced enterprise-wide).
   - Level 60 (head, this exercise) authors the regulator-
     engagement pattern, the board-reporting adaptation, the
     external-positioning posture — and holds accountability
     for the sector's overall regulatory posture.
   Any element that appears at more than one level is a
   scope-blur risk; the exercise identifies each and specifies
   the disambiguation.

8. **Refresh-cadence record.** Per adapted surface, name the
   refresh cadence per chapter 08:
   - Regulator-engagement pattern: reviewed quarterly as part
     of the regulator-inventory refresh in
     [[mod-104-regulator-engagement]] chapter 04; refreshed
     materially on trigger.
   - Board-reporting cadence and content: reviewed annually
     with the audit committee (or the equivalent primary
     committee); refreshed materially on trigger.
   - External-positioning posture: reviewed annually against
     the portfolio inventory; refreshed materially on trigger.
   - Architect-blueprint refresh: on the architect's own
     cadence; the head reads the refresh, executes the
     adaptation implications, and re-ratifies with the audit
     committee where material.

## Deliverables

- `enterprise-profile.md` — the one-page scenario scoping.
- `architect-blueprint-gap-and-fit-read.md` — the per-sector
  gap-and-fit read against the three lenses (instrument
  coverage, jurisdictional coverage, workflow fit).
- `regulator-engagement-pattern-<sector>.md` — one file per
  sector, instantiating the generic pattern per regulator.
- `board-reporting-adaptation-<sector>.md` — one file per
  sector, adapting the cluster shape to the sector's board
  conventions.
- `external-positioning-posture-<sector>.md` — one file per
  sector, populating the portfolio inventory with sector
  surfaces.
- `multi-sector-reconciliation.md` — the reconciliation record
  (only if the scenario is multi-sector).
- `scope-stack-record.md` — the level-40 / level-50 / level-60
  scope-stack record with scope-blur risks identified.
- `refresh-cadence-record.md` — the per-surface refresh cadence
  record with trigger conditions.

## Acceptance criteria

- Every sector in scope has a full four-artefact adaptation
  (regulator-engagement pattern, board-reporting adaptation,
  external-positioning posture, plus the gap-and-fit read
  against the architect blueprint). Sectors named in the
  profile but not adapted fail the exercise.
- The gap-and-fit read is concrete per lens. "Blueprint is
  adequate" without lens-by-lens analysis fails the exercise;
  every material gap has a concrete change request opened
  with the architect.
- The regulator-engagement patterns instantiate every regulator
  the sector chapter identifies. Aggregation labels ("state
  DOIs" for insurance; "sectoral regulators" for critical
  infrastructure) are acceptable only with an explicit
  aggregation rule.
- The board-reporting adaptation names the primary committee
  for AI-substantive content per sector, the audit-committee
  slice, the cluster mapping, and the refresh cadence.
  Adaptations that regenerate quarterly rather than staying
  stable fail on governance-hygiene grounds.
- The external-positioning posture uses the signed /
  considered-and-declined / under-consideration / watched
  discipline per body. Bodies whose status is "engaged" with no
  scope statement fail the exercise.
- Multi-sector reconciliation names each reconciliation
  decision with reasoning. "More stringent prevails" as a
  category label without applied instance-by-instance
  reasoning fails.
- The scope-stack record identifies every scope-blur risk with
  a specific disambiguation. Records that assume level-40 /
  level-50 / level-60 boundaries hold naturally without
  documentation fail on realism.
- The refresh-cadence record names cadence and trigger per
  surface. Category cadences without triggers fail on
  operating-readiness grounds.
- Uncertain instrument or footprint status (a state's NAIC
  bulletin adoption; a UK-subsidiary PRA SS1/23 in-scope
  determination; a federal-memorandum current status; a
  frontier-lab framework published version) carries a
  `<!-- needs-research: -->` flag rather than a guess.

## Stretch goals

- Add a change-request walk-through: the architect refreshes
  the sector blueprint materially (new instrument added; new
  jurisdiction added; workflow structure changed). Author the
  head's response — read the refresh, execute the adaptation
  implications, ratify with the audit committee where material,
  update the regulator-engagement pattern where the refresh
  affects it, update the board-reporting adaptation where
  material.
- Rehearse a failure-mode diagnosis. The audit committee has
  asked a follow-up question the head could not answer clean.
  Which of chapter 08's five failure modes (framework
  transplantation, framework proliferation, board-reporting
  misfit, external-positioning drift, head-architect blur) is
  the root cause? Author the diagnosis and the remediation
  plan.
- For a multi-sector scenario, rehearse a public-position
  conflict: the enterprise's banking-sector position on a
  policy issue (e.g., through Bank Policy Institute) conflicts
  with its insurance-sector position on the same issue (e.g.,
  through ACLI). Author the reconciliation — which position
  prevails, on what reasoning, and how the enterprise
  communicates the reconciled position to both industry bodies.
- Circulate the adaptation package to the level-50 senior
  architect (peer on the paired track) and incorporate one
  round of critique on scope-boundary questions.

## Notes and starter guidance

- The methodology is meaningful only against real sector
  content. Exercises that read the chapter 08 methodology
  without instantiating against the chapter 01-07 sector
  content miss the exercise's design. Pick at least one
  chapter's sector content and work it through.
- The single most common failure mode is the head-architect
  blur — the head authoring blueprint work that belongs at
  level 50, or the architect fronting regulator relationships
  that belong at level 60. Rehearse the scope-stack record
  before you rehearse anything else; it is where the whole
  methodology's coherence lives.
- The adaptation is not a documentation exercise. Every
  artefact — the regulator-engagement pattern, the board-
  reporting adaptation, the external-positioning posture — is
  an operating artefact the enterprise runs against. If the
  artefact does not survive contact with the sector's
  regulator, the sector's board committee, or the sector's
  industry body, the adaptation has failed.
- Multi-sector enterprises are not simply "several single-
  sector enterprises in one holding company." The
  reconciliation logic is the discipline that keeps the head
  running one program instantiated per sector, rather than
  multiple parallel programs. Multi-sector scenarios where the
  reconciliation logic is skipped end up with the framework-
  proliferation failure mode by default.
- Refresh cadences are per-surface. Regenerating the whole
  adaptation package quarterly is a governance failure; the
  adaptation is stable across quarters and refreshed on
  trigger. If the enterprise's quarterly cadence produces a
  new regulator-engagement pattern or a new board-reporting
  adaptation every quarter, the methodology has been
  misapplied.
- The exercise is the module's closing artefact. It is where
  the sector chapters stop being seven separate walk-throughs
  and become seven instances of the same underlying leadership
  discipline. Treat the deliverable accordingly — as the
  operating record that closes the module, not as an
  incremental drill.
