# Cross-Function Incident Coordination

## Motivation

Every AI incident that matters at leadership scope is a multi-
function incident. By the time the head of AI governance has
classified an event as serious under the incident-command shape
from [[01-incident-command-shape-at-leadership-scope]], the
bridge already has other seats filled: the CISO's DFIR lead is
running containment; the General Counsel has been paged for
statutory-definition interpretation and privilege posture; the
Chief Communications Officer is holding a draft external
statement; Regulator Relations is weighing whether an
introductory call to the national competent authority is
warranted ahead of the Article 73 filing; Government Affairs is
scanning the political weather. After initial containment the
audit-committee chair is on a briefing cadence; within one
business day the full board is notified.

The failure mode is coordination collapse. Three recognisable
shapes. The **parallel bridge** — a technical AI call runs
alongside the CISO's operational bridge, decisions diverge, the
operational bridge learns about corrective actions after they
are announced. The **surprised CxO** — the Chief Product
Officer whose product line is the incident's blast radius
learns from a press briefing rather than from the head; the
CFO reads a regulator-filing commitment in the audit committee
pack rather than in a peer call the day before. The
**unreturned regulator call** — the national competent
authority reaches out for informal context after seeing the
Article 73 filing; the head's function does not have a named
owner for that inbound; the call is not returned inside the
window that would preserve the standing relationship.

Each is a coordination-design failure, not an operational one.
The operational people on the bridge want the coordination to
work; they have been trained on the runbook they hold. The
head's job at incident time is to make sure the right runbooks
are being run in the right order, on the right shared surface,
with the right artefacts being written to the right pens. This
chapter takes the incident-command shape from
[[01-incident-command-shape-at-leadership-scope]] and shows how
it interfaces with each of the CxO peers whose coordination
pattern is authored in [[mod-109-cross-enterprise-leadership]].
Peace-time coordination is a series of interface documents;
incident-time coordination is those documents invoked under
time pressure, without renegotiation.

## Core concept — one bridge, multiple pens

The load-bearing move of this chapter is a two-part discipline:
**one bridge, multiple pens**. The bridge is a single shared
operational surface — the CISO's incident-bridge convention,
per [[mod-109-cross-enterprise-leadership]] chapter 01 — that
every function joins rather than duplicating. The pens are the
distinct artefacts that the incident produces, each owned by a
named function and written on a distinct medium with distinct
review discipline. The head's job on the bridge is to name
which pen holds which artefact, and to make sure each artefact
has a named owner, a named format, and a named review chain.

Seven pens matter at incident time, and the head is either the
owner or the substantive co-owner of most of them.

- **The incident timeline.** Single canonical source, DFIR-
  maintained. Every event with a timestamp — detection, first
  page, containment action, rollback, filing sent, external
  statement posted — lands here first. The head does not
  maintain a parallel timeline; the head consumes the DFIR
  timeline and annotates AI-substantive context back into it.
- **The AI-substantive account of events.** Head-owned. The
  narrative of what the AI system did, why it did it, how it
  differs from expected behaviour, what the AI-specific
  containment measures were (rollback to prior model version,
  feature-flag disable, endpoint throttle, evaluation to bound
  scope). The AI-substantive account is what the head signs
  onto the regulator filing, the board briefing, and the
  after-action report.
- **The regulator-facing filing.** Head signs. General Counsel
  reviews for interpretive gotchas and privilege posture. The
  filing content is drawn from the DFIR timeline and the AI-
  substantive account; the filing decision is the head's per
  [[03-article-73-filing-at-incident-time]] and per the US
  disclosure map in [[04-us-serious-incident-disclosure-map]].
- **The public-facing statement.** Communications delivers.
  The head owns the substance — what the AI system did and did
  not do, what customers should do or refrain from doing, what
  the enterprise is doing about it. Communications owns the
  wording, the timing, and the delivery channel. Legal
  reviews for litigation exposure. The head does not deliver
  the statement to the media directly.
