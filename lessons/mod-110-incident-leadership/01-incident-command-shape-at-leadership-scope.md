# Incident Command Shape at Leadership Scope

## Motivation

An AI-specific incident is under way. The model-serving latency
graph looks normal. The security operations centre (SOC) has
opened a ticket because a customer-facing generative-AI
assistant has begun emitting outputs that a customer support
lead flagged as "answering questions we do not answer" — an
apparent safety-alignment bypass. The Chief Information
Security Officer's on-call incident commander convenes the
enterprise incident bridge under the usual convention: DFIR
lead, SOC lead, application security lead, product owner,
communications duty officer, legal duty officer, on-call
executive. The bridge starts working the incident through the
CISO's runbook — containment, evidence preservation, blast-
radius scoping.

The head of AI governance is not on the bridge. There is no
seat convention for the head, and the on-call executive does
not know to call. Ninety minutes in, the CISO's team has
throttled the endpoint, preserved logs, and started the
forensics-timeline reconstruction. What no one on the bridge
has done is answered the AI-substantive questions: is this a
jailbreak, a training-data leakage event, a prompt-injection
compromise, a silent model regression, or an evaluator
corruption that has been hiding a quality collapse for weeks?
The AI-specific severity is unassessed. The AI-specific
containment posture — rollback to the prior model version,
feature-flag disable of the capability, throttle-down of the
affected agentic-tool call, incident-time evaluation to bound
the population who saw the affected output — is unset. When
the CEO calls the CISO at hour three asking whether this is
the kind of incident the board needs to hear about tonight,
the CISO does not have a substantive answer, and neither does
anyone else on the bridge.

This is the failure mode the chapter defends against. It has
two edges. The first edge is the SOC-only response: the CISO's
team runs a clean operational incident and never surfaces the
AI-substantive framing, because no one in the room has the
level-60 shape to name the failure class. The second edge is
positional collapse at the top: the CEO fields the audit-
committee-chair phone call, or the board-designated regulator
question, with no head-shaped view of what has actually
happened on the AI side, because the head was not incident-
command-shaped inside the response. Either edge produces the
same downstream artefact — a filing, a board note, a public
disclosure — that is either technically wrong on the AI
substance or embarrassingly thin on it. The head does not
prevent this by being *available*. The head prevents it by
being incident-command-shaped inside a specific seat, on a
specific bridge, with a specific pre-nominated delegate and a
pre-agreed presence pattern. This chapter is the shape.

The shape composes with the CISO-coordination interface
document from [[mod-109-cross-enterprise-leadership]] chapter
01 (which established the joint incident-bridge convention as
Surface 4 of the four coordination surfaces), the CxO-adjacency
map from [[mod-101-role-scope-and-leadership-shape]] chapter
06, and the board / audit-committee incident cluster from
[[mod-103-board-and-audit-committee-reporting]]. Chapters
02–07 of this module flesh it out: cross-function coordination
patterns beyond the CISO adjacency (chapter 02), Article 73
filing ownership (chapter 03), US serious-incident disclosure
map (chapter 04), post-incident learning-cycle sponsorship
(chapter 05), the difficult incident conversation (chapter
06), and calibration from public incident data (chapter 07).

## Core concept — the head is the substantive incident commander for the AI dimension, not the operational IC

Classical enterprise incident-command discipline is well
established. The Incident Command System (ICS) and the
National Incident Management System (NIMS) — originating in
US wildfire response, generalised into all-hazards emergency
management, and inherited by enterprise cybersecurity through
NIST SP 800-61 and the CISO's DFIR programme — assigns a
single operational Incident Commander who owns the incident
until it closes. <!-- needs-research: verify current NIST SP
800-61 revision is Rev. 3 (2025) and that its incident
command guidance is consistent with the ICS/NIMS lineage cited
here --> That IC directs tactical actions, controls resource
allocation, decides containment posture, and speaks with a
single voice to the bridge. Enterprise cybersecurity has
adopted the same shape: when an incident opens, the CISO's
on-call DFIR lead or SOC lead takes the IC seat and runs the
operational response until the incident is resolved and the
after-action review is commissioned.

The head of AI governance is not that IC. The head does not
direct the SOC's tactical actions, does not allocate DFIR
resources, does not authorise firewall changes, does not run
the log-collection or forensic-imaging procedure. Attempting
any of these is the shadow-SOC anti-pattern from
[[mod-109-cross-enterprise-leadership]] chapter 01 — the head
who tries to run operational incident response ends up
duplicating the CISO's function badly and losing the CISO's
respect in the process. The operational IC seat is the CISO's,
and it stays the CISO's.

