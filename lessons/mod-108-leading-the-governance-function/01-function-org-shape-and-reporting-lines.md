# The AI Governance Function — Org Shape, Reporting Lines, and Succession

## Motivation

The Head of AI Governance can author a defensible KRI portfolio
([[mod-107-program-measurement-and-maturity]] chapter 01), a
credible board pack ([[mod-103-board-and-audit-committee-reporting]]
chapter 01), and a running operating cadence
([[mod-102-running-the-program]] chapter 02) — and still be unable
to defend the program on the day the head leaves the room. If the
function's *org shape* has not been designed — if the level ladder
has been left implicit, if reporting lines have been drawn by
inheritance rather than by decision, if there is no named
successor for the head or for the level-50 architect — the program
depends on a specific person's presence, and that dependency is a
program-integrity failure the audit committee will name in the
first cycle it notices.

This chapter is how the head designs the function so it survives
the head's absence. Not headcount by role — that is the multi-year
hiring plan in chapter [[02-multi-year-hiring-plan]]. Not
individual development — that is the coaching cadence in chapter
[[03-coaching-and-career-pathing]]. This chapter is the *shape* —
what roles exist at what levels, what reports directly to the head
and what reports in via matrix, what the succession picture looks
like at each critical role, and how the shape reads to the CRO, the
CAE, and the audit committee as a legibly independent second-line
function.

The failure mode the chapter opens with is not a function without
people. It is a function where the head has hired capable people
but has never written down what each role owns, where the reporting
lines are ambiguous, and where the head is personally the
single-point-of-failure for every non-trivial governance decision.
A function shaped that way is a function that promotes the head
into unavailability and stalls when the head goes on leave, changes
role, or is displaced. The org shape is the antidote.

## Core concept — the second-line function has five archetypes

The AI-governance function at enterprise scope is built from five
role archetypes. These are the archetypes; the specific headcount
by archetype is the plan the head builds in
[[02-multi-year-hiring-plan]].

- **AI Governance Analyst (level 15).** Analyst legwork —
  intake queues for new AI systems, first-draft impact assessments,
  jurisdictional trackers, control-evidence collection, running the
  monthly and quarterly metric pipelines. The analyst is the
  function's operational load-bearer for volume; the function
  scales in analysts before it scales in any other archetype.
- **AI Risk Engineer (level 25).** Hands-on risk engineering —
  harm-model authoring, red-team execution against enterprise AI
  systems, adversarial-ML testing, fairness and privacy guardrail
  engineering, quantification of risk exposures. The risk engineer
  is the function's technical challenge capacity to the first-line
  product and engineering teams.
- **AI Evaluation Engineer (level 35).** Release-assurance
  methodology — audit-trail authoring, evaluation harnesses,
  regulator-facing evidence packages, sign-off engineering. The
  evaluation engineer is the function's methodology capacity — the
  role that turns ad hoc "we tested it" into repeatable evidence a
  certification body or a regulator inspector will accept.
- **Senior AI Governance Architect (level 50).** Architectural
  design authority — control library, policy taxonomy, cross-
  jurisdiction crosswalk, ISO/IEC 42001 AIMS scope, risk taxonomy
  and appetite, assurance architecture, evidence architecture,
  third-party program, post-market surveillance architecture,
  GRC-for-AI reference architecture, operating model, sector
  blueprints. The architect is the design authority the head
  *consumes from* and *sponsors*; see
  [[mod-101-role-scope-and-leadership-shape]] chapter 01 for the
  head-to-architect boundary.
- **Head of AI Governance (level 60).** Program leadership — the
  role the reader is preparing for. The head is the accountable
  executive for the second-line function; the head does not do
  analyst, engineer, evaluator, or architect work on the ladder
  below.

Some functions add a sixth archetype — an **Agentic Safety
Engineer (level 40)** for enterprises with frontier-agent surface —
per [[mod-101-role-scope-and-leadership-shape]] chapter 01. For
most enterprises this is a sideways-and-up specialisation on the
level-25 or level-35 role rather than a standing headcount slot,
and the head adds it when the enterprise's AI portfolio warrants
it (frontier-model deployment, autonomous-agent products at
material scope, or sector overlays that specifically demand it).

