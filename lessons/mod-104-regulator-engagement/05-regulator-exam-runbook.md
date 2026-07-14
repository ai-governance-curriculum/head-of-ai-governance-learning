# The Regulator-Examination Runbook at Leadership Scope

## Motivation

An examination is the moment where the AI governance program either
shows itself as a running program or shows itself as a story. A
regulator arrives — on-site or remote — with a scope letter, an
evidence request list, and an interview schedule. Over the days or
weeks that follow, the regulator forms a durable supervisory
impression of the enterprise. That impression sets the terms of the
next several years of engagement, drives whether findings are
written as observations or as formal instruments, and — in the
severe case — determines whether the file moves from supervision to
enforcement. The head of AI governance runs the exam for the
enterprise as its accountable executive.

The exam-runbook discipline is well-established in banking
supervision. The OCC's *Comptroller's Handbook* series
(risk-governance, model-risk-management, and corporate-and-risk-
governance booklets) describes the examination process on the
regulator side. Federal Reserve supervisory letters — the SR-letter
series, notably SR 11-7 on model-risk management and SR 21-3 / SR
23-4 on governance — describe supervisory expectations that shape
what examiners look for. The FDIC's *Risk Management Manual of
Examination Policies* codifies the same discipline for
FDIC-supervised institutions. OSFI's supervisory framework and the
PRA's *Approach to banking supervision* and associated
supervisory statements are the equivalent references outside the
US. The UK ICO's *Regulatory Action Policy* codifies the
data-protection equivalent for UK enterprises. The EU AI Act
Chapter IX (Articles 74-84) sets the market-surveillance regime
that AI-specific examinations under the Act will follow.

The head reads those regulator-side references and inverts them
into an enterprise-side runbook. Improvising an exam response is
the failure mode. Carrying a pre-designed runbook — rehearsed,
CxO-aligned, and legible to the regulator — is the discipline.
This chapter is that runbook at leadership scope. The paired
level-50 senior-ai-governance-architect owns the operational
rehearsal and the evidence-room mechanics
([[mod-102-running-the-program]]); the head owns the executive
posture, the CxO alignment, the findings-conference stance, and
the long-lived supervisory-instrument relationship.

## Core concept: six phases, one continuous relationship

A regulator examination is not a single event. It is a sequence of
six phases the head runs against a pre-designed shape:

1. **Pre-exam preparation** — from notification through the day
   before entrance.
2. **Entrance conference** — the opening meeting where scope,
   posture, and ground rules are set.
3. **Evidence-request handling** — the operational bulk of the
   exam, RFI cadence and interview scheduling.
4. **Findings conference** — the regulator's preliminary findings
   delivered back, and the enterprise's posture in response.
5. **Remediation planning** — the written commitment against each
   finding with owners, dates, and evidence-of-closure standards.
6. **Post-exam relationship management** — MOU / MRA / MRIA /
   consent-order stewardship as long-lived engagement contracts.

The phases are sequential but the relationship is continuous. The
regulator who runs the entrance conference is the same portfolio
supervisor the head will call about the next incident, the next
material change, the next voluntary disclosure. The head runs each
phase in a way that makes the next phase easier — and that keeps
the enterprise inside the *cooperative-counterparty* posture
rather than the *problem-file* posture that Chapter 01 named.

The remainder of this chapter walks each phase in its own H2.

## Phase 1 — pre-exam preparation

Notice varies by regime. Federal banking supervisors typically
issue an entry letter thirty to sixty days ahead of a full-scope
examination; OSFI's supervisory framework runs a comparable
notification cycle. The EU AI Act's market-surveillance regime
under Articles 74-84 leaves timing to national competent
authorities and is expected to normalise around comparable
notification windows. Sector regulators outside banking (FDA,
CPPA, ICO) run their own notification patterns.
<!-- needs-research: verify specific notification windows for
Federal Reserve, OCC, and FDIC full-scope exams against current
Comptroller's Handbook and FDIC RMS Manual sections. -->

The head uses the notice window to run four workstreams in
parallel:

**Assemble the evidence room.** The architect (level 50)
physically assembles what the regulator's scope letter requests or
what the regulator's chosen evidence-portal equivalent expects.
The head reviews the assembled artefact set for shape and
completeness: the AIMS policy suite; the AI risk register; the AI
system inventory with tiering; model documentation for every
in-scope system; evaluation records and monitoring outputs;
incident and near-miss register with reportability rationale;
third-party attestations and vendor register; board and committee
packs for the relevant periods; prior regulator correspondence and
open items. If a scope-relevant artefact is missing, the head
knows before the entrance conference — not during it. See
[[mod-102-running-the-program]] for the evidence-room discipline
the material lands in.