What the head is, at incident time, is the *substantive
incident commander for the AI-specific dimension*. The
distinction is the load-bearing conceptual move in this
chapter. The operational IC decides *how* the response is run.
The substantive IC for the AI dimension decides *what the AI
substance of the incident is*, which is the material every
downstream artefact — the containment decision, the severity
call, the filing, the board note, the public disclosure, the
post-incident learning commission — is built on top of. Five
decisions belong to the substantive IC on the AI side
(enumerated below), and no one else on the bridge has the
shape to make them. The CISO's SOC lead can containment-decide
on the security dimension of the incident — network isolation,
credential rotation, endpoint quarantine — but cannot decide
what a "silent model regression" means, cannot decide whether
what looks like a jailbreak is actually training-data
leakage, and cannot decide whether the AI-side containment
posture is rollback-to-prior-version or feature-flag-disable-
the-capability. Those are AI-substantive decisions, and the
head owns them.

The two IC roles run in parallel on a single bridge, not
sequentially and not on separate bridges. The operational IC
runs the bridge; the substantive IC for the AI dimension is
seated at the bridge as a co-lead. When the operational IC
asks the room "what is our containment posture," the head
answers the AI-side question; when the operational IC asks
"what is our severity," the head answers the AI-side severity
and the operational IC composes it with the security-side
severity to reach the enterprise incident-severity call. The
composition is the interface, and the interface is the head's
craft at level 60.

## The eight AI-specific incident classes

The head arrives at the bridge with an internal taxonomy of
AI-specific incident classes. The taxonomy is not the CISO's
severity taxonomy and not the ISMS risk register's category
list — those are parent-frame taxonomies the AI-specific
incident composes into. The AI-specific taxonomy is what lets
the head, in the first ninety minutes of an incident, name
which of a small enumerated set of failure classes is under
way, because the class determines the containment posture,
the severity mapping, the filing question, and the post-
incident learning commission. Eight classes cover the
substantive surface at leadership scope. Each class has a
leadership-substantive question the head answers that the
SOC cannot.

### Class 1 — Model failure

