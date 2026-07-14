# exercise-04: Reporting Pipeline and CxO Sign-Off Flow

**Estimated effort:** 3 hours

## Objective

Produce a defensible **reporting-pipeline document** and a
**CxO sign-off flow**, together sufficient to carry the packs from
exercises 01, 02, and 03 through one full reporting cycle without
last-minute scrambling. The pipeline document names every evidence
input, its producer, its cadence, its retention path, and its
quality bar. The sign-off flow names the CxO owners, the timeline
working backward from committee distribution, and the discipline
for conflicts and late-breaking material.

The deliverable is not "here is how pack production works." It is
the two documents an ISO/IEC 42006 auditor could sample against —
one to trace any value back to source, one to confirm ownership of
every conclusion — plus the addendum discipline for when the world
does not pause between evidence-lock and distribution.

## Prerequisites

- Chapter [04-cxo-content-ownership-and-signoff](../04-cxo-content-ownership-and-signoff.md)
  read and internalised.
- Chapter [05-reporting-pipeline-discipline](../05-reporting-pipeline-discipline.md)
  read and internalised.
- Exercises 01, 02, and 03 in draft or complete form. The
  pipeline and sign-off flow have to carry those three packs, so
  the pack shape has to be visible before the pipeline can be
  authored.
- Working assumption of the CxO peer group and reporting-line
  structure at the enterprise (mod-101 chapter 06).

## Steps

1. **Pipeline document.** Author the pipeline as a table. One row
   per evidence category from chapter 05 (AI-system inventory
   evidence, portfolio risk-register evidence, KRI telemetry,
   incident and near-miss log, third-party vendor evidence,
   regulator engagement log, regulatory-change monitoring log,
   audit-plan and third-line findings, external audit and
   certification-body findings, maturity-assessment posture) —
   with columns for producer (role), cadence, retention path
   (specific system of record and archive path), quality bar
   (schema, checklist, or minimum-fields specification), and
   downstream cluster reference (which cluster of which pack
   this row feeds). Extend beyond chapter 05's list if the
   enterprise runs additional evidence categories.
2. **Sign-off ownership map.** Author the mapping of each pack
   cluster (across the three packs from exercises 01-03) to a
   named CxO owner (CRO, CAE, GC, CISO, CPO/DPO, CTO, or the
   head — see chapter 04 for the distribution). Where a cluster
   has multiple contributing owners, name the primary and the
   contributors. Where an ownership is contested at the
   enterprise (a common early-program problem), name the
   contested position and the escalation path.
3. **Sign-off timeline.** Author the specific working-backward
   timeline from committee distribution (T-0) for each of the
   three packs. Chapter 04 sketches a seven-business-day
   baseline; adapt for the enterprise's committee calendar and
   pack complexity. The timeline names, per day: what is due
   from whom, in what form, to whom. Include the evidence-lock
   date and the sign-off checkpoints.
4. **Conflict-escalation discipline.** Author the half-page
   discipline for what happens when two content owners disagree
   about a cluster's content. Include the three specific
   scenarios from chapter 04 (CAE-vs-second-line factual
   disagreement, GC-vs-CISO on incident wording, CRO-wanting-to-
   backdate-against-unratified-appetite) and the head's
   response pattern for each.
5. **Addendum discipline.** Draft the addendum template for
   material events between evidence-lock (T-7) and distribution
   (T-0). Include the fields chapter 05 names (identifier,
   event, provenance, current status, recommended committee
   action, CxO sign-off). Draft one worked addendum for a
   plausible late-breaking event (a serious incident, a
   regulator notification, a stop-shipping trigger firing) that
   would land inside the reporting window.
6. **Sign-off as a control.** Author the specification for how
   sign-off is captured (which GRC-for-AI platform workflow or
   which email-and-document-control fallback), what metadata is
   preserved (signer, timestamp, document version, comments),
   and what the retention path is. Sign-off is an AIMS control;
   the specification is how it becomes inspectable.

## Deliverables

- `pipeline-document.md` (or `.csv`) — the evidence-category
  table with all six columns populated per row.
- `sign-off-ownership-map.md` — the pack-cluster-to-CxO
  mapping across the three packs.
- `sign-off-timeline.md` — the working-backward timeline per
  pack.
- `conflict-escalation-discipline.md` — the half-page
  discipline with the three scenarios.
- `addendum-template.md` and `addendum-example.md` — the
  template and one worked example.
- `sign-off-as-a-control.md` — the specification for capture,
  metadata, and retention.

## Acceptance criteria

- Every row of the pipeline has every column populated. "TBD"
  or "various" in the producer column is disqualifying. Producers
  are named as roles (not individuals) so the pipeline survives
  personnel change.
- The sign-off ownership map covers every cluster of every
  pack (exercises 01, 02, and 03). Any cluster without an
  owner is a cluster the head is implicitly claiming as their
  own — if that is the intent, the head signs; if not, an
  owner is added.
- The sign-off timeline is specific enough that an operator
  could run it from the document alone. Vague phrases ("shortly
  before distribution") are cut.
- The conflict-escalation discipline includes the head's
  response pattern for each of the three scenarios, not just
  the scenarios themselves.
- The addendum example is plausible for the enterprise's
  scenario and populated at the depth the template requires.
- The sign-off-as-a-control specification names the specific
  tool (or the fallback if none) and the retention path — not
  a generic reference to "the GRC platform."

## Stretch goals

- Draft the specific queries the head runs on the pipeline
  document itself to answer operational questions ("which
  evidence categories were late in the last three cycles";
  "which producers have never met a target date"; "which
  clusters have had ownership contested"). The pipeline is
  itself a subject of measurement.
- Draft the escalation memo template the head uses when a
  content-owner conflict has to be escalated to the audit-
  committee chair before distribution (chapter 04). Include
  one worked memo for the CAE-vs-second-line-disagreement
  scenario.
- Draft the specific instrumentation (or the specification for
  it) that would auto-produce the pipeline-adherence view for
  each cycle — timeboxes met and missed, sign-offs late,
  addenda filed. Adherence metrics are the honest way to see
  whether the discipline is holding.
- Circulate the pipeline and sign-off flow to a peer at head-of-
  program level and to the enterprise's actual (or hypothetical)
  CAE-role holder for a critique round.

## Notes and starter guidance

- The most common failure of a first-cut pipeline is that it
  is authored from the head's own function's perspective and
  under-specifies the inputs from other functions. Every
  category with an external producer (CISO, GC, CAE) has to be
  authored *with* the external producer, not for them.
- Roles, not individuals. A pipeline that names "Priya" as
  the producer of KRI-04 is a pipeline that breaks when Priya
  changes role. Name the function.
- Where sign-off is captured by email, capture *every* sign-
  off by email. Where sign-off is captured by GRC workflow,
  capture *every* sign-off by workflow. Mixed conventions are
  what create the "we thought so-and-so signed off" audit
  finding.
- The addendum discipline is what preserves comparability
  (chapter 01) across the pack archive. Silent edits to a
  distributed pack destroy comparability; addenda preserve it.
