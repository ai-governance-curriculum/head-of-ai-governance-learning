# Rehearsal — EU AI Act GPAI Timelines, JTC 21 Harmonised Standards, and Evolving AISI Methodology

## Motivation

Chapters 01 to 05 built the discipline — scanning, interpretation,
plan shape, compliance-date posture, and cross-function
coordination — for regulatory change as a general capability. The
last two chapters of this module rehearse the discipline against
specific pending changes that are in-flight during the research
window. The purpose is not to be a legal briefing on any single
regulation; that would be GC's work. The purpose is to give the
head the muscle-memory of walking each discipline component
against a real-shaped item, so that the head recognises the shape
when it lands rather than inventing a response from scratch.

This chapter takes three items that are Union-scale and
standards-scale: the EU AI Act's General-Purpose AI provisions
and the associated Code of Practice, the CEN-CENELEC JTC 21
harmonised-standards work supporting the AI Act, and the evolving
AI Safety Institute (AISI) evaluation methodology. Chapter 07
takes state-scale and sector-scale items: state AI acts, OSFI
E-23, and the Korea AI Basic Act.

Each rehearsal follows the same template: what the item is at
head level, what triage tier it earns in scanning, what the
interpretation packaging looks like, what the change-management
plan and compliance-date posture shape look like, and where
coordination and rehearsal muscle-memory pay back. The rehearsal
does not attempt a fully-priced plan — that is the exercise work
(see the exercises folder for this module). The rehearsal shapes
the plan enough that a working head has a defensible starting
point.

## Rehearsal 1 — the EU AI Act GPAI provisions and the GPAI Code of Practice

### What the item is at head level

Regulation (EU) 2024/1689 (the EU AI Act) was adopted in June
2024 and entered into force on 2 August 2024, with a phased
application schedule that carries different obligations to
different dates.
<!-- needs-research: verify the entry-into-force date of Regulation
     (EU) 2024/1689 against the EUR-Lex published text and confirm
     the specific phased application dates for GPAI provisions
     (Chapter V), prohibited practices (Chapter II), high-risk AI
     systems (Chapter III), and the general application date -->

Chapter V of the Act (Articles 51 through 56) sets out obligations
for providers of general-purpose AI models, with additional
obligations for GPAI models with systemic risk. These provisions
are among the earliest-applying substantive obligations of the
regulation, applying broadly twelve months after entry into
force (with transitional provisions for GPAI models placed on the
market before that date).
<!-- needs-research: verify the specific application date for
     Chapter V (Articles 51-56) against the EU AI Act's application
     provisions (Article 113) and confirm the transitional
     arrangements for GPAI models already on the market -->

Alongside Chapter V, the EU AI Office is convening the drafting
of a Code of Practice for GPAI providers, which is intended to
translate the Chapter V obligations into workable operating
practice ahead of any Commission delegated or implementing acts.
The Code of Practice is not a legally binding instrument; a GPAI
provider that follows an approved Code of Practice benefits from
a presumption of conformity with the Chapter V obligations the
Code addresses.
<!-- needs-research: verify the current publication status of the
     GPAI Code of Practice and the roster of participating
     stakeholders against the EU AI Office landing page on
     digital-strategy.ec.europa.eu -->

The head's operating question: does the enterprise provide a GPAI
model in scope of Chapter V, does the enterprise deploy a GPAI
model in scope of the deployer obligations elsewhere in the Act,
or neither.

### Triage tier at scanning

For a GPAI provider, this is a priority tier item. Compliance-
date proximity is close, attachment breadth is total (the entire
GPAI product surface), enforcement risk is high because the AI
Office is publicly attending to this domain, and the peer
distribution of postures is being set in the near term.

For a large deployer that consumes GPAI models from third-party
providers, this is an active tier item because deployer
obligations (Chapter III for high-risk deployments, plus
transparency and disclosure obligations elsewhere) attach at
different dates and the interaction with the provider's Chapter
V posture affects the deployer's own filings and evidence.

For an enterprise that neither provides nor deploys GPAI models
in scope (a defensible position for some sector enterprises), the
item is watch — but the watch entry names the source of
non-attachment (a specific GC opinion, versioned) and the
conditions under which the item would be promoted (a shift in
the enterprise's product plans, the AI Office's issuance of
attaching guidance, a court judgement, etc.).

### Interpretation packaging

The packaged obligation for a GPAI-provider enterprise splits
into two parts: the Chapter V baseline obligations that apply to
all GPAI models, and the additional obligations for GPAI models
with systemic risk (Article 51 and following).

