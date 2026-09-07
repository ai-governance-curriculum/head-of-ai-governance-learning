# exercise-04: RFI / RFP Response Runbook

**Estimated effort:** 3 hours

## Objective

Author the enterprise **RFI / RFP response runbook** — the
routing discipline that turns request-shaped inbound (regulator
RFIs, industry-body RFIs, academic RFIs, customer procurement
RFPs, and the industry-wide regulator RFIs adjacent to the
public-consultation cycle) into a coherent internal drafting
cycle and a defensible cumulative corpus of responses. The
deliverable is the intake register, the drafting cycle, the
customer-RFP answer library, the head-and-CRO joint operating
agreement, and the intake owner's day-one playbook.

The runbook has to survive four stress tests. First, a
regulator RFI addressed to the enterprise arrives on a Friday
afternoon with a two-week response window; the intake owner
routes it correctly on Monday morning without escalating to
the head to decide the routing. Second, a customer procurement
lead compares the enterprise's RFP answer on ISO/IEC 42001
conformance across three deals over eighteen months and finds
the answers materially consistent; the answer library is what
made that so. Third, an incoming head reads the intake
register on day one and can tell which requests are in flight,
which stances have been settled, and which archived responses
would need to be updated if the enterprise's substantive
position moves. Fourth, an audit-committee chair asks "how does
the enterprise handle inbound RFIs and RFPs" — the register is
the evidence, not the head's memory.

The runbook is not a study of chapter 04. It is the artefact
that turns chapter 04's five-category taxonomy, its internal
drafting cycle, and its lens discipline into a repeatable
process any CxO peer can follow.

## Prerequisites

- Chapter [04-rfi-rfp-response-posture](../04-rfi-rfp-response-posture.md)
  — the five-category taxonomy (regulator-addressed,
  regulator industry-wide, industry-body, academic, customer
  RFP), the internal drafting cycle (intake and stance, draft
  ownership, contributor pass, CxO peer review, head sign-off,
  submission and archive), the intake register schema, and
  the three-lens discipline (proprietary interest, industry-
  common, principled position) — read and internalised.
- Chapter [01-voluntary-code-signon-decision-process](../01-voluntary-code-signon-decision-process.md)
  for the four-move stance vocabulary (respond / decline with
  rationale / defer with revisit date / watch) that the intake-
  and-stance step inherits.
- Chapter [03-public-trust-posture](../03-public-trust-posture.md)
  for the enterprise's AI-governance publishing channel where
  public responses are archived, and the head's substantive
  register that RFI responses inhabit.
- Chapter [05-difficult-external-decisions](../05-difficult-external-decisions.md)
  for the discipline applied when the response is a decline
  or when a customer RFP asks for a commitment the enterprise
  cannot honestly make.
- Exercises 01 and 02 already completed — the voluntary-code
  register and standards-body portfolio are cited in RFP
  answers and in industry-body RFI responses; the runbook
  draws on them as evidence.
- [[mod-104-regulator-engagement]] chapter 05 (regulator exam
  runbook) and chapter 06 (public-consultation submission
  flow) — the runbook's regulator-addressed-RFI category
  feeds the exam runbook, and the industry-wide RFI
  category shares process with the public-consultation flow.
- [[mod-104-regulator-engagement]] chapter 07 (engagement-
  versus-legal-opinion boundary) — the head-and-GC boundary
  applies inside the drafting cycle.
- [[mod-102-running-the-program]] chapter 04 (regulatory
  crosswalk) and chapter 06 (AI system inventory) — the
  substantive material RFI answers draw from.
- The enterprise context one-pager from exercise 01.

## Steps

1. **Inherit the enterprise context.** Confirm the exercise-01
   context one-pager is current. The runbook's routing rules
   and answer library shape follow the context.
