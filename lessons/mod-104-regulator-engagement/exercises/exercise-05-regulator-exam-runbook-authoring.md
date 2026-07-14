# exercise-05: Regulator-Examination Runbook Authoring

**Estimated effort:** 4 hours

## Objective

Produce the **leadership-scope regulator-examination runbook** the
head of AI governance keeps ready-to-run for the enterprise —
against either a scheduled full-scope examination or a no-notice
supervisory visit from the chosen regulator. The runbook is the
six-phase artefact from chapter 05 (pre-exam preparation, entrance
conference, evidence-request handling, findings conference,
remediation planning, post-exam relationship management), authored
at the altitude the head personally runs rather than the
operational altitude the architect owns.

The deliverable is not a set of notes about how exams work. It is
the ring-binder-and-cover-sheet artefact a peer head reading it
cold could act out — phase by phase, artefact by artefact, hand-off
by hand-off — without having to ask further questions of the head
who wrote it.

## Prerequisites

- [chapter 05](../05-regulator-exam-runbook.md) — The Regulator-
  Examination Runbook at Leadership Scope — read and internalised.
- [[mod-102-running-the-program]] — the evidence-room discipline
  under which the architect assembles what the runbook indexes into.
- [[mod-103-board-and-audit-committee-reporting]] — the board-
  briefing cadence the runbook plugs the audit-committee-chair
  briefing into.
- [chapter 04](../04-sector-regulator-engagement-pattern.md) — the
  sector-specific escalation taxonomy the post-exam instrument
  vocabulary draws from.
- [chapter 07](../07-engagement-versus-legal-opinion-boundary.md) —
  the head / GC boundary the hand-off diagram encodes.
- A concrete enterprise in mind (real or hypothetical), with a
  named sector, jurisdictional footprint, and prior regulator-
  engagement history to hold as the scenario.

## Steps

1. **Regulator selection.** Pick one specific regulator against
   whom the runbook will be authored. Options include: a national
   competent authority under the EU AI Act (name the country and
   the designated NCA); a US federal banking supervisor (OCC,
   Federal Reserve, FDIC); a state Department of Insurance running
   an AI/model-governance examination; the UK ICO; the California
   Privacy Protection Agency; or another concrete choice with a
   published supervisory practice. Record why this regulator is the
   primary counterpart for the enterprise. The runbook is regulator-
   specific — vocabularies, notification windows, portal
   conventions, and instrument taxonomies differ.
2. **Pre-exam preparation section.** Author the pre-exam workstream
   the head runs in parallel with the architect's operational
   assembly. Include: the evidence-room contents index mapped
   against the RFI template the chosen regulator publishes (or a
   defensible reconstruction where none is published); the mock-
   exam rehearsal script for the executive-altitude rehearsal
   (opening framing, first-week strategic questions, portfolio
   pressure points); the CxO peer alignment agenda with named
   attendees and the written pre-exam brief each peer signs off on;
   and the board / audit-committee-chair briefing memo template.
3. **Entrance conference section.** Author the script the head runs
   at the opening meeting. Include: the enterprise opening framing
   (short, non-defensive, GC-reviewed); the point-of-contact map
   listing every evidence stream with named POC and back-up;
   ground rules the head proposes for RFI cadence and interview
   handling; and the escalation protocol for surfacing
   disagreements during the exam rather than accumulating them.
4. **Evidence-request handling section.** Author the RFI-discipline
   pack. Include: the RFI register fields (entry ID, receipt date,
   source examiner, scope, owner, GC-review status, dispatch date,
   follow-up status, SLA clock); the GC-review protocol; the
   consistency-check discipline (running consistency table across
   RFIs); the interview-debrief template; and the document-
   production stamp convention the enterprise will use (Bates or
   regulator-portal equivalent).
5. **Findings-conference posture section.** Author the three-
   posture spectrum from chapter 05 — accept-and-remediate;
   accept-but-disagree-with-characterisation; contest-with-basis —
   and the decision protocol for choosing between them. The
   protocol names: who is consulted before adopting contest-with-
   basis, what evidence base is required, how the posture is
   signalled at the conference itself versus in written follow-up,
   and the escalation to CEO or board where the finding is
   reputationally or enforcement-significant.
6. **Remediation planning section.** Author the finding-template
   the head fills for every accepted finding. Include: named owner
   (accountable executive); milestone plan with dated interim
   commitments; evidence-of-closure standard; verification path
   (third-line audit, external attestation, regulator re-inspection,
   self-certification — with the tier where each is acceptable);
   board-reporting cadence for progress against the plan; and the
   slack-inclusion discipline that keeps commit dates ones the
   enterprise can meet rather than ones it hopes to meet.
7. **Post-exam relationship management section.** Author the
   instrument-management discipline for whichever instrument the
   chosen regulator uses (MOU, MRA, MRIA, consent order, cease-and-
   desist order, civil money penalty, ICO enforcement notice, EU AI
   Act corrective-action order under Articles 79-83, or the
   sector equivalent). Include: the running record fields per live
   instrument; the enterprise reporting cadence to the regulator;
   standing board or committee visibility; and the trigger for
   escalating an aged instrument before the next supervisory cycle
   reopens it. Where a specific regulator's instrument vocabulary
   is unfamiliar, mark it `<!-- needs-research -->` rather than
   inventing terminology.
