# exercise-05: Maturity Assessment Planning Drill

**Estimated effort:** 3 hours

## Objective

Author the enterprise's **annual and multi-year AI governance
maturity assessment** as a single defensible artefact set: a composite
maturity plot across the three references the head owns (NIST AI RMF
Playbook, ISO/IEC 42001 AIMS maturity dimensions, OWASP AI Security &
Governance Checklist coverage), a year-over-year delta view, a
two-year trajectory with cost-of-move and explicit
under-investment declarations, an independent-challenge plan, and
the audit-committee reporting shape the plot lands in.

The deliverable is not "some maturity slides." It is the artefact
set the head presents at the annual maturity anchor of the AIMS
calendar (chapter 02) and defends at the audit committee. It must
survive a certification-body sampling of the underlying evidence
under ISO/IEC 42006 and it must survive an audit-committee chair
asking "what does the plot not measure, and how do you compensate?"

## Prerequisites

- Chapter [05-maturity-assessment](../05-maturity-assessment.md)
  read and internalised.
- Chapter [02-aims-operating-calendar](../02-aims-operating-calendar.md)
  — the annual maturity assessment is an anchor on the calendar and
  consumes internal-audit results, register trends, and incident
  volumes from it.
- Chapter [04-third-party-audit-interface](../04-third-party-audit-interface.md)
  — the independent-challenge plan for the plot composes with the
  third-line CAE relationship.
- Familiarity with the NIST AI RMF 1.0 core (GOVERN / MAP / MEASURE /
  MANAGE), the Playbook subcategory structure, the ISO/IEC 42001
  Harmonised Structure clauses 4 through 10 and Annex A control
  areas, and the OWASP AI Security & Governance Checklist section
  structure. At the vocabulary depth — you should be able to name
  the top-level buckets without looking them up.
- Assumed enterprise from the prior exercises, with an assumed
  sector (banking, insurance, health, public sector, frontier lab,
  tech platform, industrial) so the sector-benchmark and voluntary-
  code composition step is specific.

## Steps

1. **Reference-mapping table.** Author a table listing the three
   references and, per reference: what it measures (leadership
   shape, management system, technical control), the axis it
   contributes to the composite, the granularity at which the
   enterprise scores it (subcategory / clause / checklist section),
   the evidence classes that anchor a score at level 3 or above,
   and the tooling the score is captured in (the GRC-for-AI
   platform, an OSCAL-shaped catalogue, or the AIMS evidence
   store). No reference is collapsed into another.
2. **Five-level maturity vocabulary declaration.** Adopt (do not
   reinvent) the five-level vocabulary from chapter 05 (Initial /
   Repeatable / Defined / Managed / Optimising) and write a
   half-page vocabulary declaration that gives per-level meaning
   in your enterprise's language, and names any alternative labels
   the level-50 architect required. The vocabulary is the same
   the CRO, CISO, and CAE use for their own maturity reporting.
3. **Current-state scoring — three panels.** Score the current
   state for each of the three references at the granularity you
   declared. Do not attempt a full production self-assessment —
   pick a representative subset (at minimum: three NIST AI RMF
   subcategories per function, ten ISO/IEC 42001 Annex A control
   areas, three OWASP AI Security & Governance Checklist sections)
   and score to the five-level vocabulary. Every score at level 3
   or above carries a linked evidence citation to a specific
   artefact under AIMS document control (real or plausible).
4. **Year-over-year delta view.** Assume a prior year's scores
   (author them as a starting-year baseline, one level below the
   current-state scores on average, with two deliberate exceptions
   — one axis that regressed, one that overshot). Produce the
   colour-coded delta view chapter 05 specifies (one colour for
   improvements, one for regressions, one for holds). The
   regression must be diagnosed, not hidden.
5. **Two-year trajectory document.** Author the two-year trajectory
   document under AIMS document control. For each of the three
   axes, name: the target level per subcategory / clause / section
   for end of year 1 and end of year 2; the deliberate
   under-investment declarations (at least two axes held at level
   3 or 4 with a defended rationale for why further investment
   would be lower-return than a move elsewhere); the sector-
   benchmark posture (lead / match / lag, with a named comparator
   where the sector has one — SR 11-7 tiering for banking, GMLP
   post-market surveillance for medical devices, RSP / PF / FSF
   disclosures for frontier labs, and so on); and the regulatory-
   horizon alignment (EU AI Act GPAI obligations, high-risk
   obligations, sector supervisory changes).
6. **Cost-of-move table.** Author the cost-of-move table for the
   planned year-1 moves. Per move: the axis and subcategory / clause /
   section moving, the current level, the target level, the
   resource investment required (headcount by level per the
   architect's level ladder, tooling investment, external
   assurance retainer), the dependency on other functions (CISO,
   CRO, CAE, procurement), and the risk if the move is deferred a
   year. This table feeds the budget cycle under
   [[mod-113-budget-vendor-p-and-l-and-investment-case]].
7. **Independent-challenge plan.** Author the independent-challenge
   plan the plot's scores go through before finalisation. Name the
   party (third-line CAE, external consultant with no delivery
   relationship, peer head of AI governance), the scope of the
   challenge (evidence-base for level-3+ scores, methodology,
   sector-benchmark posture), the timing relative to the annual
   assessment anchor, the deliverable the challenge produces
   (memo, formal report, or minuted council review), and the
   provision for what happens when the challenger down-scores an
   axis the head scored higher. Preserve CAE independence per
   chapter 04.
