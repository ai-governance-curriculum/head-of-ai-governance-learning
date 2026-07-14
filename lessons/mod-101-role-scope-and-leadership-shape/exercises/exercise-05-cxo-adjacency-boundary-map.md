# exercise-05: CxO Adjacency Boundary Map

**Estimated effort:** 2 hours

## Objective

Draft a **ratifiable CxO adjacency boundary map** — nine to eleven
one-page sheets, one per adjacent officer — for a target enterprise.
Each sheet states in writing what the adjacent officer owns, what the
head owns, what is jointly owned, and which body arbitrates
disagreements. Together, the sheets are the artefact the head walks
into the audit committee with to *ratify the boundary once* rather
than *renegotiate it every quarter*.

The exercise is deliberately about *authoring the artefact*, not
about theorising the adjacencies. The audit committee will not read
theory; it will read the boundary sheets.

## Prerequisites

- Chapter [06-cxo-adjacency-positioning](../06-cxo-adjacency-positioning.md)
  read and internalised.
- The target enterprise from exercise 1, including which CxO
  designations exist and which do not (particularly whether a Chief
  AI Officer designation exists).
- The COBIT 2019 / CSF 2.0 / NIST AI RMF composition points from
  chapter 05 as the vocabulary anchor.

## Steps

1. **List the adjacencies** you will draft sheets for. The
   default nine from chapter 06: CAE, CAIO, CCO (Compliance),
   Chief Communications Officer, CISO, CIO / CTO / CDO,
   CPO / DPO, CRO, GC. Add sector-specific adjacencies (HoMRM
   for banking, CMO for health system, sector CAIO under OMB
   M-25-21 for public sector) where relevant.
2. **For each adjacency, draft the sheet.** Use the same six
   fields:
   - Adjacent officer (title, real or placeholder name).
   - They own (three bullets, drawn from that officer's
     enterprise-parent framework — COSO ERM for CRO, IIA IPPF for
     CAE, CSF 2.0 for CISO, COBIT 2019 for CIO, etc.).
   - We own (three bullets — the AI-specific extension the head
     brings, drawn from the head's second-line envelope).
   - Joint (one to three bullets — shared scope with an explicit
     arbitration body).
   - Arbitrated by (named body — audit committee / risk committee
     / CEO / board).
   - Review cadence (annual by default; on-material-change
     otherwise) and next review date.
3. **Test each sheet** for the three failure patterns from
   chapter 06:
   - **Turf war** — do two officers claim the same scope? If so,
     move the disputed item to "joint" and name the arbitration
     body.
   - **Silent abdication** — is any scope claimed by no officer?
     If so, put it in "we own" or "joint" and name the owner
     explicitly.
   - **Silent expansion** — is any of the head's scope quietly
     claiming an adjacent officer's territory? Rewrite so it is
     visibly the AI-specific extension, not the parent scope.
4. **Assemble the map** with a one-page cover sheet listing the
   sheet titles, the arbitration bodies used, and the annual
   review calendar.
5. **Circulate for signature.** Each adjacent officer signs their
   own sheet; the audit-committee chair or the CEO ratifies the
   cover sheet. (In the exercise, use placeholder signatures.)

## Deliverables

- `cxo-adjacency-boundary-map.pdf` — the assembled multi-sheet
  document, one page per adjacency plus a cover page.
- `cxo-adjacency-review-calendar.md` — the annual review calendar
  showing when each sheet is revisited and by which body.
- `cxo-adjacency-audit-committee-briefing.md` — a two-page
  briefing note explaining what the audit committee is ratifying
  and why, framed for a non-specialist director.

## Acceptance criteria

- Every adjacency in your enterprise's CxO layer is covered by a
  sheet (at least the nine defaults plus any sector-specific
  adjacencies).
- Each sheet uses the six-field template exactly. No sheet has
  "TBD" or missing fields.
- Every "they own" bullet references the adjacent officer's
  parent framework (COSO ERM, IIA IPPF, CSF 2.0, COBIT 2019,
  ISO/IEC 27001, GDPR, etc.), not a made-up vocabulary.
- No two sheets place the same scope in "we own" or in "they
  own" without a corresponding "joint" entry on both sheets
  reconciling them.
- The arbitration body for every joint scope is named, not
  vague ("senior leadership," "executive team").
- The review calendar covers every sheet with a specific
  quarterly or annual slot.

## Stretch goals

- Draft the *upgrade path* for a boundary that must be redrawn.
  Which document is edited first? What is the audit-committee
  ratification cadence for boundary changes?
- Extend the map with a **jurisdictional overlay**: for each
  adjacency, note where the boundary changes across jurisdictions
  (for example, the DPO scope in the EU is legally-defined under
  GDPR Article 37; the CPO scope in the US is not).
- Draft a two-page comparison of your enterprise's boundary map
  against a comparable enterprise in the same sector. Identify
  the boundary decisions that are sector-conventional and those
  that are enterprise-specific.

## Notes and starter guidance

- Do not write the boundary map alone. Every adjacent officer
  should own the wording of their own "they own" section. The
  head's job is to draft the "we own" and "joint" sections and
  negotiate the overlaps.
- The GC / head boundary is the one most learners get wrong.
  Re-read chapter 06 on "engaging a regulator" vs "delivering
  a legal opinion" before drafting.
- The CAIO / head boundary is the one most enterprises get
  wrong. Configuration A (CAIO exists) and Configuration B (no
  CAIO) from chapter 07 both need explicit sheets — do not
  finesse either.
