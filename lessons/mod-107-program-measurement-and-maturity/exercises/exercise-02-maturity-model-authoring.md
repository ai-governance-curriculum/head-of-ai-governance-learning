# exercise-02: Maturity Model Authoring

**Estimated effort:** 3 hours

## Objective

Author the enterprise's own **AI-governance maturity model** —
the five-axis, five-level model the annual maturity assessment
in exercise 03 scores against, with tier definitions per axis
and per scoring cell, target-level-with-rationale annotations,
sector overlays applicable to the enterprise, and the model-
version discipline that keeps the model current without eroding
year-over-year comparability. The deliverable is the artefact
the level-50 senior AI-governance architect maintains under
document control, the artefact the head takes to the AI
Governance Council for annual ratification, and the artefact
the audit committee ratifies as the basis for the year's
maturity plot.

The model has to survive three stress tests. First, a peer head
from a benchmarking exchange reads the model and can tell what
"level 4 GOVERN 2.1" would require of their enterprise to
match; the model's tier definitions are legible to someone who
has not been in the room while the model was authored. Second,
the third-line CAE opens the assessment engagement and can test
scores against the model; the model's tier definitions are
evidence-anchored and not opinion-anchored. Third, an incoming
head-of-role six months from now inherits the model and can
score against it without re-negotiating tier definitions with
the CRO, the CAE, or the audit committee. A model that only
the authoring head can score is a model that fails on the first
transition.

The model is not a set of paragraphs describing what the head
believes maturity looks like. It is the *scoring contract* the
plot is measured against, and the discipline is that every cell
of the model has an evidence set the scorer produces to make
the score.

## Prerequisites

- Chapter [02-authoring-the-maturity-model](../02-authoring-the-maturity-model.md)
  — the five input references (NIST AI RMF Playbook, ISO/IEC
  42001, IAPP AIGP body of knowledge, MLCommons AI Safety
  benchmarks, ForHumanity IAAIS), the five-level CMMI-adjacent
  scale, the tier-definition discipline (evidence sets per
  level), the deliberate-under-investment annotation, the
  composition rules (per-axis-first, composite-as-summary,
  red-on-any-axis-is-a-signal, cross-axis diagnostics), the
  assessment cadence, the sector-overlay list, and the three
  anti-patterns (single-axis model, averaged composite,
  self-scored ceiling) — read and internalised.
- Chapter [01-kri-kpi-portfolio](../01-kri-kpi-portfolio.md)
  because metric 9 (maturity progression) is the model's
  running-cadence signal into the KRI/KPI portfolio, and the
  evidence-completeness metric (metric 8) is what supports the
  level-3+ evidence-set claim.
- Chapter [03-annual-maturity-assessment](../03-annual-maturity-assessment.md)
  because the assessment is what the model is authored *for*
  — a model that cannot be run against by the four-voice
  discipline (self, second-line, third-line, external) is a
  model that will not survive the first assessment cycle.
