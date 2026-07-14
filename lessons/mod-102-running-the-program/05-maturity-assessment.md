# Running Annual and Multi-Year Maturity Assessments

## Motivation

Every board and audit committee eventually asks the same three
questions of a running AI governance program: *are we mature? are we
getting more mature? and how do we know?* A head who answers those
questions with narrative — "the program is coming together nicely" —
is not answering them. A head who answers with a maturity plot against
a published framework, dimensions the framework specifies, and a
trend against last year's plot is answering them.

Maturity assessment is that plot. It is the annual and multi-year
cadence that lifts the head's operating discipline out of "we did
things this year" and into "here is where we are on a defensible
maturity trajectory, here is where we are moving to, and here is what
each move costs." Boards understand trajectory in a way they do not
understand activity. Audit committees understand a maturity delta from
last year in a way they do not understand a raw score.

This chapter is how to run the assessment against the three
maturity references the head owns — the NIST AI RMF Playbook, the
ISO/IEC 42001 maturity dimensions the architect specified, and the
OWASP AI Security & Governance Checklist coverage — and how to feed
the resulting picture into the board and audit-committee decks under
[[mod-103-board-and-audit-committee-reporting]].

## Core concept: three references, one composite maturity picture

The three references measure different things. Confusing them or
picking one to the exclusion of the others is a common failure.

- **NIST AI RMF Playbook maturity dimensions.** The Playbook,
  organised by AI RMF subcategory (GOVERN, MAP, MEASURE, MANAGE),
  offers suggested actions at varying depths. Read at leadership
  scope (see [[mod-101-role-scope-and-leadership-shape]] chapter 02),
  the tiered actions and transparency-and-documentation practices
  let the head place the AI governance function on a maturity
  trajectory — typically expressed as *initial → repeatable →
  defined → managed → optimising* per subcategory or per subcategory
  cluster. It is the leadership-shape reference.
- **ISO/IEC 42001 maturity dimensions.** The AIMS itself has
  maturity in the sense that a management system does — the
  Harmonised Structure clauses can be evidenced at increasing depth
  and integration. The level-50 architect specifies the enterprise's
  maturity model against the AIMS clauses and controls, typically
  as a five-level scale keyed to ISO management-system practice.
  It is the operating-system reference.
- **OWASP AI Security & Governance Checklist.** OWASP publishes the
  AI Security & Governance Checklist as a technical-control-oriented
  reference for AI security practice, complementing the AI RMF and
  ISO/IEC 42001 with concrete security controls. Coverage against
  the checklist is a maturity signal in the security-and-adversarial-
  robustness dimension, and composes with the OWASP LLM Top 10 and
  the OWASP Machine Learning Security Top 10 where the enterprise
  has LLM or classical-ML surface. It is the technical-control
  reference.

The head does not pick one. The head reports a *composite* maturity
picture, with each reference contributing a distinct axis: NIST for
leadership-shape maturity, ISO/IEC 42001 for management-system
maturity, OWASP for technical-security-control maturity. Boards read
the composite; the head defends the composite; the level-50 architect
consumes the composite to prioritise the following year's design work.

## The five-level maturity vocabulary

All three references map naturally into a five-level maturity
vocabulary derived from CMMI-style progression. The head uses this
vocabulary consistently so the composite plot is legible.

- **Level 1 — Initial / ad hoc.** The activity happens; it is not
  yet consistent, documented, or reliably repeatable.
- **Level 2 — Repeatable.** The activity is repeated with basic
  documentation; individuals rather than the process ensure
  consistency.
- **Level 3 — Defined.** The activity is documented as a standard
  process; roles and responsibilities are clear; the process
  operates without reliance on specific individuals.
- **Level 4 — Managed.** The activity is measured, results are
  analysed, and the process is adjusted based on measurement. KPIs
  or maturity metrics are in place.
- **Level 5 — Optimising.** The activity is under continual
  improvement, with data-driven refinement; the process contributes
  to the enterprise's competitive posture.

