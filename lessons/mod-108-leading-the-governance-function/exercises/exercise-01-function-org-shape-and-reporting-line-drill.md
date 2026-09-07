# exercise-01: Function Org Shape and Reporting Line Drill

**Estimated effort:** 3 hours

## Objective

Author the enterprise's **AI-governance function org chart** —
the shape decision (A / B / C / D per the chapter-01 taxonomy),
the level-ladder assignments across the five role archetypes,
the reporting-line-decision table (solid-line, dotted-line, and
performance-review author per role), and the succession picture
per critical role (ready-now, ready-in-one-year, ready-in-three-
years, interim on unexpected departure). The deliverable is the
canonical, document-controlled artefact the head takes to the
CRO for annual ratification, the artefact the CAE reads as one
of the third-line-audit's inputs (chapter
[05-cae-and-third-line-coordination](../05-cae-and-third-line-coordination.md)),
the artefact an incoming head inherits on day one, and the
artefact the audit committee secretariat holds in the
governance-artefact register.

The chart has to survive three stress tests. First, the CRO's
second-line coordinator reads the chart against the other
second-line functions and asks why the AI function's shape
differs where it does — the shape rationale in the operating
charter has to carry the answer without redefinition. Second,
an incoming CAE asks who owns what in the function on their
first working session with the head — the reporting-line-
decision table has to make the answer immediate. Third, the
head goes on unexpected leave and the level-50 architect steps
in as interim — the succession picture has to describe the
interim in enough specificity that the architect knows what
they are running.

The chart is not the head's slide. It is a governance artefact.

## Prerequisites

- Chapter [01-function-org-shape-and-reporting-lines](../01-function-org-shape-and-reporting-lines.md)
  — the five role archetypes, the four shape candidates, the
  four inputs to the shape decision, the reporting-line-
  decision table format, the level-ladder mapping, and the
  four-cell succession picture — read and internalised.
- [[mod-101-role-scope-and-leadership-shape]] chapter 01 for
  the authoritative level-ladder architecture the archetype
  assignments derive from; chapter 04 for the IIA Three Lines
  Model at leadership scope that the reporting-line pattern
  respects; chapter 06 for the CxO adjacency positioning that
  fixes the head-to-CRO reporting line.
- [[mod-102-running-the-program]] chapter 02 (AIMS operating
  calendar) for the org-chart refresh cadence.
- Chapters [02-multi-year-hiring-plan](../02-multi-year-hiring-plan.md)
  and [03-coaching-and-career-pathing](../03-coaching-and-career-pathing.md)
  for downstream reads on the chart — the hiring plan builds
  headcount against the shape; the coaching cadence runs
  progression against the ladder.
- Chapter [05-cae-and-third-line-coordination](../05-cae-and-third-line-coordination.md)
  because the chart is one of the artefacts the head hands to
  the CAE on any audit engagement; the shape has to be legible
  to the CAE without a walking tour.
- A concrete enterprise in mind — sector (banking, insurance,
  health / medical device, pharma, public sector, frontier lab,
  tech platform, industrial), operating-model shape
  (centralised versus federated at enterprise scope),
  jurisdictional footprint, AI system portfolio shape
  (concentrated in one product line versus distributed across
  many), and the maturity stage of the AI-governance program
  (year one standing up versus mature multi-year). The shape
  decision depends on each of these.

## Steps

1. **Enterprise context one-pager.** Author the half-page
   context the shape decision operates against: sector,
   operating-model shape, jurisdictional footprint, AI system
   portfolio shape and scope, current CRO's operating model
   for other second-line functions (compliance, financial
   crime, model-risk-management as applicable), current
   maturity stage of the AI-governance program, and any
   sector overlays that will materially affect the shape
   (banking MRM adjacency, insurance NAIC overlay, health-and-
   medical-device SaMD overlay, EU AI Act provider / deployer
   scope, GPAI provider scope, frontier lab overlay, US
   federal M-25-21 overlay). Every subsequent artefact refers
   back to this one-pager.