- **The board briefing.** Head drafts. The CEO or Board Chair
  convenes. The audit-committee chair and risk-committee chair
  are notified out-of-cycle first per the cadence below; the
  full board follows on the standing cadence. The briefing
  composes into [[mod-103-board-and-audit-committee-reporting]]
  cluster 3 (incident and near-miss reporting).
- **The customer / deployer notification.** Communications and
  Legal jointly draft. The head owns the substance — what the
  customer or downstream deployer needs to know to protect
  their own users, what they need to do to their own
  integration, what the enterprise commits to on remediation.
  Where the enterprise is a GPAI provider, the deployer
  notification is a distinct instrument from the general
  public statement.
- **The internal all-hands note.** Communications drafts. The
  CEO or the head signs, depending on incident severity and
  the CEO's calibration. The internal note names what happened
  in terms the workforce can understand, what the enterprise
  is doing about it, what the workforce is asked to do or not
  do (typically: do not comment externally, refer press
  inquiries to Communications, refer regulator inquiries to
  Regulator Relations).

The head does not blur the pens. If the head starts drafting
the external statement, Communications loses control of the
delivery. If the head lets DFIR narrate the AI-substantive
account, the account will underweight AI-specific failure
modes the SOC has no reason to have language for. If the head
files the regulator submission without GC review, the
enterprise carries interpretive exposure GC could have caught.
The pen discipline is the shape that keeps each artefact under
the right professional standard.

## The seven coordination surfaces at incident time

Seven coordination surfaces carry the substantive work on the
bridge. Each has a peer, an owned scope, a shared artefact, and
a standing pre-incident agreement that makes the surface
survivable under time pressure. The agreements are the peace-
time coordination interfaces authored in
[[mod-109-cross-enterprise-leadership]], invoked at incident
time without renegotiation.

### Surface 1 — SOC + DFIR (the CISO's team)

**Peer.** The CISO, operationally represented by the SOC lead
and the DFIR lead on the bridge; the CISO joins for material
decisions and for external-communication sign-off. The CISO's
application security lead is on the bridge where the incident
has an application-layer dimension.

**What the peer owns.** The bridge convention itself (call
number, escalation ladder, page tree, standing observers).
Containment execution (network isolation, credential rotation,
system quarantine, evidence preservation). Digital forensics
(collection, imaging, analysis, chain of custody). The
incident timeline as the single canonical source. Coordination
with law enforcement where a criminal dimension emerges.

**What the head owns.** AI-substantive classification (is this
a genuine AI-specific failure mode, or an application-layer
failure that surfaced through an AI system). AI-specific
containment measures (rollback, feature-flag disable, endpoint
throttle, incident-time evaluation to bound scope). Mapping
the finding to MITRE ATLAS techniques and OWASP LLM Top 10
categories where relevant. The AI-substantive narrative that
lands on the DFIR timeline as annotation.

**Shared artefact.** The DFIR-maintained incident record,
with the head's AI-substantive annotations layered onto the
DFIR timeline. The record is stored in the CISO's incident-
record system; the head's function does not stand up a parallel
record.

**Standing pre-incident agreement.** The interface document
from [[mod-109-cross-enterprise-leadership]] chapter 01 — the
four coordination surfaces (AI risk register composition, red-
team finding routing, AI-specific detection engineering, AI-
incident joint response). Surface 4 of that document is what
this section invokes. The severity mapping, the evidence-
sharing protocol, the escalation ladder are all pre-agreed and
carry into the incident without renegotiation.

### Surface 2 — Communications

**Peer.** The Chief Communications Officer, operationally
represented by the incident-communications lead on the bridge;
the CCO joins for material external decisions and for CEO-
level communication sign-off.

**What the peer owns.** Public statement drafting. Media
contact routing (which reporter goes to which spokesperson,
which channel gets the first briefing, which trade press gets
the technical briefing). Holding statements — the language
issued before the full account is available, calibrated to
neither overcommit nor underinform. Customer communications
delivery. Employee-communications drafting. Sentiment
monitoring across social and traditional media. Crisis-
communication counsel to the CEO.

