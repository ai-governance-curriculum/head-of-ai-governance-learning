# exercise-02: Cross-Function Incident Coordination Runbook

**Estimated effort:** 3 hours

## Objective

Author the **cross-function incident coordination runbook** — the
single artefact the head of AI governance invokes on the bridge
without renegotiation under time pressure, operationalising the
"one bridge, multiple pens" discipline and the seven coordination
surfaces from
[[02-cross-function-incident-coordination]]. The runbook is not a
narrative document; it is a set of composed specifications
(pen-ownership register, seven surface contracts, tabletop
scenario, tabletop walkthrough, board-notification cadence,
private bridge-log template, failure-mode audit, distribution and
refresh discipline) that names owners, formats, cadences, and
escalation ladders for every coordination surface the incident
touches. Each surface contract composes into a parent CxO
interface document authored in
[[mod-109-cross-enterprise-leadership]],
[[mod-104-regulator-engagement]], or
[[mod-103-board-and-audit-committee-reporting]]; the runbook does
not renegotiate those interfaces at incident time.

The runbook has to survive three stress tests. First, the CCO's
incident-communications lead reads the Communications surface
contract without a briefing and can act on it — a contract that
requires the head to walk the CCO's lead through the approval
chain, the holding-statement convention, or the AI-substantive
review gate fails the test. Second, the GC's AI-legal lead reads
the incident-time packaging template embedded in the Legal
contract and confirms it is usable under Article 73 two-day time
pressure without further specification — a template that is a
prose aspiration rather than a fielded specification fails.
Third, the audit-committee chair reads the board-notification
cadence and can predict what a within-the-hour briefing looks
like, what a within-one-business-day briefing looks like, and
what the formal next-sitting briefing carries — a cadence that
reads as an aspiration rather than executable timing with named
owners fails.

The runbook matters because it is what the head invokes without
renegotiation under time pressure. Every minute the head spends
on the bridge inventing coordination on the fly is a minute the
incident's containment window closes on; every surface that has
to be re-scoped mid-incident is a surface where the parallel
bridge, the surprised CxO, and the unreturned regulator call
gestate. The runbook is the discipline that turns peace-time
interface documents into an incident-time operational surface.

## Prerequisites

- Chapter [[02-cross-function-incident-coordination]] — the "one
  bridge, multiple pens" discipline, the seven pens, the seven
  coordination surfaces, and the three coordination-collapse
  patterns — read and internalised.
- Chapter [[01-incident-command-shape-at-leadership-scope]] — the
  parent incident-command shape this runbook plugs into.
- The parent CxO interface documents authored in
  [[mod-109-cross-enterprise-leadership]] chapters 01 (CISO), 05
  (CCO), and 06 (GC) — the incident-time contracts compose into
  these; they do not renegotiate them.
- [[mod-104-regulator-engagement]] chapter 04 (regulator
  relationship management) and chapter 07 (engagement-versus-
  legal-opinion boundary) — the parent regulator-relations
  interface and the substantive-answer boundary at incident time.
- [[mod-103-board-and-audit-committee-reporting]] cluster 3
  (incident and near-miss reporting) — the parent board interface
  the notification cadence composes into.
- [[mod-101-role-scope-and-leadership-shape]] chapter 06 (CxO
  adjacency map) — the ratification document for all seven
  contracts.
- A concrete enterprise scenario in mind: sector, deployment
  footprint (EU Member State presence, US state presence, sector-
  specific regulatory context), CxO composition (whether the
  enterprise has a distinct Regulator Relations function or one
  embedded under GC; whether Government Affairs has a Brussels /
  Washington DC presence or is Member-State-centric; whether the
  Chief Compliance Officer is distinct from the Chief
  Communications Officer), and the current incident-bridge
  convention the CISO runs.

## Steps