**Rehearse.** The architect runs an operational mock exam — RFI
handling, interview logistics, document production mechanics. The
head runs an executive rehearsal at a different altitude:
entrance-conference opening framing, likely first-week strategic
questions, positioning on the two or three portfolio matters the
head expects the regulator to press on. The rehearsal is video-
recorded or minuted; the head watches the tape.

**Align peer CxOs.** The head walks the exam scope with each peer
who has a stake:

- General Counsel — legal exposure, privilege protocol,
  attorney-work-product boundaries, when GC attends interviews.
- Chief Risk Officer — enterprise-risk posture, where the AI
  program sits inside the parent risk framework, ERM signalling.
- Chief Information Security Officer — cyber-adjacent exposure,
  overlap with any concurrent SOC / ISO / NIST-CSF assessments.
- Chief Audit Executive — third-line independence, whether
  internal audit's own AI-related workpapers will be requested and
  under what privilege posture.
- Chief Privacy Officer or Data Protection Officer — privacy
  interfaces, DPIA production, cross-border data flow posture.
- Head of Communications and Head of Government Affairs — external
  and political posture, message discipline if the exam becomes
  public, regulator-leadership relationships.

Alignment is not a status meeting. It is a written pre-exam brief
each CxO signs off on covering their scope of engagement, their
named point-of-contact, and their escalation protocol during the
exam.

**Brief the board.** Under the cadence established in
[[mod-103-board-and-audit-committee-reporting]], the audit-committee
chair (or risk-committee chair, depending on charter) is briefed on
scope, anticipated findings-risk, and the enterprise's posture
before the entrance conference. Directors do not read exam scope
letters through minutes; the head walks the chair through it
personally.

## Phase 2 — entrance conference

The entrance conference is the opening meeting. The head
personally attends. Sending a delegate is a signal the regulator
reads. The conference has a script the head runs to:

**Enterprise opening framing.** A short, non-defensive statement
of what the enterprise does with AI, how it governs the program,
what has materially changed since prior engagement, and how the
enterprise intends to work with the exam. This is not a marketing
statement. It is the frame the regulator will carry through the
weeks that follow. The head drafts it, GC reviews it, the CEO or
the appropriate line-of-business president is briefed on it.

**Point-of-contact introductions.** The head introduces the named
point-of-contact for each evidence stream — policy suite, risk
register, inventory, model documentation, evaluations, incidents,
third parties, board records. Every stream has a named POC and a
named back-up. The regulator writes those names down; the
enterprise honours them for the duration of the exam.

**RFI ground rules.** The head and the examiner-in-charge agree —
in writing where possible — on the RFI cadence: format (regulator
portal, secure file transfer, physical delivery), SLA (typical
practice is same-day acknowledgement and a substantive-response
target the regulator names), hand-off from RFI to enterprise POC,
and the escalation path if an RFI is ambiguous or overbroad.

**Interview ground rules.** Which enterprise staff are available
for interview, notice period before interview, who from the
enterprise sits in as observer, when GC attends, whether interviews
are recorded, and the protocol for interview-transcript review.
Banking-supervisor practice and ICO enforcement practice differ on
these questions; the head confirms the regulator's practice
against the enterprise's protocol at the entrance rather than
discovering the mismatch mid-exam.

**Escalation protocol.** How disagreements are surfaced during
the exam rather than accumulated for the findings conference. The
head names — on both sides — who takes the phone call if the
enterprise believes an RFI is out of scope, or if the regulator
believes the enterprise is being unresponsive. Having a named
escalation on both sides prevents the kind of silent drift that
turns an observation into an MRA.

## Phase 3 — evidence-request handling

RFI cadence is the operational bulk of an exam. The failure modes
are all discipline failures: inconsistent responses across RFIs,
privileged material released, documents produced without
production stamps, interview positions that diverge from written
positions. The head runs the consistency discipline; the architect
runs the mechanics.

The head's discipline:

**Every RFI logged, dated, owned, tracked to close.** A single
RFI register — not per-stream registers — with entry ID, receipt
date, source examiner, scope, owner, GC-review status, dispatch
date, and follow-up status. The head reviews the register at daily
or twice-daily cadence during an active exam.

**Every response GC-reviewed before release.** No RFI response
leaves the enterprise without GC sign-off. GC is looking for two
things: privilege exposure (attorney-client, work-product, joint-
defence where applicable) and interpretive gotchas — responses
that could be read to concede a legal position the enterprise has
not decided to concede. The head does not release "on GC's behalf"
or "GC unavailable"; the head waits.