2. **The shape decision.** Author the specific shape decision
   (Shape A, B, C, or D from chapter 01, with any overlays)
   with the four-input rationale explicit. Not "we chose
   Shape B because it is popular"; "we chose Shape B because
   (i) the enterprise's operating model is federated by
   business unit, (ii) the AI portfolio is distributed across
   three product lines, (iii) the CRO's compliance function
   runs a hub-and-spoke shape with embeds and this composes,
   (iv) the program is in year two of maturity with intake
   volume that warrants embed coverage in the two largest
   product lines". Where the shape decision includes a Shape
   C overlay for a specific risk domain, name the domain and
   the rationale.

3. **The level-ladder assignments.** For each of the five role
   archetypes (analyst 15, risk engineer 25, evaluation
   engineer 35, senior architect 50, head 60) and any sixth
   archetype the enterprise warrants (agentic safety engineer
   40 in enterprises with frontier-agent surface), author:
   - The specific number of roles at each level as of today
     (or a stated near-term target — a year-one shape
     realistically has some roles unfilled).
   - The competence gate for progression to the next level,
     carrying the chapter-01 gate definitions specialised for
     the enterprise's context.
   - Any specific specialisations at the level (a fairness-
     specialist level-25, a red-team-specialist level-25, an
     evaluation-methodology-specialist level-35, a specific
     sector-overlay-specialist level-35 or level-50).

4. **The reporting-line-decision table.** For each specific
   role position on the chart (not each archetype — each
   position, so a centralised level-15 analyst and an embedded
   level-15 analyst appear as two rows), answer the three
   questions from chapter 01:
   - Solid-line report: to whom.
   - Dotted-line report: to whom, and what the dotted-line
     entitles the dotted-line partner to.
   - Performance-review author: which role writes the review.
     Where the author is not the same as the solid-line
     manager, name the exception and justify it in one
     sentence.
   Use the worked-example format from chapter 01 verbatim:
   *"The `<role>` (`<position modifier>`) reports solid-line
   to `<X>`, dotted-line to `<Y>` (which entitles `<Y>` to
   `<what>`), with performance review authored by `<Z>`."*
   The table is the head's authoritative record on who owns
   what.

5. **The matrix charter per dotted-line.** For each material
   dotted-line on the chart, author the matrix charter that
   defines what the dotted-line means. The charter answers:
   - What decisions does the dotted-line partner have veto,
     consultative, or informational rights on.
   - What is the dotted-line partner's expected time
     investment (attending which meetings, reviewing which
     artefacts, being available on which cadences).
   - What is the escalation path when the head and the
     dotted-line partner disagree on a matrix-scope matter.
   - How is the matrix relationship reviewed (annually with
     the CRO's second-line coordinator, per the chapter-01
     discipline).
   A dotted-line without a matrix charter is chapter 01's
   "matrix-charter-that-isn't" anti-pattern; the exercise
   deliberately forces the charter.

6. **The level-ladder progression documentation.** For each
   role position on the chart, and specifically for the roles
   that are currently filled, author the per-role progression
   documentation chapter 01 requires:
   - Current level.
   - Next level's competence gate.
   - Specific development actions the head and the individual
     have agreed to.
   - Honest read on time-to-readiness (in months or years, or
     "not on this ladder" where the individual is on an
     out-of-function trajectory).
   The progression documentation composes with the coaching
   cadence in chapter 03; do not re-author the coaching
   cadence here, but do reference it.