Chapter V baseline obligations include (as of the research
window and subject to GC opinion) technical documentation,
information disclosure to downstream deployers, policy on
compliance with Union copyright law, and a summary of training
content.
<!-- needs-research: verify the specific baseline obligations under
     Article 53 (technical documentation), Article 54 (information
     to downstream providers), and the copyright / training-data
     summary obligations against the EUR-Lex text -->

Systemic-risk obligations layer on: additional model evaluation
including adversarial testing, systemic-risk assessment and
mitigation, incident reporting to the AI Office and to relevant
NCAs, and cybersecurity protection for the model and its
physical infrastructure.
<!-- needs-research: verify the specific systemic-risk obligations
     under Article 55 against the EUR-Lex text and confirm the
     threshold for classification as a GPAI model with systemic
     risk (compute threshold under Article 51) -->

The packaging memo captures each obligation, the attachment
analysis (which of the enterprise's models qualify), the
technical-feasibility assessment (what evidence-production
pipelines the enterprise has and what it lacks), the operational-
cost sketch (which programs of work would be needed), and the
specific questions for GC (does the model meet the systemic-risk
threshold; if so, do the transitional provisions apply; what
defensive posture exists on the copyright-summary obligation
where training data provenance is imperfect).

### Change-management plan shape

Chapter V compliance is engineering-intensive on the provider
side. Lane A (architect and product / engineering) carries most
of the delta: technical documentation pipelines, model
evaluation suite, incident-reporting workflow to the AI Office,
cybersecurity uplift for model weights and infrastructure. Lane
B (legal) carries the copyright policy and the training-data
summary posture. Lane E (communications) carries any public
transparency posture the enterprise takes voluntarily (some GPAI
providers publish transparency reports beyond the strict
obligation; the head decides where the enterprise sits on that
distribution).

For deployers, lane C (procurement) carries a heavy load: the
enterprise's contracts with GPAI providers need to include
provisions that give the deployer the downstream information it
needs to meet its own deployer obligations. This is where
lane 7 of chapter 03 (supply-chain propagation) becomes concrete
work.

The compliance-date posture (chapter 04) for a GPAI provider
usually splits: full readiness on the baseline obligations by
the application date, transition-window posture on the systemic-
risk evaluation depth (with an interim safeguard package that
the enterprise can defend to the AI Office), deferred scope on
any models the attachment analysis excludes, and accepted risk
with board notice on the residual training-data provenance
question.

### Where the Code of Practice fits

The Code of Practice is the head's most useful lever here. A
GPAI provider that has signed on to an approved Code of Practice
walks into the compliance date with a presumption of conformity
on the Code-covered obligations. The head's decision on Code
of Practice sign-on is covered in
[[mod-106-external-positioning-and-voluntary-codes]] chapter 01.
The regulatory-change plan reflects the sign-on decision as an
input, not an output — the decision is made earlier and
separately.

### Coordination pattern

Lane A (architect + engineering): dense, weekly touchpoints
during the year running up to the compliance date. Lane B (GC):
regular touchpoints, with outside counsel engaged if the
enterprise does not have Union-law depth in-house. Lane C
(procurement): moderate load on the provider side, heavy on the
deployer side. Lane D (HR / L&D): moderate, primarily on
role-based training for evaluators and engineers who operate
the model. Lane E (communications): sensitive on the systemic-
risk determination; media interest in "which models are systemic
risk" is intense. Lane F: CISO co-owns cybersecurity uplift;
CPO / DPO co-owns training-data provenance where personal data
is involved; CFO owns the material cost of the engineering
uplift.

## Rehearsal 2 — CEN-CENELEC JTC 21 harmonised standards

### What the item is at head level

CEN-CENELEC JTC 21 (the Joint Technical Committee on Artificial
Intelligence) is the European standards body developing
harmonised standards in support of the EU AI Act's essential
requirements. When a harmonised standard is cited in the
Official Journal of the European Union (OJEU), conformity with
that standard creates a presumption of conformity with the
essential requirements it addresses under the AI Act.
<!-- needs-research: verify the JTC 21 work programme, the list of
     harmonised standards under development, and the citation
     status of any published standards in the OJEU against the
     CEN-CENELEC AI page and the OJEU harmonised-standards
     communications -->

JTC 21 works in coordination with ISO/IEC JTC 1/SC 42 (the
international AI standards body) and often adopts or adapts SC 42
standards for the European harmonised regime. This produces two
streams the head tracks: the SC 42 international workstream
(ISO/IEC 42001, ISO/IEC 42005, ISO/IEC 42006, ISO/IEC 23894,
ISO/IEC 5259 series, ISO/IEC TR 24028, ISO/IEC TR 24368, and
adjacent work items), and the JTC 21 European workstream that
translates or adapts these for OJEU citation.
<!-- needs-research: verify the current list of ISO/IEC SC 42 work
     items and their publication status against the ISO catalogue,
     and confirm the specific adaptation posture JTC 21 has taken
     against SC 42's outputs -->

The head's operating question: which harmonised standards, once
cited in the OJEU, would give the enterprise a presumption of
conformity on obligations that the enterprise otherwise carries
via bespoke evidence — and what changes to the enterprise's AIMS
and control library would be needed to move to standard-cited
evidence.

### Triage tier at scanning

Standards work is a slow-moving stream. Individual work items
enter the register at watch. Promotion to active happens when:
a draft standard reaches formal enquiry (CEN "prEN" stage or ISO
"FDIS" stage); a standard is cited in the OJEU under the AI Act's
harmonised-standards mandate; the AI Office or an NCA references
a specific standard in guidance; the enterprise's certification
body signals a shift.

A standard cited in the OJEU under the AI Act's harmonised-
standards mandate is a priority-tier item, because it changes
the enterprise's evidence posture materially.

### Interpretation packaging

Standards do not "apply" the way regulations do — they are
voluntary at legal level. Interpretation packaging captures:

- Which obligations the standard addresses, in the crosswalk
  vocabulary the level-50 architect maintains.
- The gap between the standard and the enterprise's current
  control library — where the enterprise already meets the
  standard, where it does not, and what closing the gap would
  cost.
- The evidence transition: what evidence the enterprise would
  produce to demonstrate standard conformity versus what it
  produces today.
- The specific question for GC: does adopting the standard create
  a presumption of conformity that the enterprise wants to rely
  on, and are there defensive arguments the enterprise would
  lose by adopting the standard.

### Change-management plan shape

Standards adoption is a level-50 architect-led workstream that
the head sponsors. Lane A carries most of the delta. Lane B
(GC) confirms the presumption-of-conformity effect. Lane C
(procurement) may be affected if the enterprise's certification
body's assessment methodology shifts (which happens when a
standard citation lands and the certification body updates its
audit programme). Lane D (HR / L&D) is affected on evaluator
training if the standard specifies evaluation methodology. Lane
E (communications) carries any public claim of standard
conformity — a claim the head does not make casually.

