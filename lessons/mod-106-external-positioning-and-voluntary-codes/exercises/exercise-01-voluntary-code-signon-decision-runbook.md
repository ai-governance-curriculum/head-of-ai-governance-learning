# exercise-01: Voluntary-Code Sign-on Decision Runbook

**Estimated effort:** 3 hours

## Objective

Author the enterprise **voluntary-code sign-on runbook** — the
executable process the head runs every time a code arrives on
the portfolio, plus the standing **voluntary-code register**
covering the current portfolio as of the research window. The
deliverable is the document the head hands to a successor on
day one, the document the audit-committee chair reviews at the
annual external-engagement briefing, and the document that
carries the seven-step decision process from chapter 01 into
an operating discipline any CxO peer can follow.

The runbook has to survive three stress tests. First, a
regulator asks "did the enterprise consider signing X" three
years after the decision — the register has to answer, with
rationale, without the head having to reconstruct memory.
Second, an incoming head reads the runbook and can execute the
seven-step decision on a new code without renegotiating the
process with the CxO peers. Third, a customer's procurement
lead asks "which voluntary codes has the enterprise signed on
to, and where can we read the enterprise's commitment" — the
public summary produced from the register has to answer, and
the register underneath has to back the summary.

The runbook is not a study of chapter 01. It is the artefact
that turns chapter 01 into repeatable operating discipline.

## Prerequisites

- Chapter [01-voluntary-code-signon-decision-process](../01-voluntary-code-signon-decision-process.md)
  — the seven-step decision process, the four-move stance
  discipline, the standing portfolio, and the CEO / GC / CRO /
  CFO sign-off flow — read and internalised.
- Chapter [03-public-trust-posture](../03-public-trust-posture.md)
  for the public-facing summary the register feeds. Chapter 05
  (difficult decisions) for the withdrawal-condition-set
  discipline that every signed code carries.
- [[mod-101-role-scope-and-leadership-shape]] chapter 06 (CxO
  adjacency) — the peer relationships the sign-off flow
  operates against, and the standing joint operating
  agreements the sign-off routing rides.
- [[mod-102-running-the-program]] chapters 03 (risk register),
  04 (regulatory crosswalk), 06 (AI system inventory), and 07
  (supply-chain evidence) — the operating artefacts the
  attachment analysis (step 1) presses against.
- [[mod-103-board-and-audit-committee-reporting]] chapter 03
  (risk appetite) — the appetite framework the CRO checks the
  sign-on against (step 3).
- [[mod-104-regulator-engagement]] chapter 07 (engagement-
  versus-legal-opinion boundary) — the controlling boundary
  discipline for the GC step (step 4) and for the
  public-positioning read (step 5).
- A concrete enterprise in mind — sector (banking, insurance,
  health / medical device, pharma, public sector, frontier lab,
  tech platform, industrial), jurisdictional footprint, AI
  system portfolio scope. The enterprise's exposure to each
  standing code depends on this context; make it explicit.

## Steps

1. **Enterprise context one-pager.** Author the half-page
   context the runbook operates against: sector, jurisdictional
   footprint (which of EU, US federal, US states, Canada, UK,
   APAC, other), AI system portfolio scope (Annex III
   categories where relevant, GPAI provider or deployer scope,
   frontier-model scope), current voluntary-code posture at a
   high level (any prior sign-ons), and the operating owner
   assumption (level-50 senior AI governance architect at
   minimum; document the assumption if the enterprise has a
   different structure). Every subsequent artefact refers back
   to this one-pager.