7. **The succession picture per critical role.** For each of
   the critical roles chapter 01 names (the head; the level-
   50 architect; each level-35 evaluation engineer with a
   distinct methodology surface; each level-25 risk engineer
   with a distinct craft; each embedded analyst under Shape B),
   author the four-cell succession picture:
   - Ready-now successor (a named individual, or "none" if
     that is the honest read).
   - Ready-in-one-year successor with the specific
     development path in flight.
   - Ready-in-three-years successor at a level below the
     target level today, with the development trajectory.
   - Interim plan on unexpected departure (who covers, at
     what capacity, for how long, at what cost to the
     function's other delivery).
   Where any cell reads "none", note the sourcing strategy —
   internal development, external hire, matrix arrangement —
   the head is running to fill the cell. "None" without
   sourcing strategy is chapter 01's "we'll figure it out
   later" anti-pattern.

8. **The chart itself.** Draw the canonical org chart with
   boxes per role position, labelled with role title, level,
   and incumbent (or "vacant" with recruitment status);
   solid lines for solid-line reporting; dotted lines for
   material dotted-lines (with legend explaining what each
   dotted-line means). The chart is versioned, dated, and
   the document-control metadata (owner, refresh cadence,
   distribution list) is on the chart.

9. **The one-page cover.** Author the one-page cover chapter
   01 requires: shape decision (A / B / C / D with overlays),
   the reporting-line-decision-table extract for the head-
   critical roles, the current succession-status summary
   (ready-now / ready-in-one-year / ready-in-three-years
   counts across critical roles, with material gaps flagged),
   the last-review date, the next-review date, and the
   distribution list.

10. **The failure-mode audit.** Author a short section — one
    paragraph per failure mode — naming how the artefact
    detects and recovers from each of these failure modes:
    - The invisible-ladder failure: an analyst hired without
      a documented progression picture, six months in and
      already looking externally.
    - The everyone-solid-line-to-the-head failure: a shape
      chosen against the enterprise's default without written
      rationale, the CRO's coordinator raising it at the
      annual review.
    - The "we'll figure it out later" succession failure: the
      level-50 architect resigning with no ready-now
      successor and no ready-in-one-year successor under
      development.
    - The org chart that lives on the head's laptop failure:
      changes to the function's roles without the chart
      updating, the chart no longer trusted.
    - The matrix-charter-that-isn't failure: a dotted-line
      on the chart without a written charter, the matrix
      partner and the matrixed individual holding different
      expectations of the relationship.

## Deliverables

- `enterprise-context.md` — the half-page context one-pager.
- `shape-decision.md` — the specific shape decision with the
  four-input rationale.
- `level-ladder-assignments.md` — the per-level headcount and
  progression gates.
- `reporting-line-decision-table.md` — the per-position
  reporting-line-decision table with the three-question shape.
- `matrix-charters/matrix-<partner>-<role>.md` — a matrix
  charter per material dotted-line on the chart.
- `progression-documentation/progression-<role>-<incumbent>.md`
  — per-role progression documentation for currently-filled
  roles.
- `succession-picture.md` — the four-cell succession picture
  per critical role, with sourcing strategy for any "none"
  cells.
- `org-chart.md` (or an embedded image with an accompanying
  text description) — the canonical org chart with legend.
- `cover.md` — the one-page cover summarising the artefact
  set for the CRO, CAE, CAIO, GC, and audit-committee
  secretariat distribution.
- `failure-mode-audit.md` — the five failure-mode
  detection-and-recovery paragraphs.

## Acceptance criteria

- The shape decision names one of the four candidates
  explicitly and carries the four-input rationale (operating
  model, portfolio shape, CRO's other-function shape, program
  maturity). A shape without a written rationale fails the
  criterion.
- The reporting-line-decision table has an entry for every
  role position on the chart, and every entry answers all
  three questions (solid-line, dotted-line, performance-
  review author). A row with a missing field fails the
  criterion.
- Every material dotted-line on the chart has a matrix charter
  that names the decision rights, the time investment, the
  escalation path, and the review cadence. A dotted-line
  without a charter fails the criterion.
- The succession picture has all four cells (ready-now,
  ready-in-one-year, ready-in-three-years, interim) populated
  per critical role, and any "none" cell carries the
  sourcing strategy. A blank cell or a "none" without
  sourcing strategy fails the criterion.
- The chart carries the document-control metadata (owner,
  refresh cadence, distribution list, last-review date,
  next-review date). A chart without document control is the
  head-laptop failure mode; the exercise flags it.
- The failure-mode audit names, for each of the five failure
  modes, at least one specific detection signal and one
  specific recovery action.
- Any factual claim about a specific peer enterprise's shape
  or a specific sector's org-shape convention carries a
  `<!-- needs-research: verify [specific fact] against
  [official source] -->` marker where the fact is not
  independently verifiable. No practice is guessed.

## Stretch goals

- Extend the artefact set with the **three-year forward-look
  shape**: what the head expects the function to look like at
  the end of year three under the multi-year hiring plan
  (chapter [02](../02-multi-year-hiring-plan.md)), what
  additional roles will land (agentic safety engineer at
  level 40 if the AI portfolio's frontier surface warrants
  it; additional sector-specialist level-35 or level-50
  roles as sector-overlay maturity demands), and how the
  shape decision will evolve (Shape A in year one moving to
  Shape B in year two as the function's discipline is
  established, for example).
- Author the **CRO annual-ratification agenda** — the specific
  one-page agenda the head takes to the CRO for the annual
  chart-ratification working session. Includes: what has
  changed since last year; the current shape rationale as
  restated; the current succession picture with any material
  changes; the head's specific asks (headcount authorisation,
  matrix-charter changes, ratification of an updated
  reporting line).
