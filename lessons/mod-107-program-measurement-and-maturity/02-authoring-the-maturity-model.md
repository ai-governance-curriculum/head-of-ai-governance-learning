# Authoring the Enterprise AI-Governance Maturity Model

## Motivation

A maturity plot the enterprise produces is only as defensible as
the *model* the plot is scored against. If the model is a set of
five loose paragraphs the head wrote in a document last summer,
the plot will not survive challenge — from an external auditor,
from the third-line CAE, from a peer head in a benchmarking
exchange, or from a board director who has run a maturity model
before and can smell one that has not been authored.

The head does not pick a published maturity model off the shelf.
Every published reference measures something the enterprise cares
about, and none of them measures the specific shape of the
enterprise's AI-governance program on its own. The head authors
the *enterprise's own* maturity model, drawing on the published
references as inputs, and takes the accountability for the model
that the plot is scored against.

This chapter is how the head authors that model. Chapter
[[01-kri-kpi-portfolio]] gives the running-cadence numbers; this
chapter gives the annual-cadence maturity backbone;
chapter [[03-annual-maturity-assessment]] runs the actual
assessment against the model.

The failure mode the chapter opens with is the head who "adopted
NIST AI RMF as our maturity framework" without noticing that the
NIST AI RMF is not a maturity model — it is a risk-management
framework. The Playbook contains suggested actions at varying
depths that a maturity model can be *built from*; the framework
itself is not a scale, and a plot presented as "our NIST AI RMF
maturity" without a scale specification is a plot the head cannot
defend. The chapter is the discipline that prevents that failure.

## Core concept — the five input references and what each contributes

Five published references contribute distinct axes to a
defensible enterprise maturity model. The head reads each for
what it contributes, not for what it purports to be.

### NIST AI RMF Playbook — the leadership-shape axis

The NIST AI Risk Management Framework 1.0 (AI 100-1) is a
voluntary framework organised around four functions — GOVERN,
MAP, MEASURE, MANAGE — with categories and subcategories under
each. The AI RMF Playbook, hosted at the AI Resource Center,
offers suggested actions and transparency-and-documentation
practices per subcategory.
<!-- needs-research: verify the current published state of the
NIST AI RMF Playbook against airc.nist.gov, including the AI RMF
1.0 base document and any generative-AI profile updates. Confirm
which subcategories carry the most granular Playbook actions
that a maturity scoring can lean on. -->

What the Playbook contributes to a maturity model is a *coverage*
axis — for each subcategory, has the enterprise addressed the
Playbook's suggested actions, at what depth, and with what
transparency-and-documentation evidence. The head interprets
"depth" against the enterprise's own maturity scale (below), so
that "coverage of GOVERN 1.1 at depth 4" is a defensible score
rather than an opinion. The GOVERN function in particular is
where leadership-shape maturity lives: policies, accountability
structures, workforce roles, and third-party governance.

### ISO/IEC 42001 — the management-system axis

ISO/IEC 42001:2023 is the AI management system standard,
authored on the Harmonised Structure common to ISO management-
system standards (ISO 9001, ISO/IEC 27001, ISO 22301, ISO 14001).
Its clauses 4–10 (context, leadership, planning, support,
operation, performance evaluation, improvement) plus Annex A
controls describe an AI management system a certification body
can assess conformance against.

What ISO/IEC 42001 contributes to a maturity model is a
*management-system* axis. The Harmonised Structure clauses are
not maturity levels — conformance is binary at the audit — but
the *depth* at which each clause is operating (documented,
measured, improved) maps onto a maturity scale. A clause 9.1
that produces annual monitoring outputs alone is at a different
maturity depth than a clause 9.1 that produces monthly
monitoring outputs with automated escalation to the AIMS
management review.

The head reads ISO/IEC 42001 as a management-system spine — the
model's structure — and reads the maturity depth per clause and
per Annex A control as a separate scoring layer. See
[[mod-102-running-the-program]] chapter 04 for the crosswalk the
head runs between the AIMS controls and the enterprise's specific
regulatory obligations; the crosswalk is the map, and the
maturity model puts a depth score on each map cell.

Companion standards extend the axis:

- **ISO/IEC 42005:2025** on AI system impact assessment — depth
  of the enterprise's AIA process.
- **ISO/IEC 42006:2025** on audit and certification of AI
  management systems — the certification-body-facing view of
  what mature looks like.
- **ISO/IEC 23894:2023** on AI risk management guidance —
  supporting depth on the risk-management vocabulary the model
  uses.

### IAPP AIGP body of knowledge — the practitioner-competence axis