Compliance-date posture is less date-driven for standards than
for regulation, because standards are voluntary. The head's
posture question is not "am I ready by date X" but "is adoption
the right move at date X, and if so, by what date does the
program's evidence posture shift to standard-cited". The
posture is briefed to the AI Governance Council and, for
material shifts, to the audit committee.

### Coordination pattern

Lane A carries the bulk of coordination. Lane B is
straightforward — GC needs to confirm the legal effect of
standard adoption on the enterprise's overall compliance
posture. Lane F (CxO peers): the CISO and CDO are peers if the
standard touches security or data-governance; the CAE is a peer
because standard adoption changes what third-line audit is
looking at.

## Rehearsal 3 — the evolving AI Safety Institute methodology

### What the item is at head level

The US AI Safety Institute (US AISI), the UK AI Safety Institute
(UK AISI), and their peer bodies in other jurisdictions publish
evolving methodology for evaluating AI models — with particular
attention to frontier models and to systemic risks. UK AISI's
Inspect evaluation framework is a public evaluation harness
maintained by the institute. US AISI operates the AI Safety
Institute Consortium (AISIC) which produces methodology work
products in collaboration with member organisations.
<!-- needs-research: verify the current publication cadence and
     leading work products of the UK AISI (Inspect framework) and
     US AISI / AISIC against aisi.gov.uk and the NIST-hosted AISI
     landing page -->

Unlike the EU AI Act, AISI methodology is not law. The head's
operating question is whether the enterprise's evaluation
methodology should incorporate or defer to AISI methodology, and
whether the enterprise participates in AISIC or in equivalent
consortium work.

### Triage tier at scanning

AISI publications are watched. Individual publications enter the
register at watch. Promotion to active happens when the AISI
publishes methodology that the enterprise's own evaluation
programme would need to explicitly diverge from — because
divergence creates an explanation burden if a regulator or a
third-party asks. Priority is rare on AISI methodology; when it
happens, it is because a specific evaluation-access negotiation
between AISI and the enterprise is on the table.

### Interpretation packaging