The production model has begun producing incorrect outputs at
a rate outside the tolerance the AIMS system's acceptance
criteria set. The failure can be a regression (a new model
version has landed and is worse than the version it
replaced), a drift-triggered failure (input distribution has
shifted far enough from the training distribution that the
model's calibration has collapsed), or a silent quality
collapse (the model has been degrading for long enough that
the aggregate quality is below tolerance but no single
symptom fired an alarm).

The leadership-substantive question the head answers: *is
this a change in the model, a change in the world, or a
change in the evaluator that has been hiding a change in one
of the first two*. The SOC cannot answer this. Answering it
determines whether containment is rollback (model change),
throttle-and-recalibrate (world change), or evaluator-
recovery-first (evaluator change — see class 8). The wrong
answer wastes hours of the incident.

### Class 2 — Systemic bias event

A production decision-supporting AI system has been running
for long enough that its aggregate impact on a protected
class or a systemic-disadvantage-shaped population is
population-scale — hundreds or thousands of individuals
adversely affected, often across many months, often
undetected until an internal audit, an external complaint, an
academic paper, or a regulator inquiry surfaces it. The event
is not a single moment of failure; it is a state that has
existed for the operating history of the system.

The leadership-substantive question the head answers: *what
is the affected-population estimate, what is the redress
posture, and what is the disclosure obligation to affected
individuals and to the relevant equal-treatment or anti-
discrimination regulator*. The SOC has no framing for this;
the CISO's function is not shaped for equal-treatment law or
for population-scale redress. The head composes with the head
of HR (for HR-in-AI incidents; see [[mod-109-cross-enterprise-leadership]] chapter 07 <!-- needs-research: verify
mod-109 chapter number for CHRO coordination is 07 -->), the
head of legal (for statutory interpretation), and the head of
compliance (for regulator notification).

### Class 3 — Prompt-injection compromise

A production generative-AI system has been the target of a
prompt-injection attack — the MITRE ATLAS AML.T0051 (LLM
Prompt Injection) family, adjacent to OWASP LLM Top 10 LLM01
(Prompt Injection). <!-- needs-research: verify ATLAS
technique ID AML.T0051 for "LLM Prompt Injection" and OWASP
LLM Top 10 v2 (2025) LLM01 category remains "Prompt
Injection" --> The attack has succeeded to the point of
producing an outcome outside the sanctioned behaviour surface
— tool-call misuse, sensitive-data disclosure, downstream
account or transaction impact, or a public-facing output that
violates the enterprise's speech policy.

The leadership-substantive question the head answers: *is
this a first-order injection (an attacker prompt) or a
second-order injection (poisoned content in a RAG source or
in an incoming email the assistant summarised), and what is
the containment on the AI side — prompt-hardening, tool-
allowlist tightening, RAG-source quarantine, or capability
disable*. The CISO's SOC handles the security-side dimension
(session termination, credential rotation, log preservation)
per the coordination interface from
[[mod-109-cross-enterprise-leadership]] chapter 01. The
head's answer determines the AI-side containment, which the
SOC does not know how to select.

### Class 4 — Model-extraction event

An adversary is running a systematic extraction attack
against a production model — either weight-extraction
(sufficient queries and response analysis to reconstruct
model parameters within useful tolerance) or capability-
extraction (sufficient queries to reconstruct a distilled
model that approximates the production model's behaviour on
the adversary's target task). ATLAS technique family AML.T0044
and AML.T0048-adjacent. <!-- needs-research: verify current
ATLAS technique IDs for weight-extraction and capability-
extraction / model-stealing families -->

The leadership-substantive question the head answers: *what
is the exposure on the AI-IP side, what is the containment
that does not break legitimate users (rate-limit, query-
pattern block, credential revocation, model rotation), and is
the extraction complete enough that the model itself has to
be considered exposed*. The last sub-question determines
whether the enterprise runs a model-rotation (deploy a
different fine-tune, invalidate the extracted one's utility
for the adversary's downstream task) or accepts the exposure
and treats it as an intellectual-property loss to be
prosecuted. Neither the CISO nor legal counsel can lead this
call.

### Class 5 — Jailbreak-driven downstream harm

A safety-alignment bypass — the model has been jailbroken
into producing content or taking action that its alignment
was designed to refuse — has produced downstream harm. The
harm can be to a user (harmful advice, malicious code, self-
harm-adjacent content), to a third party (defamatory output,
harassment-shaped output, exposure of a third-party's data),
or to the enterprise (regulatory-triggering output, brand-
damaging output). The jailbreak is not the incident; the
downstream harm is.

The leadership-substantive question the head answers: *what
is the scope of harm (single user, small cohort, population-
scale), what is the containment (session-level block, model-
level alignment re-tuning, capability disable, output-filter
tightening), and what is the disclosure to affected parties
and to the relevant regulator*. The head composes with the
Chief Communications Officer for public-facing disclosure,
with legal for third-party harm exposure, and with the
regulator-relations discipline from [[mod-104-regulator-engagement]] for the filing question.

### Class 6 — Third-party model provider outage or withdrawal

A model the enterprise consumes from an upstream provider —
foundation-model API, embedding API, fine-tuning platform,
guardrail service, evaluator service — has become unavailable
or has been withdrawn. Unavailability can be outage
(temporary), deprecation (announced end-of-life), or
withdrawal (immediate access removal, whether due to the
provider's policy change, the provider's own incident, a
regulator instruction to the provider, or a contract event).

The leadership-substantive question the head answers: *what
is the enterprise's AIMS exposure to the outage — which
production systems degrade, which stop, which have a
fallback, which do not — and what is the AI-side continuity
posture (invoke fallback, disable the affected capability,
degrade gracefully with user-visible communication)*. The
question composes into the enterprise's business-continuity
discipline, but the AI-specific composition (which fallback
model, at what cost, at what quality delta, with what
evaluation before we route production traffic to it) is the
head's substantive call. See [[mod-109-cross-enterprise-leadership]] chapter 03 <!-- needs-research: verify
mod-109 chapter number for the CFO / procurement / supply-
chain adjacency where AI vendor concentration is treated -->
for the parent third-party-risk framing.

### Class 7 — Dataset compromise

A dataset the enterprise's AI systems depend on has been
compromised — training-set poisoning (an adversary has
injected samples into a training or fine-tuning corpus),
evaluation-set poisoning (an adversary has injected samples
into the evaluation set, causing evaluation to systematically
under-detect a failure mode), or RAG-corpus poisoning (an
adversary has planted content in a retrieval corpus the
production system consumes at inference time). The
compromise can be historical (discovered after training
completed and models were deployed) or in-flight (discovered
during training or before deployment).

The leadership-substantive question the head answers: *what
is the affected-model blast radius (which models trained on
the compromised data, which evaluators used the compromised
evaluation set, which production systems consumed the
compromised RAG corpus), what is the AI-side remediation
(retrain-from-clean, filter-and-continue, quarantine-and-
replace), and what is the disclosure obligation if any of the
affected models are downstream of a regulator's
authorisation*. See [[mod-102-running-the-program]] chapter
06 <!-- needs-research: verify mod-102 chapter number for
supply-chain / dataset provenance discipline --> for the
parent dataset-provenance discipline this composes into.

### Class 8 — Judge / evaluator corruption

The LLM-as-judge or automated evaluator that has been signing
off on the production system's quality has itself been
compromised — either through a prompt-injection dimension in
the evaluator's own inputs, through drift in the evaluator
model, through an unnoticed regression in the evaluator's
scoring, or through evaluation-set corruption that fed
through into the evaluator's training. The consequence is
that the enterprise's evaluation function has been reporting
green while the production system's actual quality has been
degrading — sometimes for weeks.

The leadership-substantive question the head answers: *how
far back does the evaluator corruption extend, which
production sign-offs are now invalid, and what is the
recovery discipline — a shadow-evaluator run against golden
sets, a human-labelled sample re-scoring, a full re-
evaluation of the affected systems*. This is the class that
most invalidates the enterprise's own incident-time evidence
base; the head's discipline here is to trust nothing the
compromised evaluator produced. See
[[mod-102-running-the-program]] chapter 08 <!-- needs-research: verify mod-102 chapter number for the
evaluation discipline --> for the parent evaluation-integrity
framing.

The eight classes are not exhaustive and they overlap. A
prompt-injection compromise (class 3) can trigger downstream
harm (class 5) that surfaces because an evaluator was
corrupted (class 8) — the incident may sit across three
classes and the head names all three at the bridge. What the
taxonomy is for is not exhaustive classification; it is the
head's internal check that in the first ninety minutes of the
incident, the head has actually considered the substantive
possibility surface rather than defaulting to whichever class
the SOC's telemetry surfaced first.

## The five substantive decisions the head owns at incident time

Once the class is named, five decisions belong to the head.
None is delegable to the CISO's incident commander or to
legal counsel or to communications, though each composes with
one of those functions. The head making the decision does not
mean the head making it alone; the head co-decides with the
functional counterpart and signs.

### Decision 1 — Classification

Is this genuinely an AI-specific incident, or an application-
layer incident with an AI surface? The distinction is
material because the wrong classification routes the incident
into the wrong response discipline. A generative-AI assistant
returning wrong data because an upstream API returned wrong
data is an application-layer incident (SOC-owned), not an AI-
specific incident. A generative-AI assistant returning wrong
data because the model regressed after a silent fine-tune
update is an AI-specific incident (head-substantive-owned).
The two look the same on the customer-support ticket. The
head's classification separates them in the first bridge
turn.

Classification is a decision, not a diagnosis. The head does
not need to know exactly which class of the eight the
incident belongs to before classifying it as AI-specific; the
head needs to know that at least one of the eight classes is
plausibly in play, that the AI-substantive framing is
required, and that the response has to compose SOC-side and
AI-side work. The definitive class assignment comes later,
often after incident-time evaluation. The initial
classification determines who is on the bridge and what
questions the bridge is asking.

### Decision 2 — Severity

The enterprise has an incident-severity taxonomy — typically
some ordinal scale (S1 through S4 or Sev-0 through Sev-3)
with defined criteria on customer impact, financial impact,
regulatory exposure, and reputational exposure. AI-specific
severity has to map onto that taxonomy without either
inflating (every AI incident is not Sev-0) or deflating
(quality degradation that affects hundreds of thousands of
downstream users is not a Sev-3). The severity mapping
document from the CISO-coordination interface (per
[[mod-109-cross-enterprise-leadership]] chapter 01) is the
reference; the head's incident-time judgement is where the
mapping meets the specific incident.

The head answers three sub-questions to reach the severity
call:

- **Blast radius on the AI side.** Which AIMS systems are
  affected; how many users saw the affected output; how many
  downstream decisions or transactions are implicated. The
  AIMS inventory from [[mod-102-running-the-program]] chapter
  06 is the reference; incident-time evaluation may be
  required to bound the number.
- **Reversibility on the AI side.** Can the affected outputs
  be corrected — a user re-scored, a decision re-taken, a
  transaction reversed — or has the harm crystallised.
- **Regulatory-exposure surface.** Whether the incident
  plausibly triggers an Article 73 obligation, a US federal
  / state / sector obligation from chapter 04 of this module,
  or a contractual obligation to a customer or partner. The
  head's severity has to be defensible against the highest
  regulatory-exposure surface, not against the lowest.

The severity call composes with the CISO's operational
severity to produce the enterprise incident severity, which
the operational IC records. The head's call is one input; the
head does not overrule the CISO on operational severity, and
the CISO does not overrule the head on AI-substantive
severity.

### Decision 3 — Containment posture on the AI side

The CISO's team runs security-side containment (network
isolation, credential rotation, endpoint quarantine, log
preservation, evidence chain-of-custody). AI-side containment
is different. Six containment moves are in the head's
repertoire, and the head selects which combination applies:

- **Rollback to prior model version.** If a model change is
  the cause or the plausible cause, revert to the immediately
  preceding version that has passing acceptance-set
  performance.
- **Feature-flag disable.** Disable the affected capability
  end-to-end — the customer-facing surface, the internal
  tool, the agentic path — without taking the parent product
  down.
- **Throttle-down.** Reduce the traffic rate against the
  affected endpoint to a level that limits the incident's
  ongoing scope while preserving the ability to gather
  evidence.
- **Capability disable at the tool-allowlist layer.** For
  agentic systems, remove the specific tool or tool-cluster
  that the incident implicates from the agent's allowlist.
- **RAG-corpus quarantine.** For retrieval-augmented systems,
  isolate the affected corpus and route retrieval to a known-
  good fallback or degrade to no-retrieval mode.
- **Incident-time evaluation.** Commission a targeted
  evaluation against a golden set or a live-traffic sample to
  bound the incident's actual blast radius and to validate
  that the containment above has stopped the harm.

The head selects; the level-50 senior AI governance architect
executes with the platform team; the CISO records the
containment in the incident record.

### Decision 4 — External disclosure decision

The disclosure decision is the head's, in composition with
the head of legal (statutory interpretation) and the Chief
Communications Officer (delivery). Four disclosure triggers
sit on the head's incident-time checklist:

- **Article 73 (EU AI Act) serious-incident filing.** Whether
  the incident meets the "serious incident" definition and
  triggers the reporting obligation to the market-surveillance
  authorities of the affected Member States. <!-- needs-research: verify the exact "serious incident"
  definition and reporting recipient framing in Article 73(1)
  of Regulation (EU) 2024/1689, and the 15-day / 10-day /
  2-day timing bands for different serious-incident
  categories --> Chapter 03 of this module governs the
  filing.
- **US federal / state / sector serious-incident
  notifications.** Whether the incident triggers any of the
  disclosure map from chapter 04 (Colorado AI Act
  notification, NAIC bulletin notification for insurance,
  HHS OCR HIPAA breach notification where AI-triggered PHI
  exposure applies, FDA MDR for AI-enabled medical devices,
  EEOC / DOL for AI-in-HR, CPPA data-breach adjacencies).
  <!-- needs-research: verify current effective dates and
  scope of the Colorado AI Act (SB24-205) notification
  provisions, current NAIC AI-bulletin state adoption status,
  and the FDA's current AI/ML SaMD MDR reporting framework
  -->
- **Board / audit-committee notification.** Whether the
  incident triggers the notification threshold established
  under [[mod-103-board-and-audit-committee-reporting]]
  incident-and-near-miss cluster. The threshold is pre-agreed
  with the audit committee chair; the head applies it at
  incident time.
- **Public disclosure.** Whether the incident triggers a
  proactive public-communication decision (not a legal
  requirement, but a public-trust posture from
  [[mod-106-external-positioning-and-voluntary-codes]]
  chapter 03 <!-- needs-research: verify mod-106 chapter
  number for public-trust posture --> that the head has pre-
  established with the CCO).

Each trigger has an owner. The head signs the Article 73
filing (per [[mod-104-regulator-engagement]] chapter 02
general-regime discipline and chapter 03 of this module for
incident-time execution). The head signs the US serious-
incident notifications through the general counsel's
channel. The head briefs the audit committee chair; the CEO
briefs the full board. The CCO delivers public disclosure
with the head's sign-off on AI-substantive content.

### Decision 5 — Post-incident learning commissioning

The incident is not closed when containment holds. The head
commissions the post-incident learning cycle — root-cause
analysis (level-25 AI risk engineer executes; per chapter 05
of this module the head sponsors and reviews), control-
library update (from the level-50 senior AI governance
architect), policy update if warranted, evaluation-set update
to catch the class next time, and sector-share decision (do
we share the lesson with the sector via Partnership on AI,
Frontier Model Forum, MLCommons AI Safety, or an AI-scope
ISAC-equivalent, per
[[mod-106-external-positioning-and-voluntary-codes]] chapter
02 <!-- needs-research: verify mod-106 chapter number for
sector-share and standards-body participation portfolio -->).
The commissioning happens at incident-time — the head sets it
in motion before leaving the bridge — even though the work
runs for days or weeks. Chapter 05 of this module governs the
cycle.

## The single-bridge discipline

The load-bearing operational rule this chapter re-establishes
is that there is one incident bridge, and it is the CISO's.
The head joins it. The head does not stand up a parallel
"AI-only" bridge. The anti-pattern was named in
[[mod-109-cross-enterprise-leadership]] chapter 01 (Surface 4,
under the "separate incident bridge" anti-pattern), and it is
the single most common failure mode for a newly-appointed
head of AI governance who has not yet built the discipline
of composing into the CISO's convention.

The rationale is not administrative. It is that decision-
timing on an incident is faster than the coordination cost
between two bridges. If the head is running an AI-substantive
bridge in one meeting-room while the CISO is running the
operational bridge in another, the head's AI-side containment
call gets made ten minutes before the operational IC hears
about it, and the CISO's team has already committed to a
security-side containment that presupposes a different AI-
side move. The rework is expensive; the loss of the CISO's
trust in the head's coordination is more expensive.

Three concrete practices carry the single-bridge discipline
at incident time:

- **The head's seat is pre-established.** The CISO's
  incident-bridge convention names an "AI substantive lead"
  seat that the head or the head's pre-nominated delegate
  fills whenever the incident has an AI dimension. The seat
  is on the standing call template; the on-call executive
  does not have to decide whether to invite the head.
- **The head's channel is one channel.** The incident-
  coordination channel — whether Slack, Teams, a bridge
  phone line, or a dedicated incident-management tool — is
  the CISO's channel, and the head's team posts into it, not
  into a separate AI-side channel. If the head's team has a
  side-channel for AI-substantive discussion, the channel
  emits summaries into the CISO's channel at fixed intervals
  (typically every fifteen minutes at incident-time cadence)
  so the operational IC has full visibility.
- **The head's decisions are recorded in the incident
  record.** The AI-substantive decisions — classification,
  severity, containment posture, disclosure trigger
  assessment, learning commission — land in the same
  incident record the SOC uses, with the head as the
  attributed decision-maker. The record is single-source.

## The head's presence pattern

Presence is the difference between being available and being
incident-command-shaped. Availability is a phone number the
CISO can reach. Presence is a seated position on the bridge
that the CISO's operational IC treats as a peer role. The
presence pattern the head runs has four elements.

### Physical or virtual seat

For a Sev-1 or Sev-2 AI-dimensioned incident (per the
severity mapping from
[[mod-109-cross-enterprise-leadership]] chapter 01), the head
is on the bridge — physically if the enterprise runs a
physical incident command room, virtually if the bridge is
remote. For Sev-3, the head or the pre-nominated delegate is
on the bridge. For Sev-4, the level-50 senior AI governance
architect covers by default, with escalation to the head on
demand. The pattern is pre-agreed with the CISO and recorded
in the interface document.

### Cadence of engagement

The head is on the bridge for the initial ninety minutes of
the incident (the substantive-framing window; classification
and initial severity are set here), for each hourly checkpoint
on the incident's first day, and for every decision-gate the
operational IC calls where the AI-substantive dimension is
material. Between checkpoints the head steps out to do work
only the head can do — brief the CEO, brief the audit
committee chair, sign a filing, brief a regulator — and the
delegate holds the seat.

### Whose questions the head answers

The head answers questions that require the AI-substantive
frame: what class is this, what is the AI-side blast radius,
what is the AI-side containment, is this a filing trigger, is
this a board-notification trigger, what does the post-
incident commission look like. The head does not answer
questions the operational IC or the CISO's team owns: what
the SOC's evidence-preservation status is, whether the
security-side containment has taken hold, what the DFIR
timeline reconstruction shows. When those questions come to
the head, the head reflects them back to the operational IC.
The reflection is disciplined; it protects the head's
credibility for the questions the head is the right seat for.

### When the head steps out

The head leaves the bridge only for work that only the head
can do. Three cases dominate:

- **CEO / audit-committee-chair briefing.** The CEO or the
  audit committee chair needs a head-substantive view of the
  incident to make a decision — public disclosure, board
  convocation, regulator pre-notification. The head steps
  out, briefs, returns.
- **Regulator interaction.** The head is on a call with the
  competent authority — pre-filing courtesy call, filing
  clarification, follow-up interaction. The head steps out,
  runs the call per
  [[mod-104-regulator-engagement]] discipline, returns.
- **Filing signature.** The head signs an Article 73 filing
  or a US serious-incident notification, per chapters 03 and
  04. The signature is often a physical step-out because the
  filing envelope is sensitive to the head's attention and
  cannot be split across a bridge conversation.

In each case, the delegate holds the seat. The head returns
to the bridge as soon as the step-out concludes and receives
a delegate-side handover on what has happened in the head's
absence.

## The delegate pattern

The head is not always available. Holiday, illness, long-
haul travel, a conflict of interest with the specific
incident (the incident touches a system the head personally
commissioned, or a vendor the head has a governance-adjacent
relationship with), a competing incident in a different part
of the enterprise — any of these can take the head out of the
seat. The delegate pattern ensures the seat is never empty
and the substantive shape is preserved regardless.

The delegate is pre-nominated. The nomination is recorded
in the CxO-adjacency map from
[[mod-101-role-scope-and-leadership-shape]] chapter 06,
mirrored in the CISO-coordination interface document from
[[mod-109-cross-enterprise-leadership]] chapter 01, and known
to the on-call executive rota. The delegate criteria are:

- **Seniority.** The delegate is typically the senior AI
  governance architect at level 50 — the workflow-designer
  who authored the runbooks and the interface documents the
  incident response actually runs on top of. Level-50 is the
  minimum; the delegate has to have the standing to be
  treated as a peer by the CISO's operational IC.
- **Substantive fluency.** The delegate has to be able to
  answer the five substantive decisions the head owns —
  classification, severity, containment posture, disclosure
  trigger assessment, learning commission — with the same
  fluency the head brings. Building the fluency is the
  head's succession work, not a fair-weather delegation.
- **Signature authority.** For the specific artefacts the
  head signs at incident time — Article 73 filing, US
  serious-incident notification, board-visible incident
  note, joint public statement — the delegate has a pre-
  nominated signature authority per
  [[mod-104-regulator-engagement]] chapter 02 <!-- needs-research: verify mod-104 chapter number for pre-
  nominated signature-delegate discipline --> on pre-
  nominated signature delegates. The signature authority is
  narrow — it is scoped to the incident, and it is time-
  bound to the head's actual unavailability — but it exists,
  pre-authorised, before the incident opens.

The delegate is not a substitute the head trains at incident
time. The delegate rehearses in the exercise programme (the
Cross-Function Incident Coordination Runbook exercise in
this module is the primary rehearsal vehicle; the paired
`ai-incident-drill-facilitation-runbook` in the parent
`ai-strategy` catalogue is the operational rehearsal). The
delegate signs incident notes during drills so that when a
live incident lands during the head's unavailability, the
signature is not the delegate's first.

Two anti-patterns the head refuses. The first is the "I will
be reachable" pattern — the head on holiday says "call me if
anything happens" and no delegate is named. The pattern
fails the first time the head is unreachable because the
mobile signal is dead or the head is on a long-haul flight.
The second is the "any senior member of the team" pattern —
the head names the AI governance team as a pool from which
the on-call executive can pick, without a specific named
delegate. The pattern fails because no one on the pool has
the standing to make the substantive calls, and the
operational IC ends up making the AI-side calls by default.
Both patterns collapse to positional collapse — the head-
shaped seat is empty, and the CEO or the operational IC
fills the vacuum badly.

## Composition with adjacent modules and next-chapter pointer

- The **CISO-coordination interface document** in
  [[mod-109-cross-enterprise-leadership]] chapter 01 is the
  parent artefact that establishes the joint-bridge
  convention this chapter operationalises. The severity
  mapping, the escalation ladder, and the incident-record
  federation live in that document. This chapter does not
  duplicate them; it composes with them.
- The **CxO-adjacency map** in
  [[mod-101-role-scope-and-leadership-shape]] chapter 06
  records the head's seat convention and the delegate
  nomination as visible enterprise artefacts, ratified in
  the audit committee's line of sight.
- The **AIMS inventory** and **AI risk register** from
  [[mod-102-running-the-program]] chapters 03 and 06
  <!-- needs-research: verify mod-102 chapter numbers for AI
  risk register and AIMS inventory --> are the reference
  artefacts the head consults at incident-time to bound
  blast radius and to identify affected systems.
- The **board / audit-committee incident-and-near-miss
  cluster** in [[mod-103-board-and-audit-committee-reporting]] is where the incident becomes a board-
  visible artefact via the notification threshold this
  chapter's disclosure decision applies.
- The **regulator-engagement discipline** in
  [[mod-104-regulator-engagement]] carries the general-
  regime Article 73 filing framework; chapter 03 of this
  module turns it into incident-time execution.
- The **regulatory change management** work in
  [[mod-105-regulatory-change-management]] is the source of
  the head's current view of what "serious incident" means
  under each in-scope regime, updated as regimes change.
- The **public-trust posture** and **sector-share portfolio**
  in [[mod-106-external-positioning-and-voluntary-codes]]
  govern the public-disclosure and lesson-share dimensions
  of the disclosure decision.
- The **program measurement and maturity** discipline in
  [[mod-107-program-measurement-and-maturity]] is where the
  post-incident learning cycle's output — control-library
  updates, KRI / KPI adjustments — lands as programme
  evolution.

Chapter [[02-cross-function-incident-coordination]] takes the
shape this chapter establishes and turns it into the specific
coordination patterns with functions beyond the CISO —
Communications, Legal, Regulator Relations, Government
Affairs, HR, product owners, and the board — under incident-
time pressure. Chapter [[03-article-73-filing-at-incident-time]] and chapter
[[04-us-serious-incident-disclosure-map]] operationalise the
disclosure decision. Chapter
[[05-post-incident-learning-cycle-sponsorship]] governs the
learning cycle the head commissions at incident close.
Chapter [[06-difficult-incident-conversations]] rehearses the
briefings the head steps out of the bridge to give. Chapter
[[07-calibration-from-public-incident-data]] closes the
module by grounding the head's incident-readiness against
the AI Incident Database, the OECD.AI incidents monitor, and
the MIT AI Risk Repository as peer-benchmark sources.

## Summary

- The head of AI governance is not the operational incident
  commander at an AI-dimensioned incident; the CISO's SOC or
  DFIR lead is. The head is the *substantive* incident
  commander for the AI-specific dimension, seated on the
  same bridge, co-leading on the AI substance while the
  operational IC runs the operational response.
- Eight AI-specific incident classes cover the substantive
  surface at leadership scope: model failure, systemic bias
  event, prompt-injection compromise, model-extraction
  event, jailbreak-driven downstream harm, third-party
  model-provider outage or withdrawal, dataset compromise,
  and judge / evaluator corruption. Each class carries a
  leadership-substantive question the head answers that the
  SOC cannot.
- Five decisions belong to the head at incident time:
  classification (AI-specific or application-layer with AI
  surface), severity (mapping AI-specific severity onto the
  enterprise incident-severity taxonomy), containment
  posture on the AI side (six containment moves in the
  head's repertoire), external disclosure decision (four
  triggers: Article 73, US serious-incident map, board
  notification, public disclosure), and post-incident
  learning commissioning.
- The single-bridge discipline is load-bearing: one
  incident bridge, the CISO's convention, the head joins
  and holds a pre-established seat. The head's channel is
  the CISO's channel; the head's decisions land in the
  CISO's incident record. Parallel AI-only bridges are the
  named anti-pattern.
- The head's presence pattern has a pre-established seat,
  a specific cadence (initial ninety minutes, hourly
  checkpoints, decision-gates), a discipline about which
  questions the head answers, and a discipline about when
  the head steps out (CEO / audit-committee briefings,
  regulator interaction, filing signature) — all covered
  by the delegate.
- The delegate is pre-nominated (typically the senior AI
  governance architect at level 50), rehearsed in the
  exercise programme, and carries pre-authorised signature
  authority for incident-time artefacts. The "I will be
  reachable" pattern and the "any senior member of the
  team" pattern both collapse to positional collapse and
  are refused.
- This chapter is the shape. Chapters 02–07 flesh it out:
  cross-function coordination beyond the CISO, Article 73
  filing at incident time, US disclosure map, post-incident
  learning-cycle sponsorship, difficult incident
  conversations, and calibration from public incident data.