**What the head owns.** The AI-substance of every external
statement — what the AI system did and did not do, what the
containment measures are, what customers should do or refrain
from doing, what the head's function commits to on remediation
and post-incident learning. The head reviews every draft for
AI-substantive accuracy before Communications delivers.

**Shared artefact.** The public statement, the customer /
deployer notification, the employee all-hands note. Each
carries Communications' delivery wording and the head's
substantive endorsement; where legal exposure attaches, GC
reviews before delivery.

**Standing pre-incident agreement.** The coordination interface
from [[mod-109-cross-enterprise-leadership]] chapter 05 (CCO
coordination). The interface names the AI-incident spokesperson
posture (typically the CEO or a delegated CxO, not the head
directly, though the head briefs the spokesperson), the
approval chain for external statements (Communications drafts,
head reviews for substance, GC reviews for exposure, CEO signs
for material statements), and the holding-statement library
pre-drafted for common AI-incident scenario shapes.

### Surface 3 — Legal (General Counsel)

**Peer.** The General Counsel, operationally represented by
the AI-legal lead on the bridge; GC joins for material privilege
and litigation-posture decisions.

**What the peer owns.** Statutory-definition interpretation
under time pressure — is the event a "serious incident" under
EU AI Act Article 3(49) <!-- needs-research: verify Article 3(49) definition of "serious incident" in Regulation (EU) 2024/1689 -->; does it meet the state-statute definition of a covered incident (Colorado AI Act, NYC Local Law 144, California ADMT regulations where applicable); does the event trigger sector-regulator parallel obligation (SR 11-7 model-risk-management notice for a covered US bank, NAIC AI Model Bulletin obligation for a covered insurer, FDA MDR filing for an AI-enabled medical device). Litigation posture — is the incident likely to produce a claim, and how should evidence be preserved. Privilege posture — which parts of the incident-response workstream are prepared under GC direction with attorney work-product protection, which are prepared in ordinary course. GDPR Article 33 parallel-obligation coordination with the DPO where personal data is implicated. <!-- needs-research: verify GDPR Article 33 72-hour notification timeline to supervisory authority -->

**What the head owns.** The head packages the regulatory-
interpretation ask for GC — the specific article, the fact
pattern, the head's reading, the alternatives considered, the
supporting evidence — per the packaging discipline from
[[mod-109-cross-enterprise-leadership]] chapter 06. Under
incident time pressure the package is shorter (a one-page
version), but the discipline is the same. GC delivers the legal
opinion; the head signs the filing.