The vocabulary is enterprise-agnostic and matches vocabulary the CRO,
CISO, and CAE already use for their own maturity reporting; the head
does not invent a new one. Where the level-50 architect specified
alternative labels (some enterprises use the Harmonised Structure's
own language, or a bespoke five-level scale tuned to sector
practice), the head uses those instead — but the plot is always
five levels, so trend visualisation stays legible.

## Running the annual assessment

The annual maturity assessment is itself an anchor on the AIMS
operating calendar (chapter 02). It runs at a specific point in the
year — typically Q4, so its output feeds the next year's objectives
and risk-treatment plan refresh in Q1. Its inputs and outputs are
documented.

Inputs to the annual assessment:

- The prior year's assessment output.
- The current NIST AI RMF Playbook subcategory-level self-scoring.
- The current ISO/IEC 42001 AIMS clause-and-Annex-A control
  maturity self-scoring.
- The current OWASP AI Security & Governance Checklist coverage
  scoring.
- Internal audit results from the year (chapter 02) and external
  audit findings from the year (chapter 04).
- The risk register's portfolio-level trends (chapter 03).
- Incident and near-miss volumes and severity trends.
- Third-party program coverage and evidence-completeness metrics
  (chapter 07).

Outputs of the annual assessment:

- A **maturity heat map** — three panels (NIST, ISO, OWASP), each
  with subcategory or control-cluster level scores in the five-
  level vocabulary.
- A **year-over-year delta** — where the enterprise moved up,
  where it moved down, where it held. Down moves are as diagnostic
  as up moves.
- A **trajectory plot** — where the enterprise commits to move
  next year, and the two-year target, per axis.
- A **cost-of-move table** — for each planned move, the resource
  investment (people, technology, external assurance) required.
  This feeds the budget cycle under
  [[mod-113-budget-vendor-p-and-l-and-investment-case]].
- A **prioritisation recommendation** — which two or three moves
  the head recommends the enterprise prioritise, and why. Boards
  read this section first.
- An **assumptions and limitations section** — a candid statement
  of what the assessment does not measure, what the scores mean and
  what they do not mean. Boards trust an assessment that acknowledges
  its own limits.

## Self-assessment discipline — defending the scoring

Maturity self-assessment is fragile. The head is scoring their own
function against dimensions the same function operates. Two
disciplines defend against the fragility.

First, **evidence-anchored scoring**. Every score at level 3
(defined) or above requires linked evidence. A level-3 GOVERN 2 score
requires the operating-model RACI document and the AI governance
council charter under document control; a level-4 GOVERN 2 score
requires those plus measurement of council-attendance quorum,
decision throughput, and escalation-loop-close rate. A score claimed
without evidence is a level 2 by default.

Second, **independent challenge**. The assessment is challenged by
an independent party before it is finalised. The three practical
options: the third-line CAE conducts an assurance review of the
scores (preserving CAE independence — chapter 04 — the CAE does not
set the scores, only assures the evidence base for them); an
external consultant with no delivery relationship with the AI
governance function reviews; or a peer head of AI governance at a
comparable enterprise conducts a friendly-fire review. Any of the
three defends the plot at the audit committee; none of the three is
optional if the plot is to be taken seriously.

Where the assessment is used for regulatory or examination
disclosure (some sector regulators expect maturity self-assessment
as an input to examination scoping), the independent-challenge
requirement is stricter — third-line CAE or external is defensible;
peer-review is not. The head aligns with the regulatory-affairs
function on which regimes apply.

## Multi-year trajectory — reading the plot as a road map

A maturity plot at a single point in time is not the goal. The goal
is a *trajectory* — a two- or three-year path that the plot walks the
enterprise through, and against which the plot's actual movement is
measured each annual cycle.

The head owns the trajectory. Concretely, that means:

- **Explicit targets, per axis.** For each of NIST, ISO, and OWASP,
  the head names — with council ratification and audit-committee
  visibility — what maturity level the enterprise is targeting per
  subcategory or control cluster, two years out.
- **Deliberate under-investment.** Not every subcategory should be
  targeted at level 5. Enterprise resources are finite; overshooting
  in one area starves another. The head names which axes the
  enterprise deliberately holds at level 3 or 4 because further
  investment would be lower-return than a move in a different area.
  This is a mature governance discipline; boards value it precisely
  because it is uncomfortable to say aloud.
