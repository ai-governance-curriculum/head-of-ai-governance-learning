# exercise-01: Incident Command Shape At Leadership Scope

**Estimated effort:** 3 hours

## Objective

Author the head's **incident-command-shape artefact set** — the
governance-artefact bundle that operationalises chapter
[[01-incident-command-shape-at-leadership-scope]] and plugs
directly into the CISO's incident-bridge convention established
as Surface 4 in [[mod-109-cross-enterprise-leadership]] chapter
01. The set is not a single document; it is eight discrete
artefacts (context one-pager, seat charter, taxonomy briefing,
five-decision playbook, delegate rehearsal cadence, bridge-
conduct discipline, CISO-interface stress test, audit-committee
summary) that together define the head's presence on the
enterprise incident bridge, the substantive decisions the head
owns, the delegate pattern that keeps the seat filled when the
head is unreachable, and the audit-committee-visible ratification
of the whole shape.

The artefact set has to survive three stress tests. First, the
CISO's on-call incident commander reads the "AI Substantive
Lead" seat charter cold and confirms the interface — the seat,
the presence pattern by severity, the escalation ladder, the
signature authority, the channel discipline — without a
briefing from the head. A charter that requires a walk-through
from the head fails the test the first time the head is
unreachable. Second, the pre-nominated delegate reads the
delegate rehearsal cadence document and confirms readiness to
hold the seat at a Sev-3 or lower incident with the head on the
sidelines — a cadence that reads as an aspiration rather than a
scheduled programme fails the test. Third, the audit committee
chair reads the five-decision playbook and can trust that the
head has actually rehearsed the substantive calls the head owns
at incident time — a playbook that reads as a taxonomy of
concepts rather than a decision instrument fails the test.

The artefact set matters because it is a governance artefact,
not a personal readiness aide. It ratifies in the CxO adjacency
map from [[mod-101-role-scope-and-leadership-shape]] chapter 06
as a visible enterprise commitment, it is referenced in the
board / audit-committee incident-and-near-miss cluster from
[[mod-103-board-and-audit-committee-reporting]], and it is the
document the enterprise falls back on when the head is on a
long-haul flight and a Sev-1 lands. Nothing about the set is
private to the head.

## Prerequisites

- Chapter [[01-incident-command-shape-at-leadership-scope]] —
  the two-IC distinction (operational IC versus substantive IC
  for the AI dimension), the eight AI-specific incident
  classes, the five substantive decisions, the single-bridge
  discipline, the presence pattern, and the delegate pattern —
  read and internalised.
- [[mod-109-cross-enterprise-leadership]] chapter 01 — the
  CISO-coordination interface document, Surface 4 (joint
  incident-bridge convention), the severity mapping, and the
  separate-incident-bridge anti-pattern.
- [[mod-101-role-scope-and-leadership-shape]] chapter 06 — the
  CxO adjacency map the seat charter and delegate nomination
  ratify into.
- [[mod-103-board-and-audit-committee-reporting]] cluster 3 —
  the incident-and-near-miss reporting cadence, the
  notification threshold, and the audit-committee's line of
  sight on incident-time discipline.
- Baseline familiarity with MITRE ATLAS technique families and
  OWASP LLM Top 10 v2 categories per the primary sources in
  `resources.md` — the taxonomy briefing references specific
  ATLAS techniques and OWASP categories per class.
- A concrete enterprise in mind — sector, AI portfolio shape
  and scale (see [[mod-102-running-the-program]] chapter 06
  AIMS inventory), the current CISO's incident-bridge
  convention (bridge-line versus dedicated tool; standing
  seat template; on-call executive rota), whether a formal
  AIMS under ISO/IEC 42001 is in place, and whether the
  enterprise's AI portfolio touches EU market surveillance
  under Article 73.

## Steps

1. **Enterprise context one-pager.** Author the half-page
   context every subsequent artefact composes against: sector,
   AI portfolio scope (customer-facing generative-AI systems,
   internal decision-supporting systems, agentic-tool systems,
   third-party model-provider footprint), the CISO's current
   incident-bridge convention (bridge platform, standing seat
   template, escalation ladder, severity taxonomy), the current
   incident-management tool (ServiceNow / Jira / PagerDuty /
   dedicated IR platform), and the current on-call executive
   rota discipline (who is paged for what severity). Do not
   invent detail; where the current convention is unclear,
   record the ambiguity as a discovery item the interface
   stress test resolves.