**Every response consistent with prior responses.** The head
personally runs the consistency check across RFIs. Regulators
compare answers. An inventory count that differs by six systems
between the third RFI and the seventh RFI without an explanation
is the finding that generates the next finding. The head keeps a
running consistency table cross-referenced to prior responses.

**Every document produced under a production stamp.** Bates-
numbering is the US-litigation convention; the regulator-portal
equivalent (production reference numbers, secure-hash manifests)
serves the same function in supervisory practice. Every page
produced is uniquely identifiable so that a later reference — from
the regulator, from GC, from a plaintiff — can be traced to the
original production event.

**Every interview has an internal debrief.** Immediately after each
interview, the enterprise POC and GC (where GC attended) capture
what was asked, what was answered, what was promised as follow-up,
and what the interviewee felt was pressed on. The debrief is not
a transcript — it is the enterprise's internal record of the
interaction. It informs the consistency table and the findings-
conference preparation.

## Phase 4 — findings conference

At the end of the on-site or on-portal phase, the regulator
communicates preliminary findings. The findings conference is the
moment where the head's posture matters most. The head responds
under a pre-agreed posture spectrum:

**Accept and remediate.** The finding is factually correct and
the enterprise commits, at the conference, to a remediation plan
against it. This is the default posture where the finding is
defensible on the record. Accepting cleanly — without hedging,
without minimising, without qualifying — buys the enterprise
supervisory credit that carries into later engagement.

**Accept but disagree with the characterisation.** The underlying
facts are correct but the regulator's characterisation of them is
stronger than the record supports. Example: a control gap the
regulator characterises as "systemic" that the enterprise reads as
"scoped to one line of business". Head takes the technical
position at the conference; GC takes the legal position — usually
in the subsequent written response, not at the conference itself.

**Contest with basis.** The finding is factually or legally wrong
and the enterprise intends to respond formally. The head does not
adopt this posture alone at the conference. Contest-with-basis is
a joint call with GC and — for reputationally-significant matters
— with the CEO, and for matters that could reach public
enforcement, with the board or the appropriate board committee.
At the conference the head signals that a written response will
follow through GC on a stated timeline; the head does not
litigate the finding across the table.

The head reads the room. Escalating a finding into open
disagreement at the conference where a more measured written
response would have served better is a preventable error. Under-
responding to a finding that will crystallise into an MRA if not
pushed back on is a different preventable error. Judgement here
is the substance of the role.

## Phase 5 — remediation planning

The head owns the remediation plan for every finding the
enterprise has accepted, with or without disagreement on
characterisation. The plan is a written commitment to the
regulator and — through the audit committee — to the board.

Every finding has, at minimum:

- Named owner (accountable executive, not a team).
- Milestone plan with dated interim commitments, not just an end
  date.
- Evidence-of-closure standard — what the enterprise will produce
  to demonstrate the finding has been remediated. If the standard
  is "the regulator agrees", the plan says so.
- Verification path — third-line internal audit, external
  attestation, regulator re-inspection, or self-certification.
  Higher-severity findings should not be self-certified.
- Board-reporting cadence — how the audit-committee or risk-
  committee will see progress against the plan and any slippage.

The plan is documented in the format the regulator expects. Banking
supervisors expect a written remediation plan with specific dates
tied to specific findings; some supervisors expect quarterly
written progress reports. UK ICO enforcement notices carry
compliance dates set in the notice. EU AI Act Chapter IX corrective-
action expectations under Articles 79-83 will normalise around
comparable practice.
<!-- needs-research: verify format expectations for remediation
plans against current OCC Comptroller's Handbook examination
sections and Federal Reserve SR-letter guidance. -->

Missing a remediation date is worse than the original finding.
Missing a date signals that the enterprise cannot deliver against
its own commitments, which is the supervisory concern the finding
was surfacing in the first place. The head builds slack into the
plan — commit dates the enterprise can meet, not dates the
enterprise hopes to meet — and manages the plan against those
dates with the same discipline as any other enterprise commitment.

## Phase 6 — post-exam relationship management

Exams produce instruments. Instruments live longer than exams. The
head manages the instrument portfolio as a set of long-lived
engagement contracts with the regulator.

**Memorandum of Understanding (MOU).** An informal supervisory
agreement between the regulator and the enterprise, typically
below the threshold of formal enforcement. Not public in most
cases. Binding on the enterprise's conduct for its duration.
Common across US federal banking supervisors as an alternative to
formal action.

**Matter Requiring Attention (MRA).** An OCC-origin instrument —
a formal finding in a supervisory letter that the enterprise is
required to address. Adopted in practice by other US federal
banking supervisors under their own vocabularies. An MRA is not an
enforcement action but it is on the enterprise's supervisory
record and it is one of the inputs to the CAMELS composite (or
the equivalent supervisory rating).
<!-- needs-research: verify current MRA / MRIA definitional
language against the OCC Comptroller's Handbook Corporate and
Risk Governance booklet. -->