2. **Portfolio register schema.** Author the register schema
   the runbook maintains, using the columns from chapter 01:
   code identifier and canonical citation; current state
   (signed / declined-with-rationale / deferred-with-revisit-
   date / watched); state-entry date and rationale;
   commitment scope if signed; operating owner if signed;
   revisit date if deferred; audit-committee visibility;
   withdrawal condition set if signed; public-facing artefact
   link. Name the storage location — the register lives in the
   GRC-for-AI stack (not on the head's laptop), with access
   control (read for CxO peers, audit-committee chair, and
   external auditors under NDA; write for head and level-50
   architect). Name the retention posture (retain per the
   enterprise's records-management schedule, with public-
   commitment history retained for at least the enterprise's
   audit-cycle horizon plus the audit committee's memory
   horizon).
3. **Populate the register — the standing portfolio.** For each
   of the standing bodies chapter 01 names — EU AI Office GPAI
   Code of Practice, G7 Hiroshima Process Code of Conduct,
   White House Voluntary AI Commitments, Frontier Model Forum,
   Partnership on AI, MLCommons AI Safety Working Group, US
   AISI Consortium (AISIC) — populate the register with the
   enterprise's current state and one-paragraph rationale for
   the state. Where the enterprise's rationale references a
   current-status uncertainty about the body itself (e.g. the
   White House Voluntary Commitments post EO 14179, AISIC's
   current organisational status), mark with
   `<!-- needs-research: verify [specific fact] against
   [official source] -->` rather than guessing. Where the
   enterprise's rationale references a peer-signatory pattern,
   note the pattern as a program-management input, not as a
   floor.
4. **The seven-step decision runbook.** Author the runbook the
   head follows for a new code arriving on the portfolio.
   For each step:
   - **Step 1 — attachment analysis.** Owner (level-50
     architect); deliverable (attachment table with row per
     code commitment and columns for attachment surface,
     current-state readiness, and gap); acceptance criterion
     (every code commitment has a specific attachment; no row
     reads "applies broadly" or "TBD"); cross-reference
     (the level-50 architect's crosswalk in
     [[mod-102-running-the-program]] chapter 04).
   - **Step 2 — cost estimate.** Owner (CFO office);
     deliverable (a number — headcount, dollars, calendar
     weeks — with a confidence band, plus opportunity cost and
     risk-adjusted misfire cost); acceptance criterion (the
     estimate is a number, not a phrase; the confidence band
     is not the answer).
   - **Step 3 — appetite check.** Owner (CRO); deliverable
     (a signed determination that the sign-on sits within
     appetite, or, if outside, the exception routing per
     [[mod-103-board-and-audit-committee-reporting]] chapter
     03); acceptance criterion (both directions checked —
     signing outside appetite *and* not signing outside
     appetite — with the CRO's explicit call).
   - **Step 4 — legal exposure read.** Owner (GC); deliverable
     (a legal-exposure characterisation covering enforceable-
     commitment and ancillary-exposure questions); acceptance
     criterion (GC does not recommend sign / don't sign — GC
     characterises exposure and the head weighs it, per
     [[mod-104-regulator-engagement]] chapter 07).
   - **Step 5 — public-positioning read.** Owner
     (Communications and Government Affairs jointly);
     deliverable (a public-positioning brief covering the
     political context, the peer-signatory pattern, the
     narrative implications of signing vs declining, and the
     messaging that would need to accompany the decision);
     acceptance criterion (the brief is Communications-
     substantive, not Communications-endorsement — the head
     decides, the brief informs).
   - **Step 6 — head's one-page recommendation.** Owner
     (head); deliverable (a one-page recommendation with
     stance, commitment scope, operating-owner assignment,
     condition set, and exit path); acceptance criterion
     (genuinely one page; if longer, the head has not yet
     compressed the decision enough).
   - **Step 7 — sign-off routing.** Owner (head, convening
     the sign-off room of CEO, GC, CRO, CFO, and, for material
     codes, the audit-committee chair as ratifier);
     deliverable (signed recommendation with all named CxO
     accountabilities affirmed); acceptance criterion (no
     silent CxO peer; disagreement convened and resolved
     before sign-on, not after).
   For each step, name the SLA — how many business days the
   step is expected to take from prior-step completion — so
   that the runbook's end-to-end wall-clock is predictable and
   the head can commit to an external-facing decision date.
5. **The four-move stance vocabulary.** Author the one-page
   vocabulary card the runbook uses — sign, decline with
   rationale, defer with revisit date, watch — with the
   specific definition of each, the register field that carries
   it, and the audit-committee visibility rule per stance
   (signed and material codes appear in the annual external-
   engagement briefing; declined codes appear if the decline
   is externally questioned; deferred codes appear on revisit;
   watched codes appear as an aggregate count). The vocabulary
   is the discipline the CxO peers agree to use in every
   sign-on conversation.
6. **Coordination interfaces.** Author the four short
   coordination contracts the runbook depends on:
   - **With Government Affairs.** How the runbook coordinates
     with the enterprise's Government Affairs strategy — GA
     owns industry-body strategy at large; the head owns
     AI-governance-substantive sign-on decisions. Who calls
     the joint session when a code sits at the intersection.
   - **With Communications.** How the runbook coordinates
     with the CCO's own messaging — the public-facing
     artefact for each stance (chapter 03 detail) is CCO-
     delivered on head substance. Who owns the media
     preparation if the stance attracts inbound press.
   - **With Sales.** How the runbook interacts with sales
     commitments in customer RFPs (chapter 04) — the register
     is the authoritative source for what the enterprise has
     signed, and sales' answer library draws from the register
     rather than from prior-sales-response memory.
   - **With the audit committee.** The visibility cadence —
     annual external-engagement briefing at minimum, on-
     material-change otherwise, on-material-sign-on ratified
     by the audit-committee chair before the enterprise goes
     public.
7. **The sign-on decision walk-through.** Select one candidate
   from the standing portfolio the enterprise is not currently
   signed to but could plausibly sign (the enterprise's own
   context makes the choice). Walk the seven-step runbook
   against the candidate, producing each step's deliverable in
   condensed form (a paragraph or table per step is enough for
   the exercise, but the shape has to be right). The
   walk-through is the head's own dry-run — if the runbook
   cannot be executed against a real candidate, the runbook is
   under-authored.
8. **The failure-mode audit.** Author a short section —
   one paragraph per failure — naming how the runbook detects
   and recovers from each of these failure modes:
   - A CxO peer signs off in silence (i.e. does not affirm the
     specific accountability the sign-off carries).
   - The register's public-facing summary drifts from the
     underlying register content (a stance changes internally
     but the summary is not updated).
   - A signed code's operating-owner assignment goes stale
     (the named owner leaves the enterprise; the code's
     obligations continue).
   - A decline decision is never revisited (the monitoring
     commitment lapses; the code's context changes and the
     head does not notice).
   - A sales team commits the enterprise to a bespoke AI-
     governance obligation in a customer RFP that
     contradicts a voluntary-code commitment on the register.

## Deliverables

- `enterprise-context.md` — the half-page context one-pager.
- `register-schema.md` — the register schema with columns,
  storage location, access control, retention.
- `register-populated.md` — the register populated with the
  standing portfolio (seven bodies), current state, one-
  paragraph rationale, needs-research markers where required.
- `runbook-seven-steps.md` — the seven-step decision runbook
  with owner, deliverable, acceptance criterion, and SLA per
  step.
- `stance-vocabulary.md` — the four-move stance vocabulary
  card.
- `coordination-contracts.md` — the four coordination
  contracts (Government Affairs, Communications, Sales, audit
  committee).
- `walkthrough.md` — the seven-step walk-through against one
  selected candidate code, with each step's condensed
  deliverable.
- `failure-mode-audit.md` — the five failure-mode
  detection-and-recovery paragraphs.

## Acceptance criteria

- Every row of the populated register has a specific state
  (sign / decline / defer / watch), a state-entry date, and a
  one-paragraph rationale. No row reads "under review" or
  "TBD".
- Any factual claim about a body's current status (e.g. the
  current publication cadence of the GPAI Code of Practice,
  the current organisational status of AISIC, the current
  membership roster of the Frontier Model Forum) carries a
  `<!-- needs-research: verify [specific fact] against
  [official source] -->` marker where the fact is not
  independently verifiable. No status is guessed.
- Every runbook step has a named single owner (not "the
  team" or "the sign-off room" as a diffuse group), a
  concrete deliverable (not "review" or "consideration"), a
  specific acceptance criterion, and a numeric SLA in business
  days.
- The four-move stance vocabulary is applied consistently in
  the populated register. A code that appears with a fifth
  state (e.g. "under review") flags a discipline break.
- The walk-through against the selected candidate produces
  each step's deliverable in condensed form. A walk-through
  that skips a step (typically step 2 or step 5, which are
  cross-functional and easier to hand-wave) fails the
  criterion — the discipline exists to force every step.
- The head's one-page recommendation in the walk-through is
  genuinely one page. Longer recommendations are recorded as
  the head having failed the discipline; the exercise then
  requires the head to compress and re-issue.
- The failure-mode audit names, for each of the five failure
  modes, at least one specific detection signal and one
  specific recovery action.
- The register schema explicitly names withdrawal-condition-
  set as a field on signed codes. A signed code without a
  withdrawal condition set fails the criterion — chapter 05's
  withdrawal discipline depends on the field.
- The public-facing summary — a subset of the register that
  the enterprise publishes on its AI-governance channel — is
  named, and the discipline for keeping the summary in sync
  with the underlying register (typically an update trigger on
  every state change) is written down.

## Stretch goals

- Extend the register with a **five-year forward look** —
  which codes the head expects to enter the portfolio over the
  next five years (e.g. successor codes to the GPAI Code once
  the AI Act is fully applying, new sector-specific voluntary
  codes emerging from NAIC AI work, new AISI-network codes
  that may be published), each with the horizon-scanning
  source (per [[mod-105-regulatory-change-management]]
  chapter 01) and the expected first-decision date. The
  forward look feeds the annual external-engagement briefing
  as forward-looking substance.
- Author the **audit-committee briefing pack** for the annual
  external-engagement briefing, drawing directly from the
  populated register. The pack is a two-to-three-page summary
  that a committee director can read in ten minutes and act
  on: signed codes (with operating-owner and next-cycle key
  activity), declined codes (with rationale), material
  deferrals (with revisit date), and the forward-look
  candidates. Use the pack shape convention from
  [[mod-103-board-and-audit-committee-reporting]] chapter 01.
- Draft the **sign-on decision debrief template** — the
  short after-action review the head runs after each sign-on
  decision (whether the decision was to sign, decline, or
  defer). The debrief captures what the runbook produced,
  what was easy, what was hard, what the CxO peers
  contributed, and what would improve the next decision.
  Debriefs feed the annual runbook review.
- Extend the coordination contracts with the **head-and-CFO
  agreement on the sign-on cost line** — where in the annual
  AI-governance budget ([[mod-113-budget-vendor-p-and-l-and-
  investment-case]]) voluntary-code costs appear, how they
  are classified (program cost, compliance cost, external-
  engagement cost), how variance is reported. Voluntary-code
  costs that are unbudgeted are voluntary-code costs the CFO
  will push back on at year-end.
- Draft the **decline-decision defence packet** for one code
  the enterprise declined. The packet is what the head hands
  to Communications if a journalist asks "why didn't the
  enterprise sign X" — the one-paragraph statement, the
  underlying rationale, the enterprise's continued engagement
  on the underlying subject matter, and the anticipated
  follow-up questions with prepared answers. Chapter 05's
  decline discipline is the shape.

## Notes and starter guidance

The most common first-cut failure of the runbook is a
register that reads as a set of narrative paragraphs rather
than a structured table with disciplined fields. The narrative
form flatters the head (the head has an opinion about every
code) but it does not survive audit. A regulator or a
certification body who asks "what is your voluntary-code
portfolio" wants to see the table — one row per code, one
state per row, one operating owner per signed code. Force the
register into the table form even if it feels
under-descriptive; add explanatory paragraphs alongside if
needed, but the table is the artefact.

The second common failure is the seven-step runbook that
skips step 5 (public-positioning read) because the head
believes the enterprise's decision on this code is not
"political". Every sign-on decision on a voluntary code is
political in the specific sense chapter 01 uses — it will be
read by external audiences, and the head who has not asked
"how will this be read" has not done the work. Force the step
even when the read is "no notable positioning implications";
that itself is a positioning read.

On the sign-off routing (step 7) — the temptation is to
convene the sign-off as a serial process (CFO reviews, then
CRO reviews, then GC reviews, then CEO signs). Serial routing
takes longer and produces a decision no CxO has jointly owned.
Chapter 01 is explicit that the sign-off is a room — the CxOs
either meet or read a shared document simultaneously — and
the head's runbook step 7 should specify the joint format,
not serial forwarding.

On the walk-through — pick a candidate the head has real
opinions about, not the easiest one. A walk-through against a
code the enterprise obviously will not sign teaches nothing;
a walk-through against a code the head is uncertain about
teaches everything. The exercise is calibration; use it.

On the register storage — resist the pull to put the register
in a slide deck or a document the head owns personally. The
register is a governance artefact in the same class as the
regulatory-change register and the risk register; it lives
where those live (the GRC-for-AI stack), with the same
integrity and access controls. A register that lives on the
head's laptop is a register that fails audit when the head is
on holiday.

The runbook is a living artefact. Version it, date it, review
it at the annual external-engagement briefing, update it when
the standing portfolio shifts materially (a new body emerges,
a code the enterprise is signed to undergoes material
revision, a peer's high-profile sign-on or withdrawal changes
the political context). A runbook that has not been touched
in two years is a runbook that no longer reflects the
discipline it claims to describe.