8. **GC and Government Affairs hand-off diagram.** Author the six-
   phase runbook as an annotated diagram (ASCII, table, or figure
   reference) with GC-must-be-present points and GA-should-be-
   consulted points marked on each phase. Chapter 07's head / GC
   boundary is the source of truth for the GC annotations; the
   Government Affairs invocation is the political-territory
   threshold from chapter 05.

## Deliverables

- `regulator-selection.md` — the chosen regulator, the enterprise
  rationale, and the supervisory-practice reference base.
- `phase-1-pre-exam.md` — evidence-room index, rehearsal script,
  CxO alignment agenda, board-chair briefing memo template.
- `phase-2-entrance-conference.md` — opening framing, POC map,
  ground rules, escalation protocol.
- `phase-3-evidence-handling.md` — RFI register schema, GC-review
  protocol, consistency-check discipline, interview-debrief
  template, production-stamp convention.
- `phase-4-findings-posture.md` — three postures with decision
  protocol.
- `phase-5-remediation.md` — finding template and slack-inclusion
  discipline.
- `phase-6-post-exam-instruments.md` — instrument-management
  discipline for the chosen regulator's instrument set.
- `gc-and-ga-handoff.md` — the annotated six-phase diagram with
  legal-and-political hand-off points.

## Acceptance criteria

- Every phase names a specific artefact the head produces at that
  phase — not "prepare for the exam" but "produce the evidence-
  room contents index against the RFI template regulator X
  publishes." A reader can point to the artefact for each phase.
- Every phase has a named signer (role, not team), an SLA (clock
  time or business days), and an escalation path (named role on
  both enterprise and regulator side where the regulator side is
  knowable).
- The GC hand-off is drawn on every phase where legal
  interpretation might be needed, not only where it is certain to
  be needed. Under-annotation of the GC hand-off is a failure
  mode; over-annotation is acceptable.
- The runbook is defensibly rehearsable: a peer at head-of-role
  level, reading it cold without prior briefing, can act out each
  phase against the chosen regulator without asking further
  questions. Ambiguity that requires a phone call to the author
  fails this criterion.
- Regulator-specific vocabulary is used precisely. Terms borrowed
  from another regulator's regime (importing MRA vocabulary into a
  jurisdiction that does not use it) are flagged and replaced with
  the correct term, or the uncertainty is marked
  `<!-- needs-research -->`.

## Stretch goals

- Author a **table-top exercise script** the head can run once a
  year with the CxO peer group — scenario prompt, injects at set
  intervals, decision points, and after-action review structure —
  that rehearses phases 1 through 4 of the runbook against a
  simulated notification from the chosen regulator.
- Author a **lessons-learned template** for the post-exam
  retrospective the head runs with the peer CxOs after an actual
  examination closes. The template captures what the runbook got
  right, what it got wrong, what has to change before the next
  cycle, and how the changes are tabled to the audit committee.
- Author a **no-notice supervisory-visit variant** of phases 1
  through 3 — the compressed version the head runs when the
  entry letter arrives with no notice, common in state DOI and
  ICO practice for cause-based visits. The variant re-orders and
  compresses; it does not skip phases.
- Extend the post-exam section with an **instrument-portfolio
  dashboard** — the single-page view of every live instrument
  across regulators the head keeps in front of the audit-committee
  chair on the cadence set by
  [[mod-103-board-and-audit-committee-reporting]].

## Notes and starter guidance

- Resist the urge to author the runbook regulator-agnostically.
  Chapter 05 lists a spread of regulator-side references
  precisely because the shape differs. A runbook authored to the
  OCC Comptroller's Handbook reads differently to one authored to
  an EU AI Act NCA under Articles 74-84 differently to one
  authored to the UK ICO Regulatory Action Policy. Pick one and
  commit to its vocabulary; extensibility comes later.
- The pre-exam preparation section is the section most first-cut
  runbooks under-invest in. The exam is won or lost in the notice
  window; the entrance conference is where the position becomes
  visible. If the pre-exam section is shorter than the entrance-
  conference section, the runbook is under-authored.
- The GC hand-off diagram is not a courtesy. Chapter 07 treats the
  head / GC boundary as a first-order concern. Under-annotating
  GC on the runbook is the failure mode that produces the RFI
  response released without GC review — the single most common
  preventable failure in an active examination.
- Where the chosen regulator has not published the artefact the
  runbook needs (an RFI template, a specific interview protocol,
  a published instrument taxonomy), reconstruct defensibly from
  the closest analogue and mark the reconstruction
  `<!-- needs-research -->` for verification against the actual
  regulator publication before the runbook is put into service.
- The runbook is a living artefact. Author it at the version-1
  altitude a head could put into service on day one of the role,
  not the perfected version that emerges after three exam cycles.
  Perfection is the enemy of a runbook that exists.