1. **Enterprise context one-pager.** Author the half-page context
   the runbook operates against: sector; deployment footprint (EU
   Member States where the AI systems are placed on the market or
   put into service, US states where covered systems operate,
   sector regulator surface); CxO composition (which of CISO, CCO,
   GC, Regulator Relations, Government Affairs, CPO / DPO, CRO,
   CHRO, Chief Compliance Officer exist as distinct roles versus
   embedded); current incident-bridge convention (CISO's call
   number, page tree, standing observers, severity taxonomy).
   Every subsequent artefact references this one-pager.

2. **Pen-ownership register.** Author the machine-parseable table
   of the seven pens from chapter 02 (DFIR timeline, AI-
   substantive account of events, regulator-facing filing, public-
   facing statement, board briefing, customer / deployer
   notification, internal all-hands note). For each pen: named
   owner (specific role, not "the head" or "Communications"), named
   format (specific artefact template with location or reference),
   named review chain (each reviewer with the scope of their
   review — substantive, exposure, delivery). The table is
   machine-parseable so the runbook can be rendered into the
   incident-management system's runbook module; a prose paragraph
   per pen fails the criterion.

3. **Coordination-surface contract set.** Author the seven
   contracts — one per surface from chapter 02: SOC + DFIR,
   Communications, Legal, Regulator Relations, Government Affairs,
   Board, Adjacent CxOs. Each contract has four elements at
   minimum: **owner** on each side (named role at incident time —
   the CISO's SOC lead, the CCO's incident-communications lead,
   the GC's AI-legal lead, the Regulator Relations named contact,
   the Government Affairs political-context lead, the CEO for the
   board interaction, the specific CxO for each adjacent surface);
   **format** (the specific artefact template each surface
   produces); **cadence** (the timing convention on each surface,
   including bridge-refresh frequency, external-posture-refresh
   frequency, board-briefing frequency); **escalation ladder**
   (where the interface breaks, how the head and the peer
   escalate). Each contract explicitly references its parent
   interface document from
   [[mod-109-cross-enterprise-leadership]],
   [[mod-104-regulator-engagement]], or
   [[mod-103-board-and-audit-committee-reporting]] — the incident-
   time contract composes with the parent; it does not re-
   negotiate it.

4. **Tabletop scenario.** Author the specific incident narrative
   the runbook is stress-tested against: a prompt-injection-
   triggered downstream harm event affecting users across three
   EU Member States and a US employment context, with a GPAI
   upstream provider dimension. The narrative is one to two pages
   and names: the affected AI system (referenced against the AIMS
   inventory pattern from [[mod-102-running-the-program]] chapter
   06), the detection signal, the initial severity assessment, the
   Member-State distribution of affected users, the US employment-
   context dimension (which employer, which employment decision
   type), the GPAI upstream provider's identity or class, and the
   two-hour, twelve-hour, and forty-eight-hour incident-clock
   markers. The same scenario is reused in the exercise 03 filing
   drill; author it with enough specificity that both exercises
   can be run against it without further scoping.

5. **Tabletop walkthrough.** Run the runbook against the scenario
   end to end in narrative form. Note, at each incident-clock
   marker, which surface contract fires, which artefact lands on
   which pen, and where the coordination surfaces hand off to each
   other (DFIR timeline receives the head's AI-substantive
   annotation at hour one; Communications drafts the holding
   statement at hour three with the head's substantive review;
   Legal is engaged on the Article 73 filing-decision question at
   hour six; Regulator Relations makes the pre-filing introductory
   call at hour eighteen; the board is briefed at the twenty-four-
   hour mark; and so on). The walkthrough exposes gaps in the
   contracts — where a handoff has no named owner, where two
   contracts collide on the same pen, where a cadence assumes a
   parallel workstream that has not been authored.

6. **Board notification cadence artefact.** Author the executable
   timing artefact for serious incidents, per chapter 02: within
   the hour of serious-incident classification (audit-committee
   chair and risk-committee chair notified out-of-cycle); within
   one business day (full board); formal briefing at the next
   scheduled sitting; regular status updates until closure. For
   each moment name the responsible drafter (typically the head
   for the briefing note), the deliverer (typically the CEO or
   board chair), and the template (the out-of-cycle briefing pack
   template, the full-board notification template, the formal-
   briefing pack template, the standing status-update template).
   Reference sector-specific legal overlays where relevant
   (SR 11-7 for US banks, Form 8-K Item 1.05 for US public
   companies, NAIC AI Model Bulletin for insurers) with `<!--
   needs-research -->` markers where the specific obligation is
   not independently verifiable.

