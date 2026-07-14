# exercise-02: NIST AI RMF GOVERN Function at Leadership Scope

**Estimated effort:** 2 hours

## Objective

Author the head's **one-page GOVERN answer** for a target enterprise
— the six-cluster answer described in chapter 02 that discharges the
head's second-line accountability under NIST AI RMF 1.0 to the audit
committee. Ratify each answer against the AI RMF Playbook by naming
one implemented Playbook suggested action (or one written waiver) per
GOVERN subcategory, and make explicit where the Generative AI Profile
(NIST AI 600-1) overlays each cluster.

The exercise is deliberately not "map the entire framework." That is
level-15 or level-25 work. The exercise is *reading the framework as
leadership shape* and producing the one-page artefact the head
actually walks into an audit-committee meeting with.

## Prerequisites

- Chapter [02-nist-ai-rmf-govern-leadership-shape](../02-nist-ai-rmf-govern-leadership-shape.md)
  read and internalised.
- Access to
  [NIST AI RMF 1.0 (AI 100-1)](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-1.pdf),
  the [AI RMF Playbook](https://airc.nist.gov/AI_RMF_Knowledge_Base/Playbook),
  and the [Generative AI Profile (AI 600-1)](https://airc.nist.gov/AI_RMF_Knowledge_Base/AI_RMF/Uses/GenAI-Profile).
  All are public.
- The target enterprise from exercise 1.

## Steps

1. **Confirm the six GOVERN categories** — GOVERN 1 through GOVERN 6 —
   and read the AI RMF 1.0 text for each carefully. Do not paraphrase
   yet; take the framework's own words.
2. **For each category, write the head's answer in one sentence.**
   The sentence must name (a) the accountable executive, (b) the
   artefact or cadence that discharges the category, and (c) the
   evidence store where the artefact lives. Use the audit-committee
   example in chapter 02 as a shape reference.
3. **For each category, name one implemented Playbook suggested
   action** per subcategory (or one written, dated waiver with the
   justification). This is the coverage-discipline test.
4. **Overlay the Generative AI Profile.** For each of GOVERN 1
   (policy for GenAI), GOVERN 3 (workforce implications of GenAI),
   GOVERN 5 (public trust posture in the GenAI era), and GOVERN 6
   (third-party foundation-model providers), name the specific
   AI 600-1 action or transparency-and-documentation practice the
   enterprise has adopted.
5. **Apply the three anti-checklist tests** from chapter 02: named
   accountable executive per row? machine-consumable evidence?
   externally observable presence? Rewrite any row that fails.
6. **Format** as a one-page PDF plus a machine-readable table
   (CSV or JSON) for the AIMS evidence store.

## Deliverables

- `govern-one-page.pdf` — the head's board-ready one-page GOVERN
  answer.
- `govern-coverage.csv` — one row per Playbook subcategory, with
  columns: category, subcategory, implemented Playbook action or
  waiver, evidence artefact, accountable executive, next review
  date.
- `genai-profile-overlay.md` — the AI 600-1 overlay narrative for
  the four GenAI-critical GOVERN categories.

## Acceptance criteria

- The one-page GOVERN answer covers all six categories with one
  sentence each, and passes the three anti-checklist tests.
- The coverage CSV has 100% coverage of the Playbook subcategories
  under GOVERN — every row shows either an implemented Playbook
  action *or* a dated, justified waiver. No rows are silently
  omitted.
- The AI 600-1 overlay explicitly maps to GOVERN 1, 3, 5, and 6 and
  names the AI 600-1 action / practice adopted.
- Every "accountable executive" cell names a specific role at level
  60 or below (not "the AI governance function" as a whole).
- Evidence artefacts named are machine-consumable (OSCAL, CycloneDX
  ML-BOM, SPDX 3.0 AI, model card, system card, dated attestation),
  not slide decks or screenshots.

## Stretch goals

- Draft the *maturity plot* for the AI governance function against
  the Playbook's tiered suggested actions, positioning the function
  on an initial → repeatable → defined → managed → optimising
  trajectory. Note the two or three most impactful next moves.
- Author a one-page CISO-facing note that maps the head's GOVERN
  answer to the CSF 2.0 GOVERN function categories (see chapter 05
  for the isomorphism), so the head and the CISO can compare notes.
- Draft the annual review calendar for GOVERN — when does each
  category get re-tested, by whom, and what evidence refresh is
  required. Feed this into the AIMS operating calendar in module
  102.

## Notes and starter guidance

- The temptation to write "we are GOVERN 1.1 compliant" is a
  checklist trap. Write instead "our parent AI policy is in force,
  reviewed on [date] by [executive], expiring [date], and any
  operational exception has an owner, expiry, and report line" —
  that is the leadership-scope answer.
- If any category has no evidence store, note it as a gap; do not
  fill it in with the aspirational answer. Leadership credibility
  depends on being visibly honest about gaps.
- Do not confuse GOVERN with the compliance-obligation crosswalk.
  GOVERN is the *shape* of the second-line function; the crosswalk
  (level-50 architect deliverable) is what turns specific
  regulations into specific controls. Both are needed; they are
  different artefacts.