The ladder is what the enterprise's HR system reads; the archetype
descriptions are what the function reads. Both are authored by the
head with the level-50 architect and ratified by HR and the CRO
before first hire against the shape.

## Reporting-line decisions — directly reporting versus matrixed

Not every role in the function reports solid-line to the head.
The choice between solid-line reporting and matrixed reporting is
one of the most consequential design decisions the head makes,
and it is a decision the head takes explicitly rather than
inheriting from whatever shape the enterprise happened to have
when the head arrived.

Four common shapes.

**Shape A — fully-centralised.** All second-line AI-governance
roles report solid-line to the head. The head has full authority
over hiring, performance, career progression, and termination.
The advantage is unambiguous accountability — the head owns
outcomes because the head owns the people. The disadvantage is
distance from first-line product and engineering — a fully-
centralised function tends toward the *operational-distance
failure* that chapter [[04-second-line-independence-balance]]
opens with, where product engineers experience the second line
as a bureaucracy outside their world.

**Shape B — hub-and-spoke with product embeds.** The
architects, evaluation engineers, and risk engineers report
solid-line to the head at the hub; a subset of analysts and
possibly one risk engineer per major product line is embedded
in-product, matrixed to the head and dotted-line to the product
leadership. The advantage is closeness — the embedded analyst
sits in the product's rituals, knows the systems in flight
before the intake queue does, and translates the second-line
framework into product-native language. The disadvantage is
independence pressure — the embedded analyst hears the product's
reasons for shipping every day and can drift into first-line
sympathies without disciplined counterweight.

**Shape C — federated by risk domain.** The function is
organised around AI risk domains — model risk, third-party AI
risk, fairness and safety, compliance — with a lead per domain
reporting solid-line to the head, and the analysts and engineers
distributed among the domain leads. The advantage is domain
depth — the fairness lead builds a fairness bench, the model
risk lead builds a model-risk bench, and the function has
identifiable expertise per domain the CRO and CAE can consult.
The disadvantage is fragmentation — a new AI system that
touches multiple domains hits the intake queue and requires
handoffs between domains that may not be well-coordinated.

**Shape D — matrixed-from-source with a small hub.** The head
runs a small hub (a level-50 architect, one or two level-15
analysts) and the rest of the function's capacity is matrixed
from product, engineering, risk, audit, or legal. The advantage
is minimal standing headcount and rapid access to specialist
depth already inside the enterprise. The disadvantage is severe
independence pressure — the matrixed engineer's performance
review is written by their solid-line product manager, and no
amount of matrix-authority language changes the incentive shape
that creates.

Most established enterprises land at Shape B (hub-and-spoke with
embeds) as their steady-state, occasionally with Shape C overlays
for specific domains (a dedicated fairness lead in a customer-
facing consumer business, a dedicated third-party-risk lead in an
enterprise-heavy SaaS business). Shape A is common in the first
year of a function's standup while the head is still building
credibility with product; Shape D is common in very small
enterprises or as an interim before Shape A or B becomes
warranted.

The head does not pick a shape from fashion. The head picks a
shape from four inputs: the enterprise's own operating model
(centralised versus federated), the enterprise's AI portfolio
shape (concentrated in one product line versus distributed), the
CRO's operating model for other second-line functions (the head
does not run a shape that reads foreign to the CRO's other
second-line reports), and the maturity of the AI-governance
program (early programs need centralisation to build discipline;
mature programs can absorb the distributed complexity of Shape B
or C).

The shape decision is written down. It goes into the function's
operating charter — reviewed annually, ratified by the CRO,
copied to the CAE — so an incoming successor or an incoming CRO
inherits the reasoning rather than only the artefact.

## The reporting-line-decision table

