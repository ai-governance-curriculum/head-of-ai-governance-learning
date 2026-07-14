# exercise-03: ISO/IEC 38507 Board Shape Annotation

**Estimated effort:** 2 hours

## Objective

Produce an **audit-committee-ready annotation of ISO/IEC 38507:2022**
that maps each of the standard's five clusters of board-facing
considerations (governance and stewardship of AI use; policies for AI
use including risk appetite; culture and values; compliance
obligations for AI use; risk of AI use, including reliance risk and
third-party risk) to a specific artefact your head-of-AI-governance
function will produce for the audit committee, at a stated cadence,
under a named accountable executive.

The annotation is the head's proof — to themselves and to the audit
committee — that the head has read ISO/IEC 38507 as *the board's
standard* and not as another management standard.

## Prerequisites

- Chapter [03-iso-38507-board-shape](../03-iso-38507-board-shape.md)
  read and internalised.
- Access to
  [ISO/IEC 38507:2022](https://www.iso.org/standard/56641.html) —
  paid access via ISO or a national standards body; do not paraphrase
  the standard's text into your annotation, but do reference the
  clause numbers.
- Familiarity with the [ISO/IEC 38500:2015](https://www.iso.org/standard/62816.html)
  evaluate → direct → monitor loop that ISO/IEC 38507 specialises.
- The target enterprise from exercise 1.

## Steps

1. **Confirm the five clusters** in ISO/IEC 38507 and list them in the
   annotation exactly as the standard names them (do not rename to
   match your own vocabulary; the audit committee will look up the
   standard).
2. **For each cluster**, name three artefacts the head produces for
   the audit committee, taken from chapter 03's list. Add or remove
   artefacts to fit your enterprise; the count of three is a
   guideline, not a hard rule.
3. **For each artefact**, name:
   - The accountable executive (must be head at level 60 or below).
   - The cadence (quarterly, monthly, annual, on-material-change).
   - The evidence store where the artefact lives (AIMS document
     control, GRC platform, model registry).
   - The composition point in COSO ERM or ISO 31000 (whichever your
     enterprise runs as the parent risk framework) — because
     ISO/IEC 38507 does not replace the parent framework; it is the
     AI-specific lens on top.
4. **Draft the evaluate → direct → monitor loop** for your target
   enterprise's annual AI governance calendar:
   - When does the board *evaluate* the enterprise's AI trajectory?
   - What does the board *direct* as output of the evaluation?
   - When does the board *monitor* conformance and performance?
5. **Test the annotation against chapter 03's audit-committee
   agenda example.** If a director asked "what does the standard's
   'culture and values' cluster actually mean here?" would your
   annotation answer them in one paragraph? Rewrite until it does.
6. **Include the "not in scope for the board" note** — one paragraph
   explicitly stating what management holds and what the board does
   not decide. The paragraph is what stops the board pack from
   drifting into implementation minutiae.

## Deliverables

- `iso-38507-annotation.pdf` — a five-page PDF, one page per cluster,
  ratified by the head and circulated to the audit-committee chair
  ahead of the annual review.
- `evaluate-direct-monitor-loop.md` — the annual calendar mapping
  each verb to a board meeting, with owners and inputs.
- `not-in-scope-for-the-board.md` — the one-paragraph management-
  scope statement.

## Acceptance criteria

- Every cluster is named exactly as ISO/IEC 38507 names it, with the
  standard's clause number referenced.
- Every artefact has a named accountable executive at level 60 or
  below, a stated cadence, and a machine-consumable evidence store.
- Every artefact is mapped to a composition point in the parent risk
  framework (COSO ERM or ISO 31000).
- The evaluate → direct → monitor loop identifies a specific board
  meeting per verb; no verb is uncovered in the annual calendar.
- The "not in scope" paragraph explicitly names at least three
  decisions the board does not take, drawing from chapter 03.

## Stretch goals

- Extend the annotation with the *reliance risk* deep dive that
  ISO/IEC 38507 explicitly asks the board to consider. Draft the
  reliance-risk indicator set (automation-bias monitors,
  deskilling signal, over-trust metrics) your enterprise would
  operate, and where the indicators live in the AIMS.
- Draft a two-page comparison of ISO/IEC 38507's five clusters
  against IoD AI-governance guidance and NACD AI Oversight
  Blueprint. Note where the three references converge and where
  they diverge.
- Draft the *escalation* pattern from the annotation: what happens
  if any cluster's artefacts miss cadence or degrade? Which board
  meeting hears the escalation?

## Notes and starter guidance

- ISO/IEC 38507 is a *short* standard by ISO conventions and is
  written to be read by directors. Do not translate it into
  operations-team language. Preserve the governing-body voice.
- The single most common annotation error is quietly mapping the
  culture-and-values cluster down to a workforce-training metric
  only. Culture and values is broader; include the raise-a-concern
  channel, the psychological-safety pulse, and the near-miss
  cadence.
- The point of the annotation is to make the head reachable to the
  board. When in doubt, prefer plain English board-vocabulary over
  ISO or NIST terminology; the goal is the board pack, not the
  auditor pack.