- [[mod-102-running-the-program]] chapter 04 (the level-50
  architect's regulatory crosswalk) — the ISO/IEC 42001 axis's
  scoring cells map onto the crosswalk's control set. Chapter
  06 (AI system inventory) and chapter 07 (supply-chain
  evidence) are the evidence surfaces the level-3+ claims are
  supported from.
- [[mod-103-board-and-audit-committee-reporting]] chapter 03
  (risk-appetite framework) — the reference the target-level
  rationale on axes where appetite is the controlling
  constraint.
- [[mod-105-regulatory-change-management]] chapter 01 (horizon
  scanning) — the input that drives sector-overlay refreshes as
  regimes evolve.
- [[mod-106-external-positioning-and-voluntary-codes]] chapter
  02 (standards-body participation portfolio) — informs which
  reference bodies the head reads as sector benchmarks and
  what standing engagement the head has with the reference-
  producing communities.
- Exercise 01 (KRI/KPI portfolio design) already completed —
  metric 9 (maturity progression) is defined against this
  model, and the model's operating cadence rides on the AIMS
  operating calendar the portfolio does.
- A concrete enterprise in mind — sector, jurisdictional
  footprint, AI system portfolio scope, and the standards-body
  and certification-body engagements the enterprise already
  runs. The sector overlays applicable depend on this context;
  make it explicit and consistent with exercise 01's
  enterprise context one-pager.

## Steps

1. **Reuse the enterprise context one-pager from exercise 01.**
   The model must be scored against the same enterprise. Add a
   short model-scope note to the top of the context one-pager
   naming which sector overlays the model will carry, which
   reference axes are in scope for the enterprise's current
   maturity, and which references are documented-as-out-of-
   scope (with the reason — a frontier-lab capability-tier
   axis is not applicable to a regional insurer, but the
   documented exclusion is what an incoming head needs to
   understand *why* the axis is missing).

2. **Author the model spine — the five-level scale.** Restate
   the five-level scale (Level 1 Initial / ad hoc through
   Level 5 Optimising) verbatim from chapter 02, adapted only
   where the enterprise already uses a bespoke tiering the CRO
   and CAE run against for adjacent maturity work (some banks
   use OSFI E-23-aligned tiering; some frontier labs use RSP /
   Preparedness / FSF capability-tier language). Where the
   enterprise uses a bespoke scale, cross-walk the bespoke
   language onto the five-level scale so the plot stays
   legible when it is set beside peer plots. The scale
   discipline is that a single five-level vocabulary is used
   across every axis and every overlay — no axis is scored on
   a different scale, because the plot has to remain
   comparable end-to-end.

3. **Author each of the five base-axis descriptions.** For
   each axis — NIST AI RMF Playbook (leadership-shape),
   ISO/IEC 42001 (management-system), IAPP AIGP body of
   knowledge (practitioner-competence), MLCommons AI Safety
   benchmarks (technical-evaluation), ForHumanity IAAIS
   (independent-audit-readiness) — write a half-page
   description that:
   - Names the reference document and version the axis is
     anchored on (e.g. NIST AI RMF 1.0 plus the Playbook
     current version, ISO/IEC 42001:2023 clauses 4–10 plus
     Annex A, IAPP AIGP BoK current version, current
     MLCommons AI Safety benchmarks, current ForHumanity
     IAAIS criterion base).
   - Names what the axis measures — the specific dimension of
     enterprise AI-governance maturity it captures — in one
     sentence.
   - Names the axis owner on the head's team — usually the
     level-50 architect for the ISO axis, may be different for
     the AIGP axis (which is often the head's people leader
     from [[mod-108-leading-the-governance-function]]), the
     MLCommons axis (which may be a technical-evaluation
     lead), and the IAAIS axis (which may be an ethics-and-
     independent-audit-readiness lead if the enterprise has
     one).
   - Names the axis granularity — for the ISO axis, per
     clause and per Annex A control; for the NIST axis, per
     subcategory; for the AIGP axis, per BoK domain; for the
     MLCommons axis, per benchmark suite; for the IAAIS axis,
     per criterion cluster.
   - Marks any factual claim about the reference's current
     state (specific subcategories, current examination
     blueprint, current benchmark version, current criterion
     scope) with a
     `<!-- needs-research: verify [specific fact] against
     [official source] -->` where the fact is not
     independently verified at authoring time.

4. **Author the tier-definition contract per axis.** For each
   axis, author the tier-definition table that specifies what
   evidence set is required for level 2 through level 5. Chapter
   02 gives the evidence-set discipline (level 2: documented
   procedure + record of one execution; level 3: procedure +
   accountable owner + RACI + training record + consistent
   execution; level 4: level 3 + KPI/KRI + target range +
   measurement + one management adjustment; level 5: level 4 +
   improvement plan + iterative improvement over cycles +
   informing peer practice). Adapt the discipline to each axis:
   - The ISO axis's evidence set for level 4 is not the same as
     the NIST axis's evidence set for level 4 — the ISO axis is
     management-system-oriented (the clause is operating with
     measurement) and the NIST axis is subcategory-coverage-
     oriented (the subcategory is being addressed with
     Playbook-suggested actions at depth). Author each
     accordingly.
   - Where a level's evidence set requires an artefact from
     another module, name the module and the specific artefact
     — a level-4 GOVERN 2.1 evidence set that requires the
     AIMS operating calendar's management review output cites
     the AIMS operating calendar directly, so the scorer knows
     where to look.
   - Do not leave any level's evidence set as "to be
     determined". A level without an evidence set is a level
     the scorer will interpret differently in year one and
     year two, and the plot's year-over-year comparability
     will not survive.

5. **Author the target-level-with-rationale annotations per
   cell.** For each cell of each axis, annotate:
   - **The current level** — where the enterprise is scored
     at authoring (this is a first-cut position; exercise 03
     will produce the ratified score).
   - **The target level on a two-year horizon** — where the
     enterprise is choosing to target.
   - **The rationale for the target level** — why this
     target and not a higher target. The rationale is a
     genuine sentence explaining the choice: resource
     constraint, sector-peer-adequate, lower-return-versus-
     alternative-investment, deliberate under-investment
     while regulatory position stabilises, or "leading" where
     the enterprise chooses to lead the sector on that
     dimension.
   The discipline is that not every cell targets level 5. A
   model that implicitly targets level 5 across the board is a
   model that will oversell capacity; deliberate under-
   investment is what the audit committee reads as mature.
   Chapter 02 is explicit on this point.

6. **Author the sector overlays applicable to the
   enterprise.** For each sector overlay in scope — banking
   (SR 11-7 or OSFI E-23), insurance (NAIC AI Model Bulletin,
   Colorado Reg 10-1-1 where applicable), health / medical
   device (FDA GMLP, PCCP), public sector (OMB M-25-21),
   frontier labs (RSP / Preparedness / FSF depending on
   enterprise identity), EU AI Act high-risk provider or
   deployer (Annex III / Article 26) — author the overlay
   axis with the same discipline as the base axes:
   reference-anchored description, tier-definition table with
   evidence sets, target-level-with-rationale annotation per
   cell. Do not author overlays the enterprise is not in
   scope for; do document in the model README which overlays
   were considered and excluded, with the reason. An overlay
   documented-as-excluded is a signal to an incoming head or a
   sector regulator that the exclusion is deliberate rather
   than an oversight.

7. **Author the composition rules.** Restate chapter 02's
   composition rules verbatim in the model itself — per-axis
   reporting first, composite as a summary read with an
   interpretation note, red on any axis as a signal not an
   average, cross-axis diagnostics named. The composition rules
   are the discipline that keeps the plot legible; if they
   live only in chapter 02 and not in the model artefact, the
   next scorer will forget them.

8. **Author the assessment cadence.** State the model's
   operating cadence on the AIMS operating calendar: the
   annual full assessment (typically Q4), the mid-year
   trajectory read (six-month mark), the annual model-version
   review (before the assessment runs), and the sector-overlay
   refresh cadence (as regimes evolve, driven by the
   horizon-scanning system in
   [[mod-105-regulatory-change-management]] chapter 01). The
   cadence is what keeps the model from decaying between
   assessments.

9. **Author the model-version discipline.** Version the model
   explicitly. State how model-version changes are ratified:
   material changes (adding an axis, moving a tier definition,
   changing a target level) at the AI Governance Council with
   audit-committee ratification where the change touches the
   committee's line of sight; minor changes (clarification of
   tier language without changing the evidence set) at the
   level-50 architect's discretion, minuted. State the
   discipline that a model change made mid-year does not
   apply to the year in flight — the plot scores against the
   ratified model at the start of the year, so year-over-year
   comparability survives.