**Matter Requiring Immediate Attention (MRIA).** The higher-
severity OCC-origin variant, indicating a finding the enterprise
must address on an accelerated timeline. Ignoring an MRIA is the
predicate for a consent order.

**Consent order / cease-and-desist order / civil money penalty.**
Formal enforcement actions under statutory authority — the FDIA
for FDIC, the FRA for the Federal Reserve, the National Bank Act
for OCC, the ICO's statutory powers for UK data protection. These
instruments are typically public, carry monetary or operational
consequences, and place the enterprise under formal compliance
obligations enforceable by the regulator. Consent orders are
negotiated; cease-and-desist orders can be issued unilaterally.

The head manages each live instrument with a running record: the
instrument text and its citations, the enterprise's committed
plan, evidence of ongoing compliance, status reporting cadence to
the regulator, and standing board or committee visibility. The
head does not let an instrument age quietly. Instruments that age
quietly become the subject of the next supervisory cycle.

## The GC and Government Affairs hand-off

Three principals share the regulator relationship at leadership
scope. The head runs the sequence:

**Head of AI governance.** Fronts the technical relationship
across all six phases. Owns the enterprise's posture, the
consistency of response, the remediation plan, and the standing
supervisory-instrument portfolio. Is the regulator's named
counterpart for AI-specific matters.

**General Counsel.** Owns legal interpretation, privilege, and
adverse-action defence. Reviews every RFI response before release,
attends interviews under the pre-agreed protocol, drafts formal
written responses to findings under contest-with-basis posture,
and takes the lead if the file moves toward enforcement. Any
moment involving formal legal position, litigation posture, or a
public regulatory statement requires GC on the line. Chapter 07 of
this module deals in detail with the boundary — where the head's
technical engagement ends and GC's legal engagement begins.

**Government Affairs.** Owns political relationships with
regulator leadership rather than staff-level examination.
Government Affairs is invoked where the engagement involves
legislative interaction, regulator-principal meetings, or public
positioning — rare in the course of a routine examination, real
in the course of a high-visibility one. The head does not run
that engagement directly; the head briefs Government Affairs so
that the enterprise voice is consistent across the staff-level
supervisory channel and the leadership-level political channel.

The sequence matters. The head fronts first; GC steps in at the
legal-position boundary; Government Affairs is invoked only when
the matter crosses into political territory. Inverting the
sequence — Government Affairs contacting a regulator whose
examination the head has not briefed them on, or GC opening
correspondence the head is unaware of — is how the enterprise
signals to the regulator that its house is not in order. The head
holds the sequence.

## Summary

- A regulator examination is a six-phase sequence — pre-exam
  preparation, entrance conference, evidence-request handling,
  findings conference, remediation planning, post-exam
  relationship — the head runs against a pre-designed runbook.
- The runbook inverts the regulator-side references: OCC
  Comptroller's Handbook, Federal Reserve SR-letters, FDIC Risk
  Management Manual, OSFI supervisory framework, PRA supervisory
  statements, UK ICO Regulatory Action Policy, EU AI Act Chapter
  IX (Articles 74-84) for market surveillance.
- Pre-exam preparation is four workstreams in parallel — evidence-
  room assembly (architect-owned mechanics; head-owned shape),
  executive rehearsal, peer-CxO alignment with written brief, and
  audit-committee-chair briefing per
  [[mod-103-board-and-audit-committee-reporting]].
- Entrance-conference script: opening framing, named POCs, RFI
  ground rules, interview ground rules, named escalation protocol
  on both sides.
- RFI discipline is a consistency discipline — every RFI logged,
  every response GC-reviewed, every response cross-checked against
  prior responses, every document produced under a production
  stamp, every interview debriefed. The head runs the consistency
  check personally.
- Findings-conference posture spectrum: accept-and-remediate;
  accept-but-disagree-with-characterisation; contest-with-basis.
  Contest-with-basis is never the head's call alone.
- Remediation plans have owners, milestones, evidence-of-closure
  standards, verification paths, and board-reporting cadence.
  Missing a remediation date is worse than the original finding.
- Post-exam instruments — MOU, MRA, MRIA, consent order, cease-
  and-desist, civil money penalty — are long-lived engagement
  contracts with running records and board visibility. Chapter 04
  of this module extends the MRA/MRIA vocabulary into sector-
  specific escalation taxonomy.
- The head fronts the technical relationship, GC covers legal
  interpretation and adverse-action defence, Government Affairs
  covers political interaction with regulator leadership. Chapter
  07 deals with the head/GC boundary in detail.
