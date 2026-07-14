# exercise-06: Public-Consultation Submission Flow Authoring

**Estimated effort:** 3 hours

## Objective

Author the enterprise's **public-consultation submission flow** —
the internal drafting cycle that carries a request-for-comment from
horizon-scan trigger, through stance decision, through drafting and
CxO peer review, through head sign-off, to submission and archive.
The deliverable is the flow document plus one worked-example
submission draft filed against a real, currently-open (or
recently-closed) consultation.

The pack is not "notes on how consultations should work." It is the
process the head would run on the next request-for-comment that
lands in the enterprise's inbox, together with a first-cut worked
draft that could go to CxO peer review as-is.

## Prerequisites

- [chapter 06](../06-public-consultation-submission-flow.md) —
  Owning the Public-Consultation Submission Flow — read and
  internalised.
- [[mod-105-regulatory-change-management]] — the horizon-scanning
  discipline that surfaces consultations in the first place; the
  flow authored here consumes its output feed.
- [[mod-106-external-positioning-and-voluntary-codes]] — the
  voluntary-code engagement pattern (Frontier Model Forum,
  Partnership on AI, MLCommons, EU GPAI Code) that runs adjacent
  to formal consultation submission.
- [chapter 07](../07-engagement-versus-legal-opinion-boundary.md)
  — the GC boundary on positions the enterprise takes on the
  public record.
- A concrete enterprise in mind, with an assumed sector, an
  approximate AI portfolio scale, and a jurisdictional footprint
  that tells you which consultation surfaces bind the enterprise.
  Where the enterprise is hypothetical, hold a working assumption
  and record it.

## Steps

1. **Consultation portfolio selection.** From chapter 06's standing
   list — NIST AI RMF and AISI, EU AI Office GPAI Code and
   guidance, CEN-CENELEC JTC 21 (via mirror committee), ISO/IEC
   JTC 1/SC 42, CPPA ADMT rulemaking, FDA GMLP and PCCP dockets,
   UK ICO consultations, state-AG rulemakings (Colorado AI Act
   and comparable), sector-regulator consultations (Federal
   Reserve, NAIC, EBA, ECB, sector equivalents) — select a
   working subset of at least five surfaces the enterprise will
   engage with as standing portfolio. For each surface record a
   one-line rationale for inclusion and a named owner.
2. **Trigger-to-submission flow diagram.** Draw the pipeline
   from horizon-scan trigger through stance decision (submit /
   co-sign / observe / decline) through internal drafting cycle
   through CxO peer review through head sign-off through
   submission channel through archive. The diagram names an
   owner at every stage — trigger owner, stance decider, draft
   owner, subject-matter contributors, peer reviewers, signatory,
   escalation signers. A stage without a named owner is a stage
   that will slip the window.
3. **Internal drafting-cycle roster.** For each named role on the
   flow diagram, author a one-line role definition and the
   handoff the role is accountable for. Record the escalation
   thresholds pre-agreed with CEO, GC, and (where applicable)
   the board chair — the size, visibility, or divergence-from-
   industry that promotes a submission from head sign-off to
   CEO or GC or board-chair sign-off. Thresholds are set once,
   not negotiated per submission.
4. **Position-lens discipline artefact.** Author the internal
   decision-record template the head fills for each submission,
   which states explicitly which of the three lenses — proprietary
   interest, industry-common, or principled — the submission is
   written in. The template records the lens choice, the
   rationale, the sign-off, and the archive reference. One
   submission, one lens.
5. **Industry-body-composition discipline.** Author the short
   decision rule the head applies to determine whether a given
   consultation warrants direct submission alone, industry-body
   co-signature alone, both aligned, or both divergent with
   explicit signposting. Name the industry bodies the enterprise
   is a member of (BSA, ITI, Chamber of Digital Commerce,
   INCOMPAS, sector trade associations) and record the signatory
   thresholds each body applies.
6. **Archive discipline.** Author the versioning, retention, and
   retrieval standard for submissions. Concretely: the fields on
   every archived record (docket cross-reference, stance memo,
   lens, draft owner, signatory, filed version, drafting version
   history, peer-review comment record, retention date), the
   directory or GRC-tool location, and the retrieval convention
   that lets a cold reader find any prior submission by
   consultation, date, or lens.
7. **Worked-example submission draft.** Select one real,
   currently-open consultation — or a recently-closed one if
   nothing consequential is open in the enterprise's binding
   jurisdictions — and draft a full submission to it. The draft
   is short (500-800 words) but complete: it opens on the
   enterprise's position, argues from a specific rationale,
   makes a specific ask on the specific docket question, and is
   written in a single named lens declared on the accompanying
   internal decision record.