10. **Author the failure-mode audit.** Author a short section
    — one paragraph per failure mode — naming how the model
    surfaces and recovers from each of these failure modes:
    - A tier definition that has drifted between years such
      that a level-4 score in year one and a level-4 score in
      year two are not the same claim.
    - A sector-overlay reference that has been superseded by a
      new regime version, and the overlay has not been
      refreshed, so the scorer is scoring against a stale
      reference.
    - A model that has silently accumulated the "single-axis"
      anti-pattern — all axes deferring to ISO / all axes
      deferring to NIST — because one axis owner has been the
      most active and the others have drifted.
    - A target-level annotation that has quietly ratcheted
      upward without a documented ratification (a "we're
      going to level 5 on GOVERN" that was never taken to the
      AI Governance Council).
    - A model whose composition rule (per-axis-first) is
      being violated in reporting because the audit committee
      asked for a single number and the head has quietly
      started reporting one without the per-axis breakdown.

## Deliverables

- `model/README.md` — the model overview: version, ratification
  history, axes in scope, sector overlays in scope,
  overlays-considered-but-excluded, model-version discipline,
  composition rules, assessment cadence.
- `model/scale.md` — the five-level scale, plus any bespoke-
  tiering cross-walk where the enterprise uses OSFI E-23 /
  RSP / Preparedness / FSF / other adjacent tiering.