2. **The "AI Substantive Lead" seat charter.** Author the
   charter (two to four pages) that establishes the head's
   pre-established seat on the CISO's standing bridge template.
   The charter names: the seat title on the standing call
   template exactly as it appears; the presence pattern by
   severity (Sev-1 / Sev-2 head or delegate mandatory on the
   bridge; Sev-3 head or delegate on the bridge; Sev-4 level-50
   architect covers with escalation to head on demand); the
   delegate nomination by name, role, and seniority; the pre-
   authorised signature authority for incident-time artefacts
   (Article 73 filings, US serious-incident notifications,
   board-visible incident notes, joint public statements),
   scoped to incident and time-bounded to head's actual
   unavailability; and the escalation ladder when the interface
   breaks. Write the charter in the CISO's operational
   vocabulary, not in AI-governance vocabulary.

3. **The eight-class incident-taxonomy briefing document.**
   Author the level-60 reference the head consults in the first
   ninety minutes of an incident — one page per class, in the
   order chapter 01 established: model failure, systemic bias
   event, prompt-injection compromise, model-extraction event,
   jailbreak-driven downstream harm, third-party model provider
   outage or withdrawal, dataset compromise, judge / evaluator
   corruption. Each class page carries four elements: (a) the
   leadership-substantive question the head answers that the
   SOC cannot; (b) the containment options in the head's
   repertoire specific to that class (a subset of the six
   containment moves from chapter 01 plus class-specific
   moves); (c) the disclosure-trigger hooks (Article 73, US
   serious-incident map, board notification, public
   disclosure); (d) the RCA hooks (which post-incident
   learning-cycle probes the class opens by default). Reference
   the specific ATLAS technique families and OWASP LLM Top 10
   categories for classes where they apply, and mark each
   reference with a `<!-- needs-research: verify [claim]
   against [official source] -->` marker per the standing
   research-discipline requirement.

4. **The five-decision decision-support playbook.** Author the
   playbook the head walks in the first ninety minutes and at
   each hourly checkpoint. For each of the five decisions —
   classification, severity, containment posture on the AI side,
   external disclosure, post-incident learning commissioning —
   name: (a) the sub-questions the head answers to reach the
   decision; (b) the peers the head co-decides with (functional
   counterparts named by role — CISO / SOC lead for severity
   composition, GC for statutory interpretation on disclosure,
   CCO for public-facing disclosure delivery, CAIO / CIO / CTO
   for containment execution, head of HR for population-scale
   redress in class 2, and so on); (c) the artefact the
   decision lands on (severity call in the incident record,
   containment posture in the change-management ticket, filing
   in the regulator envelope, learning commission in the post-
   incident review charter); (d) the record where the decision
   is captured with the head as attributed decision-maker (the
   single incident record per the single-bridge discipline,
   not a parallel AI-side record).

5. **The delegate rehearsal cadence document.** Author the
   cadence — not a training plan, a scheduled programme — that
   keeps the delegate incident-command-shaped. At minimum:
   quarterly tabletop rehearsal against a scenario drawn from
   the eight-class taxonomy, with the delegate walking the
   five-decision playbook end-to-end and the head observing;
   the delegate signs incident notes and rehearsed filings
   during drills so the signature is not first-in-life on a
   live incident; the delegate holds the seat for at least one
   live incident bridge per year (Sev-3 or lower) with the head
   on the sidelines and available on a back-channel only for
   escalation-shaped questions; annual cadence for refreshing
   the delegate's substantive fluency against the taxonomy as
   the AI portfolio evolves. Name the rehearsal facilitator
   (the paired `ai-incident-drill-facilitation-runbook` in the
   parent `ai-strategy` catalogue is the operational vehicle)
   and the calendar owner.

6. **The bridge-conduct discipline artefact.** Author the
   head's own conduct rules on the bridge as a one- to two-
   page discipline document. The document names, verbatim,
   the three triggers on which the head speaks — (a) a decision
   is on the table where the head owns the substantive call,
   (b) an AI-substantive question is being answered by someone
   who is not shaped to answer it, (c) the head is invoking a
   coordination surface with a functional peer that the
   operational IC needs visibility on. It names the discipline
   about what the head does not answer (SOC-owned questions on
   evidence preservation, DFIR timeline, security-side
   containment) and how the head reflects them back to the
   operational IC. It names the handover discipline on step-out
   (what the delegate is briefed on before the head leaves the
   bridge, what timing the head commits to for return) and the
   receive-handover discipline on return (what the delegate
   briefs the head on, what the head confirms before resuming
   the seat).

