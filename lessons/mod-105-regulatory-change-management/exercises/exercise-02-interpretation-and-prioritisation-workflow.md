# exercise-02: Interpretation and Prioritisation Workflow

**Estimated effort:** 3 hours

## Objective

Author the enterprise **interpretation-and-prioritisation workflow**
the head runs against every landing regulatory obligation, and then
exercise the workflow against three specific in-flight items so the
workflow lands with muscle memory rather than as a theoretical
diagram.

The workflow has the seven steps chapter 02 names — intake,
packaging, legal opinion, portfolio prioritisation, handoff to the
architect, change-management plan authoring, disposition — each with
an owner, an artefact, and an SLA. It has the four-axis priority
framework the head personally adjudicates at step 4 — compliance-
date proximity, attachment breadth, enforcement risk, program-
carrying capacity.

The deliverable is two-part. Part one is the workflow specification
itself — the document the desk uses to run any interpretation. Part
two is three worked interpretation packages that exercise the
workflow against three specific items drawn from chapter 06 and
chapter 07's rehearsal roster (EU AI Act GPAI obligations, CEN-
CENELEC JTC 21 harmonised standards, Colorado SB 24-205, Texas
TRAIGA, OSFI E-23, Korea AI Basic Act, evolving AISI methodology).
The worked packages are the exercise's calibration — they show that
the workflow produces defensible interpretations rather than
plausible-sounding paragraphs.

## Prerequisites

- Chapter [02](../02-interpretation-and-prioritisation.md) —
  the seven-step workflow and the four-axis priority framework —
  read and internalised.
- Chapter [01](../01-horizon-scanning-cadence.md) — the escalation
  rules that promote items into interpretation. Exercise 01's
  scanning-system design is a strong prerequisite; the
  interpretation workflow reads inputs from it.
- [[mod-102-running-the-program]] chapters 04 and 06 — the level-
  50 architect's regulatory crosswalk and the AI system inventory
  the packaging step's attachment analysis leans on.
- [[mod-104-regulator-engagement]] chapter 07 — the head-and-GC
  boundary and the five-component packaging discipline the
  interpretation workflow imports.
- [[mod-107-program-measurement-and-maturity]] chapter 01 — the
  KRI portfolio that reads disposition timestamps to produce
  median-time-to-interpretation.
- Three rehearsal items chosen from the roster in chapters 06 and
  07. Pick items with different shapes — for example: an EU AI Act
  GPAI obligation (enterprise-scale, hard compliance date, GC-
  heavy), a Colorado AI Act obligation (state, sectoral overlay
  for insurers, evolving), and a JTC 21 harmonised standard
  citation (soft-into-hard on OJEU citation, architect-heavy,
  presumption-of-conformity mechanic).

## Steps

1. **Workflow specification.** Author the seven-step workflow as
   the operating document the desk uses. For each step: named
   owner (specific role — desk owner, GC, head, level-50
   architect), input artefact, output artefact, SLA (active items
   30 days end-to-end to step 5; priority items 14 days), and
   the escalation trigger when the step misses its SLA. This is
   the workflow document; parts 2–4 of the exercise exercise it.
