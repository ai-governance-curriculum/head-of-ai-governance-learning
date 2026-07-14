# Level Ladder Scope and Where Leadership Authority Begins and Ends

## Motivation

A Head of AI Governance role that never publishes its scope on the level
ladder degrades in one of two directions inside eighteen months. Either the
head is sucked downward — re-authoring the control library, red-lining
model-card templates, running vendor-risk questionnaires line-by-line —
because no one below is trusted to deliver, and the head ends up doing
level-25 engineer work at level-60 pay. Or the head is pushed upward past
their authority — signing off on AI product strategy, negotiating the
enterprise AI budget envelope with the CFO, taking the CEO seat in press
interviews — and then discovering, at the first real conflict, that the CAIO
or the CEO never actually delegated any of it.

The level ladder is the antidote. It says, in writing and in advance: which
role owns the *deliverable*, which role owns the *decision*, which role owns
the *sponsorship*, and which role owns the *appeal*. The head lives at
level 60, which is a very particular altitude — high enough to be the
accountable executive for the second line of defence in the AI Governance
family, but not so high that AI strategy or the enterprise AI P&L is inside
scope.

This chapter draws the exact scope map so that neither drift is defensible
after week two.

## Core concept: the AI Governance family ladder from 15 to 70

The AI Governance family, at the levels relevant to this role, looks like:

| Level | Role | Family | Primary output |
|---|---|---|---|
| 15 | `ai-governance-analyst` | AI Governance | Analyst legwork — intake queues, first-draft impact assessments, jurisdictional trackers, model-card drafts, control-evidence collection |
| 25 | `ai-risk-engineer` | AI Governance | Hands-on engineering craft — harm-model authoring, red-team, adversarial-ML, fairness / privacy / guardrail engineering, quantification |
| 35 | `ai-evaluation-engineer` | AI Governance | Release-assurance methodology — audit-trail, evaluation harnesses, regulator-facing evidence packages, sign-off engineering |
| 40 | `agentic-safety-engineer` | AI Governance (sideways-and-up) | Frontier-agent methodology — dangerous-capability evaluation, tripwire design, RSP / Preparedness / FSF operating patterns |
| 50 | `senior-ai-governance-architect` | AI Governance | Architectural design authority — control library, policy taxonomy, cross-jurisdiction crosswalk, ISO/IEC 42001 AIMS scope, risk taxonomy + appetite, assurance architecture, evidence architecture, third-party program, post-market surveillance architecture, GRC-for-AI reference architecture, operating model, sector blueprints |
| **60** | **`head-of-ai-governance` (this role)** | **AI Governance** | **Program leadership — running the program the architect designed, board and audit-committee reporting, direct regulator engagement, incident leadership, function leadership, cross-CxO coordination, function budget and vendor P&L** |
| 70 | `chief-ai-officer` | AI Strategy (executive) | AI strategy, AI portfolio P&L, external positioning at CEO / board-seat scope, enterprise-wide AI budget envelope |

The head consumes from the levels below and reports up (or matrixes) to the
level above. Everything hangs on being precise about that verb — *consume*,
*sponsor*, *challenge*, *deliver*, *defer*.

## What the head consumes from level 50

`senior-ai-governance-architect` at level 50 is the head's most important
supplier. The head does not re-design the twelve architectural deliverables
that role owns. The head consumes them, sponsors them at CxO and board
scope, and defends them under regulator or audit challenge. Concretely,
what the head takes as a given operating design and *runs*:

- **Control library** — the enumerated set of AI controls the enterprise
  operates against, keyed to ISO/IEC 42001 Annex A controls, NIST AI RMF
  categories, ISO/IEC 27001 Annex A where they compose, and sector-specific
  controls (SR 11-7 for banking, GMLP for medical devices, NAIC AI Model
  Bulletin for insurance).
- **Policy taxonomy** — the parent AI policy, sub-policies, standards,
  procedures, and work instructions, with the ownership matrix.
- **Cross-jurisdiction crosswalk** — the machine-readable map from EU AI
  Act obligations → NIST AI RMF categories → ISO/IEC 42001 controls →
  sector rule → enterprise control ID, so a change to one regulation
  propagates predictably.
- **ISO/IEC 42001 AIMS scope** — the AIMS statement of applicability,
  scope boundary, and interface to the parent ISMS under ISO/IEC 27001.
- **Risk taxonomy and appetite framework** — how AI risks are named,
  measured, and appetite-set, aligned to ISO 31000 and ISO/IEC 23894.
- **Assurance architecture** — how a given AI system is proven fit for
  purpose before release, mapping to ISO/IEC 42005 impact assessment and
  release-assurance methodology at level 35.