For each role in the function, the head answers three questions
explicitly: to whom does the role report solid-line, to whom
dotted-line, and who writes the performance review. The three
questions have different answers per role, and the answers are on
the org chart the CRO and the CAE read.

| Question | What it decides |
|---|---|
| Solid-line report | The accountable manager. Owns objectives, deliverables, resourcing, and escalations. |
| Dotted-line report | The matrix partner. Consulted on objectives, has visibility, has veto on specific dimensions defined in the matrix charter. |
| Performance-review author | The person whose written opinion is the record of the year's performance. This is the *incentive owner*. If the performance-review author is not the same as the solid-line report, the person is being asked to serve two masters — a specific and named exception, not a default. |

For each role in the function, the head authors a one-line
statement: *"The `<role>` reports solid-line to `<X>`, dotted-line
to `<Y>`, with performance review authored by `<Z>`."* The statement
is on the function's operating charter and reviewed annually.

A worked example for a hub-and-spoke shape:

- *"The centralised **AI Governance Analyst** (control-evidence
  collection cluster) reports solid-line to the head, dotted-line
  to the Chief Risk Officer's second-line coordinator, with
  performance review authored by the head."*
- *"The embedded **AI Governance Analyst** (Product Line A) reports
  solid-line to the head, dotted-line to the Product Line A VP,
  with performance review co-authored by the head (as accountable
  executive for the function) and the Product Line A VP (as the
  operational context in which the analyst delivers), reconciled
  by the head."*
- *"The **AI Risk Engineer** reports solid-line to the head,
  dotted-line to the Chief Information Security Officer for
  offensive-security tooling authority, with performance review
  authored by the head."*
- *"The **AI Evaluation Engineer** reports solid-line to the head,
  dotted-line to the CAIO's release-management function for cross-
  program methodology coordination, with performance review
  authored by the head."*
- *"The **Senior AI Governance Architect** reports solid-line to
  the head, dotted-line to the CRO's second-line architecture
  council, with performance review authored by the head."*
- *"The **Head of AI Governance** reports solid-line to the CRO,
  dotted-line to the CAIO for AI-strategic-alignment coordination
  and to the General Counsel for legal-privilege coordination on
  regulator engagements, with performance review authored by the
  CRO with input from the CAIO and General Counsel."*

The head reports to the CRO in most enterprise shapes; some
enterprises route the head to the General Counsel, the Chief
Compliance Officer, or (rarely) the CAIO. The choice is a CxO-
scope decision the head does not unilaterally take; where the
head has a view, the head takes it into the CRO succession
conversation or the CxO-adjacency conversation
([[mod-101-role-scope-and-leadership-shape]] chapter 06) rather
than into the org chart.

## Level-ladder mapping — how a role progresses

The five archetypes are the level-15 → level-25 → level-35 →
level-50 → level-60 ladder. Progression through the ladder is
neither automatic nor guaranteed, but it is *possible*, and the
head owes every hire a clear picture of what progression looks
like from where they are today.

The ladder is not a single-file line. Each transition has
specific competence gates the head writes down and holds the
line on.

- **Level 15 → level 25.** The analyst has moved from executing
  first-draft impact assessments and evidence-collection to
  independently authoring risk analyses, running one specific
  engineering craft (harm-modelling, red-team, or fairness) to
  depth, and taking accountability for a small risk-engineering
  deliverable end-to-end. The gate is *technical craft depth on
  one domain* — the analyst who does everything competently at
  level 15 is not yet a level-25 engineer; the level-25 engineer
  is technically better than the level-15 analyst at their chosen
  domain, and the head does not promote laterally-competent
  analysts into engineer roles they will underperform.
- **Level 25 → level 35.** The risk engineer has moved from
  individual craft to *methodology* — the difference between
  running a good red-team on one system and authoring the red-team
  methodology the enterprise runs across systems, evolves against
  new attack shapes, and defends to certification bodies and
  regulators. The gate is *repeatable, defensible methodology
  authorship* — the engineer whose work depends on their personal
  touch is not yet at level 35; the level-35 evaluator writes the
  methodology that a competent level-25 engineer can execute
  reliably.