7. **Private bridge-log template.** Author the head's own
   private-log template used during the bridge: decision-made
   (with timestamp, the head's position, the reasoning in one or
   two sentences); AI-substantive-answer-given (with the question
   asked, the head's answer, the confidence level); coordination-
   surface-invoked (with the surface, the specific artefact
   produced, the timestamp). The template is not the DFIR record
   and does not duplicate it; it is the head's own artefact,
   consulted post-incident during the after-action review per
   [[05-post-incident-learning-cycle-sponsorship]] to calibrate
   the head's bridge conduct against outcomes.

8. **Failure-mode audit.** Author one paragraph per failure mode
   naming the detection signal and the recovery action for each of
   the three coordination-collapse patterns from chapter 02: the
   **parallel bridge** (a technical AI call running alongside the
   CISO's operational bridge, with decisions diverging); the
   **surprised CxO** (a CxO whose function is in the incident's
   blast radius learning from a press briefing or the audit-
   committee pack rather than from the head); the **unreturned
   regulator call** (a national competent authority reaching out
   for informal context after the Article 73 filing and not being
   returned inside the window that preserves the standing
   relationship). Each paragraph names at least one specific
   detection signal (an operational indicator the head or the
   head's function will see) and one specific recovery action (a
   named intervention with a named owner).

9. **Distribution list.** Author the distribution list for the
   runbook — who receives the current version, on what cadence,
   and in what format. Include, at minimum: the CISO's SOC lead
   and DFIR lead; the CCO's incident-communications lead; the GC's
   AI-legal lead; the Regulator Relations named contact for each
   material NCA; the Government Affairs political-context lead;
   the CEO's chief of staff; the audit-committee secretariat; the
   CAE; each adjacent CxO on the standing incident-notification
   list. Name the storage location that makes the runbook
   available when systems are down — the runbook lives in the
   incident-management platform, in a printed copy at each named
   principal's location, in an offline mirror on a device the head
   carries. A runbook only accessible on the enterprise SSO fails
   the offline-availability discipline.

10. **Version-and-refresh discipline.** Author the version-and-
    refresh section: the runbook is refreshed annually at the
    joint CISO-and-head interface review from
    [[mod-109-cross-enterprise-leadership]] chapter 01, and after
    every serious incident that stress-tests it (drawn from the
    after-action review per
    [[05-post-incident-learning-cycle-sponsorship]]). Name the
    change-history discipline — every version carries a date,
    a change-log entry naming what changed and why, a named author
    for the change, and a named review-and-approval trail. The
    prior version is retained; the runbook is not overwritten in
    place.

## Deliverables

- `enterprise-context.md` — the half-page context one-pager.
- `pen-ownership-register.md` — the machine-parseable seven-pen
  table with owner, format, review chain per pen.
- `contracts/contract-soc-dfir.md` — the SOC + DFIR surface
  contract, composing into
  [[mod-109-cross-enterprise-leadership]] chapter 01 Surface 4.
- `contracts/contract-communications.md` — the Communications
  surface contract, composing into
  [[mod-109-cross-enterprise-leadership]] chapter 05.
- `contracts/contract-legal.md` — the Legal surface contract, with
  the incident-time packaging template, composing into
  [[mod-109-cross-enterprise-leadership]] chapter 06 and
  [[mod-104-regulator-engagement]] chapter 07.
- `contracts/contract-regulator-relations.md` — the Regulator
  Relations surface contract, composing into
  [[mod-104-regulator-engagement]] chapter 04.
- `contracts/contract-government-affairs.md` — the Government
  Affairs surface contract, composing into
  [[mod-109-cross-enterprise-leadership]] chapter 08.
- `contracts/contract-board.md` — the Board surface contract,
  composing into [[mod-103-board-and-audit-committee-reporting]]
  cluster 3.
- `contracts/contract-adjacent-cxos.md` — the CxO peer surface
  contract, composing into
  [[mod-101-role-scope-and-leadership-shape]] chapter 06 and the
  relevant chapters of [[mod-109-cross-enterprise-leadership]].
- `tabletop-scenario.md` — the one-to-two-page prompt-injection
  scenario spanning three EU Member States, a US employment
  context, and a GPAI upstream provider.
- `tabletop-walkthrough.md` — the runbook-against-scenario
  walkthrough.
- `board-notification-cadence.md` — the executable timing artefact
  with drafter, deliverer, and template per moment.
- `private-bridge-log-template.md` — the head's private log
  template.
- `failure-mode-audit.md` — the detection-and-recovery paragraph
  per coordination-collapse pattern.
- `distribution-and-refresh.md` — the distribution list, the
  offline-availability discipline, the version-and-refresh
  section.

## Acceptance criteria

- The pen-ownership register has all seven pens (DFIR timeline,
  AI-substantive account, regulator filing, public statement,
  board briefing, customer / deployer notification, internal all-
  hands note); each pen names a specific owner (role, not
  function), a specific format (template with reference), and a
  specific review chain (each reviewer with review scope). A pen
  with an unnamed owner or a prose format description fails the
  criterion.
- Each of the seven surface contracts has all four elements
  (owner on each side, format, cadence, escalation ladder) and
  explicitly references its parent interface document from
  [[mod-109-cross-enterprise-leadership]],
  [[mod-104-regulator-engagement]], or
  [[mod-103-board-and-audit-committee-reporting]]. A contract
  that duplicates the parent interface document's boundaries
  rather than composing with them fails the criterion.
- The tabletop scenario is a specific narrative (named AI system,
  named Member States, named US employment context, named GPAI
  upstream provider dimension, named incident-clock markers), not
  a placeholder. A generic "an incident occurs affecting users"
  scenario fails the criterion.
- The tabletop walkthrough shows the runbook end to end without
  gaps — every incident-clock marker is covered, every handoff
  between surfaces is named, every artefact lands on a named pen.
  A walkthrough that skips a coordination surface or leaves an
  artefact unowned fails the criterion.
- The board-notification cadence artefact names the drafter and
  the deliverer for each of the four moments (within-the-hour,
  within-one-business-day, formal-next-sitting, regular-status-
  until-closure) and names the template for each. A cadence
  expressed as an aspiration ("the audit-committee chair should
  be notified promptly") fails the criterion.
- The failure-mode audit names, for each of the three
  coordination-collapse patterns (parallel bridge, surprised CxO,
  unreturned regulator call), at least one specific detection
  signal and one specific recovery action with a named owner.
- The distribution list includes the offline-availability
  discipline — the runbook is available when the enterprise SSO
  or incident-management platform is unavailable. A distribution
  list that only names the online location fails the criterion.
- Any factual claim about a specific NCA's introductory-call
  expectation, a specific sector regulator's incident-
  notification obligation, a specific Article 73 sub-clause, or a
  specific enterprise's coordination convention carries a `<!--
  needs-research: verify [specific fact] against [official source]
  -->` marker where the fact is not independently verifiable from
  primary sources. No practice is guessed.

## Stretch goals

- Extend the deliverable with a **rehearsed CCO drill**: a
  specific reporter-interview scenario (a named trade-press
  reporter with a specific question set about the AI-substantive
  account, an inbound from a broad-audience outlet with a
  specific narrative angle) that the CCO handles as the delivery
  spokesperson with the head as substantive brief-holder. The
  drill produces the head's brief-holder script and the CCO's
  spokesperson notes.
- Extend the deliverable with a **rehearsed GC packaging drill**
  under Article 73 two-day pressure per
  [[03-article-73-filing-at-incident-time]]: the head packages the
  regulatory-interpretation ask into the one-page incident-time
  template; the GC's AI-legal lead delivers the opinion inside a
  four-hour window; the head incorporates the opinion into the
  filing sign-off. The drill produces the packaging template
  worked through end-to-end and any protocol changes the drill
  surfaces.
- Extend the tabletop scenario with the **GPAI upstream provider
  coordination dimension**: the head has to coordinate with a
  counterpart at the upstream provider (their head of AI
  governance or equivalent) on the AI-substantive account, the
  shared-with-both filing content, and the joint remediation
  posture. Author the counterpart coordination contract as an
  eighth surface contract.
- Extend the failure-mode audit with a **live-incident narrative
  per failure mode**: for each of the parallel bridge, the
  surprised CxO, and the unreturned regulator call, a specific
  narrative in which the failure surfaces during the tabletop
  scenario, the runbook's detection signal fires, and the
  recovery action restores the coordination. The narratives are
  rehearsal artefacts for the head's function.
- Author the **joint annual audit-committee appearance briefing**
  (head + CISO + CCO + GC) that reads the runbook to the
  committee: the artefact each of the four principals brings, the
  seating pattern, the question the audit-committee chair is
  expected to open with, and the runbook sections each principal
  is prepared to answer against. The briefing composes with
  [[mod-103-board-and-audit-committee-reporting]] cluster 3.

## Notes and starter guidance

The most common first-cut failure on this exercise is contracts
written as prose rather than as specifications. A Communications
contract that says "the CCO's incident-communications lead
coordinates with the head on external statements" is not a
contract; a contract that names the CCO's lead by role, names the
holding-statement library, names the approval chain
(Communications drafts, head reviews for AI-substance within
thirty minutes, GC reviews for exposure within one hour, CEO
signs for material statements), names the cadence (external-
posture refresh every two hours during the containment phase,
every twelve hours during the remediation phase), and names the
escalation ladder (CCO joins the bridge for material decisions;
if the CCO's lead and the head disagree on substance, the CEO
adjudicates), is. Force the specification depth even where the
enterprise's convention is adapted.

The second common failure is contracts that duplicate CISO / CCO
/ GC boundaries the parent interface documents from
[[mod-109-cross-enterprise-leadership]] already cover. The
incident-time contract composes; it does not renegotiate. If the
SOC + DFIR contract restates the four surfaces of the CISO
interface document, the contract is redundant and will conflict
with the parent under version drift. The incident-time contract
names how the parent is invoked under time pressure — which
surface of the parent fires when, which named owner is on the
bridge, which artefact from the parent gets used at incident
time. The parent interface remains the authoritative document;
the runbook is the invocation script.

The third common failure is board cadence written as an
aspiration rather than as executable timing with named owners. A
cadence that says "the board is notified promptly of material
incidents on a cadence appropriate to the incident's severity" is
not executable. A cadence that says "within one hour of the
head's serious-incident classification, the head drafts a two-
paragraph briefing note (template at [reference]) and the CEO
delivers it by phone call to the audit-committee chair and the
risk-committee chair, followed by the written note by encrypted
email within a further thirty minutes" is executable. Force the
timing, the drafter, the deliverer, and the template for each of
the four moments.

The fourth common failure is a tabletop scenario too generic to
stress-test the coordination surfaces. A scenario that says "an
AI system produces incorrect outputs affecting users" does not
stress-test Regulator Relations (no named NCA), does not stress-
test Government Affairs (no Member-State political context), does
not stress-test the GPAI provider dimension of the AI Act's
value-chain obligations, and does not stress-test the US
employment-context dimension that pulls in CHRO and EEOC / DOL
surface. Force the scenario's specificity: named Member States
where users are affected, a named US state and a named employment
decision type, a named GPAI upstream provider or provider class,
and named incident-clock markers so the walkthrough has a
timeline to trace against. The scenario is reused in the exercise
03 Article 73 filing drill; a scenario that under-specifies the
substrate for the filing drill will have to be re-authored.