8. **Cycle rehearsal.** Read the worked draft back against the
   flow document. Confirm that every stage the flow requires has
   been executed against the worked draft (or explicitly marked
   as pending, with the pending party named), and that the
   internal decision record for the worked draft is populated.

## Deliverables

- `consultation-portfolio.md` — the working subset of at least
  five consultation surfaces with rationale and named owner per
  surface.
- `submission-flow.md` — the flow document with the trigger-to-
  submission diagram, the drafting-cycle roster, and the
  escalation thresholds.
- `lens-decision-record-template.md` — the position-lens
  discipline artefact template.
- `industry-body-composition.md` — the decision rule for direct
  versus co-signed versus combined filings.
- `archive-standard.md` — the versioning, retention, and
  retrieval standard.
- `worked-submission-draft.md` — the 500-800-word draft
  submission to a specific real docket.
- `worked-submission-decision-record.md` — the populated lens
  decision record accompanying the worked draft.

## Acceptance criteria

- The consultation portfolio has at least five named surfaces,
  each with a named owner and a rationale that ties the surface
  to the enterprise's binding jurisdictions or capability
  exposure. "Because it is on the list" is not a rationale.
- The flow diagram has a named owner at every stage —
  including the escalation stages. No stage reads "TBD" or
  "the team."
- The escalation thresholds are specific enough that an
  incoming head can determine, from reading the document
  alone, whether a given submission requires CEO or GC or
  board-chair sign-off without reconvening the thresholds
  conversation.
- Every consultation surface in the portfolio has a documented
  default stance (submit / co-sign / observe / decline) and a
  rationale for that default. Actual per-consultation stance
  decisions still get made per docket; the portfolio-level
  default sets the starting point.
- The worked draft is written in a single named lens; the lens
  is declared on the internal decision record; the draft does
  not mix lenses.
- The archive discipline is retrievable-cold — an incoming
  head, given the archive and no other context, can find any
  prior submission by consultation, date, or lens using only
  the standard the artefact describes.
- The worked draft names a specific docket, a specific
  question inside that docket, a specific position, and a
  specific ask. A draft that argues around the docket without
  answering a docket question is not a submission.

## Stretch goals

- Circulate the worked draft to a peer at head-of-role or
  senior-architect level — or to an internal CxO if the
  enterprise is real — for one round of peer critique, and
  incorporate the critique into a revised draft. Record what
  the peer changed and what the head accepted or rejected, and
  what the accept-reject rationale was.
- Author a short retrospective (one page) on a real
  consultation the enterprise has previously submitted to,
  covering: what was filed, in which lens, what the enterprise
  now sees as the strong and weak paragraphs, and what the
  next drafting cycle should carry forward or drop. Where no
  real prior submission exists, write the retrospective as a
  forward-looking one on the worked example — what the head
  will want to know about this submission twelve months out.
- Produce the flow in a form directly importable into whichever
  GRC-for-AI platform the enterprise has selected (Credo AI,
  Holistic AI, ModelOp, Monitaur, ServiceNow AI Control Tower,
  IBM watsonx.governance, or the actual platform), so the
  portfolio, the stance, and the archive are machine-queryable
  rather than only human-readable.

## Notes and starter guidance

- The failure mode chapter 06 warns about is the mixed-lens
  submission — the paragraph that opens on principle, argues
  from proprietary interest, and closes on industry consensus.
  The lens decision-record artefact exists specifically to
  block this failure at drafting time, not to catch it after
  filing. Populate the record before the draft, not after.
- Resist the temptation to make the portfolio exhaustive.
  Every surface in the portfolio is a standing commitment of
  head-owned drafting capacity. Five surfaces the enterprise
  actually engages with beats fifteen surfaces the enterprise
  aspires to engage with; the aspirational surfaces slip and
  the slippage is the credibility incident.
- The worked draft is where the flow is stress-tested. If you
  cannot populate the decision record — if you cannot name the
  lens, the ask, the reviewer roster, or the sign-off path —
  the flow document is under-specified and needs revision
  before the draft is finished.
- Where a consultation surface, docket status, or industry-body
  policy is uncertain, mark it explicitly as needs-research and
  proceed. Do not fabricate a docket number, comment window, or
  signatory-body threshold; the archive discipline this exercise
  is teaching depends on records being trustworthy.
- The archive is the artefact that outlasts the head. Build it
  for the four cold readers chapter 06 names — successor,
  plaintiff's counsel, journalist, incoming regulator — not for
  the head's own current convenience.
