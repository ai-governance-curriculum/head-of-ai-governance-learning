# exercise-03: Article 73 and US Serious-Incident Filing Drill

**Estimated effort:** 3 hours

## Objective

Produce the **parallel-filing drill artefact set** — the full stack of
decision records, evidence assemblies, routing registers, content plans,
and timelines that walk a single, specific serious incident through the
EU Article 73 filing path and every applicable US federal / state /
sector disclosure path in parallel. The drill is not a theoretical
walkthrough; it is the enterprise's proof, produced outside incident
time, that its filing discipline holds when the clock is actually
running. Every artefact in the set is one the head would produce in the
first 24 to 96 hours of a live serious incident, drafted against a
pre-selected scenario dense enough to stress-test the routing decisions,
the multi-jurisdiction timeline discipline, and the content-composition
sequence from [[03-article-73-filing-at-incident-time]] and
[[04-us-serious-incident-disclosure-map]].

The drill has to survive three stress tests. First, the General Counsel
reads the classification-meeting minutes and confirms the Article 3(49)
characterisation, the Article 73 paragraph selection, and any parallel
US legal characterisations are defensible against the reconstructed
facts — a classification record that lets the technical peers drift into
legal argument or the legal peers into technical assertion fails the
test. Second, Regulator Relations reads the multi-Member-State routing
register and confirms every affected national CA is named, the
lead-NCA rationale is explicit, and the GPAI AI Office coordination
decision (if any) is captured — a register that collapses multiple CAs
into "the EU regulator" fails the test. Third, the CFO reads the SEC
8-K Item 1.05 materiality assessment and confirms the disclosure
decision is documented at the depth an audit committee would expect —
a materiality assessment that reads as an ex-post rationalisation
rather than a contemporaneous decision fails the test.

The drill matters because filing discipline is a capability the head
cannot rehearse into being once an incident lands. The artefact set is
what the enterprise points to when the audit-committee chair asks
whether the head is ready to run a parallel EU / US serious-incident
filing sequence under time pressure. A head who cannot produce the
drill artefacts outside incident time will not produce them inside
incident time either. The drill is the pre-position.

## Prerequisites

- Chapters [[03-article-73-filing-at-incident-time]] and
  [[04-us-serious-incident-disclosure-map]] read and internalised — the
  classification meeting shape, the awareness-date evidence stack, the
  multi-Member-State routing decision, the filing-content composition
  pattern, and the US disclosure map by obligation.
- [[mod-104-regulator-engagement]] chapter 02 (the general Article 73
  regime — three timelines, seven-question filing-defence discipline,
  signature ownership, boundary with GC) and chapter 04 (regulator
  relationship management across the durable engagement sequence).
- [[mod-109-cross-enterprise-leadership]] chapter 06 (GC coordination
  — packaging discipline, when the head owns the filing signature and
  when GC owns the legal characterisation).
- [[02-cross-function-incident-coordination]] for the seven pens (the
  seven coordination surfaces the incident-time filing decision runs
  across).
- Primary sources: Regulation (EU) 2024/1689 Articles 3(49) and 73;
  Colorado AI Act (SB24-205); NAIC Model Bulletin on the Use of AI
  Systems by Insurers; 45 CFR §§ 164.400–414 (HIPAA breach
  notification); 21 CFR Part 803 (Medical Device Reporting); SEC
  Form 8-K Item 1.05. Additional statute-and-regulator references per
  the disclosure obligations the chosen scenario triggers (EEOC / DOL,
  CPPA, state Attorneys General, SR 11-7 for the model-risk-management
  overlay).
- A concrete enterprise scenario in mind — do not open the exercise
  without one. The scenario shape is the single biggest determinant of
  drill quality; a generic scenario produces a generic drill.

## Steps

1. **Scenario selection.** Pick a specific serious-incident scenario
   shape and document it as a one-page narrative. Suggested shapes,
   any of which will exercise the full parallel-filing map:
   - A Colorado-scope high-risk hiring AI where systemic bias was
     surfaced by an external academic paper — the deployer enterprise
     is US-headquartered but has users in three EU Member States, so
     the incident implicates the Colorado AI Act consumer-notification
     regime, an EEOC / DOL adjacency, a possible SEC 8-K materiality
     call, and the EU Article 73 path across three national CAs.
   - A medical-device SaMD AI whose calibration drift resulted in a
     mis-triage event, with both EU (multi-Member-State) patient
     exposure and US patient exposure — the incident implicates FDA
     MDR filing under 21 CFR Part 803, potential HHS OCR HIPAA breach
     notification if PHI exposure applies, EU MDR / IVDR overlap, and
     Article 73 filing across affected Member States.
   - A GPAI-provider incident where an upstream model exposure
     (unexpected capability elicitation, systemic evaluation failure,
     alignment-relevant behaviour) implicates deployer enterprises
     across the EU — the incident routes to the EU AI Office directly
     alongside national CA filings, cascades to downstream deployer
     notification, and implicates US-side disclosure at the deployers
     rather than at the provider.
   The narrative names the affected AI system(s), the affected
   populations by jurisdiction, the harm categories in play, and the
   reconstructed sequence from originating signal through incident-
   bridge escalation. Every subsequent artefact in the drill
   references this narrative.

