# CISO Coordination Pattern — Extending Security into AI Without Building a Shadow SOC

## Motivation

The head of AI governance and the Chief Information Security
Officer share a hazard surface that neither of them can carry
alone. The CISO owns the enterprise's cybersecurity program at
parent scope — ISMS under ISO/IEC 27001, controls mapped to the
NIST Cybersecurity Framework (CSF) 2.0, security operations
(the SOC), digital forensics and incident response (DFIR), and
the security report line to the audit committee. The head owns
the AI-specific *extension* of that program: prompt injection,
model extraction, adversarial-ML, training-data poisoning,
jailbreak-driven downstream harm, and the routing of AI red-
team findings into the CISO's operational stack.

Neither role wants the other to try to build the whole program
alone. A head who attempts to run AI security independently of
the CISO ends up standing up a shadow SOC — separate detection
stack, separate incident bridge, separate telemetry — that the
enterprise cannot afford and that the CISO's team will not
respect. A CISO who tries to absorb the AI-specific extension
without the head's technical framing ends up either missing the
novel failure modes (because they do not fit CSF categories the
SOC has instrumented) or treating them as noise. The
coordination pattern in this chapter is what prevents both
failures.

The pattern draws directly from CISA / NCSC "Guidelines for
Secure AI System Development" (November 2023), the follow-on
CISA "Deploying AI Systems Securely" (April 2024), MITRE
ATLAS, OWASP LLM Top 10 (v1.1, 2023) and OWASP LLM Applications
& Generative AI Security (v2, 2025), and NIST SP 800-218A
"Secure Software Development Practices for Generative AI and
Dual-Use Foundation Models" — with ISO/IEC 27001 / 27002 and
NIST CSF 2.0 as the parent frameworks the extension composes
into. The interface design is the head's craft at level 60,
with `senior-ai-governance-architect` (level 50) implementing
against it and the CISO's SOC lead running the operational
runbook on the security side.

## Core concept — the interface, not the runbook

The head designs the *interface*; the CISO runs the *runbook*.
The distinction is the load-bearing move in this chapter and
the one heads most commonly get wrong.

An **interface** is a contract: an inbound signal specification
(the SOC receives red-team findings in this format, at this
severity taxonomy, with this evidence artefact attached), an
outbound signal specification (the SOC returns triage status,
detection-engineering follow-through, and closure evidence in
this format, at this cadence), and a set of joint-authored
detection rules that live in the SOC's SIEM under the SOC's
change-management discipline. A **runbook** is the SOC-side
operating procedure: who is paged when, what the triage checklist
is, how the incident bridge is convened, how DFIR proceeds.

