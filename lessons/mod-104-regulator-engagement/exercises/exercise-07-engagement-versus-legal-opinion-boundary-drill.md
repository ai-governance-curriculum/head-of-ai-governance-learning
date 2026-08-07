# exercise-07: Engagement Versus Legal Opinion Boundary Drill

**Estimated effort:** 2 hours

## Objective

Rehearse the **head-and-General-Counsel boundary** from chapter 07
until it is a reflex rather than an improvisation. The deliverable is
a small pack of artefacts — a classified interaction inventory, five
worked packaging memos, a disagreement-resolution protocol, and a
signed joint operating agreement between the head and GC — that a
successor or a stand-in could pick up cold and use to stay on the
correct side of the boundary under time pressure.

The exercise is not a study of the four quadrants; chapter 07 already
does that. The exercise is the artefact set the head circulates
internally so that (a) their own function knows when to route to GC,
(b) GC knows what the head has and has not decided, and (c) a
regulator never gets a split answer from head and GC on the same day.

## Prerequisites

- Chapter [07-engagement-versus-legal-opinion-boundary](../07-engagement-versus-legal-opinion-boundary.md)
  read and internalised. The four-quadrant map, the five-component
  packaging discipline, the technical-position discipline, and the
  disagreement discipline are the load-bearing constructs.
- Chapter [02-article-72-and-73-filings](../02-article-72-and-73-filings.md)
  for the Q2 (technical position with legal exposure) example the
  drill uses.
- Chapter [05-regulator-exam-runbook](../05-regulator-exam-runbook.md)
  for the Q4 (litigation posture / adverse regulatory action)
  example the drill uses.
- Chapter [06-public-consultation-submission-flow](../06-public-consultation-submission-flow.md)
  for the Q3 (legal position on technical facts) example.
- [[mod-101-role-scope-and-leadership-shape]] chapter 06 (CxO
  adjacency) for the head-and-GC boundary framing the drill
  extends.
- A concrete enterprise in mind, with a working GC counterpart (real
  named GC, or a placeholder GC role at a hypothetical enterprise)
  the artefacts are written against.

## Steps

1. **Interaction inventory.** List ten upcoming or hypothetical
   regulator-facing interactions the head is or would be involved
   in over the next twelve months. Cover breadth deliberately: at
   least one AI Safety Institute engagement, at least one EU AI
   Act NCA touch (Article 72 or 73), at least one sector-regulator
   examination interaction, at least one public-consultation
   submission, at least one MRA/MRIA-tier follow-up or equivalent
   adverse-action-adjacent interaction, and at least one incident
   filing. For each interaction record: the counterpart body, the
   trigger, the artefact the interaction produces, and the date
   window.
2. **Quadrant classification.** For every interaction on the
   inventory, assign it to Q1 (technical, no legal exposure), Q2
   (technical with legal exposure), Q3 (legal on technical facts),
   or Q4 (litigation / adverse action). Record the classification
   rationale in one sentence per interaction. Any interaction the
   head cannot classify without asking GC is flagged with a
   `needs-quadrant-confirmation` marker rather than guessed.
3. **Owner / signer / privilege overlay.** Beside each classified
   interaction, add three columns: **owner** (head, head-framed-
   by-GC, GC-with-head-fact-ratification, GC-end-to-end), **signer**
   (whose name goes on the outgoing artefact), and **privilege
   posture** (public / privileged / mixed with named work-product
   segments). No row is left blank.
4. **Packaging memo — five worked passes.** Select five
   interactions from the inventory that the head must package for
   GC (typically the Q2, Q3, and mixed cases). For each, author a
   packaging memo using the five components from chapter 07:
   - Plain-English summary of what the regulation requires
     (operational statement, not legal interpretation).
   - Attachment analysis (specific systems, decisions, actors,
     business lines, or data flows the obligation attaches to).
   - Technical-feasibility assessment (what the enterprise can do,
     what it cannot yet do, delta to close).
   - Operational-cost assessment (engineering effort, run-cost,
     vendor spend, opportunity cost — defensible estimate, not
     placeholder).
   - The specific question for GC (does the obligation attach in
     this way, on these facts, and what defences exist if a
     regulator disagrees).
   Each memo is one page, dated, signed by the head, addressed to
   GC by name.
5. **Technical-position dossier — one worked pass.** Select one
   interaction where the head will front the technical position
   under regulator questioning (typically a Q1 or the head's side
   of a Q2). Author the dossier as a five-question brief the head
   uses to prepare: what does this system do; how did we know;
   what safeguards are in place; what have we changed since a
   prior finding; what is our own view of residual risk. Each
   answer is backed by named evidence in the running-program
   evidence base — not a rhetorical position.
6. **Disagreement-resolution protocol.** Author the internal
   protocol the head and GC follow when they disagree on framing
   for a live regulator interaction. The protocol specifies: how
   the disagreement is surfaced (scheduled joint session, not
   hallway conversation); how it is documented (statement of
   positions, rationale each side, resolution reached); when the
   audit-committee chair is briefed; the default rule for time-
   critical unresolved disagreement (GC on legal interpretation,
   head on technical fact); the escalation to CEO for mixed cases
   where the two cannot be cleanly separated; and the rule that a
   disagreement is never presented to a regulator.
7. **Joint operating agreement.** Author the one-page joint
   operating agreement between the head and GC that codifies
   everything above. The agreement covers: the four-quadrant
   classification convention; the packaging convention; the
   technical-position convention; the disagreement-resolution
   protocol; the review cadence (annual by default; on-material-
   change otherwise); and the ratification signature block for
   both head and GC. The audit-committee chair signs the cover
   page ratifying the agreement.