- Draft the **CAE handoff note** — the specific note the head
  hands to the CAE at the first working meeting after any
  material change to the chart. The note is short (one page)
  and covers what has changed, why, and what the head expects
  the CAE to read against the change.
- Author the **onboarding orientation** for a new team member
  reading the chart on their first week. The orientation
  covers what the shape means for their working day (where
  they sit, who they report to, who they matrix with, what
  the dotted-lines entitle their matrix partners to), and
  the progression documentation covers what their next-level
  gate looks like.
- Draft the **matrix-charter reconciliation** — a specific
  case-study rehearsal of a matrix disagreement (an embedded
  analyst's product-line VP asks for the analyst's time on a
  first-line project that the head has not prioritised for
  second-line support). Walk the matrix charter's escalation
  path through the case study, producing the specific
  resolution and the minute that goes into the annual
  charter review.

## Notes and starter guidance

The most common first-cut failure is the head who authors the
shape decision without the four-input rationale — the shape
"just is what we have". A shape without written rationale is a
shape the CRO's coordinator will challenge at the annual
review, and the head loses the argument in the room. Force the
four inputs into the artefact — even where the rationale is
"we inherited Shape A and the four inputs support keeping it";
the writing is what makes the decision defensible.

The second common failure is the reporting-line-decision table
that carries only the archetypes, not the specific positions.
A single row for "AI Governance Analyst" masks the fact that
the centralised analyst and the embedded analyst have
different reporting shapes; the table has to enumerate the
positions, not the archetypes. This is the source of ambiguity
that the CAE surfaces on the first audit and that the analyst
themselves experiences as unclear expectations.

The third common failure is the succession picture that reads
optimistically. Every critical role has a ready-now successor
named, ready-in-one-year successors under development, ready-
in-three-years successors identified — and none of it is
honest. The CRO reads the optimism and mistrusts the whole
artefact. Force the honest read; where a cell is genuinely
empty, write "none, sourcing strategy is [X]". "None with
sourcing strategy" is more credible than "someone will step
up", and it is what the CRO's own succession planning depends
on.

On the matrix charter — the temptation is to write generic
charters that read as boilerplate. A generic charter is
useless. Force specificity: which specific meetings does the
dotted-line partner attend; which specific artefacts do they
review; on which specific dimensions do they have veto (an
embedded analyst's product-line VP may have veto over the
analyst's travel and over one-off assignment allocation, but
not over the analyst's substantive findings — the specificity
is what preserves the head's authority on the substance).

The chart is a living artefact. Version it, date it, refresh
it at least annually and at any material org change, and
distribute the current version to the CRO, CAE, CAIO, GC, and
audit-committee secretariat. A chart that has not been
refreshed in a year is a chart that no longer describes the
function; a chart that lives on the head's laptop is a chart
that no one else can act on when the head is unavailable. The
document-control discipline is what turns the chart from a
slide into a governance artefact.