- **Sector-benchmark posture.** The trajectory is contextualised
  against sector benchmarks where available — MIT AI Risk
  Repository framings, MLCommons AI Safety benchmark participation,
  peer disclosure via the Anthropic Responsible Scaling Policy /
  OpenAI Preparedness Framework / Google DeepMind Frontier Safety
  Framework where the enterprise is a frontier lab, sector-body
  peer benchmarks in banking or health. The head does not benchmark
  in isolation; the head names where the enterprise chooses to lead,
  match, or lag the sector.
- **Regulatory-horizon alignment.** The trajectory anticipates
  known regulatory milestones (EU AI Act GPAI obligations from
  August 2025, high-risk system obligations from August 2026 and
  2027, sector-specific supervisory changes). Maturity moves that
  target those milestones are prioritised over those that do not.

The two-year trajectory is a document, not a slide. It is under
AIMS document control and reviewed at each annual assessment.

## Feeding maturity into board and audit-committee decks

Board and audit-committee decks (see
[[mod-103-board-and-audit-committee-reporting]]) treat maturity as a
standing item on an annual cadence, with a mid-year read-through if
the trajectory is off pace. The head's discipline in that reporting:

- **One plot per axis, then a composite.** Boards want to see the
  NIST plot, the ISO plot, and the OWASP plot before they see the
  composite; the composite averages the three, which loses signal
  a board reads directly from the individual axes.
- **Year-over-year delta, coloured.** Improvements are one colour,
  regressions are another, holds are a third. Deltas surface the
  board's attention on regressions.
- **The trajectory line.** Overlay the two-year target on the
  current plot. The board reads at a glance where the plot is
  ahead of, on, or behind the trajectory.
- **The three or four asks.** The audit committee's role is to
  authorise the resources the trajectory requires. The head names
  the specific resource asks — headcount, tooling, external
  assurance — that the year's trajectory move depends on.
- **The limits of the plot.** Boards trust decks that state what
  the maturity plot does not measure. A well-authored deck names
  the two or three dimensions of AI risk the plot understates, and
  what the enterprise does to compensate.

An audit committee that receives the plot annually, with an on-pace
mid-year read, and understands the trajectory ratifies the head's
investment plan. An audit committee that receives narrative and
selectively-quoted scores does not. The difference is the head's
authoring discipline.

## Composition with sector and voluntary-code maturity references

The three headline references — NIST, ISO/IEC 42001, OWASP — do not
cover every maturity dimension a sector or voluntary-code framework
imposes. The head composes them with sector-specific references
where applicable:

- **Banking.** Federal Reserve SR 11-7 and OCC 2011-12 model-risk-
  management maturity references (implicit in the guidance) and OSFI
  E-23 tiering; the enterprise's model-risk-management function
  usually has its own maturity plot the head coordinates with.
- **Insurance.** NAIC AI Model Bulletin adoption and state-by-state
  insurance-department expectations create a state-level maturity
  dimension the head tracks.
- **Health.** FDA GMLP predetermined change control plan (PCCP)
  maturity is a distinct dimension for medical-device-adjacent AI;
  post-market surveillance maturity under FDA and EU MDR/IVDR
  regimes composes separately.
- **Public sector.** OMB M-25-21 governance requirements set a
  federal-agency-specific maturity baseline; sector agencies (Defense,
  Health and Human Services, Intelligence Community) impose deeper
  requirements.
- **Frontier labs.** Responsible Scaling Policy (Anthropic),
  Preparedness Framework (OpenAI), and Frontier Safety Framework
  (Google DeepMind) maturity plots are the sector reference for
  frontier-lab-scoped AI governance; peer disclosure at the
  Frontier Model Forum sets an informal expectations bar.
- **Voluntary codes.** The EU AI Office GPAI Code of Practice
  signatory obligations, the G7 Hiroshima Process Code of Conduct,
  the Bletchley Declaration signatory disclosures, and equivalents
  create maturity commitments the head is accountable for. See
  [[mod-106-external-positioning-and-voluntary-codes]].