2. **Classification-meeting artefact.** Author the verbatim decision
   record from the 4+1 classification meeting the head convenes per
   [[03-article-73-filing-at-incident-time]]:
   - Attendees: head (chairing), General Counsel (or the pre-named
     senior AI-litigation counsel delegate), senior AI governance
     architect at level 50, CISO's incident lead, plus DPO if
     personal data is implicated. Name every attendee by role, not
     just by function.
   - Timing: meeting called at T+X against the awareness clock, meeting
     duration, next checkpoint.
   - Article 3(49) characterisation: the harm category the event falls
     under, the evidence supporting that characterisation, the
     dissenting view (if any) captured.
   - Article 73 paragraph selection: which paragraph governs the
     timeline; where a boundary paragraph is in play, the reasoning
     for the selected paragraph and the more-onerous alternative the
     head would file under if the classification does not close in
     time.
   - Awareness date assertion: the date-time the enterprise is
     asserting as the awareness date, and a one-line reference to the
     evidence stack supporting it (see step 3).
   - Applicable timeline: the deadline the enterprise is filing
     against, in wall-clock hours.
   - Next checkpoint: when the meeting reconvenes if the
     characterisation shifts.

3. **Awareness-date evidence stack.** Assemble the four evidence
   sources named in [[03-article-73-filing-at-incident-time]],
   timestamped, in the order the enterprise received them:
   - The **originating alert or ticket** — the first signal in the
     enterprise's monitoring, the customer complaint, the peer
     notification, the media report, or (for the hiring-AI scenario)
     the external academic paper. Raw record captured, not
     paraphrased.
   - The **incident-bridge minutes** — the running notes from the
     bridge the CISO's incident lead is chairing, with every
     escalation, hand-off, and decision timestamped and attributed.
   - The **escalation record** — the sequence of who was notified
     when, up to and including the moment the head was pulled in.
   - The **classification-meeting notes** from step 2.
   Each source has a timestamp and an evidentiary provenance line
   (system of record, author, retrieval method). Where a source would
   be paraphrased in the drill for confidentiality, mark the
   paraphrase and describe what the raw record would contain.

4. **Multi-Member-State routing register.** Author the register that
   drives the EU side of the parallel filing:
   - Every Member State whose users, customers, or protected
     populations were exposed to the incident, with a one-line
     scoping note (why that Member State is in scope, which
     population, which harm signal). Geographic ambiguity resolves
     toward inclusion.
   - The national CA for each Member State (named to the specific
     authority — no "the German regulator" placeholders).
   - The lead-NCA selection and the rationale for that selection
     (Member State of EU seat, most concentrated harm, existing
     Regulator-Relations relationship depth from
     [[mod-104-regulator-engagement]] chapter 01, or a combination).
   - The GPAI AI Office coordination decision: whether the AI Office
     is on the engagement map alongside the national CAs, and if so,
     whether notification runs via the national CA, directly, or in
     parallel. Where uncertain, mark the entry with a needs-research
     marker rather than assume.
   - For each recipient, the responsible internal lead (Regulator
     Relations named contact) and the transmission mechanism
     (portal, formal letter, secure channel).