- **Level 35 → level 50.** The evaluation engineer has moved
  from methodology within a domain to *architecture across
  domains* — the ability to author the enterprise's control
  library across the full AI-risk surface, to reconcile
  competing framework requirements, and to write the operating
  design the head runs. The gate is *architectural authorship at
  enterprise scope* — an evaluator who has authored the release-
  assurance methodology for one product line has not
  automatically shown architectural range across the enterprise;
  the level-50 architect authors design that composes with the
  ISMS, with the model-risk-management framework, with the
  privacy program, and with sector overlays.
- **Level 50 → level 60.** The architect has moved from design
  authority to program leadership. This is the transition the
  head themselves made (or will make) at some point, and it is a
  step that most level-50 architects do not take — the design
  craft and the program-leadership craft are legitimately
  different disciplines, and an architect who is world-class at
  the former can be a mediocre head. The gate is *demonstrated
  program leadership at scale* — successful sponsorship of
  large-scope design at board level, credible cross-CxO
  coordination, and demonstrated capacity for the difficult-
  conversation shape in
  [[mod-103-board-and-audit-committee-reporting]] chapter 06. See
  chapter [[03-coaching-and-career-pathing]] for how the head
  develops a level-50 architect toward level-60 readiness
  intentionally, and chapter [[07-difficult-people-leadership-conversations]]
  for the conversation the head has when an architect is
  genuinely not going to make the level-60 transition.

Not every level transition is upward-only. A level-25 engineer
who has developed depth on the evaluation-engineer craft and
wants to build methodology authority moves to level-35; a level-
35 evaluator who prefers the individual-contributor risk-
engineer craft over methodology authorship may stay at level-35
for years, and the head respects that choice. The ladder is a
map, not an obligation.

The level-ladder mapping is documented per-role at hire and
reviewed at each performance cycle. The documentation includes
the current level, the next level's competence gate, the
specific development actions the individual and the head have
agreed to, and the honest read on time-to-readiness. See
chapter [[03-coaching-and-career-pathing]] for the cadence.

## Succession planning — the head's discipline

The head's own succession is the audit committee's
responsibility (via the CRO in most reporting shapes), not the
head's. But the head owns succession for every role below the
head — and the head owes the CRO an *honest* succession picture
for the head's own role, so that the CRO's own succession
planning has real inputs to work from.

Succession is authored per role, reviewed annually, and
minuted with the CRO. For each of the critical roles in the
function, the head answers four questions.

1. **Who is the ready-now successor.** A named individual (or,
   honestly, none). If none, the head names the fact — "no
   ready-now successor" — and does not paper it over.
2. **Who is the ready-in-one-year successor.** A named
   individual with a specific development path in flight. If
   none, the head names the fact and describes the sourcing
   strategy (internal development, external hire, or matrix
   arrangement).
3. **Who is the ready-in-three-years successor.** A named
   individual (typically at a level below the target level today),
   with a development trajectory that composes with the coaching
   cadence in chapter [[03-coaching-and-career-pathing]].
4. **What the interim looks like on unexpected departure.** If
   the incumbent leaves tomorrow, what does the function do
   between the departure and the successor's readiness? Who
   covers, at what capacity, for how long, and at what cost to
   the rest of the function's delivery?

The critical roles the head plans succession for:

- **The head themselves.** Honest read to the CRO. Typically the
  ready-now successor is either the level-50 architect (if the
  architect has been developed for the transition) or an external
  hire; the ready-in-three-years successor is a level-35 or
  level-50 individual under active development. The head who
  presents "myself" as the only defensible occupant of the head
  role is a head who has failed at succession planning; that read
  is what the audit committee escalates.
- **The level-50 architect.** The single most technically load-
  bearing role in the function. A level-50 architect who leaves
  without a successor picture leaves the function running on
  documented artefacts alone, and documented artefacts age
  faster than a live design authority can maintain. The ready-
  now successor is typically an external hire (the level-50
  bench in most sectors is genuinely thin); the ready-in-three-
  years successor is a level-35 evaluation engineer under
  intentional development.