Composition is not consolidation. Each additional reference is a
distinct axis or overlay on the composite picture. The head owns
which references are in scope, why, and what a mature score on each
looks like.

## Example — a two-year trajectory presentation

A worked example. At the annual assessment, the enterprise is at:

- NIST AI RMF Playbook composite: GOVERN 3.5, MAP 3.0, MEASURE 2.5,
  MANAGE 3.0.
- ISO/IEC 42001 composite: clauses 4–6 at 4.0, clauses 7–8 at 3.0,
  clauses 9–10 at 3.5.
- OWASP AI Security & Governance Checklist composite: 65% coverage
  at level 3+, 30% at level 2, 5% at level 1.

Two-year trajectory the head recommends:

- **NIST.** Move MEASURE from 2.5 to 3.5 by investing in evaluation-
  harness maturity at level 35 (the evaluation engineer's craft).
  Hold GOVERN at 3.5 in year one, move to 4.0 in year two after the
  council-attendance and decision-throughput metrics stabilise.
- **ISO.** Move clauses 7–8 (Support, Operation) from 3.0 to 3.5 by
  investing in competence-assessment automation and control-
  operation evidence tooling. Hold clauses 4–6.
- **OWASP.** Move the level-1-coverage 5% to level-2 minimum by
  end of year one, and lift the level-2 coverage 30% to level-3
  minimum by end of year two.

Deliberate under-investment: the head names that MANAGE will hold at
3.0 through the trajectory because the enterprise's incident-
response function is level-5 mature and the marginal move on MANAGE
is lower-return than the moves above.

Cost-of-move: three additional FTE at level 25 / 35 in year one; one
additional FTE at level 15 in year two; investment in the OSCAL /
CycloneDX evidence tooling; external red-team retainer for the OWASP
coverage moves.

Ask of the audit committee: endorsement of the trajectory, approval
of the three FTE ask, and approval of the tooling investment in the
year-one budget.

The audit committee sees the plot, the deltas, the trajectory, and
the asks. It debates the deliberate under-investment on MANAGE
(uncomfortable, but the enterprise has the incident-response cover
to defend it) and ratifies the trajectory. The output is a minuted
decision the head executes against for the year.

## Common failure modes

- **Score inflation.** Self-scored maturity drifts upward without
  evidence. The independent-challenge discipline prevents this;
  without it, year-over-year growth becomes decorative.
- **Composite-only reporting.** Reporting the composite without
  the per-axis plot hides where regressions or under-investment
  are living. Boards see through this quickly.
- **No under-investment declaration.** Naming every axis as
  level-5-in-two-years is not ambitious, it is unbudgeted. Boards
  discount trajectories that promise everything.
- **Detached from budget.** A trajectory without cost-of-move
  becomes aspirational. The head's job is to walk the trajectory
  into the budget cycle explicitly.
- **One-off assessment.** A maturity plot delivered once and not
  revisited is not maturity assessment; it is a snapshot.

## Summary

- Maturity assessment converts the head's operating discipline into
  a defensible trajectory, using three references — the NIST AI
  RMF Playbook, ISO/IEC 42001 AIMS maturity dimensions, and the
  OWASP AI Security & Governance Checklist — each on a distinct
  axis.
- A five-level vocabulary (Initial → Repeatable → Defined →
  Managed → Optimising) is used consistently so that composite,
  per-axis, and year-over-year plots are legible.
- Scoring is evidence-anchored; every level-3+ claim has linked
  evidence in AIMS document control. Independent challenge (CAE,
  external consultant, or peer head) defends the plot before it
  reaches the audit committee.
- The two-year trajectory is a document under AIMS document
  control, with explicit targets per axis, deliberate under-
  investment declarations, sector benchmarking, and regulatory-
  horizon alignment.
- Board and audit-committee reporting shows per-axis plots and
  the composite, year-over-year deltas coloured for improvements
  and regressions, the trajectory line, the specific resource
  asks, and an explicit limits-of-the-plot section.
- Composition with sector-specific references (SR 11-7, NAIC AI
  Model Bulletin, GMLP, OMB M-25-21, RSP / Preparedness / FSF for
  frontier labs, voluntary codes) adds axes without collapsing
  them into a single number.