2. **The intake register schema.** Author the schema chapter
   04 defines. One row per arrival. Columns:
   - Request identifier and source body (name, jurisdiction,
     regulator / industry-body / academic / customer, contact
     if named).
   - Arrival date and stated response window (with weekend
     and holiday-adjusted deadline).
   - Category (regulator-addressed / regulator industry-wide /
     industry-body / academic / customer RFP) and initial
     routing.
   - Intake owner and date the intake conversation was
     convened.
   - Stance decision (respond / decline with rationale /
     defer with revisit date / watch) and date.
   - Lens applied (proprietary interest / industry-common /
     principled position) — recorded on the stance memo,
     re-confirmed at head sign-off.
   - Draft owner (if responding) and named contributors.
   - CxO peer reviewers (GC, CTO, CRO, Communications,
     Government Affairs, any sector-specific CxO — CISO for
     security-adjacent, CPO / DPO for privacy-adjacent).
   - Sign-off routing (head; escalation to CEO or GC where
     the response is high-visibility per chapter 04).
   - Submission date and channel (with any docket number or
     acknowledgement reference).
   - Archive link to the response, the stance memo, and the
     contributor / reviewer record.
   - Public-visibility posture (public, semi-public through
     the requester's summary, private).
   - Cross-references — voluntary-code register row, standards-
     body portfolio row, prior-response archive entries the
     current response relies on for consistency.
   Name the storage location (the GRC-for-AI stack, alongside
   the voluntary-code and standards-body registers), the
   access control (read for CxO peers, audit-committee chair,
   external auditors under NDA; write for intake owner, head,
   level-50 architect), and the retention posture (indefinite
   for regulator responses; per the enterprise's records
   schedule for customer RFP responses, with attention to
   contract lifecycle since RFP commitments follow the
   contract).
3. **The five-category routing rules.** Author, one paragraph
   per category, the specific routing rule the intake owner
   applies on arrival. For each category, name:
   - The intake owner (typically a named delegate on the
     head's office).
   - The stance-conversation participants (who is convened
     within one week).
   - The default lens family (regulator RFIs are typically
     industry-common or principled; customer RFPs are
     typically proprietary interest).
   - The escalation trigger (which arrivals escalate to CEO,
     GC, or both).
   - The interaction with adjacent processes (regulator-
     addressed RFIs feed the exam runbook from
     [[mod-104-regulator-engagement]] chapter 05; industry-
     wide RFIs share process with the public-consultation
     flow from [[mod-104-regulator-engagement]] chapter 06).
   - The public-visibility default (regulator RFIs are
     public unless the regulator has marked otherwise;
     industry-body RFIs are semi-public through the body's
     reporting; academic RFIs are semi-public through the
     research once published; customer RFPs are private but
     the enterprise's response accretes to the answer
     library).
4. **The internal drafting cycle.** Author the six-step cycle
   chapter 04 defines. For each step:
   - **Intake and stance.** Owner (intake owner);
     deliverable (register row opened, stance memo drafted,
     four-move stance decision recorded); acceptance
     criterion (intake within one business day of arrival,
     stance conversation convened within one week);
     escalation (any arrival that misses the intake window
     surfaces to the head).
   - **Draft ownership.** Owner (single named draft owner —
     the level-50 architect or a domain lead, never the
     intake owner and never Communications); deliverable
     (working draft with contributor list); acceptance
     criterion (a single named owner; joint drafts are not
     drafts).
   - **Contributor pass.** Owner (draft owner);
     deliverable (contributions from named contributors on
     the same time-boxed schedule as the public-consultation
     cycle); acceptance criterion (late contributions do
     not enter the draft; the discipline is what keeps the
     draft moving to CxO peer review on schedule).
   - **CxO peer review.** Owner (draft owner routes);
     deliverable (near-final draft reviewed by GC, CTO,
     CRO, Communications, Government Affairs, sector-
     specific CxO); acceptance criterion (time-boxed; no-
     response reviewers are recorded as no comment; silence
     is a position, not an oversight).
   - **Head sign-off.** Owner (head; for high-visibility
     responses, escalation to CEO or GC per the
     [[mod-104-regulator-engagement]] chapter 06
     escalation matrix); deliverable (signed response);
     acceptance criterion (the head's signature on the
     substantive content; the lens is re-confirmed at
     sign-off; the response is checked against prior-
     archive entries for consistency).
   - **Submission and archive.** Owner (intake owner);
     deliverable (submitted response with acknowledgement
     captured; archive complete); acceptance criterion
     (the response is versioned, dated, cross-referenced
     to the request, and archived with the stance memo
     and contributor / reviewer record).
   For each step, name the SLA (how many business days
   from prior-step completion) and the failure escalation
   (if a step is not completed within its SLA, whom does
   the intake owner surface to).
5. **The customer-RFP answer library.** Author the standing
   answer library shape chapter 04 requires:
   - **Answer categories.** The standard AI-governance RFP
     questions the library covers — AIMS conformance
     (ISO/IEC 42001 or equivalent), NIST AI RMF
     implementation, incident-reporting practice, data-
     provenance and model-provenance documentation,
     evaluation and red-teaming practice, voluntary-code
     alignment, and sector-specific questions (FDA
     GMLP / PCCP where relevant, CFPB adverse-action
     practice, EU AI Act deployer / provider posture, and
     equivalents).
   - **Answer format.** For each category, the standing
     answer format — a short substantive paragraph with
     evidence pointer (the specific artefact in the
     enterprise's own operating discipline that
     substantiates the claim). The answer is head-approved
     substance; the sales team tailors the wrapper (the
     customer-specific opening and the customer-context
     framing) but does not modify the substance.
   - **Versioning.** Every answer is versioned and dated.
     A customer that later cites the enterprise's answer
     is citing a specific version. Answer updates are
     tracked; the version history is retained so an audit
     can trace what the enterprise committed to when.
   - **Escalation trigger.** The written trigger that
     forces sales to route to the head for a decision
     before the response goes out. Trigger cases:
     any question the answer library does not cover; any
     customer request for a commitment more aggressive
     than the standing answer (a tighter incident
     notification SLA than the enterprise's standard, an
     evaluation the enterprise does not currently run, a
     voluntary-code sign-on the enterprise has not signed
     to); any question that would require the enterprise
     to take a position inconsistent with a regulator-
     facing filing or a public position paper.
   - **Cross-reference.** Every answer that references a
     voluntary code, a standards-body role, or a
     regulator-facing filing is explicitly cross-linked
     to the register row that substantiates it.
6. **The head-and-CRO joint operating agreement.** Author the
   two-page agreement chapter 04 requires between the head
   and the Chief Revenue Officer (or Chief Commercial
   Officer). Sections:
   - **The library.** Head substance; sales delivery.
     Named ownership: head owns the substantive content;
     sales owns the customer-facing wrapper and the
     integration into the RFP response document.
   - **The escalation trigger.** The written trigger
     itself (chapter 04 defines the shape; the agreement
     names the specific cases), the routing rule (sales
     surfaces to the head via a named channel within a
     named SLA), and the response SLA (the head answers
     within a named window; if the head's answer requires
     more time than the RFP allows, the head or Government
     Affairs contacts the customer to negotiate the
     window).
   - **The archive.** Sales' RFP responses are archived
     alongside the intake register; the enterprise's
     cumulative RFP-response corpus is a governance
     artefact, not a private commercial file.
   - **The audit hook.** The head runs a periodic audit
     of a sample of RFP responses (quarterly for
     enterprises with high RFP volume; annually
     otherwise) to check for substantive drift from the
     answer library and for uncleared bespoke commitments.
     Drift or uncleared commitments surface to the head's
     review with the CRO before the next audit cycle.
   - **Ratification.** The CEO ratifies the agreement; the
     audit-committee chair sees it.
7. **The regulator-RFI standing envelope.** Author the
   standing operating envelope for the recurring regulator
   RFI sources chapter 04 names — CPPA (ADMT), EU AI Office
   (GPAI implementation), NIST (AI RMF and adjacent), US
   AISI (evaluation methodology), sector regulators (Fed,
   OCC, NAIC, FDA, EBA / ECB, MHRA, EMA, and equivalents),
   and the AISI-network national bodies (UK AISI, CAISI,
   AI Verify Foundation / IMDA, and equivalents). One block
   per body:
   - Expected channel(s) for RFI issuance.
   - Expected cadence and typical response window.
   - Default routing (which intake owner, which stance
     conversation participants).
   - Named prior responses in the archive (index only —
     the responses themselves are in the archive with
     access controls).
   - Any `<!-- needs-research: verify [specific fact]
     against [official source] -->` markers where the
     body's current organisational status or issuing
     channels are not independently verifiable.
8. **The intake-owner day-one playbook.** Author the short
   playbook a new intake owner reads on their first day.
   Cover: the register (where it lives, how to open a row),
   the routing decision (the five categories with a decision
   tree), the stance-conversation participants per category
   (with named-role references, not named individuals), the
   escalation triggers (what surfaces to the head
   immediately, what waits for the weekly review), the SLA
   ladder (intake within one business day, stance
   conversation within one week, submission within the
   response window minus a two-day margin for CxO peer
   review and head sign-off), and the failure escalation
   (whom to surface to if any step misses its SLA).
9. **The response walk-through.** Select one hypothetical
   arrival from each of the five categories — a plausible
   regulator RFI, a plausible industry-wide regulator RFI,
   a plausible industry-body RFI, a plausible academic RFI,
   and a plausible customer RFP with AI-governance content.
   Walk each arrival through the intake, stance, drafting
   cycle, and archive at condensed form (a paragraph per
   step is enough). The walk-throughs are the runbook's
   own dry-run; if any arrival exposes a routing rule the
   runbook has not authored, the runbook is under-authored.
10. **The failure-mode audit.** Author a short section — one
    paragraph per failure — naming how the runbook detects
    and recovers from each of these failure modes:
    - **The scramble arrival.** A regulator RFI arrives on
      a Friday afternoon and is discovered on Monday; the
      one-business-day intake SLA is already missed.
    - **The scope drift.** The draft owner extends the
      response to cover material outside the request; the
      response reads as marketing.
    - **The substantive contradiction.** The response
      contradicts a prior filing or a public position
      paper; the head signs off without catching the
      inconsistency.
    - **The uncleared bespoke commitment.** Sales
      commits the enterprise to a customer-specific SLA
      or evaluation without the escalation trigger being
      pulled; the commitment enters the contract.
    - **The archive gap.** A response is submitted but
      not archived; a subsequent inquiry cannot
      reconstruct what the enterprise said.

## Deliverables

- `intake-register-schema.md` — the register schema with
  columns, storage location, access control, retention.
- `routing-rules-per-category.md` — the five-category
  routing rules.
- `drafting-cycle-runbook.md` — the six-step cycle with
  owner, deliverable, acceptance criterion, and SLA per
  step.
- `answer-library-shape.md` — the customer-RFP answer
  library structure, format, versioning, and escalation
  trigger.
- `head-and-cro-joint-operating-agreement.md` — the
  two-page agreement.
- `regulator-rfi-standing-envelope.md` — the standing
  operating envelope per recurring regulator source.
- `intake-owner-day-one-playbook.md` — the short
  playbook for a new intake owner.
- `walkthroughs.md` — one walk-through per category (five
  in total).
- `failure-mode-audit.md` — the five failure-mode
  detection-and-recovery paragraphs.

## Acceptance criteria

- The intake register schema names all thirteen columns
  chapter 04 requires (or the equivalent, adapted to the
  enterprise's storage stack), with the lens field
  explicitly present so the three-lens discipline is
  captured on record.
- Every category has a specific routing rule with an
  intake owner, a stance-conversation participant list,
  a default lens, an escalation trigger, and a public-
  visibility default.
- The drafting cycle has all six steps in the order
  chapter 04 defines. Each step has a single named owner
  (not "the team"), a concrete deliverable, an
  acceptance criterion, and a numeric SLA in business
  days. The head sign-off step names the escalation to
  CEO or GC by reference to the standing escalation
  matrix.
- The answer library covers the standard categories
  chapter 04 names and any sector-specific categories
  the enterprise's context requires. Every answer has a
  version and a date; every answer that references a
  register (voluntary-code, standards-body, or
  regulatory) is cross-linked.
- The head-and-CRO joint operating agreement names the
  substance-vs-delivery split, the escalation trigger,
  the archive discipline, the audit hook, and CEO
  ratification.
- The regulator-RFI standing envelope covers all bodies
  chapter 04 names in the enterprise's jurisdictional
  footprint. Any factual claim about a body's current
  issuing channel or cadence that is not independently
  verifiable carries a `<!-- needs-research: verify
  [specific fact] against [official source] -->` marker.
- The intake-owner day-one playbook is short (one to two
  pages) and self-contained; a new intake owner should be
  able to route the next arrival correctly on day one.
- The walk-throughs cover all five categories. A walk-
  through that skips a step of the drafting cycle fails
  the criterion.
- The failure-mode audit names, for each of the five
  failure modes, at least one specific detection signal
  and one specific recovery action.
- The runbook composes with the voluntary-code register
  from exercise 01, the standards-body portfolio from
  exercise 02, the public-trust plan from exercise 03,
  and the regulator-engagement register from
  [[mod-104-regulator-engagement]]. Cross-references
  are explicit.

## Stretch goals

- Extend the register with a **rolling twelve-month
  volume dashboard** — arrivals per category per month,
  average time-to-submit against response window, stance
  distribution (respond / decline / defer / watch), and
  escalation frequency. The dashboard feeds the annual
  external-engagement briefing and surfaces trends the
  head would otherwise miss (a category becoming more
  frequent than the runbook was designed for, an
  intake owner overloaded, a specific regulator's RFI
  cadence increasing).
- Author the **cross-response consistency audit** shape
  — the periodic review that samples a set of the
  enterprise's responses across categories against a
  specific substantive topic (e.g. the enterprise's
  standing position on model-evaluation methodology,
  or on incident-reporting SLA), and checks for
  substantive drift. The audit is what chapter 04's
  "cumulative corpus" discipline turns into.
- Author the **decline-response template** for RFI
  categories where the enterprise declines to respond
  (chapter 05's decline discipline applied to RFIs) —
  the one-paragraph statement, the substantive
  rationale, and the archive entry the enterprise
  produces even for declines so the register carries
  the record.
- Draft the **customer-RFP escalation packet** the head
  hands back to sales for a specific RFP question that
  requires a bespoke commitment. The packet is what
  sales carries back to the customer to renegotiate,
  drop, or accept the standing answer — with the
  substantive rationale and, where the head is willing
  to move, the specific alternative commitment.
- Extend the head-and-CRO agreement with an
  **antitrust-adjacent-questions protocol** — the
  narrow class of customer-RFP or industry-body-RFI
  questions where the enterprise's answer touches
  price coordination or market-share signalling. GC
  reviews these before response, per the standing
  antitrust boundary. Chapter 03's peer-coordination
  discipline is analogous.

## Notes and starter guidance

The most common first-cut failure of the runbook is a
routing rule that reads as "regulator RFIs go to the
head, industry-body RFIs go to the level-50 architect,
academic RFIs go to Communications". That is not a
routing rule; that is a summary sentence. The routing
rule names the intake owner (who opens the register
row), the stance-conversation participants (who is
called into the room within one week), the default lens
(which of the three lenses the response is drafted in
absent a specific reason to shift), and the escalation
trigger (what surfaces to the head immediately). Without
those four, the intake owner has no operating
instructions on Monday morning.

The second common failure is a drafting cycle that lets
the intake owner also be the draft owner because the
intake owner "already has context". Chapter 04 is
explicit that the two roles are separate — the intake
owner runs process, the draft owner runs substance —
and collapsing them produces responses that are process-
heavy and substance-light. Force the split even where
the enterprise's headcount pressure argues against it.

On the answer library — the pull is to author the
library as long-form marketing prose the sales team can
cut and paste. Chapter 04's discipline is short
substantive paragraphs with evidence pointers, cross-
linked to registers. The library is *not* a data-room
document; it is the head's substantive commitments in
compressed form.

On the escalation trigger — the pull is to write it
loosely so sales does not surface every question. Loose
triggers mean sales freelance on borderline questions.
Chapter 04's discipline is that any commitment more
aggressive than the standing answer, or any question the
library does not cover, or any question that would
create inconsistency with a public position, surfaces to
the head. Sales' initial pushback that "this is too
much friction" is exactly the friction the enterprise
wants; the head's downstream defence of a bespoke
commitment is where the friction is worth it.

On the walk-throughs — pick arrivals that are
plausible-hard, not obvious. An academic RFI from a
university whose researcher has been critical of the
enterprise is more instructive than one from a
sympathetic researcher. A customer RFP from a public-
sector procurement with jurisdictional exposure the
enterprise has never handled is more instructive than
one from a well-known customer.

The runbook is a living artefact. Version it, date it,
review it at the annual external-engagement briefing,
update it when the standing envelope shifts materially
(a regulator changes issuing channels, a new category
of RFI emerges, a customer-RFP category becomes
frequent enough to warrant its own routing rule). A
runbook that has not been touched in a year is a
runbook the intake owner is silently improvising
against.