- **The level-35 evaluation engineer(s).** Each evaluation
  engineer has a distinct methodology surface; each surface
  needs a named successor with a development path.
- **The level-25 risk engineer(s).** Distinct crafts (red-team,
  fairness, adversarial-ML) each have a small talent pool, and
  the head's succession picture per craft is honest about
  whether the enterprise's own bench is deep enough to backfill.
- **Any embedded analyst positions** (Shape B). An embedded
  analyst who leaves takes their product-line context with
  them; the head plans for continuity.

The head does not plan succession only for the roles the head
would find easy to replace. Succession discipline reads on the
roles the head would find *hard* to replace — and the CRO reads
the head's discipline on those hard cases as the signal of
whether the head is running a function that survives departures
or a function that depends on lucky retention.

## The org-chart artefact

The function has one canonical org chart. It is under document
control (versioned in the same system as the AIMS scope
statement — see [[mod-102-running-the-program]] chapter 04),
refreshed at least annually and at any material org change, and
distributed to the CRO, the CAE, the CAIO, the General Counsel,
and the audit committee secretariat.

The chart includes:

- **Boxes for each role,** labelled with role title, level, and
  incumbent (or "vacant" with the recruitment status).
- **Solid lines** for solid-line reporting.
- **Dotted lines** for material dotted-line reporting; the chart
  legend explains what each dotted-line means (matrix authority,
  performance-review co-authorship, escalation adjacency).
- **A one-page cover** summarising the shape decision (A / B /
  C / D per the taxonomy above), the reporting-line-decision
  table extract for the head-critical roles, and the current
  succession-status summary (ready-now / ready-in-one-year /
  ready-in-three-years counts across critical roles, with
  material gaps flagged).

The chart is not the head's slide. It is a governance artefact.
The CRO and the CAE both read it; changes to it are minuted;
material re-shapings (a move from Shape A to Shape B, a
consolidation of federated domains, a matrix change on a
material role) go through the same change-management ratification
as any other second-line design change.

## Anti-patterns the head does not permit

**The invisible ladder.** The function has hires but no
published ladder. Analysts do not know how they progress to
engineer; engineers do not know how they progress to evaluator.
The result is that talented analysts leave for external
opportunities that offer clearer progression, and the head
loses the internal bench that would have carried succession.
The remedy is the published level-ladder mapping and the
progression conversation as part of the coaching cadence
(chapter [[03-coaching-and-career-pathing]]).

**The everyone-solid-line-to-the-head shape without justification.**
The head has drawn Shape A because Shape A is the shape the head
had at the head's previous enterprise, or because it is the
shape that felt most authoritative on arrival. But the enterprise
runs its other second-line functions matrix-heavy, and Shape A
reads as the head refusing the enterprise's operating model. The
remedy is the shape-decision written down with the four inputs
above, and Shape A justified explicitly if chosen against the
enterprise's default.

**The "we'll figure it out later" succession posture.** The head
lists all critical roles as "no ready-now successor" and treats
it as acceptable because succession is a future problem. The
audit committee reads this as key-person dependency, and the
head loses the discipline argument in the room. The remedy is
the honest succession read with active development in flight for
every critical role — a "no ready-now successor" is acceptable
for a role only if the "ready-in-one-year" and "ready-in-three-
years" cells are filled with named individuals under active
development.

**The org chart that lives on the head's laptop.** The chart
exists but is not under document control, is not distributed to
the CRO and CAE, and is not refreshed on a cadence. Changes to
the function happen without the chart moving, so the chart
becomes progressively wrong until nobody trusts it. The remedy
is the canonical version-controlled chart with an owner (the
head's own executive assistant or a level-15 analyst on
operations), a refresh cadence, and a distribution list.