The IAPP Artificial Intelligence Governance Professional (AIGP)
certification is anchored on a published Body of Knowledge (BoK)
that enumerates the domains and competencies an AI governance
professional is expected to hold.
<!-- needs-research: verify the current version of the IAPP AIGP
Body of Knowledge against iapp.org, including the specific
domains and the current examination blueprint. Confirm the BoK's
adjacency to the AIGP examination and its intended use as a
practitioner-competence reference. -->

What the AIGP BoK contributes to a maturity model is a
*practitioner-competence* axis. Enterprise AI-governance maturity
is not only a matter of documented processes and management-
system depth; it is a matter of whether the people running the
processes hold the competencies to run them well. A high maturity
score on the ISO axis coexisting with a low AIGP-BoK-coverage
score on the head's own team is a diagnostic — the processes are
authored, but the people running them are not yet trained. That
diagnostic feeds the training and certification investment in
chapter [[05-program-cost-management]].

The head reads the BoK against the team's current certification
and competence profile, and against the sector-specific
competencies the sector-program-leadership chapter of
[[mod-111-sector-program-leadership]] adds.

### MLCommons AI Safety and evaluation benchmarks — the technical-evaluation axis

MLCommons is the open engineering consortium best known for the
MLPerf benchmark suites. The AI Safety Working Group develops
evaluation suites for AI safety hazards, including the AILuminate
benchmark for text-based safety hazards.
<!-- needs-research: verify the current published state of
MLCommons AI Safety benchmarks against
mlcommons.org/working-groups/ai-safety/ai-safety/, including
AILuminate current version and coverage, and any adjacent
benchmark suites the working group has published. Confirm the
current recommended-practice framing for enterprise participation
in the benchmark cycle. -->

What MLCommons benchmarking contributes to a maturity model is a
*technical-evaluation* axis — whether the enterprise's AI
evaluation practice is at the depth of running published
industry-reference benchmarks, or is producing bespoke internal
evaluations only, or is not producing evaluations at all. For
enterprises with generative-AI surface, the axis is directly
comparable to peer disclosure and to certification-body
expectations; for enterprises with only classical-ML surface, the
axis is thinner but the shape carries — running published
benchmarks (Aequitas, Fairlearn, IBM AIF360-family evaluations,
whatever is in current publication) at cadence is a maturity
signal.

The axis composes with the OWASP AI Security & Governance
Checklist / OWASP LLM Top 10 / OWASP Machine Learning Security
Top 10 coverage the level-50 architect maintains for the
enterprise's security-and-adversarial-robustness posture — see
[[mod-102-running-the-program]] chapter 05.

### ForHumanity IAAIS — the independent-audit-readiness axis

ForHumanity's Independent Audit of AI Systems (IAAIS) programme
publishes criteria for independent auditors auditing AI systems
against a defensible criterion base.
<!-- needs-research: verify the current published state of the
ForHumanity IAAIS criteria and any adjacent ForHumanity certified
auditor programme against forhumanity.center. Confirm the
criteria's current scope (algorithmic bias, ethics, privacy,
trust — or the current organisation of criteria) and the
intended use as an audit criterion set rather than as a
management-system standard. -->

What IAAIS contributes to a maturity model is an *independent-
audit-readiness* axis. The IAAIS criteria are the shape of what
an independent auditor with an ethics-and-trust-oriented
methodology tests against; the enterprise's readiness against
those criteria is a distinct depth from ISO/IEC 42001 clause
maturity (which is management-system-oriented) or NIST RMF
coverage (which is risk-management-oriented). The axis is a
useful counter-signal — enterprises with high maturity on the
first two axes can nonetheless have gaps on the ethics-and-
independent-audit-readiness axis, and the audit committee reads
that gap as consequential.

## The five-level vocabulary — one scale, applied uniformly

The five references above measure different things, but the
maturity *scale* is common across all axes. The head uses a
single five-level vocabulary derived from CMMI-style progression
so that scores are legible when plotted together and comparable
across axes and across years.

- **Level 1 — Initial / ad hoc.** The activity happens; it is
  not yet consistent, documented, or reliably repeatable.
- **Level 2 — Repeatable.** The activity is repeated with basic
  documentation; individuals rather than the process ensure
  consistency.
- **Level 3 — Defined.** The activity is documented as a
  standard process; roles and responsibilities are clear; the
  process operates without reliance on specific individuals.
- **Level 4 — Managed.** The activity is measured, results are
  analysed, and the process is adjusted based on measurement.
  KPIs or maturity metrics are in place.