Packaging captures: the specific methodology component (a
benchmark, an adversarial protocol, a scoring rubric, an
elicitation technique); the enterprise's current position (does
the enterprise already evaluate this way, or differently, or not
at all); the operational implication of adopting the AISI
methodology (evaluation-team capacity, tooling, cost); and the
question for GC (whether adopting or diverging from AISI
methodology has any legal-position implications, particularly for
enterprises with sector regulators that treat AISI as a
reference).

### Change-management plan shape

For most enterprises, AISI methodology is absorbed into the
enterprise's evaluation harness as evolutionary work, not as a
plan-and-rollout regulatory-change event. The plan shape is
lightweight — Lane A carries the technical work; Lane E may
carry a communications posture if the enterprise chooses to
publish its comparison to AISI baselines; Lane F carries the
CISO peer if evaluation touches security.

For frontier-lab enterprises, AISI methodology is closer to
priority-tier work — the enterprise's evaluation posture is a
material part of its relationship with the AISI, and shifts in
AISI methodology drive the enterprise's own evaluation programme.
The plan shape is heavier and coordination is dense.
Cross-reference: [[mod-111-sector-program-leadership]] chapter 05
(frontier-lab program leadership).

### Coordination pattern

Lane A is the primary coordination lane — the enterprise's
evaluation engineering team (see the level-35 AI evaluation
engineer role) is the operating team. The head sponsors the
adoption or divergence decision at the AI Governance Council.

## What the three rehearsals have in common

Three patterns worth naming.

- **Instrument type shapes the plan shape.** A binding regulation
  (rehearsal 1) drives a heavy plan with all seven lanes active
  and a firm compliance-date posture. A voluntary standard
  (rehearsal 2) drives a plan that is architecturally
  significant but date-loose. A methodology publication
  (rehearsal 3) drives lightweight, evaluation-team-owned work
  for most enterprises and heavier work for frontier labs. The
  head calibrates the plan shape to the instrument type; the
  head does not overuse the seven-lane machinery for
  methodology-scale items.
- **The AI Office is the recurring counterparty.** In all three
  rehearsals, the EU AI Office appears — as the GPAI Code
  convener, as the receiver of OJEU citation nominations from
  JTC 21, as an interested party in AISI-adjacent methodology.
  The head's relationship posture with the AI Office (indirect
  via industry bodies unless the enterprise is a GPAI provider,
  per [[mod-104-regulator-engagement]] chapter 01) shapes how
  the head engages each of these items.
- **The compliance-date logic differs.** Regulation has a hard
  date. Standards have citation dates that create presumption-of-
  conformity thresholds. Methodology has no dates but has
  supervisory-expectation drift. The head's compliance-date
  posture discipline (chapter 04) applies to all three but with
  different weight on the aligned-posture moves.

## The one-sentence summary

The Union-scale rehearsals — GPAI provisions and Code, JTC 21
harmonised standards, AISI methodology — put the head's general
discipline against three specific in-flight items so the head has
muscle memory when the items land; the shared pattern is that
instrument type shapes plan shape, the AI Office is the recurring
counterparty, and the compliance-date logic differs in weight
across the three.

## Summary

- The EU AI Act GPAI provisions (Chapter V, Articles 51-56) plus
  the associated Code of Practice are priority-tier for a GPAI
  provider, active-tier for a deployer, watch-tier with named
  non-attachment for enterprises outside scope. The plan is
  seven-lane; the coordination pattern is dense across
  architect / engineering, legal, procurement (deployer),
  communications, and CxO adjacencies.
- CEN-CENELEC JTC 21 harmonised standards are watch-tier at
  work-programme level; promotion happens on formal enquiry, on
  OJEU citation, or on certification-body signal. Interpretation
  packages evidence transitions, not obligations. The compliance-
  date logic is presumption-of-conformity-driven, not date-
  driven.
- The evolving AI Safety Institute methodology is watch-tier for
  most enterprises and priority-tier for frontier labs. The plan
  shape is lightweight for most enterprises; the coordination
  runs through the level-35 evaluation engineering team.
- Common patterns: instrument type shapes plan shape; the AI
  Office is the recurring counterparty; the compliance-date
  logic differs by instrument type.
- The rehearsal muscle-memory is what the head brings to the
  moment the item actually lands, so the response is
  disciplined rather than improvised.
- Chapter 07 turns to state-scale and sector-scale rehearsals —
  Colorado AI Act, Texas TRAIGA, Korea AI Basic Act, OSFI E-23
  — where the compliance-date logic is often harder and the
  attachment analysis is often thinner.