- `model/axis-01-nist-ai-rmf-playbook.md` — the NIST axis:
  description, granularity (per subcategory), tier-definition
  table with evidence sets, target-level-with-rationale
  annotations per cell.
- `model/axis-02-iso-iec-42001.md` — the ISO axis: description,
  granularity (per clause and per Annex A control), tier-
  definition table, target-level annotations. Includes
  composition notes for companion standards (ISO/IEC 42005,
  ISO/IEC 42006, ISO/IEC 23894) if in scope.
- `model/axis-03-iapp-aigp-body-of-knowledge.md` — the AIGP
  axis: description, granularity (per BoK domain), tier-
  definition table, target-level annotations.
- `model/axis-04-mlcommons-ai-safety.md` — the MLCommons axis:
  description, granularity (per benchmark suite), tier-
  definition table, target-level annotations. Includes
  composition notes for OWASP AI Security & Governance
  Checklist / OWASP LLM Top 10 / OWASP Machine Learning
  Security Top 10 if in scope.
- `model/axis-05-forhumanity-iaais.md` — the IAAIS axis:
  description, granularity (per criterion cluster), tier-
  definition table, target-level annotations.
- `model/overlay-<sector>.md` — one file per sector overlay in
  scope for the enterprise, with the same shape as the base
  axes.
- `model/composition-rules.md` — the composition rules
  transcribed into the model artefact (per-axis-first,
  composite-as-summary, red-on-any-axis, cross-axis
  diagnostics).
- `model/cadence.md` — the assessment cadence (annual full
  assessment, mid-year trajectory read, annual model-version
  review, sector-overlay refresh).
- `model/version-history.md` — the version history and
  ratification record.
- `model/failure-mode-audit.md` — the five failure-mode
  detection-and-recovery paragraphs.

## Acceptance criteria

- Every base axis has a reference document and version named.
  A description that reads "NIST AI RMF, generally" fails the
  criterion — the model must name the version the assessment
  is scored against.
- Every axis has an owner named as a role, not a person. Roles
  are stable across incumbency changes; people are not.
- Every axis has tier definitions for level 2 through level 5.
  A level without an evidence set fails the criterion — the
  chapter is explicit that scoring without evidence sets is
  opinion.
- Every cell has a current level, a target level, and a
  rationale for the target. A rationale reading "grow to
  level 5" without the *why* fails the criterion. Deliberate
  under-investment is one of the mature choices; the rationale
  is what surfaces it.
- Every sector overlay in scope has been authored with the
  same discipline as a base axis (reference-anchored,
  evidence-set tier definitions, target-level annotations).
  Overlays out of scope are documented in the README with the
  reason.
- The scale is a single five-level vocabulary across every
  axis and every overlay. A model that scores one axis on a
  four-level scale and another on a six-level scale fails the
  criterion; plot legibility depends on a single scale.
- The composition rules are inside the model artefact, not
  only in chapter 02. A model artefact that does not carry
  the composition rules is a model that will be scored
  incorrectly by the next scorer.
- The model-version discipline names how material and minor
  changes are ratified, and states the mid-year-change-does-
  not-apply-to-the-year-in-flight rule. Without the rule,
  year-over-year comparability erodes silently.
- The failure-mode audit names, for each of the five failure
  modes, at least one specific detection signal and one
  specific recovery action.
- Any factual claim about a specific reference's current
  version, current scope, or current examination blueprint
  carries a
  `<!-- needs-research: verify [specific fact] against
  [official source] -->` marker where the fact is not
  independently verifiable. The chapter carries several such
  markers by design; the model does not silently drop them.

## Stretch goals