- **Level 5 — Optimising.** The activity is under continual
  improvement, with data-driven refinement; the process
  contributes to the enterprise's competitive posture.

The vocabulary matches the vocabulary the CISO, CRO, and CAE
already use for adjacent maturity work — the head does not
invent a new scale. Enterprises that use bespoke sector-tuned
scales (some banks use OSFI E-23-aligned tiering; some frontier
labs use RSP / Preparedness / FSF capability-tier language) use
those instead — but the plot is always five levels, so trend
visualisation stays legible and the audit-committee director who
has seen a maturity plot before recognises this one.

## The tier definitions — what "level 3 GOVERN 2.1" actually means

The head's model has to answer the question "what does level 3
on this axis at this cell actually require". Without that answer,
scoring is opinion. The tier definitions are the load-bearing
craft of the model.

The discipline: for each axis and, where the axis has
subcategories or clauses, for each subcategory or clause, the
model specifies:

- **What level 2 requires.** The minimum evidence set for the
  activity being repeatable — typically a documented procedure
  and a record of at least one execution against it.
- **What level 3 requires.** The evidence set for the activity
  being a defined standard process — documented procedure,
  named accountable owner, roles-and-responsibilities RACI,
  training record for role-holders, and a record of consistent
  execution over the reporting period.
- **What level 4 requires.** The evidence set for the activity
  being measured and adjusted — a KPI or maturity metric in
  chapter [[01-kri-kpi-portfolio]], a target range, a
  measurement cadence, evidence of the target range being
  monitored, and evidence of at least one management adjustment
  based on measurement.
- **What level 5 requires.** The evidence set for the activity
  being under continual improvement — level 4 plus a documented
  improvement plan, evidence of iterative improvement over
  multiple cycles, and, ideally, evidence that the practice is
  informing peer practice through standards-body participation
  ([[mod-106-external-positioning-and-voluntary-codes]] chapter
  02) or peer disclosure.

The tier definitions are the model's contract with the scorer.
An architect scoring "level 4 GOVERN 2.1" against the model is
committing that the evidence set for level 4 is in place. An
external auditor testing the score can then test against the
same evidence set — and the score either survives the audit or
does not.

The tier definitions are written by the level-50 architect, not
by the head personally. The head reviews and ratifies them; the
architect authors. This is the same pattern as the AIMS control-
set authorship in [[mod-102-running-the-program]] chapter 04.

## Deliberate under-investment — building the "we will not target level 5" discipline into the model

The maturity model has to permit — and the head has to
articulate — the discipline of *deliberate under-investment*.
Not every axis, and not every subcategory, should be targeted at
level 5. Enterprise resources are finite. A model that implicitly
assumes every axis will reach level 5 in a two-year horizon is a
model that will oversell capacity and disappoint the board.

The model supports this by carrying two annotations per axis and
per subcategory:

- **Target level.** What the enterprise is targeting on a
  two-year horizon.
- **Rationale for the target level.** Why this target and not a
  higher target — resource constraint, lower-return compared to
  another investment, sector-benchmark-adequate, deliberate
  choice not to lead on this dimension.

The rationale is where deliberate under-investment lives. A
subcategory where the enterprise's target is level 3 in year two
carries a rationale that names the reason: "the enterprise's
incident-response function is level-5 mature and the marginal
return on further MANAGE maturity is lower than the return on
MEASURE investment"; or "sector peers as evidenced by the
sector-body disclosure surface are operating at level 3 on this
subcategory and level-3 is defensible against peer benchmark";
or "this dimension is under active regulatory-change monitoring
and the enterprise will target level 4 only once the regulatory
target has stabilised".

Boards read deliberate under-investment as *mature*. Boards read
"everything to level 5" as *unbudgeted*. The head sets the
posture in the model, not in the annual assessment; the
assessment then reports against the target rather than against
an unstated ceiling of five.

## Composition rules — how the axes plot together

The five axes are distinct, and the composite plot is not their
average. Averaging launders red axes into amber and hides the
signal the axis carries. The head's composition rules:

- **Report per axis first.** The audit committee sees the NIST
  plot, the ISO plot, the AIGP plot, the MLCommons plot, and the
  IAAIS plot before it sees any composite view.
- **The composite is a summary read.** If the head produces a
  composite (some audit committees ask for one for the trajectory
  view), the composite carries a note stating what it is and what
  it is not — "arithmetic mean of per-axis composite scores,
  weighted equally; does not reflect axis-specific severity".