8. **Audit-committee reporting shape.** Author the audit-committee
   pack section for maturity, following the discipline in chapter
   05: one plot per axis, then the composite; year-over-year
   deltas coloured; the trajectory line overlaid on the current
   plot; three or four specific resource asks tied to the
   trajectory; and the explicit limits-of-the-plot section (the
   two or three dimensions of AI risk the plot understates and
   what the enterprise does to compensate). Include a worked
   example applying the shape to the drill data.
9. **Sector-and-voluntary-code composition addendum.** Author a
   half-page addendum showing which sector-specific and
   voluntary-code maturity references compose onto your plot as
   additional axes or overlays. Name the specific references for
   your assumed sector (from the chapter 05 list) and, where the
   enterprise is a signatory to a voluntary code (EU AI Office
   GPAI Code of Practice, G7 Hiroshima Process Code of Conduct,
   Bletchley Declaration, or others per
   [[mod-106-external-positioning-and-voluntary-codes]]), the
   maturity commitments the code imposes.

## Deliverables

- `maturity-reference-mapping.md` — the three-reference mapping
  table.
- `maturity-vocabulary-declaration.md` — the half-page vocabulary
  declaration.
- `current-state-scoring.md` — the three panels of scores with
  per-score evidence citations.
- `year-over-year-delta.md` — the colour-coded delta view with
  regression diagnosis.
- `two-year-trajectory.md` — the trajectory document with per-axis
  targets, under-investment declarations, benchmark posture, and
  regulatory-horizon alignment.
- `cost-of-move-table.md` (or `.csv`) — the year-1 cost-of-move
  table with dependencies and defer-a-year risk.
- `independent-challenge-plan.md` — the challenge plan with named
  party, scope, timing, deliverable, and down-score handling.
- `audit-committee-maturity-section.md` — the pack section with a
  worked example on the drill data.
- `sector-and-voluntary-code-addendum.md` — the composition
  addendum.

## Acceptance criteria

- The three references contribute distinct axes; no axis is
  collapsed or averaged away before the composite.
- Every level-3+ score in the current-state scoring is anchored to
  a specific evidence citation; a score claimed without evidence
  is called out as level 2 by default.
- The year-over-year delta view shows at least one regression and
  one hold as well as improvements; every regression carries a
  diagnosis, not silence.
- The two-year trajectory names deliberate under-investment on at
  least two axes, with defended rationale each; a trajectory that
  targets level 5 everywhere is disqualifying.
- The cost-of-move table has, per move, a specific resource ask
  in named roles at named levels (per the level-50 architect's
  ladder), not a lump sum.
- The independent-challenge plan preserves third-line CAE
  independence if the CAE is the challenger; the CAE assures the
  evidence base and does not set the scores. See chapter 04.
- The audit-committee reporting shape includes an explicit
  limits-of-the-plot section naming at least two AI-risk
  dimensions the plot understates.
- The sector-and-voluntary-code addendum names at least one
  specific sector reference and at least one voluntary-code
  commitment applicable to the assumed enterprise; generic
  references are disqualifying.

## Stretch goals

- Author the plot in a way that lets an audit committee read the
  same picture two years later without you present. Include a
  short reader's note (three to five sentences) inside the pack
  section explaining what a level-4 GOVERN score means, what a
  regression from level 4 to level 3 in an axis implies for the
  operating discipline, and what the enterprise does when a
  trajectory line is not being walked.
- Draft the mid-year read-through pack chapter 05 alludes to (the
  audit-committee mid-year check on whether the trajectory is on
  pace). Include the specific triggers for lifting a mid-year
  read to a formal re-assessment (typically two or more axes
  falling half a level behind pace, a material incident that
  invalidates a score, or a regulatory change that reshuffles
  priorities).
- Extend the cost-of-move table with a "cost-of-lag" column — the
  regulatory, incident, or reputational cost the enterprise
  accepts by deferring the move for one budget cycle. Boards read
  cost-of-lag more readily than cost-of-move.
- Add a fourth-axis prototype: a sector-specific composite axis
  built from two or three of the sector-and-voluntary-code
  references, scored on the same five-level vocabulary. Show how
  it lands in the pack alongside the three headline axes without
  overwhelming them.

## Notes and starter guidance

- Score inflation is the single largest failure mode. Force
  yourself to score to the *evidence* — if the evidence would not
  survive a five-minute skim by an ISO/IEC 42006 auditor, the
  score is a level 2 regardless of how the function feels about
  it. Chapter 05's evidence-anchored scoring section is the
  discipline.
- The under-investment declarations are the mark of a mature
  trajectory. Boards discount trajectories that promise everything;
  boards ratify trajectories that name what the enterprise is
  choosing not to invest in and why. Do not skip this step.
- The regression in the year-over-year delta is the most
  audit-visible signal in the pack. If your assumed baseline has
  no regression, invent one that is plausible for your enterprise
  and diagnose it honestly — a re-org that lost a subject-matter
  owner, a control-library gap that only surfaced under audit, a
  vendor evidence expiry that was not caught. Regressions read as
  candour when they are diagnosed; they read as concealment when
  they are hidden.
- The composite is the last thing you produce, not the first. If
  you find yourself averaging before you have per-axis plots, you
  are hiding signal. Chapter 05's "one plot per axis, then a
  composite" rule is load-bearing.
- Sample-test the pack by asking: could the audit-committee chair,
  reading the pack cold six months later, tell what the enterprise
  is investing in, what it is holding, what it is declining to
  invest in and why, and what the plot does not measure? If not,
  the pack is under-authored.