- Author the **cross-axis diagnostic matrix** — the small set
  of two-axis pairs where a specific score combination reads
  as a specific diagnostic. Chapter 02 names the GOVERN-at-4
  / clause-5-at-3 diagnostic ("leadership-shape maturity has
  outrun management-system maturity"); the stretch is to
  extend that with a further three-to-five cross-axis
  diagnostics that the level-50 architect commits to naming in
  the assessment output when the combination appears (an
  AIGP-BoK-at-2 with an ISO-clause-9-at-4 diagnostic; an
  MLCommons-at-1 with an IAAIS-at-4 diagnostic; etc.).
- Author the **peer-benchmarking mapping note** — for each
  base axis, name the specific peer-institution disclosure or
  benchmarking source the head expects to compare against
  (per exercise 03's peer set). The mapping is what the head
  hands to the level-50 architect when the assessment cycle
  opens so the architect knows which peer signals to seek and
  which peer signals will not be available for the axis. See
  [[mod-106-external-positioning-and-voluntary-codes]] chapter
  02 for the standing external-engagement surface the mapping
  draws from.
- Draft the **audit-committee ratification pack** for the
  model's first-year adoption. The pack is a short
  presentation the audit committee ratifies the model at: the
  five axes, the sector overlays, the assessment cadence, the
  model-version discipline, the composition rules, and the
  head's specific ask (ratification of the model as the basis
  for the following year's plot). Use the pack shape
  convention from
  [[mod-103-board-and-audit-committee-reporting]] chapter 02.
- Author the **model-change proposal template** — the short
  document the level-50 architect uses to propose a model
  change (new axis, tier-definition revision, overlay
  refresh) to the AI Governance Council. The template's
  discipline is that a model change requires the specific
  change proposed, the specific rationale (why now), the
  specific impact on year-over-year comparability, and the
  specific ratification path.
- Draft the **incoming-head handover note on the model** — the
  one-page note an outgoing head hands to an incoming head
  explaining the model's current state, the pending
  refreshes, the axis owners, and the model's known
  limitations. The discipline is that the model is portable
  across incumbency; a model that only the authoring head can
  interpret is a model that fails on the first transition.

## Notes and starter guidance

The most common first-cut failure of the model is the head who
authors the model as a set of paragraphs describing what
maturity "looks like" without evidence sets per level. Prose
alone is not a scoring contract — the level-50 architect
scoring against prose will interpret the prose differently in
year one and year two, and the plot's year-over-year
comparability will not survive. Start each level with an
explicit evidence-set claim: "level 3 requires the following
artefacts, produced by these owners, at this cadence, held in
these systems of record". Then, and only then, add the
descriptive prose that motivates the evidence set.

The second common failure is the head who authors the axes but
skips the composition rules and the assessment cadence,
treating them as chapter 02's concern rather than the model's.
The composition rules and the cadence *are* the model, in the
same way the tier definitions are. Without them, the next
scorer picks a composition of their own — often the averaged-
composite anti-pattern the chapter refuses — and the plot
stops carrying the signal the head authored it to carry.

On sector overlays — the temptation is to author every overlay
"just in case". Only author the overlays the enterprise is
actually in scope for; document the excluded overlays in the
README with the reason. An overlay that has been half-authored
against a sector the enterprise is not in is a maintenance
liability with no operating value.

On the target-level rationale — resist the aspirational
rationale ("we want to lead the sector"). The chapter is
explicit that boards read deliberate under-investment as
mature and read "everything to level 5" as unbudgeted. The
rationale is where the head's strategic choice about where to
lead, where to match, and where to lag is written down. That
choice belongs to the head, not to the level-50 architect;
the head does the strategic call and the architect does the
tier-definition craft.

On the failure-mode audit — pick the failures the head has
actually seen (or has seen in a peer's program), not
hypothetical failures. The audit is stronger when it names
concrete detection signals from actual experience.

The model is a living artefact. Version it, date it, review it
annually at the model-version review before the assessment,
refresh sector overlays as regimes evolve, and treat model
changes with the same document-control discipline the head
applies to the AIMS control set. A model that has not been
touched in a year is a model that no longer reflects the
maturity landscape it purports to score against.