- **Red on any axis is a signal, not an average.** A single axis
  at level 1 or level 2 in the base of the plot warrants the
  committee's attention even if the composite is level 3.
  Composite arithmetic that promotes an axis-1 signal to
  composite-3 is a discipline break.
- **Cross-axis diagnostics are named.** If GOVERN (NIST) is at
  level 4 and clause 5 (ISO) is at level 3, the model's
  interpretation is that leadership-shape maturity has outrun
  management-system maturity — the interpretation is diagnostic
  and it names the corrective. Cross-axis interpretation is where
  the level-50 architect earns their level.

## Assessment cadence — the model's operating rhythm

The model has an operating cadence, without which it decays.

- **Annual full assessment.** The full assessment against all
  five axes runs on the AIMS operating calendar (see
  [[mod-102-running-the-program]] chapter 02), typically in Q4
  so the output feeds the next year's objectives and risk-
  treatment plan refresh in Q1.
- **Mid-year trajectory read.** A lighter read at the six-month
  mark tests whether the year's trajectory move is on pace. The
  mid-year read is not a re-score; it is a read on evidence
  accumulation against the year's planned moves. If the moves
  are on pace, the mid-year read reports "on trajectory". If the
  moves are behind, the read reports the specific slippage and
  what the head is doing about it.
- **Model-version review.** The model itself — the tier
  definitions, the axes in scope, the sector overlays — is
  reviewed annually before the assessment runs, so that the
  assessment scores against a current model rather than against
  last year's model plus this year's assumptions. Version-
  controlled changes are minuted at the AI Governance Council;
  material changes are ratified at the audit committee before
  the annual assessment.
- **Sector-overlay refresh.** Sector maturity references (SR
  11-7, OSFI E-23, NAIC AI Model Bulletin, GMLP, OMB M-25-21,
  RSP / Preparedness / FSF for frontier labs, EU AI Act GPAI
  Code of Practice for signatories) are refreshed as the
  underlying regime evolves. The scanning system in
  [[mod-105-regulatory-change-management]] chapter 01 catches
  the regime changes; the model owner (level-50 architect)
  translates them into overlay updates.

An assessment that runs annually without a mid-year read is an
assessment the audit committee experiences as a surprise every
Q4. An assessment with a mid-year read is one the audit
committee experiences as a trajectory it can track. The
difference is the head's authoring choice.

## Composition with sector overlays

The base five-axis model composes with sector overlays where the
enterprise operates in a regulated sector. The overlays add
axes; they do not modify the base.

- **Banking (US and Canada).** Add a model-risk-management (MRM)
  axis anchored on Federal Reserve SR 11-7 and OCC 2011-12 (US)
  or OSFI E-23 (Canada) maturity. The enterprise's MRM function
  usually owns the axis; the head consumes it into the composite.
- **Insurance (US).** Add a NAIC AI Model Bulletin adoption
  coverage axis and, where the Colorado Division of Insurance
  Regulation 10-1-1 applies, a Regulation-10-1-1-conformance
  axis.
- **Health / medical device.** Add an FDA Good Machine Learning
  Practice (GMLP) axis for enterprises with AI/ML SaMD surface,
  and a Predetermined Change Control Plan (PCCP) maturity axis.
- **Public sector (US federal).** Add an OMB M-25-21 governance
  requirements axis, and, for federal contractors, agency-specific
  minimum practice axes as they apply.
- **Frontier labs.** Add a capability-tier framework maturity axis
  (Responsible Scaling Policy for Anthropic-comparable enterprises;
  Preparedness Framework for OpenAI-comparable enterprises;
  Frontier Safety Framework for Google DeepMind-comparable
  enterprises) at the depth [[mod-103-board-and-audit-committee-reporting]]
  chapter 07 develops.
- **EU AI Act — high-risk system provider or deployer.** Add an
  Annex III / Article 26 obligation coverage axis at the
  depth the enterprise's Article 26 or Article 16 posture
  requires.

Composition is additive. Each overlay is a distinct axis with
its own five-level tier definitions authored by the level-50
architect. The base composite reports base axes; the sector-
composite reports base plus overlays; both are on the annual
plot.

## Anti-patterns the head does not permit

Three anti-patterns the head names and refuses to permit in the
model.

**The single-axis model.** "Our maturity model is ISO/IEC 42001
clause maturity" is an under-authored model. The management-
system axis is one of five; treating it as the whole is a
discipline break the audit committee will notice the moment a
sector regulator asks about the enterprise's NIST RMF coverage
and the head has no answer.

**The averaged composite.** A single "AI governance maturity"
number aggregating the axes into a mean. The composite is
readable but it launders red axes into amber and amber axes
into green. The remedy is the per-axis reporting discipline
above.