The head co-designs the interface. The head does not write the
runbook. If the head tries to write the runbook, one of two
things happens: the SOC ignores it (because it does not match
the SOC's operational language) or the SOC follows it and
diverges from the CISO's other runbooks (because it was written
by someone outside the SOC's discipline). Either failure mode
costs the head credibility with the CISO the next time an
interface change is proposed.

## The four coordination surfaces

Four surfaces between the head and the CISO carry the
substantive work. Each has an interface, a cadence, and a joint
owner.

### Surface 1 — the AI risk register / ISMS composition

The enterprise's ISMS risk register is the CISO's artefact under
ISO/IEC 27001 clause 6.1.2. The head's AI risk register
(authored under [[mod-102-running-the-program]] chapter 03) is
a portfolio that composes *into* the ISMS register at the
AI-specific rows — training-data confidentiality, model
integrity, evaluation-set poisoning exposure, deployment-time
prompt injection, RAG source poisoning, agent-tool exposure,
model-weight exfiltration risk, third-party model supply-chain
risk. The composition is not a copy; the head keeps the AI-
specific detail in the AI register and pushes summary rows into
the ISMS register through a joint-authored template the CISO's
ISMS lead and the head's level-50 architect maintain together.

Cadence: annual joint review at the ISMS management review
(ISO/IEC 27001 clause 9.3), quarterly delta review through the
enterprise risk committee, per-incident review whenever a new
class of AI risk surfaces. Joint owner: the CISO's ISMS lead
and the head's level-50 architect.

### Surface 2 — AI red-team finding routing

The head's evaluation function runs AI red-team exercises
(per [[mod-102-running-the-program]] chapter 08 evaluation
discipline; the level-35 `ai-evaluation-engineer` executes,
level-50 architect designs the exercise). Findings that
surface security-relevant vulnerabilities — jailbreak that
leads to sensitive-data disclosure; prompt injection that
allows agent-tool misuse; adversarial input that triggers
denial of service on a production endpoint; training-set
poisoning that persists past retraining — route into the CISO's
vulnerability-management stream, not into the head's own
"track for later" list.

The interface is the finding template. Every finding lands in
the CISO's SIEM or vulnerability-management platform through
the SOC's ingestion API with, at minimum: the finding class
(mapped to MITRE ATLAS technique IDs where available and OWASP
LLM Top 10 categories where applicable), the affected system
(referenced against the AIMS inventory ID from
[[mod-102-running-the-program]] chapter 06), the reproducible
proof-of-concept (with confidentiality controls), the head's
recommended severity (with the mapping to the CISO's severity
taxonomy stated explicitly), and the exploitation-conditions
description. The SOC does its own severity triage; the head's
recommendation is one input, not the decision.

Cadence: findings routed within one business day of the head's
review; SOC triage acknowledged within the CISO's standard SLA
(typically 5 business days for below-severity-critical
findings); closure evidence returned to the head's evaluation
function on the SOC's remediation cycle. Joint owner: the
level-50 architect on the head's side and the CISO's application
security lead.

### Surface 3 — AI-specific detection engineering

The SOC's SIEM has standing detection rules for classical
cybersecurity events. AI-specific events are new, and the
detection engineering has to be built. The head does not build
it; the head contributes the *specifications* and the SOC's
detection engineering team implements them.

Examples of specifications the head brings:

- **Prompt-injection detection.** A specification for what a
  suspicious prompt-injection pattern looks like at the API
  gateway or the model-serving layer — instruction-override
  patterns, RAG-poisoning indicators, agentic tool-call
  anomalies. The specification names the observable, the
  detection window, and the expected false-positive rate. The
  SOC's detection engineer implements the rule against the
  SIEM's language.
- **Model-extraction detection.** A specification for query
  patterns that suggest model-extraction — query-volume
  anomalies from a single principal, systematic input-space
  probing, credential rotation coordinated with query bursts.
  The SOC implements against its telemetry.
- **Training-data leakage detection at inference.** A
  specification for output patterns that indicate memorised
  training-data disclosure — verbatim regurgitation of
  identifiable substrings, PII fingerprints matching the
  training-set's PII masking record. The SOC implements against
  the model-serving audit stream.
- **Agent tool-use anomaly.** A specification for agentic
  systems making tool calls outside the sanctioned tool
  allowlist or above the sanctioned rate. The SOC implements
  against the agent-runtime audit log.

Cadence: quarterly joint detection-engineering review; ad-hoc
specification when a new AI system class enters production or a
new red-team finding surfaces a detection gap. Joint owner: the
CISO's detection engineering lead and the head's level-35
`ai-evaluation-engineer`, with the level-50 architect as the
interface owner.

### Surface 4 — AI-incident joint response

When an incident lands that has an AI-specific dimension —
whether the CISO's SOC surfaces it first (as a security
incident that turns out to have an AI cause) or the head's
function surfaces it first (as an AI-safety incident that has a
security dimension) — the response runs on the CISO's incident-
bridge convention with the head as a co-lead on the AI-
substance side. This is the surface where the boundary map
from [[mod-101-role-scope-and-leadership-shape]] chapter 06 and
the incident-leadership discipline from
[[mod-110-incident-leadership]] meet.

The interface, at incident time:

- The CISO's incident bridge is the operational bridge; the
  head joins it, does not stand up a separate one.