2. **Packaging template.** Author the packaged-obligation memo
   template as a reusable artefact. It has the five components
   chapter 02 names — plain-English summary (two to three
   sentences, operational vocabulary), attachment analysis
   (specific systems / decisions / actors / data flows, drawn
   from the architect's crosswalk and inventory), technical-
   feasibility sketch, operational-cost sketch (defensible
   estimate, not full P&L), and the specific interpretive
   question for GC. The template is what the desk fills in; a
   memo that omits a component gets returned to packaging.
3. **Priority-adjudication template.** Author the four-axis
   priority-adjudication template the head fills in at step 4.
   For each axis: compliance-date proximity (hard vs soft dates,
   distance), attachment breadth (enterprise-scale, business-line,
   bounded), enforcement risk (regulator history, enterprise
   history, political / market salience, peer enforcement), and
   program-carrying capacity (what is already in flight, marginal
   cost, what gives if this becomes priority). Include the
   rebalancing moves chapter 02 lists (compress a lower-priority
   item, escalate to CxO, accept enforcement risk with board
   notice) and the written-ranking output format. This template
   is what the head personally uses at the monthly portfolio
   review.
4. **Worked package one — the EU AI Act GPAI obligation.** Pick a
   specific GPAI obligation currently landing (choose from
   provider-facing obligations under Article 53, systemic-risk
   provider obligations under Article 55, or the GPAI Code of
   Practice as it is finalised — cite the specific article, and
   use `<!-- needs-research: verify current status of GPAI Code
   of Practice adoption and its interaction with Article 55
   presumption of adequacy against digital-strategy.ec.europa.eu
   -->` where the current status is uncertain). Run the item
   through the packaging template and the priority-adjudication
   template. Produce: packaged memo, priority ranking with
   reasoning, hand-off note to the level-50 architect. The
   worked package should be defensible under audit — no vague
   attachment claims, no numeric priority score without
   reasoning, no drafted legal conclusion.
5. **Worked package two — a state AI act obligation.** Pick a
   state AI act obligation — Colorado SB 24-205's obligations on
   developers or deployers of "high-risk AI systems", Texas
   TRAIGA (see needs-research below), or an NAIC AI Model
   Bulletin adoption in a specific state. Run the item through
   the same two templates. The exercise here is different —
   state acts often have narrower attachment but overlay onto
   sectoral supervision the enterprise already carries; the
   priority-adjudication has to reflect that overlay. Use
   `<!-- needs-research: verify [state AI act] current effective
   date and any implementing regulations against [state
   legislature / AG] before citing at audit-committee depth -->`
   where the state-act status is uncertain — do not guess
   effective dates.
6. **Worked package three — a harmonised standard citation.**
   Pick a CEN-CENELEC JTC 21 harmonised standard currently
   moving toward OJEU citation (see needs-research below on the
   specific standards under Commission standardisation-request
   M/593). Run the item through the two templates. The exercise
   here is again different — a standard citation is a soft-into-
   hard event (soft while the standard is under work, hard at
   OJEU citation because it creates a presumption of conformity
   under Article 40). The compliance-date-proximity axis has to
   reflect that mechanic, and the attachment breadth is often
   architect-heavy (control-library rewrite) more than product-
   heavy.
7. **Batching decision.** For the three worked packages, apply
   the batching discipline chapter 02 names. Do any two of them
   share attachment, share crosswalk impact, or share GC opinion
   input? If yes, author the batching decision (which packages
   are batched, why, what the batched change-management plan
   looks like at a sketch level). If no, author why not, so a
   reviewer can see the decision was made rather than avoided.
8. **Adjacent-workflow feed.** For each of the three worked
   packages, name the adjacent workflow feed chapter 02 names:
   what the risk register update looks like
   ([[mod-102-running-the-program]] chapter 03), what the
   procurement-pipeline trigger looks like (chapter 04 of that
   module), what the board-pack line looks like
   ([[mod-103-board-and-audit-committee-reporting]] chapter 01
   cluster 5). The feed is short (one line per adjacent
   workflow); the point is that the interpretation output has
   already been sketched into the workflows it feeds.

## Deliverables

- `workflow-spec.md` — the seven-step operating document (owner
  / input / output / SLA / escalation per step).
- `packaging-template.md` — the reusable packaged-obligation memo
  template with the five components.
- `priority-template.md` — the four-axis priority-adjudication
  template with rebalancing-moves annex.
- `package-01-gpai.md` — the EU AI Act GPAI worked package
  (packaged memo, priority ranking, architect hand-off).
- `package-02-state.md` — the state AI act worked package.
- `package-03-standard.md` — the harmonised-standard worked
  package.
- `batching-decision.md` — the batching adjudication across the
  three packages.
- `adjacent-feed.md` — the short per-package feed into risk
  register, procurement pipeline, board pack.

## Acceptance criteria

- Every step in `workflow-spec.md` has a named owner (specific
  role), an input artefact, an output artefact, an SLA, and an
  escalation trigger. No step reads "the desk decides" without
  the escalation trigger named.
- The packaging template's five components are enforced — a memo
  authored against the template that omits a component is
  detectably incomplete. The template's plain-English summary
  format is two-to-three-sentence operational-vocabulary
  ("requires the enterprise to do X on Y systems by Z"), not
  "the regulation says X" prose.
- The priority template produces a **written ranking with
  reasoning**, not a numeric score. The four axes are each
  explicitly considered even where an axis is not the driver;
  silence on an axis is a defect.
- Every worked package's attachment analysis names specific
  systems (or specific system classes) inside and outside the
  scope, drawn from the enterprise-context assumption. "Multiple
  high-risk systems" without enumeration is under-authored.
- Every worked package's operational-cost sketch is defensible
  — engineering effort (person-quarters or person-weeks at a
  named grain), vendor spend (order-of-magnitude), opportunity
  cost (specific feature-scope reduction), not "significant" or
  "material".
- Every worked package's "specific question for GC" is a
  precise interpretive question the desk cannot answer alone, not
  a general "is this a problem?" — for example, "does Article 55
  attach to model M given its training-compute footprint estimate
  and its integration into product P?" — the specificity is the
  test.
- No worked package contains a legal conclusion in desk
  vocabulary ("we are compliant", "we are non-compliant", "this
  does not apply to us"). Legal conclusions belong in the GC
  opinion, which the workflow references but does not restate.
- Every state AI act citation and every GPAI-Code-of-Practice
  citation is marked with a `<!-- needs-research: ... -->` where
  the current status is uncertain, naming the specific fact and
  the official source to verify.
- The batching decision is made and defended, not skipped. Where
  the decision is "do not batch", the reasoning is written.
- The adjacent-feed artefact is populated for every package
  against risk register, procurement pipeline, and board pack.

## Stretch goals

- Author the **rejection template** — the desk memo that closes
  an item at packaging with "does not warrant interpretation" and
  the head's counter-signature. Chapter 02 does not name the
  rejection template explicitly, but the workflow needs one: not
  every landing obligation should reach step 4. Design the
  rejection so that the register memory (chapter 01) shows the
  item was seen, packaged partially, closed with reasoning.
- Author the **SLA-miss operating procedure** — what happens
  when an active item misses the 30-day SLA or a priority item
  misses the 14-day SLA. Who is telemetered, what escalation
  fires, how the desk's performance is coached
  ([[mod-108-leading-the-governance-function]] chapter 02) versus
  when a systemic capacity issue is escalated.
- Author the **cross-crosswalk trace** annex — for the three
  worked packages, sketch how each interpretation output would
  land in the level-50 architect's control-library update
  ([[mod-102-running-the-program]] chapter 04). This is the
  trace the change-management plan (chapter 03) operationalises.
- Extend the priority-adjudication template with the **rebalance
  authorisation record** — where the head makes a rebalancing
  move (compress a lower-priority item, escalate, accept
  enforcement risk), name the committee that endorses the move,
  the audit-committee awareness posture, and the register entry
  that records the decision.

## Notes and starter guidance

The most common first-cut failure is a workflow specification
that reads as a diagram — seven boxes connected by arrows,
labels but no owners or SLAs. The workflow is only useful if a
desk owner can read step N and know whose desk the item lands on
next and by when. Force the specification to be operational: if
an intake step names "assigned to the desk", it is under-
authored; if it names "assigned to a specific analyst by the
desk lead within 24 hours of promotion at the weekly digest read",
it is executable.

The second common failure is legal drift in the packaging step.
The packaging memo is a program-management artefact. It
translates the obligation into operational terms and names the
question for GC; it does not draft the answer. A memo that says
"we interpret Article 53 to require X" has already crossed the
GC boundary. A memo that says "on our system inventory, the
Article 53 obligation attaches to systems S1, S2, S3 (per the
crosswalk); we would need X, Y, Z operational changes to comply;
the specific question for GC is whether the attachment reads
correctly on our facts and whether the systemic-risk threshold
under Article 55 pulls S1 into a heavier obligation" is in the
right posture. The distinction is what
[[mod-104-regulator-engagement]] chapter 07 calls out — read it
first if the memos drift.

On the priority framework — the four axes are a discipline, not
a formula. The head's job is to weigh the axes in writing so a
reviewer can see the reasoning. A priority ranking that reduces
to "these are the top three because we said so" is the failure
mode chapter 02 warns against; a ranking that says "item A is
top priority because compliance-date proximity is Q3 (six months
away) and attachment breadth is enterprise-scale; item B is
second because attachment is smaller but enforcement risk is
high given the recent Colorado AG action against a peer; item C
is third because it is architect-heavy and the crosswalk update
carries a longer runway than the compliance date allows" is
defensible reasoning.

On the worked packages — resist the pull to author a fourth or
fifth package because "we cover more of the roster that way".
Three worked packages against different item shapes exercises
the workflow more thoroughly than seven packages against the
same shape. If the head cannot show the workflow adapts to the
three different shapes, more packages will not fix the workflow.

On the batching discipline — batching is where the head's
portfolio judgment shows. It is easy to run three items in
parallel and never notice that the underlying crosswalk update
overlaps. Force the batching decision, in writing, even where
the answer is "do not batch, because...". A workflow that never
batches is producing more crosswalk churn than the architect can
absorb.

The three worked packages become the seed of the change-
management plan drills in exercise 03. If the packaging is not
solid here, exercise 03's plans will be too.