- **Evidence architecture** — the machine-readable evidence store,
  keyed to control IDs, using OSCAL / CycloneDX ML-BOM / SPDX 3.0 AI
  profile / model cards / system cards / dataset cards / SLSA
  attestation.
- **Third-party program** — the tiering, questionnaire, evidence-request,
  and continuous-monitoring pattern for AI vendors, aligned to SR 23-4
  interagency third-party guidance and ISO/IEC 27036 for information
  security in supplier relationships.
- **Post-market surveillance architecture** — the operating design for EU
  AI Act Article 72 post-market monitoring and Article 73 serious-incident
  reporting.
- **GRC-for-AI reference architecture** — the integration pattern with
  the platform choice (Credo AI, Holistic AI, ModelOp, Monitaur,
  ServiceNow AI Control Tower, IBM watsonx.governance, or an equivalent).
- **Operating model** — how the AI governance function actually operates
  (RACI, cadences, escalation paths, first-line embed pattern).
- **Sector blueprints** — the sector-specific overlay on top of the
  enterprise design (banking / insurance / health / pharma / public
  sector / frontier lab / critical infrastructure).

*Consume* means: the head reads these to sponsor-and-defend depth, can
argue every trade-off in a board room, and challenges the architect for
gaps — but does not re-author. If the head is re-authoring, either the
architect is under-scoped, the head is over-reaching, or the operating
design was never actually finished. All three are load-bearing problems.

## What the head sponsors and challenges — levels 35 and 40