**Shared artefact.** The regulator filing (head signs, GC
reviews for interpretive exposure and privilege posture). The
litigation-hold notice (GC issues; the head's team implements
against the AIMS artefacts, the risk register, the incident
log, the evaluation results). The privilege posture on the
incident record (GC directs; the head's team executes).

**Standing pre-incident agreement.** The GC coordination
interface from [[mod-109-cross-enterprise-leadership]] chapter
06, plus the engagement-versus-legal-opinion boundary from
[[mod-104-regulator-engagement]] chapter 07. The pre-incident
agreement names the incident-time packaging template (the one-
page version), the standing privilege posture on evaluation
evidence and incident records, and the mixed-engagement
protocol for regulator interactions that straddle operational
and legal exposure.

### Surface 4 — Regulator Relations

**Peer.** The Regulator Relations function — organisationally
this may sit under GC, under a stand-alone Regulatory Affairs
unit, or under Government Affairs depending on the enterprise's
shape. Operationally, the standing relationship-manager for
each national competent authority and for each material sector
regulator.

**What the peer owns.** The standing NCA relationship — the
named contact at the national market-surveillance authority
for the EU AI Act, at the sector supervisor (FRB / OCC / FDIC
for US banking, FDA CDRH for US medical devices, EEOC / DOL
for US employment, NAIC-designated regulators for US insurance,
CPPA for California data protection). The pre-incident
introductory call — where the standing relationship warrants,
Regulator Relations makes an introductory call to the NCA
before the Article 73 filing lands, so that the filing does not
arrive cold. The post-filing correspondence coordination —
which subsequent regulator inquiries route through Regulator
Relations versus which land with the head directly.

**What the head owns.** The substantive filing content. The
substantive answer to any regulator inquiry that follows.
Where the regulator asks a substantive question that goes
beyond the filing's operational scope, the head engages GC
before answering, per the over-explaining anti-pattern from
[[mod-109-cross-enterprise-leadership]] chapter 06.

**Shared artefact.** The regulator filing itself; the pre-
filing introductory-call briefing note (Regulator Relations
delivers, head briefs); the post-filing correspondence log.

**Standing pre-incident agreement.** The relationship map from
[[mod-104-regulator-engagement]] chapter 04 (regulator
relationship management). The map names the standing contact
at each material regulator, the introductory-call convention
(when it fires, who delivers it, what briefing note it
carries), the post-filing correspondence-routing protocol, and
the escalation ladder when a regulator's response falls outside
the standing relationship's scope. In peace time the map is
refreshed on a standing cadence; at incident time the head
consults it and Regulator Relations executes.

### Surface 5 — Government Affairs

**Peer.** The Government Affairs function, operationally
represented by the political-context lead on the bridge; the
Government Affairs Head joins for material political decisions.

**What the peer owns.** The political weather-check — is there
any parallel political context that shapes the incident's
external landscape (a pending regulatory review the enterprise
is a subject of, a pending legislative debate touching the
enterprise's sector, an active election cycle in a Member State
where the incident's blast radius is concentrated). The
Member-State political contacts — where a national-level
political response is possible (a minister's office asking for
context, a parliamentary committee requesting a briefing, a
national ombudsman opening an inquiry). The EU institutional
contacts — the European Parliament committee that has taken
interest, the Council working-party that has scheduled a
review, the AI Office's political-facing side. Sensitivity to
any parallel political context that shapes the enterprise's
external posture.

**What the head owns.** The AI-substantive briefing that
Government Affairs carries into political engagement. The head
does not engage political actors directly; the head briefs
Government Affairs, who engages.

**Shared artefact.** The political-context briefing note
(Government Affairs drafts, head reviews for AI-substantive
accuracy). Where a parliamentary committee or minister's office
requests a briefing, the briefing is delivered by Government
Affairs with the head as substantive co-briefer where the
matter warrants the head's presence.

**Standing pre-incident agreement.** The Government Affairs
coordination interface from [[mod-109-cross-enterprise-leadership]]
chapter 08. <!-- needs-research: confirm mod-109 chapter 08 is the Government Affairs coordination pattern per that module's manifest --> The interface names the standing political-context briefing cadence,
the pre-agreed protocol for parliamentary and minister's-office
inquiries, and the escalation ladder when the political
dimension outweighs the operational one.

### Surface 6 — The board (CEO, audit-committee chair, board chair as appropriate)

**Peer.** The board, operationally represented at incident time
by the CEO (who convenes the board briefing), the audit-
committee chair (who is the standing incident-and-near-miss
recipient per [[mod-103-board-and-audit-committee-reporting]]
cluster 3), the risk-committee chair (where the enterprise has
a separate risk committee), and the board chair (for material
incidents warranting full-board out-of-cycle attention).

**What the peer owns.** Board-level governance oversight of
the incident — the board is not on the operational bridge; the
board consumes the head's briefing and exercises its oversight
role. The audit committee's standing charge on internal
control, risk oversight, and material-incident disclosure
composes into how the audit-committee chair engages during the
incident. The board's fiduciary duties on shareholder
communication (for listed enterprises) shape when and how the
incident is externally disclosed under securities-law regime.

**What the head owns.** The board briefing itself — head
drafts, CEO or Board Chair convenes. The briefing carries the
AI-substantive account, the containment status, the regulator-
filing status, the customer / deployer notification status, the
external-communications posture, the projected remediation
timeline, the residual-risk assessment. The head signs the
briefing.

**Shared artefact.** The out-of-cycle briefing pack (head
drafts, CEO reviews, delivered to audit-committee chair and
risk-committee chair within the hour of serious classification);
the one-business-day full-board notification (head drafts, CEO
delivers); the formal next-sitting briefing (head drafts, CEO
presents, head presents on AI substance).

**Standing pre-incident agreement.** The board-reporting
interface from [[mod-103-board-and-audit-committee-reporting]]
cluster 3 (incident and near-miss reporting). The interface
names the serious-incident classification threshold, the out-
of-cycle briefing cadence, the briefing pack template, and the
escalation ladder from audit-committee chair to full board to
board chair.

### Surface 7 — CxO peers with an adjacent surface

**Peer.** Any other CxO whose function is materially adjacent
to the incident's blast radius. The specific CxOs depend on
the incident shape.

- **CPO / DPO (privacy dimension).** Where the incident
  implicates personal data — data-subject impact, data-
  processing outside the notified purpose, cross-border
  transfer under regulatory scrutiny. The DPO owns the GDPR
  Article 33 supervisory-authority notification and the
  Article 34 data-subject notification decision. <!-- needs-research: verify GDPR Article 33 and Article 34 notification obligations -->
  The head coordinates on the AI-specific dimension of the
  privacy breach.
- **CRO (enterprise-risk-register update).** The Chief Risk
  Officer's enterprise risk register is updated for material
  incidents on a defined cadence. The head coordinates the
  AI-specific risk-register update into the CRO's parent
  register, per the risk-register composition discipline from
  [[mod-102-running-the-program]] chapter 03.
- **CHRO (if AI-in-HR incident).** Where the incident touches
  an AI system used in employment decisions — hiring,
  performance evaluation, termination, promotion — the Chief
  Human Resources Officer is a substantive peer. The CHRO
  owns the employee-facing communication where the incident
  affects individual employees; the head owns the AI-
  substantive account of what the system did.
- **CCO / Chief Compliance Officer (parent compliance
  framework interaction).** Where the enterprise has a
  standing compliance function — for financial-services
  enterprises this is typically the Chief Compliance Officer
  under the parent compliance framework; for other regulated
  sectors the shape varies — the CCO's compliance-monitoring
  and compliance-reporting workstream composes with the head's
  incident response. The head coordinates with the CCO on how
  the incident is characterised in the parent compliance
  framework's reporting.

**What the head owns.** The AI-substantive account of the
incident, carried into each adjacent CxO's parent function's
reporting on the head's initiative. The head does not wait for
each CxO to ask.

**Shared artefact.** The peer briefing note tailored to each
CxO's function — a privacy-dimension briefing for the DPO, an
enterprise-risk briefing for the CRO, an employee-communication
briefing for the CHRO, a compliance-framework briefing for the
CCO.

**Standing pre-incident agreement.** The CxO adjacency map
from [[mod-101-role-scope-and-leadership-shape]] chapter 06,
plus the specific coordination interfaces authored in
[[mod-109-cross-enterprise-leadership]] for each CxO peer. The
adjacency map names which CxOs are on the standing incident-
notification list and which are notified on incident-shape
triggers.

## The pre-incident coordination contracts

The seven surfaces above are unmanageable at incident time
without a pre-agreed contract for each surface. The head does
not invent the coordination pattern on the bridge; the head
invokes a pre-negotiated interface.

Each contract has four elements at minimum. **Owner** — the
named individual on each side of the coordination surface at
incident time (the CISO's SOC lead, the CCO's incident-
communications lead, the GC's AI-legal lead, the Regulator
Relations named contact for the material NCA, the Government
Affairs political-context lead, the CEO for board interaction,
the specific CxO for each adjacent surface). **Format** — the
specific artefact template each surface produces (the DFIR
timeline schema, the external-statement approval chain, the
incident-time GC packaging template, the pre-filing
introductory-call briefing note, the political-context briefing
note, the out-of-cycle board briefing pack, the CxO peer
briefing note). **Cadence** — the timing convention on each
surface (how often the DFIR timeline is refreshed on the
bridge, how often Communications refreshes external posture,
how often the board is briefed post-classification). **Escalation**
— where the interface breaks, how the head and the peer
escalate (typically peer conversation first, then CEO or board
chair per the escalation ladder in each parent interface
document).

Point the contracts back to their parent interface documents:

- SOC + DFIR contract composes into the CISO interface
  document from [[mod-109-cross-enterprise-leadership]]
  chapter 01 (specifically Surface 4 of that document, AI-
  incident joint response).
- Communications contract composes into the CCO interface
  document from [[mod-109-cross-enterprise-leadership]]
  chapter 05.
- Legal contract composes into the GC interface document from
  [[mod-109-cross-enterprise-leadership]] chapter 06.
- Regulator Relations contract composes into the regulator-
  engagement discipline from [[mod-104-regulator-engagement]],
  particularly chapter 04 on regulator relationship
  management.
- Government Affairs contract composes into the Government
  Affairs interface document from
  [[mod-109-cross-enterprise-leadership]] chapter 08.
- Board contract composes into
  [[mod-103-board-and-audit-committee-reporting]] cluster 3.
- CxO peer contracts compose into the CxO adjacency map from
  [[mod-101-role-scope-and-leadership-shape]] chapter 06 and
  the specific chapters of
  [[mod-109-cross-enterprise-leadership]] covering each peer.

All seven contracts are ratified in the CxO adjacency map from
[[mod-101-role-scope-and-leadership-shape]] chapter 06 and
appear as named-and-owned lines in the audit-committee-visible
version of the map. The audit committee sees the shape of the
coordination even if it does not see the operational detail.

## The board notification cadence for serious incidents

The specific cadence for serious incidents — the ones that
warrant out-of-cycle board attention rather than routine
inclusion in the next standing report — is the following
pattern:

1. **Within the hour of the head's serious-incident
   classification.** The audit-committee chair and the risk-
   committee chair are notified out-of-cycle. Notification is
   typically a phone call from the CEO (with the head on the
   line) followed by a written briefing note. The head drafts
   the briefing note; the CEO delivers.
2. **Within one business day.** The full board is notified. The
   CEO delivers written notification with the head's briefing
   attached. Where the board chair judges the incident warrants
   a board-level call before the next scheduled sitting, the
   chair convenes an out-of-cycle call. The head is on the
   call as substantive co-briefer.
3. **Formal briefing on the next scheduled board sitting.** The
   full account — the AI-substantive narrative, the containment
   trajectory, the regulator-filing status, the external-
   communications posture, the customer / deployer notification
   status, the projected remediation, the residual-risk
   assessment, the after-action-review commissioning — is
   delivered at the next standing board sitting. The head
   presents on AI substance; the CEO presents the enterprise-
   wide posture.
4. **Regular status updates until closure.** From formal
   briefing to closure the head delivers a standing status
   update on each subsequent sitting or on a cadence the board
   chair sets. Closure is declared when the incident is fully
   contained, the regulator filing and any follow-ups are
   complete, the remediation is delivered, the after-action
   review is closed, and the control-library update is
   committed.

This cadence is a **leadership expectation**, not a legal
requirement per se — the pattern is the discipline enterprises
adopt for material AI incidents, informed by the general
fiduciary posture on material risk and by the audit-committee's
standing charge on internal control. Sector-specific
requirements may layer specific legal obligations on top: for
US banks the audit-committee notification of material MRM
incidents composes into SR 11-7 governance <!-- needs-research: verify SR 11-7 audit committee reporting expectations for material MRM incidents -->; for
US public companies the material-disclosure obligation under
securities law may require SEC filing on the incident (Form 8-K
Item 1.05 for cybersecurity incidents, with AI-specific
interpretation still evolving <!-- needs-research: verify Form 8-K Item 1.05 scope and any SEC guidance on AI-specific material incidents -->);
for regulated insurers the NAIC AI Model Bulletin composes into
the parent enterprise-risk-management framework's incident
reporting <!-- needs-research: verify NAIC AI Model Bulletin incident-notification expectations -->.
The head names the sector-specific legal layer explicitly in
the pre-incident contract with the board so that the incident-
time cadence is not confused for the legal-obligation timeline.

## The bridge conduct discipline

The head is on the bridge to make decisions the incident needs
made, not to demonstrate technical fluency. This discipline is
easier to state than to hold, because incidents are the
environment where the head's AI-substantive expertise is most
visible and most tempting to spend.

Two anti-patterns illustrate the cost of getting the discipline
wrong.

**The head who monologues on the bridge.** The head takes the
bridge as an opportunity to narrate the AI-substantive account
in exhaustive detail — how the model produces the output, what
the loss function's shape is, why the training-data
distribution is the way it is. The narration is technically
correct and largely irrelevant to the decisions the SOC needs
to make in the next fifteen minutes. The SOC's oxygen drains;
the bridge falls behind on containment; the DFIR lead cannot
get a word in to ask the operational questions that need
asking. The remedy is: the head does not narrate. The head
answers AI-substantive questions the bridge is asking, and
otherwise defers to the operational rhythm.

**The head who is silent on the bridge.** The head listens to
the SOC narrate the incident and does not speak, either from a
belief that operational containment is the SOC's territory or
from a reluctance to interject. The bridge cannot infer what
the head thinks; when the head is asked "what is your read on
the AI-side," the head hesitates and the bridge loses
confidence in the AI-substantive lead's presence. The remedy
is: the head speaks when a decision is on the table or when an
AI-substantive question needs an AI-substantive answer; the
head volunteers the AI-substantive classification early in the
bridge's rhythm; the head names what the head is watching for.

The prescription. The head speaks under three conditions.
First, **a decision is on the table** — a rollback, a feature-
flag disable, a customer-notification trigger, a regulator-
filing gate, an escalation of severity. The head names the
head's position and the reasoning in one or two sentences.
Second, **an AI-substantive question needs an AI-substantive
answer** — the SOC asks whether a specific behaviour is
expected model behaviour or anomalous, whether an observed
output pattern indicates prompt injection or user error, whether
a specific containment action would compromise post-hoc
investigation. The head answers and names the confidence level.
Third, **the head is invoking a coordination surface** — the
head names that the head is engaging GC on a specific packaging
ask, that the head is escalating to the board out-of-cycle,
that the head is invoking the Regulator Relations pre-filing
call. Otherwise the head observes. The bridge is not a stage;
it is a shared operational surface, and every minute the head
spends on oxygen the head is not spending on decisions is a
minute the incident's window closes on.

A specific artefact supports the discipline. The head keeps a
short private log during the bridge — decisions the head made,
AI-substantive answers the head gave with confidence level,
coordination surfaces the head invoked with timestamp. The log
is not the DFIR record; it is the head's own artefact,
consulted post-incident during the after-action review to
calibrate the head's bridge conduct against outcomes. The log
is a level-60 discipline that composes with the RCA-
sponsorship discipline in
[[05-post-incident-learning-cycle-sponsorship]].

## Composition with adjacent modules

- The **incident-command shape** in
  [[01-incident-command-shape-at-leadership-scope]] is the
  parent shape this chapter's coordination surfaces plug into.
- The **CISO coordination pattern** in
  [[mod-109-cross-enterprise-leadership]] chapter 01 is the
  parent interface for Surface 1; specifically its Surface 4
  (AI-incident joint response) is what this chapter invokes
  under time pressure.
- The **CCO coordination pattern** in
  [[mod-109-cross-enterprise-leadership]] chapter 05 is the
  parent interface for Surface 2.
- The **GC coordination pattern** in
  [[mod-109-cross-enterprise-leadership]] chapter 06 is the
  parent interface for Surface 3, with the incident-time
  packaging template as the short-form version of that
  chapter's packaging discipline.
- The **regulator relationship management** in
  [[mod-104-regulator-engagement]] chapter 04 is the parent
  interface for Surface 4; the **engagement-versus-legal-
  opinion boundary** in chapter 07 governs how the head
  answers regulator inquiries that follow the filing.
- The **Government Affairs coordination pattern** in
  [[mod-109-cross-enterprise-leadership]] chapter 08 <!-- needs-research: confirm chapter 08 is Government Affairs per the mod-109 manifest --> is
  the parent interface for Surface 5.
- The **board and audit-committee reporting** discipline in
  [[mod-103-board-and-audit-committee-reporting]] cluster 3 is
  the parent for Surface 6, specifically the incident-and-
  near-miss reporting pattern.
- The **CxO adjacency map** in
  [[mod-101-role-scope-and-leadership-shape]] chapter 06 is
  the parent ratification document for all seven contracts.
- The **AI risk register** and **AIMS inventory** in
  [[mod-102-running-the-program]] chapters 03 and 06 are the
  reference artefacts the AI-substantive account and the
  regulator filing name systems against.
- The **Article 73 filing discipline** in
  [[03-article-73-filing-at-incident-time]] and the **US
  disclosure map** in [[04-us-serious-incident-disclosure-map]]
  are the next chapters, turning to the specific filing
  instruments each surface produces.
- The **post-incident learning cycle** in
  [[05-post-incident-learning-cycle-sponsorship]] is where
  the head's private bridge log and the DFIR record are
  reconciled and where the coordination surfaces themselves
  are reviewed for interface stress.

Chapter [[03-article-73-filing-at-incident-time]] turns to the
specific Article 73 filing instrument — the decision to file,
the filing content, the sign-off, the follow-up regulator
correspondence — as owned by the head at incident time under
the coordination surfaces this chapter establishes.

## Summary

- Every AI incident that matters at leadership scope is a
  multi-function incident. Coordination collapse — the
  parallel bridge, the surprised CxO, the unreturned regulator
  call — is the failure mode this chapter defends against.
- The load-bearing move is **one bridge, multiple pens**. The
  bridge is the CISO's incident-bridge convention that every
  function joins. The seven pens — DFIR timeline, AI-
  substantive account, regulator filing, public statement,
  board briefing, customer / deployer notification, internal
  all-hands note — each have a named owner, a named format,
  and a named review chain. The head does not blur the pens.
- Seven coordination surfaces carry the substantive work on
  the bridge: SOC + DFIR, Communications, Legal, Regulator
  Relations, Government Affairs, the board, and the CxO peers
  with an adjacent surface. Each surface has a peer, an owned
  scope, a shared artefact, and a standing pre-incident
  contract invoked without renegotiation.
- The pre-incident contracts have four elements each — owner,
  format, cadence, escalation — and compose into the parent
  interface documents in
  [[mod-109-cross-enterprise-leadership]],
  [[mod-104-regulator-engagement]], and
  [[mod-103-board-and-audit-committee-reporting]]. All seven
  are ratified in the CxO adjacency map from
  [[mod-101-role-scope-and-leadership-shape]] chapter 06.
- The board cadence for serious incidents: audit-committee
  chair and risk-committee chair notified out-of-cycle within
  the hour; full board within one business day; formal
  briefing at the next scheduled sitting; regular status until
  closure. This is a leadership expectation, not a legal
  requirement per se, though sector-specific legal obligations
  may apply and are named in the pre-incident contract.
- The bridge conduct discipline: the head speaks when a
  decision is on the table, when an AI-substantive question
  needs an AI-substantive answer, or when the head is invoking
  a coordination surface. Otherwise the head observes. The two
  anti-patterns to refuse are the monologuing head who steals
  oxygen from the SOC and the silent head who leaves the
  bridge uncertain of the AI-substantive lead's presence.
- The head keeps a private bridge log during the incident —
  decisions made, AI-substantive answers given, coordination
  surfaces invoked — consulted post-incident against outcomes
  in the after-action review per
  [[05-post-incident-learning-cycle-sponsorship]].