5. **US disclosure map applied to the scenario.** Walk the map from
   [[04-us-serious-incident-disclosure-map]] against the scenario and
   name every triggered obligation. For each triggered obligation:
   - The specific statute, regulation, or supervisory expectation
     (e.g. Colorado AI Act SB24-205 consumer-notification provision;
     45 CFR § 164.404 individual notification and § 164.408 HHS
     notification; 21 CFR § 803.50 manufacturer MDR; SEC Form 8-K
     Item 1.05).
   - The specific recipient (Colorado AG; HHS OCR; FDA CDRH; SEC
     via EDGAR; state AG per state; CPPA; EEOC or DOL office; NAIC
     domiciliary regulator).
   - The awareness-based timeline (e.g. HIPAA 60 days from
     discovery; SEC 8-K four business days from materiality
     determination; FDA MDR 30 days for reportable events, 5 days
     for events requiring remedial action; Colorado AI Act statutory
     timing).
   - The responsible internal lead (GC, DPO, CISO, CMO for medical
     device, CFO for SEC, HR for EEOC).
   - The sign-off routing (who clears, who signs, who transmits).
   Where an obligation is boundary — the scenario is close to the
   triggering threshold but does not clearly cross it — capture the
   analysis and the decision anyway, with the reasoning. Missing an
   obligation the scenario triggers is a drill failure; capturing a
   boundary obligation with reasoning is not.

6. **Article 73 filing content plan.** Content-only plan against the
   pre-built template referenced in
   [[03-article-73-filing-at-incident-time]] and rehearsed against
   [[mod-104-regulator-engagement]] chapter 02. Do not draft the
   filing itself; draft the section-by-section content plan the
   architect would fill in. Sections:
   - Enterprise identity and role (provider or deployer, EU seat,
     representative if applicable).
   - Affected AI system identity (AIMS inventory reference,
     deployment surface).
   - Awareness date (with the evidence-stack cross-reference from
     step 3).
   - Causal-link assertion (what the enterprise is asserting about
     the link between the AI system's behaviour and the harm, at the
     specificity the evidence supports and no further).
   - Applicable Article 73 paragraph.
   - Recipient national CA (per the routing register in step 4).
   - The **seven-question filing-defence discipline** answers from
     [[mod-104-regulator-engagement]] chapter 02 — one content-plan
     paragraph per question, naming what the filing says, what
     evidence it relies on, and what qualification (if any) it
     preserves. A content plan missing any of the seven questions
     fails the acceptance criterion.

7. **US filing content plans.** One content plan per triggered US
   obligation from step 5, each matching the specific recipient's
   expected format. The content plan names, for each obligation:
   - The recipient-specific header and identity metadata (e.g. HHS
     OCR breach report fields; SEC 8-K Item 1.05 disclosure elements
     — nature and scope of incident, material impact assessment,
     remediation status; FDA MDR fields per 21 CFR § 803.52; Colorado
     AI Act consumer-notification content elements).
   - The factual account, at the depth the recipient expects and no
     further.
   - The materiality / risk / harm characterisation the recipient
     requires (SEC materiality analysis; HHS risk-of-harm assessment
     under the four-factor breach analysis; FDA event characterisation
     — malfunction, serious injury, death).
   - The remediation posture and any commitments the enterprise is
     willing to make on the record.
   - The sign-off block per the sign-off routing named in step 5.
   Store one content plan per triggered obligation in the
   deliverables subdirectory; do not collapse multiple obligations
   into a single plan even where the recipients overlap.

