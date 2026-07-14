# exercise-02: AIMS Operating Calendar Authoring

**Estimated effort:** 3 hours

## Objective

Author an **ISO/IEC 42001 AIMS annual operating calendar** for the
enterprise you would run (or already run) the AIMS at, mapping the
seven operative clauses (4 through 10) to the ten anchor events, with
named owners, pre-read discipline, retained-evidence rules, and
composition with the parent ISMS calendar under ISO/IEC 27001. The
deliverable must be defensible to an ISO/IEC 42001 certification body
under ISO/IEC 42006 sampling.

## Prerequisites

- Chapter [02-aims-operating-calendar](../02-aims-operating-calendar.md)
  read and internalised.
- Chapter [01-governance-council-and-minute-discipline](../01-governance-council-and-minute-discipline.md)
  — the council pack from exercise 01 (or a draft), because the
  calendar's anchor outputs are consumed by the council.
- Familiarity with the level-50 architect's AIMS scope statement
  and statement of applicability. If you are building for a
  hypothetical enterprise, make one working assumption about scope
  and one about SoA and record it in the pack.
- A concrete enterprise in mind, with an assumed sector, an
  assumed AIMS operating-year start month, and an assumption about
  ISMS coexistence (parent 27001-certified, or not).

## Steps

1. **Clause-to-anchor mapping.** Author a table mapping each of
   ISO/IEC 42001 clauses 4 through 10 to the ten anchor events
   named in chapter 02. Note where a single clause spans multiple
   anchors (clause 6 spans anchor 1, 2, and 5) and where a single
   anchor covers multiple clauses (anchor 8 management review
   covers most of clauses 5, 9, and 10 in its inputs). Deviations
   from ten anchors are permitted — justify each.
2. **The calendar.** Author the twelve-month calendar (rows are
   months; columns are anchors) with, for each anchor: window
   (weeks), owner, pre-read owner, accountable executive, minuted
   output, and evidence retention rule. Align to a real
   operating-year assumption — regulatory year-end, financial
   year-end, and parent-ISMS calendar all shift placement.
3. **Management-review agenda template.** Author the
   management-review agenda template under clause 9.3 with:
   required inputs (per chapter 02's list, at minimum), required
   outputs, and a pre-read structure that supplies each input as
   a named artefact traceable to a document-control ID. The
   template is the artefact the level-50 architect and the
   accountable-executive co-chair operate from.
4. **Internal-audit programme plan.** Author a three-year
   internal-audit programme plan showing how every AIMS clause and
   every applicable Annex A control is covered at least once,
   weighted by risk. The plan names auditor independence
   provisions (which auditor cannot audit which activity), the
   composition with the ISMS internal-audit programme, and the
   round scheduling within each year.
5. **Non-conformity and corrective-action register template.**
   Author the register template following the chapter 02 field
   set (ID, source, description, severity, owner, containment due,
   corrective-action-plan due, closure due, effectiveness-review
   due). Include a worked example of an ageing dashboard the head
   uses monthly.
6. **Competence matrix skeleton.** Author the competence matrix
   skeleton — named roles (analyst, risk engineer, evaluation
   engineer, agentic-safety engineer, first-line owners, third-party
   procurement staff, GRC operators) mapped to competence areas
   (technical, methodological, regulatory, sector-specific). The
   skeleton is populated with the competence *categories* only —
   per-person evidence is populated in operation, not in this
   exercise.
7. **ISMS composition note.** Write a half-page note describing how
   the AIMS calendar composes with the parent ISMS calendar
   (assuming ISMS present). Identify: shared clauses, shared
   governance bodies, shared document control, distinct-scope
   sections, shared audit vehicles. If ISMS is not present at your
   assumed enterprise, note the implication for evidence-tooling
   maturity.
8. **Failure-mode watch note.** Write a half-page note describing
   which of the three chapter-02 failure modes (calendar-without-
   evidence, evidence-without-decisions, ageing debt) your
   calendar is most vulnerable to and the specific controls you
   have written in to defend against it.

## Deliverables

- `aims-calendar.pdf` (or `.md` collection with calendar as an
  embedded table) — the twelve-month calendar plus the clause-to-
  anchor mapping.
- `management-review-agenda-template.md` — the clause 9.3 agenda
  template with input and output structure.
- `internal-audit-programme-plan.md` — the three-year plan.
- `non-conformity-register-template.md` and an ageing-dashboard
  example.
- `competence-matrix-skeleton.md` — the role-to-competence
  categories.
- `isms-composition.md` — the half-page composition note.
- `failure-mode-watch.md` — the half-page failure-mode note.

## Acceptance criteria

- Every one of clauses 4 through 10 is mapped to at least one
  anchor event.
- Every anchor event has: window, owner, pre-read owner,
  accountable executive, minuted output, evidence retention rule.
- The management-review agenda template names all of the clause
  9.3 required inputs (previous-review actions, external and
  internal issues, interested-party feedback, performance
  information, resource adequacy, continual-improvement
  opportunities) and required outputs (continual-improvement
  decisions, AIMS-change needs, resource-allocation actions).
- The internal-audit programme plan covers every AIMS clause and
  every applicable Annex A control at least once in the three-
  year cycle, with named auditor-independence provisions.
- The non-conformity register template has every field from
  chapter 02, and the ageing dashboard example makes the ageing
  pattern legible (not a raw list, an aggregate view).
- The competence matrix skeleton names at least six roles and at
  least four competence categories per role.
- The ISMS composition note names shared, distinct, and
  interfaced elements.
- The failure-mode watch note names the specific control you have
  written in, not a generic mitigation.

## Stretch goals

- Draft the certification-body engagement window playbook — how
  the calendar handles a certification-body stage-1, stage-2,
  surveillance, or recertification visit; how audit-liaison work
  scales; how post-visit remediation windows are booked.
- Extend the internal-audit programme plan with a specific
  auditor-independence resolution for a two-person AI governance
  team (where co-source with the third-line CAE or an external
  auditor is the only defensible option).
- Extend the competence matrix skeleton with sector-specific
  competences for the sector you assumed (model-risk-management
  competences in banking, GMLP competences in medical devices,
  NAIC-model-bulletin competences in insurance, OMB-M-25-21
  competences in public sector, RSP / PF / FSF competences in a
  frontier lab).
- Author the calendar in a way that is directly importable into
  the GRC-for-AI platform the level-50 architect selected, with
  structured metadata per anchor.

## Notes and starter guidance

- Do not attempt to author a "perfect" calendar. Author one
  defensible calendar for one assumed enterprise. Every anchor's
  window, owner, and evidence rule should survive an auditor
  reading them in the abstract.
- Chapter 02's ten anchors are a minimum. Some enterprises add an
  anchor for board-facing reporting integration (usually placed
  at Q3 to align with the ratified board pack); some add a
  specific anchor for sector-supervisor examination preparation.
  Add anchors, do not delete.
- The management-review anchor (anchor 8) is the single most
  audit-visible artefact. If you have limited time, invest
  disproportionate depth there.
- Test the calendar by picking any month and asking: what is
  happening this month, who owns it, what evidence lands, and
  what a certification body would see if they visited that week.
  If any answer is vague, revise.