- The head is the substantive lead on AI-classification: is
  this a genuine AI-specific failure mode, or an application-
  layer failure that surfaced through an AI system.
- The CISO is the operational lead on containment; the head is
  the substantive lead on the AI-side containment measures
  (rollback to prior model version, feature-flag disable of the
  affected AI capability, throttle-down of the affected
  endpoint, incident-time evaluation to determine scope).
- Joint sign-off on external communications (the Chief
  Communications Officer runs the delivery per chapter 10 of
  this module).
- Joint after-action review, with the head owning the AI-
  specific learnings and the CISO owning the SOC-side
  learnings. Both feed the joint report to the audit committee.

## The interface document

The four surfaces above are consolidated in a single
interface document, co-signed by the head and the CISO,
ratified in the audit-committee-visible CxO adjacency map from
[[mod-101-role-scope-and-leadership-shape]] chapter 06. The
document is short — 6 to 12 pages — and it has, at minimum:

1. **Scope statement.** What is in scope for the interface
   (AI-specific security concerns as defined against MITRE
   ATLAS and OWASP LLM Top 10) and what is not (classical
   application-security concerns that happen to touch AI
   systems, which route through the SOC's standard process).
2. **The four surfaces**, each with the inbound and outbound
   signal specification, cadence, and joint owner.
3. **The severity mapping.** How AI-specific severity — often
   expressed against ATLAS or against the head's own AIMS-
   severity taxonomy — maps to the CISO's incident severity
   levels. Without the mapping, every AI finding routes into
   the CISO's stack at ambiguous severity and the SOC triages
   inconsistently.
4. **The evidence-sharing protocol.** How the head's evaluation
   evidence is stored, retrieved, and referenced from the
   CISO's incident-record system. Where the AIMS evidence
   store and the CISO's evidence store are federated versus
   duplicated.
5. **The escalation ladder.** When the interface breaks — the
   SOC does not triage a finding inside SLA; a specification
   does not turn into a detection rule inside a quarter; an
   incident co-response diverges into two separate bridges —
   how the head and the CISO escalate. Typically: head and
   CISO peer-conversation first, then the CEO or the audit
   committee chair.
6. **The joint audit-committee appearance.** Once a year, the
   head and the CISO appear jointly at the audit committee's
   security-and-AI review, presenting the interface's
   effectiveness against the four-surface cadences and the
   incident record. The joint appearance is the discipline
   that keeps the interface honest across turnover on either
   side.
7. **The review cadence.** Annual review of the interface
   document itself, with the joint owners named per surface,
   the version history maintained.

## Where the shadow-SOC pattern appears

Three concrete anti-patterns the head does not permit,
because each of them is a shadow-SOC pattern in disguise.

**The parallel triage queue.** The head's team maintains its
own list of "AI security findings we are working on" that does
not appear in the CISO's SIEM or vulnerability-management
system. The list is defensible in the head's own eyes
("these are AI-specific, the SOC does not have context") and
indefensible to the audit committee ("why is there an
AI-security finding open for six months that the CISO has
never seen"). The remedy is: every AI red-team finding with a
security dimension routes into the CISO's stack. The head's
tracking is a *pointer* to the CISO's record, not a duplicate
of it.

**The separate incident bridge.** During an AI incident, the
head stands up a separate technical bridge — "the AI-specific
call" — parallel to the CISO's incident bridge. The
communication paths diverge; decisions get made on the head's
bridge without the CISO's operational context; the CISO learns
about corrective actions after they are announced. The remedy
is: one bridge, the CISO's convention, the head joins and
co-leads on AI substance.

**The head-owned detection rule.** The head's team writes a
detection rule against the head's own tooling stack, outside the
SOC's SIEM and outside the SOC's change-management. The rule
fires; the head's team investigates; the SOC learns about the
event later. The remedy is: detection rules live in the SOC's
SIEM under the SOC's change-management, with the head
contributing the specification and the SOC implementing.

## Where the discipline earns its keep — the ATLAS-mapped
finding

The load-bearing test of whether the coordination pattern
works is a specific scenario. The head's evaluation function
discovers, through red-team testing, that a production
generative-AI system is vulnerable to a prompt-injection
attack that escalates into an agentic-tool misuse, mapped to
MITRE ATLAS technique AML.T0051 (LLM Prompt Injection) and
AML.T0053 (LLM Plugin Compromise). The vulnerability's blast
radius includes exfiltration of a customer PII field through
the agent's tool-calling of a database read.

If the coordination pattern is working, the following happens
within one business day: the finding lands in the CISO's
vulnerability-management platform with the ATLAS technique
IDs, the affected AIMS system ID, the reproducible PoC, the
severity recommendation, and the exploitation-conditions
description. The SOC's application security lead
acknowledges, triages against the CISO's severity taxonomy,
and either agrees with the head's severity recommendation or
opens a peer discussion. The detection-engineering lead is
notified so a detection rule can be scoped for similar
patterns at the SIEM. The head's level-50 architect and the
CISO's app-sec lead co-scope the remediation — a combination
of prompt-hardening, tool-allowlist tightening, and post-hoc
output filtering — with the affected product owner (the
conflict-management chapter of this module governs what
happens if the product owner resists).

If the coordination pattern is not working, one of the anti-
patterns above surfaces. The head's team investigates alone,
the SOC learns about the finding six weeks later at the
quarterly review, and the audit committee reads about a
production AI vulnerability that ran for two months without
the CISO's function being engaged. That is the failure mode
the interface document exists to prevent.

## Composition with adjacent modules

- The **CxO adjacency map** in
  [[mod-101-role-scope-and-leadership-shape]] chapter 06 is
  the parent boundary document this chapter's interface
  document lives inside.
- The **AI risk register** in [[mod-102-running-the-program]]
  chapter 03 is the AI-scope register that composes into the
  CISO's ISMS register.
- The **evaluation discipline** in
  [[mod-102-running-the-program]] chapter 08 is the source of
  the red-team findings that route through Surface 2.
- The **AIMS inventory** in [[mod-102-running-the-program]]
  chapter 06 is the reference the finding template names the
  affected system against.
- The **incident-leadership discipline** in
  [[mod-110-incident-leadership]] is where Surface 4 becomes
  operational under time pressure.
- The **communications-coordination chapter** in this module
  (chapter 10) governs the external-communication side of the
  joint incident response.

## Summary

- The head designs the *interface* with the CISO; the CISO
  runs the *runbook*. Confusing the two produces either a
  shadow SOC (head's mistake) or a missed novel failure mode
  (CISO's mistake). Neither survives audit-committee scrutiny.
- Four surfaces carry the coordination: AI risk register
  composition into the ISMS register, AI red-team finding
  routing into the SOC's vulnerability-management stream,
  AI-specific detection engineering (head specifies, SOC
  implements), and AI-incident joint response on the CISO's
  incident bridge.
- The interface document — 6 to 12 pages, co-signed by head
  and CISO, ratified in the CxO adjacency map — carries
  scope, the four surfaces, the severity mapping, the
  evidence protocol, the escalation ladder, the annual joint
  audit-committee appearance, and the review cadence.
- Three anti-patterns the head refuses to run: the parallel
  triage queue, the separate incident bridge, and the head-
  owned detection rule outside the SOC's SIEM.
- The load-bearing test is the specific scenario — an ATLAS-
  mapped finding on a production generative-AI system that
  the head's evaluation function surfaces. The pattern works
  if the finding is in the CISO's stack within one business
  day, triaged inside SLA, and remediated through joint work.
- The chapter feeds the CxO-adjacency ratification cycle and
  the incident-leadership discipline in
  [[mod-110-incident-leadership]]. Chapter
  [[02-cio-cto-cdo-coordination]] turns to the technical-
  platform adjacencies (CIO, CTO, CDO) that the AIMS runtime
  physically plugs into.