7. **The interface-with-CISO stress test.** Walk the seat
   charter through the CISO's on-call convention with a
   specific SOC lead in mind (name the role — SOC manager, DFIR
   lead, whoever holds the operational IC seat under the
   current convention; a stand-in reader in the head's own
   function can substitute if the SOC lead is not available for
   the exercise). Adjust the charter's language, the severity
   mapping (which AI-side severity maps to which enterprise
   severity level under the CISO's taxonomy), the channel
   routing (which channel the head posts into, at what cadence
   summaries emit from any AI-substantive side channel into the
   main channel), and the seat convention on the standing
   template until the SOC lead reads the charter cold and
   confirms the interface. Capture the adjustments made and the
   residual open items in the stress-test artefact.

8. **The audit-committee-visible summary.** Compress the entire
   artefact set into a one-page summary that goes into the CxO
   adjacency map from [[mod-101-role-scope-and-leadership-shape]]
   chapter 06 as a ratified line item. The summary names: the
   seat convention (title, position on template, presence
   pattern by severity); the delegate by role and seniority;
   the five decisions the head owns with one line per decision;
   the disclosure triggers the head applies at incident time
   with cross-references to chapters 03 and 04 of this module;
   the rehearsal cadence in one sentence; the interface
   document (the CISO-coordination interface from
   [[mod-109-cross-enterprise-leadership]] chapter 01) the
   summary composes with. Write it as a governance artefact for
   the audit-committee secretariat's line of sight, not as a
   deck the head presents.

## Deliverables

- `enterprise-context.md` — the half-page enterprise context
  one-pager.
- `seat-charter-ai-substantive-lead.md` — the "AI Substantive
  Lead" seat charter for the CISO's standing bridge template.
- `incident-taxonomy-briefing.md` — the eight-class level-60
  reference document (one page per class, four elements per
  class).
- `five-decision-playbook.md` — the classification, severity,
  containment, disclosure, and learning-commission playbook.
- `delegate-rehearsal-cadence.md` — the scheduled rehearsal
  programme with quarterly tabletop, drill signature
  discipline, annual live-incident seat-holding, and calendar
  ownership.
- `bridge-conduct-discipline.md` — the head's on-bridge
  conduct rules, speak-triggers, reflect-back discipline, and
  step-out / return handover protocol.
- `ciso-interface-stress-test.md` — the SOC-lead-read stress
  test with adjustments made and residual open items captured.
- `audit-committee-summary.md` — the one-page CxO-adjacency-
  map ratification summary.

## Acceptance criteria

- The seat charter names the seat title on the CISO's standing
  bridge template exactly, and names the presence pattern by
  severity across all four severity levels (Sev-1 through
  Sev-4) with explicit head / delegate / level-50 architect
  assignment per level. A charter that names presence
  generically ("head is on the bridge for significant
  incidents") fails the criterion.
- The delegate is pre-nominated by name and role in the seat
  charter, at level 50 (senior AI governance architect)
  minimum, with the substantive-fluency, signature-authority,
  and rehearsal discipline elements from chapter 01 all
  explicitly captured. A delegate named as "a senior member of
  the AI governance team" or an unnamed pool fails the
  criterion.
- The five-decision playbook covers all five decisions
  (classification, severity, containment posture, external
  disclosure, learning commissioning) with the four required
  elements per decision (sub-questions, co-deciding peers,
  landing artefact, record of capture). A playbook missing a
  decision or reducing one to a heading fails the criterion.
- The taxonomy briefing covers all eight classes verbatim as
  named in chapter 01, in the specified order, with the four
  required elements per class (leadership-substantive question,
  containment options, disclosure-trigger hooks, RCA hooks).
- The bridge-conduct discipline names the three speak-triggers
  verbatim (decision on the table where the head owns the
  substantive call; AI-substantive question needing an AI-
  substantive answer that no one else on the bridge can give;
  invoking a coordination surface with a functional peer). A
  discipline that paraphrases or collapses the triggers fails
  the criterion.
- The interface stress test names a specific SOC lead role
  under the current CISO convention (or a named stand-in
  reader), records the adjustments the read forced, and passes
  the readability test — the SOC lead can read the seat charter
  cold and confirm the interface without a briefing.
- The audit-committee summary is one page, references the CxO
  adjacency map from [[mod-101-role-scope-and-leadership-shape]]
  chapter 06 as the ratification vehicle, and reads as a
  governance artefact for the audit-committee secretariat, not
  as a presentation deck.
- Any factual claim about a specific ATLAS technique, an OWASP
  LLM Top 10 category, or a regulatory obligation (Article 73
  timing, Colorado AI Act notification scope, NAIC bulletin
  adoption, HHS OCR breach thresholds, FDA MDR scope) carries a
  `<!-- needs-research: verify [claim] against [official
  source] -->` marker where the claim is not independently
  verifiable from the cited primary sources. No obligation is
  guessed.

## Stretch goals

- Extend the delegate discipline into a **two-deep succession
  plan** — the delegate has a delegate — with the same
  substantive-fluency and signature-authority discipline
  applied at the second level, and with the second-deep named
  role differing from the first (for example, level-50
  architect as first-deep, level-40 risk engineer as second-
  deep with narrower signature authority).
- Author a **rehearsed handoff-scenario tabletop** in which
  the head is unreachable (long-haul flight, hard conflict of
  interest with the specific incident, competing incident in
  a different part of the enterprise) and the delegate is
  first-time-on-bridge. The tabletop names the scenario, the
  seat-charter provisions that carry, the escalation the
  delegate uses if the substantive call exceeds delegate
  fluency, and the post-incident review point where the
  head's absence is examined.
- Author the **"external counsel" cover memo** the seat
  charter references for privilege posture — the memo the
  general counsel signs that governs when incident-time work
  product is privileged, when external counsel is engaged
  before evidence collection begins, and how the head's
  substantive artefacts (playbook pages, taxonomy briefing
  annotations, decision records) are treated for privilege.
  Compose with [[mod-104-regulator-engagement]] on legal-
  privilege discipline.
- Extend the playbook with a **decision-tree walk-through for
  one specific incident class** end-to-end — jailbreak-driven
  downstream harm is the recommended class, given the density
  of the disclosure decision. The walk-through takes a
  hypothetical incident from initial classification through
  severity, containment selection from the six-move
  repertoire, disclosure-trigger evaluation against all four
  triggers, and learning-cycle commission, with the head's
  substantive call named at each node.
- Author the **head-of-role annual self-review artefact
  against the playbook** — the yearly document the head writes
  reviewing their own performance against the five decisions
  on incidents that occurred in the year (or, in a quiet year,
  against tabletop rehearsals). The self-review composes with
  the coaching-and-career-pathing cadence in
  [[mod-108-leading-the-governance-function]] and with the
  program-measurement discipline in
  [[mod-107-program-measurement-and-maturity]].

## Notes and starter guidance

The most common first-cut failure on this exercise is the seat
charter that reads as an AI-governance manifesto rather than
an operational insert into the CISO's convention. A charter
that argues for the head's importance, that explains why AI
incidents are different, that motivates the need for a seat,
is a charter that will not be adopted onto the CISO's standing
template. The remedy is to draft the charter with the CISO's
on-call incident commander as the sole reader — someone with
ICS / NIMS lineage, standing bridge discipline, and no patience
for governance vocabulary — and to translate every substantive
claim into that reader's operational language. The charter is
adopted only if the CISO's IC can pick it up cold and treat it
as a template addition.

The second common failure is the five-decision playbook that
reads as an academic taxonomy of concepts rather than a
decision instrument. A playbook that describes what
classification means, what severity means, what containment
means, but does not put the head in front of the actual sub-
questions the head answers to reach the decision, is a playbook
that will not be consulted at the first ninety minutes. Force
the sub-question depth. Each decision should read as a script
the head walks: "Sub-question 1: [specific question]. Answer
lands where: [named artefact]. Co-decider: [named role]. Sub-
question 2: ..." — instrumental, not descriptive.

The third common failure is the delegate rehearsal that is a
document, not a cadence. A document says "the delegate
rehearses quarterly against a tabletop scenario". A cadence
names the calendar owner, the facilitator, the scenario
selection discipline, the last rehearsal date, the next
rehearsal date, and the post-rehearsal delta the delegate has
to close before the next quarter. If the delegate rehearsal
does not appear on the head's own calendar and on the CxO
adjacency map's line-of-sight commitments, it is a document,
not a cadence.

The fourth common failure is the audit-committee summary that
is a marketing deck rather than a one-page governance
artefact. A deck sells; an artefact ratifies. The summary
should read as if the audit-committee secretariat is filing it
into the committee's record — sober vocabulary, cross-
references to the CxO adjacency map and the CISO-coordination
interface, no motivational language, no self-promotion, and
one page. If the head is tempted to add a second page for
context, the context belongs in the underlying artefacts, not
in the summary.