8. **Parallel-filing coordination timeline.** A Gantt-style artefact
   showing every recipient in scope, the applicable awareness-based
   timeline, the internal sign-off owner, and the transmission
   confirmation checkpoint. The timeline shows:
   - Article 73 timing per paragraph (immediate, 72-hour, or the
     paragraph-specific band per the scenario's characterisation)
     against each affected national CA.
   - HIPAA 60-day individual notification and 60-day / annual HHS
     notification per breach size.
   - Colorado AI Act statutory timing per the SB24-205 provision the
     scenario triggers.
   - SEC 8-K four-business-day timing from the materiality
     determination.
   - FDA MDR 30-day (reportable) or 5-day (remedial action) timing.
   - Any state AG, EEOC / DOL, CPPA, or NAIC timing the scenario
     triggers.
   Every recipient has a distinct row; the artefact shows the
   internal sign-off dependencies as swim-lane cross-connects. A
   timeline that collapses recipients into a single "external
   regulators" lane fails the drill.

9. **Filing-decision meeting minutes.** The verbatim decision record
   from the under-60-minutes filing-decision meeting the head
   convenes per [[03-article-73-filing-at-incident-time]]. Four
   agenda items in order:
   1. Classification confirmation — GC restates the Article 3(49)
      position, the Article 73 paragraph, the awareness date, and
      the applicable timeline; the head confirms; any shift since
      the classification meeting is captured.
   2. Filing content review — the architect walks the filing content
      plans (both the Article 73 plan and the US plans) against the
      seven-question discipline and the recipient-specific
      requirements; GC and the CISO's incident lead sign off on
      their respective clearance surfaces; the head signs.
   3. Sign-off routing and transmission — Regulator Relations
      confirms the recipient list, the transmission mechanism per
      recipient, the confirmation-of-receipt tracking, and the
      filing-recipients register status.
   4. External-comms coordination — Comms restates the customer,
      press, employee, partner, and (where applicable)
      patient / affected-consumer posture that has to be aligned
      with the filing content; the head confirms alignment.
   The meeting record names attendees, timing, and every decision
   verbatim. Duration recorded — if the drill's simulated meeting
   would run past 60 minutes, that is a drill signal that upstream
   work was not closed and the head would adjourn.

10. **Follow-up interaction posture note.** A short note capturing the
    head's personal ownership of follow-up across every filing in the
    scenario. Contents:
    - A statement that the head personally owns the follow-up
      sequence — the written-information-request response, the
      follow-up meeting, the on-site inspection (if called), and the
      corrective-action plan against its named dates — across every
      recipient, EU and US.
    - A register of open filings the drill has just produced, with,
      for each: the recipient, the filing date (simulated), the next
      expected interaction, the open information requests (if
      anticipated), the open corrective-action commitments, and the
      responsible internal lead.
    - Named delegation boundaries — where the architect, GC, or
      Regulator Relations accompanies but does not substitute for
      the head, and where a deputy is pre-named for continuity if
      the head is unavailable.

## Deliverables

- `scenario-narrative.md` — the one-page scenario narrative from
  step 1.
- `classification-meeting-minutes.md` — the 4+1 classification-meeting
  verbatim decision record.
- `awareness-date-evidence-stack.md` — the four-source evidence
  assembly, timestamped.
- `multi-member-state-routing-register.md` — the EU routing register
  including lead-NCA selection and GPAI AI Office coordination
  decision.
- `us-disclosure-map-applied.md` — the US disclosure-map application
  enumerating every triggered obligation.
- `article-73-filing-content-plan.md` — the section-by-section
  content plan against the Article 73 template, including the
  seven-question filing-defence discipline answers.
- `us-filing-content-plans/plan-{obligation}.md` — one content plan
  per triggered US obligation (e.g. `plan-sec-8k.md`,
  `plan-hipaa-breach.md`, `plan-fda-mdr.md`, `plan-colorado-ai-act.md`,
  `plan-eeoc.md`, `plan-cppa.md`, `plan-state-ag-{state}.md`).
- `parallel-filing-timeline.md` — the Gantt-style parallel-filing
  coordination timeline.
- `filing-decision-meeting-minutes.md` — the under-60-minutes
  filing-decision meeting verbatim record.
- `follow-up-posture-note.md` — the head's personal follow-up
  ownership statement and open-filings register.

## Acceptance criteria

- The scenario narrative is a specific incident with named affected
  populations, named jurisdictions, and a reconstructed sequence
  from originating signal to head escalation. A generic scenario
  ("a bias event in a hiring AI") fails; a specific scenario ("a
  hiring AI deployed to 12,000 Colorado applicants and to
  applicants in DE / FR / NL, with bias surfaced by [named paper]
  on [date]") passes.
- The classification-meeting artefact names every participant by
  role and captures the Article 3(49) characterisation, the
  Article 73 paragraph selection, the awareness date, and the next
  checkpoint verbatim. A missing participant or an unresolved
  characterisation fails the criterion.
- The awareness-date evidence stack has all four evidence sources
  present, each with a timestamp and a provenance line. A missing
  source or an untimestamped source fails.
- The multi-Member-State routing register names every affected
  Member State's specific national CA, the lead-NCA rationale, and
  the GPAI AI Office coordination decision. "The EU regulator" as
  a recipient fails; a routing register that omits a Member State
  the scenario implicates fails.
- The US disclosure map application enumerates every obligation
  the scenario triggers. Missing an obligation the scenario
  clearly triggers is a fail; capturing a boundary obligation with
  documented reasoning is not.
- The Article 73 filing content plan covers every one of the seven
  questions in the filing-defence discipline. A missing question is
  a fail; a question answered with "TBD" without a needs-research
  marker is a fail.
- The parallel-filing timeline shows each recipient's timing
  distinct from the others. A single collapsed timeline across
  multiple recipients — or a timeline that uses one Article 73
  band as a proxy for all EU recipients where the scenario's
  characterisation would push different paragraphs — fails.
- The filing-decision meeting minutes cover the four named agenda
  items and are recorded at a duration under 60 minutes of agenda
  coverage. A meeting record that runs longer indicates upstream
  drift and fails.
- The follow-up posture note names the head as personally owning
  follow-up across every filing in the register. A posture that
  hands follow-up to the architect or to GC once the acute phase
  is over fails.
- Any factual claim about a specific statute article number, an
  awareness-based timeline in wall-clock terms, a regulator
  recipient's name or filing mechanism, or a specific form field
  carries a `<!-- needs-research: verify [specific fact] against
  [official source] -->` marker where the fact is not independently
  verifiable from the cited primary sources. No obligation, no
  timeline, and no recipient name is guessed.

## Stretch goals

- Extend the drill to a **GPAI-provider coordination scenario** —
  the enterprise is a deployer of an upstream GPAI model and the
  incident implicates the upstream model's behaviour. Author the
  coordination artefact set with the upstream provider: the joint
  factual account, the alignment on causal-link assertion in each
  side's filing, the escalation channel to the upstream
  provider's head-of-AI-governance counterpart, and the fallback
  where the upstream provider will not align.
- Extend to a **supplemental-filing scenario** — new information
  arrives 72 hours after the initial Article 73 filing and 48 hours
  after the SEC 8-K filing. Author the decision record the head
  runs on whether the new information triggers a supplemental
  filing, an 8-K amendment, or capture in the follow-up sequence.
  Include GC's characterisation and the head's final call, with
  reasoning.
- Extend to a **rehearsed follow-up inspection** — the lead NCA
  calls an on-site inspection following the initial filing. Author
  the inspection host-of-record artefact set: the opening-meeting
  script, the inspector-interaction posture, the document-production
  register, the closing-meeting agenda, and the head's personal
  attendance discipline.
- Author the **CEO briefing note that accompanies the audit-
  committee-chair out-of-cycle notification** — the one- to two-page
  written brief the head sends to the CEO in parallel with (not
  after) the parallel-filing sequence, covering the classification,
  the recipients and timelines in scope, the material posture
  decisions the head has taken, and the CEO-escalation points the
  head anticipates.
- Extend the drill with a **regulator-follow-up-letter dry run** —
  simulate the written information request the lead NCA sends
  within a small number of weeks of the filing, and produce the
  response artefact discipline: the architect-drafted answer, the
  GC-cleared cover letter, the head-signed transmission.

## Notes and starter guidance

The most common first-cut failure is a scenario too generic to
stress-test the disclosure map. A "bias event in a hiring AI"
scenario does not force the drill to decide whether Colorado AI Act
notification triggers, whether the enterprise's EU deployment
implicates three or five Member States, whether the SEC materiality
analysis crosses the 8-K Item 1.05 threshold, or whether the EEOC
adjacency is live. A scenario with named populations, named
jurisdictions, named triggering evidence, and a reconstructed
sequence forces those decisions. Spend the first 20 minutes on the
scenario; the drill quality depends on it more than on any other
step.

The second common failure is a filing content plan that reads as a
legal brief rather than as the seven-question discipline. The
Article 73 plan is not a memo justifying the enterprise's position;
it is a section-by-section content plan that names, for each of the
seven questions, what the filing says and what evidence it relies
on. A content plan that argues the enterprise's position at length
in every section indicates the head has let GC's advisory posture
displace the head's own filing-composition discipline. GC clears
legal; the head owns the composition. Force the seven-question
structure and refuse to let any single answer expand into a brief.

The third common failure is a parallel-filing timeline that treats
every recipient as identical. Article 73 timelines and paragraph
selection, HIPAA 60-day timing, SEC 8-K four-business-day timing,
FDA MDR 30 / 5 day timing, Colorado AI Act statutory timing, and
state AG / CPPA timing all diverge — some run from awareness,
some from discovery, some from materiality determination, some
from the incident event itself. A timeline that shows every
recipient hitting the same wall-clock deadline is a timeline that
has not been engaged with the sources. Draft the timeline against
the specific triggering event per obligation, mark the divergences,
and let the internal sign-off swim lanes carry the coordination
load rather than the timeline pretending to be simple.

The fourth common failure is a classification meeting that widens
past 4+1 and drifts into a briefing. The classification meeting is
the head, GC, the senior AI governance architect, the CISO's
incident lead, and the DPO if personal data is in scope — no
more. Comms, Government Affairs, Regulator Relations, the CRO,
and the board interface come in at the filing-decision meeting,
not at classification. A drill that stages a 14-person
classification meeting has misread the shape from
[[03-article-73-filing-at-incident-time]] and produces a
classification record that does not close. Keep the meeting
small, named, and decision-forcing.