**The matrix-charter-that-isn't.** The head has drawn dotted-
lines on the org chart but has not authored the matrix charter
that says what each dotted-line means. Dotted lines without
charter are decorative; matrixed partners do not know what they
are entitled to expect and neither do the matrixed individuals.
The remedy is the matrix-charter-per-dotted-line, ratified by
both parties (the head and the matrix partner), reviewed
annually.

## Composition with adjacent modules

- **The level-ladder architecture** in
  [[mod-101-role-scope-and-leadership-shape]] chapter 01 is the
  authoritative source for the archetype level assignments.
  This chapter runs the shape decision on top of that ladder,
  not against it.
- **The IIA Three Lines Model** in
  [[mod-101-role-scope-and-leadership-shape]] chapter 04 sets
  the second-line-versus-first-line boundary the shape has to
  respect. Chapter [[04-second-line-independence-balance]] runs
  that boundary as an operating discipline.
- **The CxO adjacency positioning** in
  [[mod-101-role-scope-and-leadership-shape]] chapter 06 is
  where the head-to-CRO reporting line lives; the shape decision
  here composes with that adjacency.
- **The AIMS operating calendar** in
  [[mod-102-running-the-program]] chapter 02 is where the org-
  chart refresh cadence lives.
- **The multi-year hiring plan** in
  [[02-multi-year-hiring-plan]] takes the shape as its input and
  builds the headcount trajectory across years.
- **The coaching cadence** in
  [[03-coaching-and-career-pathing]] runs the progression
  conversations the level-ladder mapping frames.
- **The CAE coordination** in
  [[05-cae-and-third-line-coordination]] uses the org chart as
  one of its authoritative artefacts; the CAE tests whether the
  function's shape is what the head describes it is.
- **The succession discipline** feeds
  [[mod-112-certifications-career-path-community-leadership]]
  where the head's community and certification investments
  strengthen the internal succession bench.

## Summary

- The AI-governance function is built from five role archetypes
  on the level ladder: analyst (15), risk engineer (25),
  evaluation engineer (35), senior architect (50), and head (60),
  with agentic safety engineer (40) as a sideways-and-up
  specialisation where the AI portfolio warrants it.
- The head picks a shape explicitly from four candidates —
  fully-centralised (A), hub-and-spoke with product embeds (B),
  federated by risk domain (C), or matrixed-from-source with a
  small hub (D) — based on the enterprise's operating model, AI
  portfolio shape, CRO's other-function shape, and the program's
  maturity. The shape decision is written into the function's
  operating charter.
- For each role, the head writes down the solid-line report, the
  dotted-line report, and the performance-review author. Where
  the performance-review author is not the solid-line manager,
  the exception is named and justified.
- The level-ladder mapping is documented per role at hire, with
  a specific competence gate for each next level. Progression is
  possible; automatic promotion is not.
- Succession is planned per critical role with a ready-now
  successor, a ready-in-one-year successor, a ready-in-three-
  years successor, and an interim plan on unexpected departure.
  The head names "no successor" honestly where it applies rather
  than papering over the gap.
- The org chart is a canonical, document-controlled artefact
  distributed to the CRO, the CAE, the CAIO, the General
  Counsel, and the audit committee secretariat. It is refreshed
  at least annually and at any material org change.
- Four anti-patterns the head refuses: the invisible ladder, the
  everyone-solid-line-to-the-head shape without justification,
  the "we'll figure it out later" succession posture, and the
  org chart that lives on the head's laptop; plus the matrix-
  charter-that-isn't when dotted lines lack a written matrix
  charter.
- Chapter [[02-multi-year-hiring-plan]] takes the shape and
  builds the multi-year headcount trajectory; chapter
  [[03-coaching-and-career-pathing]] runs the coaching and
  progression cadence against the ladder; chapter
  [[04-second-line-independence-balance]] runs the shape as an
  operating discipline against the first-line closeness/
  independence balance; chapter
  [[05-cae-and-third-line-coordination]] hands the shape to the
  CAE as one of the third-line-audit-programme's read artefacts.