8. **Adjacent-boundary annexes.** Author short (half-page)
   annexes for the four adjacent boundaries chapter 07 names —
   Government Affairs, Communications, Investor Relations, CISO
   — each specifying what the head provides, what the adjacent
   function owns, and the escalation trigger for handing the
   front seat to the adjacent function. The annexes attach to
   the joint operating agreement so that the boundary set is
   coherent across all five functions the head coordinates with.

## Deliverables

- `interaction-inventory.md` — the ten-interaction inventory with
  counterpart, trigger, artefact, and date window per row.
- `quadrant-classification.md` — the classified inventory with
  quadrant, rationale, owner, signer, and privilege posture per
  row.
- `packaging-memos/` — five worked packaging memos (one file
  each), one page apiece, dated and signed by the head.
- `technical-position-dossier.md` — the five-question brief for
  the selected front-the-technical-position interaction.
- `disagreement-resolution-protocol.md` — the internal protocol
  covering surfacing, documenting, audit-committee-chair
  briefing, default rules, CEO escalation, and never-to-regulator
  rule.
- `joint-operating-agreement.md` — the one-page agreement
  between head and GC with signature block and audit-committee-
  chair ratification.
- `adjacent-boundary-annexes.md` (or four separate files) — the
  half-page annexes for Government Affairs, Communications,
  Investor Relations, and CISO.

## Acceptance criteria

- Every interaction on the inventory is classified into exactly
  one of Q1, Q2, Q3, Q4 — or flagged
  `needs-quadrant-confirmation` with a specific question for GC.
  No row is left silent.
- Every classified interaction has a named owner, a named signer,
  and a specific privilege posture. No row reads "TBD," "the
  team," or "review."
- The five packaging memos each carry all five components
  explicitly labelled (plain summary, attachment analysis,
  technical feasibility, operational cost, question for GC). A
  memo that fuses components or skips one fails the criterion —
  the components exist to force the head to do the work.
- The operational-cost assessment on every packaging memo names
  a defensible estimate (headcount, dollars, calendar weeks). "To
  be determined" is not an estimate.
- The technical-position dossier answers all five questions from
  chapter 07 (what the system does, how the enterprise knows,
  what safeguards, what has changed, residual-risk view), each
  cross-referenced to specific evidence in the running-program
  evidence base — not rhetorical assertion.
- The disagreement-resolution protocol covers all six moves from
  chapter 07 explicitly (surfacing, documenting, audit-chair
  briefing, default rule on legal-vs-technical, CEO escalation
  for mixed cases, never-to-regulator rule).
- The joint operating agreement is one page — no more — and is
  signed (placeholder signatures acceptable) by head, GC, and the
  audit-committee chair ratifying.
- Every adjacent-boundary annex names the head's contribution,
  the adjacent function's ownership, and the specific trigger
  that hands the front seat to that function.

## Stretch goals

- Run the disagreement-resolution protocol against one
  deliberately-constructed hypothetical disagreement — a case
  where the head reads a proposed rule as attaching to a system
  and GC reads it as not attaching, or vice versa. Author the
  full paper trail as the protocol requires: the statement of
  positions, rationale each side, resolution reached, and the
  briefing note that goes to the audit-committee chair. The
  scenario is clearly labelled hypothetical and does not
  reference any live matter.
- Draft an **on-call phone-tree** covering the four quadrants —
  who the head calls when a regulator lands mid-interaction and
  the quadrant is not yet clear, who GC calls when the request
  is technical rather than legal, who is on the joint bridge
  when the quadrant is Q2 or mixed. Tie the phone tree back to
  the joint operating agreement so that the escalation matches
  the classification.
- Circulate the joint operating agreement to a peer at head-of-
  role or general-counsel level for one round of critique before
  finalising, and record what the peer changed and what the head
  accepted or rejected with rationale.
- Extend the interaction inventory into a **rolling twelve-month
  view** that ties each classified interaction back to the
  regulator-engagement cluster of the quarterly board pack in
  [[mod-103-board-and-audit-committee-reporting]], so the
  boundary discipline surfaces to the audit committee as a
  running artefact rather than a one-shot ratification.

## Notes and starter guidance

- The single most common failure of a first-cut boundary drill is
  false certainty. Every row of the classification table that
  reads Q1 or Q2 without a moment of doubt is a row worth
  re-examining. Regulators are inventive about turning what looks
  like a Q1 technical exchange into a Q3 legal position; if the
  head has not asked "could this become Q3 mid-conversation" for
  every Q1 row, the boundary is under-tested.
- The packaging memos are the load-bearing artefact of the
  exercise. Chapter 07 is explicit that packaging is neither
  lay-legal analysis nor mechanical forwarding — the memo is what
  proves the head did the technical-position work only they can
  do. A packaging memo that reads as a legal brief is over-
  reaching; a packaging memo that reads as a forwarded email is
  under-reaching. Aim for the middle: what the regulation
  requires operationally, what it attaches to at the enterprise,
  what the enterprise can and cannot do, what it costs, and the
  specific question GC is being asked.
- The disagreement-resolution protocol is protective for both
  head and GC. Author it in a form both parties will co-sign, not
  in a form that reads as the head imposing terms on GC. Send GC
  the draft; incorporate their edits; sign together.
- The joint operating agreement is the artefact that survives
  personnel change. The successor head or successor GC picks up
  the agreement, sees the four-quadrant convention, sees the
  packaging convention, sees the disagreement-resolution
  protocol, and does not have to renegotiate the boundary from
  scratch. Write it for that successor reader.
- Chapter 07's one-sentence compression — *engagement is what the
  head does; a legal opinion is what General Counsel delivers,
  and the head does not deliver legal opinions* — belongs on the
  cover of the joint operating agreement. The rest of the pack
  operationalises that sentence.