`ai-evaluation-engineer` (level 35) owns release-assurance methodology:
evaluation harnesses, audit-trail engineering, regulator-facing evidence
packaging, the sign-off engineering pattern. The head sponsors this work
in front of the audit committee ("here is how a high-risk system gets
released under our AIMS") and signs the release-decision packet — but the
methodology is the level-35 role's craft, not the head's.

`agentic-safety-engineer` at level 40 owns frontier-agent methodology —
dangerous-capability evaluation, tripwire design, rollback triggers,
operational discipline behind a Responsible Scaling Policy /
Preparedness Framework / Frontier Safety Framework. The head *sponsors*
that program, *reviews* the tripwire and rollback decisions, and *takes
them to the board* — but the head does not design the evaluation suite.
If the head is drafting elicitation prompts, that is drift.

## What the head staffs and directs — levels 15 and 25

`ai-risk-engineer` (level 25) owns the hands-on engineering craft of AI
risk — building the fairness monitor, running the adversarial-ML campaign,
engineering the guardrail. The head sponsors and challenges. The head does
not build.

`ai-governance-analyst` (level 15) owns operational analyst legwork — the
intake queue, first-draft impact assessments, jurisdictional trackers,
control-evidence collection, model-card authoring at analyst tier. The
head staffs and directs. The head does not draft the tracker.

The failure mode at both levels is *rescue drift* — the head personally
saves a delivery that a lower-level role was struggling with, and quietly
adopts the responsibility. Two rescues in and the head has silently
inherited a level-25 or level-15 job on top of the level-60 job. The way
this is prevented is coaching, escalating gaps to hiring, or accepting a
brief delay — not by doing the work yourself. See
[[04-three-lines-at-leadership-scope]] on operational-distance failure.

## What level 70 inherits, extends, or holds without delegation

`chief-ai-officer` at level 70 (where the designation exists — it does
not exist everywhere) holds four things the head does not:

1. **AI strategy** — the enterprise's AI thesis, portfolio priorities,
   build-versus-buy at strategy scope, technology-family selection.
2. **AI portfolio P&L** — the revenue, unit-economic, and margin
   accountability for the AI portfolio.
3. **External positioning at CEO / board-seat scope** — testifying at
   Senate / Congress / European Parliament hearings, chairing at Frontier
   Model Forum board scope, media as the enterprise's AI voice.
4. **Enterprise AI budget envelope** — the top-line AI investment,
   negotiated against the CFO / CEO / board, of which the AI governance
   function budget is one line.

In many enterprises the CAIO designation does not exist yet. Where that
is true, these four things are typically split among the CEO, CIO, CTO,
CDO, and CFO. The head negotiates directly with whichever officer holds
each fragment, but does not attempt to consolidate the CAIO role by
default. See [[07-engagement-contract-authoring]] for how to write the
upward engagement contract in both configurations.

Where the CAIO designation *does* exist, the head typically reports to
the CAIO or matrixes to CAIO + CRO. Two common reporting-line variants:

- **CAIO-report** — head reports solid-line to CAIO, dotted-line to CRO
  (or to CRO + audit committee). Common in enterprises that see AI as
  primarily a growth story, with governance as a subordinate function.
- **CRO-report with CAIO matrix** — head reports solid-line to CRO,
  dotted-line to CAIO. Common in heavily-regulated sectors (banking,
  insurance, pharma) that see AI risk as a risk-line accountability.

Neither is inherently correct. What matters is that the head *knows*
which they are, *has it in writing*, and *has the escalation path from
head to audit committee* preserved regardless. That last invariant —
independent access to the audit committee — is what protects second-line
independence and cannot be conceded to any solid-line manager. It is a
non-negotiable feature of the level-60 role in a Three-Lines-of-Defence
enterprise.

## Where leadership authority begins and ends

The head's leadership authority is:

- **Begins** at the second line of defence for the AI Governance family
  — the authoritative accountable executive for the AI risk framework,
  the AIMS, the AI risk register at portfolio cadence, the AI control
  library operation, second-line challenge of first-line decisions, and
  the interface to the third-line and to regulators.
- **Ends** at strategy, portfolio P&L, and enterprise-wide budget
  envelope — those belong to level 70 or, in its absence, to the CEO /
  CIO / CTO / CDO / CFO stack.
- **Excludes** legal opinion authorship (General Counsel), enterprise
  privacy program leadership (CPO / DPO), enterprise risk parent
  framework ownership (CRO), third-line audit independence (CAE),
  enterprise crisis communications (CCO), and SOC / DFIR runbook
  execution (CISO / Security Operations).

Everything in [[06-cxo-adjacency-positioning]] elaborates the last two
lines. Everything in [[07-engagement-contract-authoring]] operationalises
the first two.

## Example — a stop-shipping decision, level-mapped

Consider a concrete case: a customer-facing generative feature was
approved by first-line product for release; a red-team campaign three
weeks pre-launch surfaces a prompt-injection path that leaks another
customer's data. Who does what.

- **level 15 (analyst)** — pulls the evidence bundle, updates the AI
  system inventory record, drafts the incident intake.
- **level 25 (risk engineer)** — reproduces the exploit, quantifies the
  blast radius against the fairness / privacy / security taxonomy,
  authors the harm model.
- **level 35 (evaluation engineer)** — decides whether the failure
  crosses the release-assurance sign-off threshold under the enterprise
  methodology, packages the regulator-facing evidence.
- **level 40 (agentic safety, if the feature is agentic)** — reviews
  whether an RSP / Preparedness / FSF tripwire has been hit, recommends
  the rollback trigger.
- **level 50 (architect)** — advises whether the failure signals a gap
  in the control library, the risk taxonomy, or the assurance
  architecture that needs a design change.
- **level 60 (head — you)** — chairs the stop-shipping decision at the
  governance council, takes the call with the CIO / CTO / CDO / CPO /
  GC / CRO, briefs the audit-committee chair, decides on Article 73
  notification with GC, sponsors the fix roadmap with the CAIO / CEO
  where the P&L impact is board-relevant.
- **level 70 (CAIO)** — signs off on the P&L and public positioning
  consequences, briefs the CEO, decides on external comms.

The head does not run the exploit reproduction. The head does not draft
the intake ticket. The head does not sign the legal opinion. The head
*owns the decision to stop shipping* and the *cross-CxO coordination and
regulator interface* that flow from it.

## What "leadership shape" means in this module

The four analytic lenses in the chapters that follow — NIST AI RMF
GOVERN, ISO/IEC 38507, IIA Three Lines, and the COBIT / CSF sibling
composition — each define the *shape* of leadership authority at level
60 from a different angle. GOVERN says what a second-line function must
do to be credible. ISO/IEC 38507 says what the board holds the head
accountable for. Three Lines says how the head coordinates across the
three tiers of assurance. COBIT and CSF say how the AI governance
function composes with enterprise IT governance and cybersecurity
governance at enterprise scale. Together they define the four walls of
the level-60 room. Everything the head does at level 60 lives inside
those four walls.

## Summary

- The head at level 60 consumes the level-50 architect's twelve
  operating deliverables, sponsors levels 35 and 40, staffs and
  directs levels 25 and 15, reports or matrixes to level 70, and
  never re-authors what the levels below own.
- Leadership authority begins at the second line of defence for the AI
  Governance family and ends at AI strategy, AI portfolio P&L, and the
  enterprise-wide AI budget envelope.
- Independent access to the audit committee is the non-negotiable
  invariant of the level-60 role and must survive every reporting-line
  variation.
- The failure modes are downward drift (rescue-authoring at level 25 /
  15) and upward over-reach (signing off on strategy or portfolio
  P&L). Both are prevented by writing the engagement contract in
  advance, not renegotiating it under pressure.