**The self-scored ceiling.** The model that permits any score
without a specification of what evidence is required for that
score. Level 4 has to *mean* something — a set of evidence a
scorer produces — or the plot is opinion. The tier definitions
are the discipline; a level-4 score without the level-4
evidence set fails the audit and, more importantly, the head
loses the ability to defend the plot at the audit committee.

## Composition with adjacent modules

The maturity model composes with the adjacent modules the head
runs:

- The **AIMS operating calendar** in [[mod-102-running-the-program]]
  chapter 02 carries the annual assessment cadence and the
  mid-year read as calendar events.
- The **AIMS control set** in [[mod-102-running-the-program]]
  chapter 04 is the source of the ISO/IEC 42001 axis's scoring
  cells.
- The **evidence discipline** in [[mod-102-running-the-program]]
  chapter 06 (inventory) and chapter 07 (supply-chain evidence)
  is where the level-3+ evidence-set claims are supported.
- The **AI Governance Council** in [[mod-102-running-the-program]]
  chapter 01 ratifies material model-version changes.
- The **risk-appetite framework** in [[mod-103-board-and-audit-committee-reporting]]
  chapter 03 is the reference for the appetite-anchored
  target-level rationale on axes where appetite is the
  controlling constraint.
- The **audit committee** in [[mod-103-board-and-audit-committee-reporting]]
  chapter 02 is the ratifying body for material model changes
  and for the trajectory the annual assessment reports against.
- The **regulatory-change discipline** in
  [[mod-105-regulatory-change-management]] chapter 01 feeds
  sector-overlay refreshes.
- The **standards-body participation portfolio** in
  [[mod-106-external-positioning-and-voluntary-codes]] chapter
  02 informs which reference bodies the head reads as sector
  benchmarks and what standing engagement the head has with the
  reference-producing communities.
- The **staffing and hiring plan** in [[mod-108-leading-the-governance-function]]
  is the corrective when the AIGP-BoK axis flags a competence
  gap.
- Chapter [[03-annual-maturity-assessment]] carries the
  assessment itself; chapter [[04-roi-reporting-to-cfo]]
  carries the ROI framing the maturity trajectory anchors on;
  chapter [[05-program-cost-management]] carries the cost of
  the moves the trajectory commits to; chapter
  [[06-difficult-measurement-conversations]] carries the
  rehearsal for when the maturity plot goes red or when peers
  have surpassed the enterprise.

## Summary

- The head authors the enterprise's own maturity model. Off-the-
  shelf references are inputs, not the model. The head is
  accountable for the model the plot is scored against.
- Five reference axes contribute distinct dimensions: NIST AI
  RMF Playbook (leadership shape), ISO/IEC 42001 (management
  system), IAPP AIGP body of knowledge (practitioner
  competence), MLCommons AI Safety benchmarks (technical
  evaluation), and ForHumanity IAAIS (independent-audit
  readiness).
- The scale is a common five-level vocabulary
  (Initial → Repeatable → Defined → Managed → Optimising) across
  all axes. The head does not invent a bespoke scale where a
  CMMI-adjacent scale is already in enterprise use.
- Tier definitions specify, per axis and per scoring cell, what
  evidence set is required for level 2 through level 5. Without
  the definitions, scoring is opinion. Level-50 architect
  authors; head ratifies.
- The model carries per-cell target levels *and* target-level
  rationales. Deliberate under-investment is a mature discipline
  and lives in the rationale annotation, not in a footnote to
  the plot.
- Composition rules: per-axis reporting first; composite as a
  summary read with an explicit interpretation note; red on any
  axis is a signal, not an average; cross-axis diagnostics are
  named.
- Assessment cadence: annual full assessment (Q4), mid-year
  trajectory read (six-month mark), annual model-version review
  before the assessment, sector-overlay refresh as regimes
  evolve.
- Sector overlays are additive: banking (SR 11-7 / OSFI E-23),
  insurance (NAIC AI Model Bulletin / Colorado Reg 10-1-1),
  health / medical device (GMLP / PCCP), public sector (OMB
  M-25-21), frontier labs (capability-tier frameworks), EU AI
  Act high-risk provider or deployer.
- Three anti-patterns the head refuses: the single-axis model,
  the averaged composite, and the self-scored ceiling.
- Chapter [[03-annual-maturity-assessment]] turns to running
  the assessment against the model; chapter
  [[04-roi-reporting-to-cfo]] turns to the ROI shape the
  maturity trajectory anchors on.
