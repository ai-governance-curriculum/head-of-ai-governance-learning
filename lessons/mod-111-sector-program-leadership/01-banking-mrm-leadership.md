# Banking — Leading AI Governance Inside the Model-Risk-Management Regime

## Motivation

A bank does not ask "how do we govern AI." A bank asks "how do we
govern models," and every AI system the bank operates gets pulled
into that answer whether or not the AI system's builders think of it
as a model. The examiner from the Federal Reserve, the OCC, or the
FDIC arrives with SR 11-7 and OCC Bulletin 2011-12 in hand, opens
the conversation on model inventory, model validation, and model
monitoring, and expects every AI system in scope to be answered for
against those instruments. If the head of AI governance shows up
with an AI-specific control framework that has no line into the
enterprise's Model Risk Management (MRM) framework, the examiner
reads the bank as having built a parallel program that MRM does not
supervise — and that reading survives the examination.

That is the leadership problem this chapter opens with. Chapter 04
of [[mod-104-regulator-engagement]] introduced banking as one sector
cluster among several. This chapter is depth: what the head of AI
governance actually does, day to day, quarter to quarter, to lead an
AI governance program inside an enterprise that is already
supervised as a bank. It also settles the reporting-line question —
head as a peer of the Chief Model Risk Officer (CMRO), or head as an
AI specialist positioned under MRM — that mod-101 flagged and this
chapter now resolves against the banking-specific instruments.

## Core concept — the AI program lives inside MRM, not beside it

SR 11-7 defines a model, in substance, as a quantitative method,
system, or approach that applies statistical, economic, financial,
or mathematical theories, techniques, and assumptions to process
input data into quantitative estimates. OCC Bulletin 2011-12 tracks
the same definition. Read literally, that captures almost every
supervised or unsupervised learning system a modern bank operates,
including large-language-model-based systems where the model output
is a probability distribution over tokens that the bank acts on. The
US interagency posture — Federal Reserve, OCC, and FDIC — has been
consistent since 2011 that AI/ML systems are models within the SR
11-7 / OCC 2011-12 perimeter.

<!-- needs-research: verify current Federal Reserve, OCC, and FDIC
positioning on whether generative-AI systems used in customer-facing
or credit-decisioning contexts are treated as models under SR 11-7 /
OCC 2011-12, and whether any interagency statement or Q&A has been
issued distinguishing GenAI treatment from traditional ML.
Interagency positioning is evolving through 2025-2026. -->

The operational consequence is that the head of AI governance is
running an AI program inside the MRM program, not adjacent to it.
The AI inventory is a view of the MRM model inventory. AI validation
is a specialisation of model validation under Section IV of SR 11-7.
AI monitoring is a specialisation of ongoing monitoring under
Section V. AI change management flows through the MRM change-
management process. Third-party AI is governed by the SR 23-4
interagency third-party guidance layered on top of MRM. The head who
tries to run an AI framework outside this perimeter is building a
positioning artefact, not an operating program the examiner will
credit.

## The three US federal instruments the head owns line-by-line

### SR 11-7 (Federal Reserve, 2011) and OCC Bulletin 2011-12 (2011)

SR 11-7 is organised around four functional areas: development and
implementation, use, validation, and governance. OCC Bulletin
2011-12 is functionally parallel. The head reads both, section by
section, against every AI use case in the inventory, and can point
to a concrete artefact for each section:

- Development and implementation (Section IV): documented model
  purpose, data selection, algorithm choice, and implementation
  testing. For an AI system, this is the AI model card plus
  training-data lineage plus the pre-deployment evaluation record.
- Use (Section V-A): the model's use is aligned with the purpose
  documented at development. For an AI system, this is the use-case
  restriction the enterprise commits the model to and the drift
  monitoring that detects use-case creep.
- Validation (Section V-B, V-C, V-D): independent effective
  challenge, ongoing monitoring, and outcomes analysis. For an AI
  system, this is the independent validation package — evaluation
  against a held-out and shifted-distribution test set, bias/fair-
  lending analysis where applicable, robustness testing — signed by
  a validator who does not report to the AI system's developer.
- Governance (Section VI): policy, roles, model risk assessment,
  and reporting to the board. This is where the head personally
  signs into the framework, at the same tier as the CMRO signs into
  the enterprise MRM policy.

### SR 23-4 / OCC Bulletin 2023-17 / FDIC FIL-29-2023 — interagency third-party risk

The 2023 interagency third-party risk management guidance replaced
each agency's prior separate guidance. For an AI program, the
guidance's lifecycle stages — planning, due diligence and third-
party selection, contract negotiation, ongoing monitoring, and
termination — attach to every foundation-model API, every managed
ML platform, every model-derived data feed. Where a third-party AI
provider produces model output the bank acts on, the bank's model
inventory reflects the third-party model, the validation package
references the third-party's evaluations plus the bank's own,
contractual audit rights and data-use restrictions are in scope, and
concentration risk on the third-party provider is monitored.

<!-- needs-research: verify current OCC Bulletin number for the
interagency third-party risk guidance issued in June 2023 (commonly
cited as OCC Bulletin 2023-17), and the FDIC's FIL companion; the
interagency package was issued together but numbered separately by
each agency. -->

### The OCC Comptroller's Handbook Model Risk Management booklet

The OCC handbook's MRM booklet is the on-the-ground examiner
reference at OCC-supervised banks. Examiners work from the booklet
checklists. The head reads the booklet in advance of any OCC
examination, cross-walks the AI program against the booklet's
control expectations, and identifies where AI-specific evidence
sits inside each control area.

## OSFI E-23 and PRA SS1/23 — the Canadian and UK overlays

For a Canadian federally-regulated financial institution, OSFI
Guideline E-23 on model risk management is the primary instrument.
E-23 was revised and expanded in 2024-2025 to explicitly cover AI/ML
model risk within the same framework, using the same lifecycle
structure — model identification, development, validation,
deployment, monitoring, and decommissioning — that E-23 has applied
to conventional models. OSFI Guideline B-10 on third-party risk
management sits alongside E-23 the way SR 23-4 sits alongside SR
11-7. OSFI additionally issued the Financial Industry Forum on AI
principles (FIFAI EDGE — Explainability, Data, Governance, Ethics)
which the head reads as the interpretive lens OSFI applies over the
E-23 baseline.

<!-- needs-research: verify the exact publication date and current
version of OSFI Guideline E-23 as revised; the guideline was
consulted on in 2023 and issued in updated form in 2024, with
subsequent updates possible through 2025-2026. Confirm citation
against osfi-bsif.gc.ca. -->

For a UK bank, PRA Supervisory Statement SS1/23 on model risk
management principles for banks (issued May 2023, effective May
2024) is the primary instrument. SS1/23's five principles — model
identification and MRM classification, governance, development and
validation, deployment and use, and independent model validation —
frame the head's program design for the UK entity. SS1/23 explicitly
covers AI/ML models within its scope; the head does not need a
separate framework to defend AI treatment under SS1/23.

At the EU level, banks under the Single Supervisory Mechanism apply
the ECB Guide to Internal Models (for internal-ratings-based, market
risk, and counterparty credit risk models) and the EBA Guidelines on
Internal Governance (EBA/GL/2021/05). Neither is AI-specific.
Together with the incoming EU AI Act obligations for high-risk AI
systems used in creditworthiness and life or health insurance
pricing (Annex III), they form the EU-side model-governance surface
the head reconciles to the group MRM framework.

## The head's relationship with the Chief Model Risk Officer

The head of AI governance sits somewhere on a spectrum with respect
to the CMRO. Three placements recur in practice; the head chooses
the placement that fits the enterprise and defends it to the board.

### Placement A — head as a peer of the CMRO

The head reports to the CRO alongside the CMRO. The head owns the
AI-specific dimensions of the MRM framework and the AI-specific
external engagements (EU AI Office, US AISI, EU AI Act filings under
Articles 72 and 73). The CMRO owns the MRM framework at the
enterprise level. The two functions co-sign the AI portion of the
model inventory, the AI-specific validation standard, and the AI
elements of the third-party risk package. This placement is common
at large banks where the AI portfolio has grown to a scale that
requires a dedicated leader but the MRM function retains authority
over model classification and validation independence.

### Placement B — head as an AI specialist under the CMRO

The head reports to the CMRO. The head runs the AI specialisation
of MRM — AI model inventory, AI validation methodology, AI
monitoring, foundation-model-specific controls — inside the MRM
framework and under the CMRO's authority. The head still fronts
AI-specific external engagements but does so under the CMRO's line.
This placement is common at mid-size banks where a dedicated AI
governance function is warranted but the CRO's org design does not
support two peer positions.

### Placement C — head as an enterprise-wide role above MRM's AI perimeter

The head reports to the CEO, the COO, or the Chief Compliance
Officer, and the CMRO reports separately to the CRO. The head's AI
program covers the whole enterprise, including non-model AI uses
that would not fall inside the MRM perimeter under SR 11-7 (internal
productivity tools, marketing personalisation, customer-service
chatbots where no acted-upon quantitative estimate is produced). The
head and the CMRO share a written protocol on where the perimeter
runs, who owns what at the boundary, and how joint reporting to the
board is structured. This placement is common where the enterprise
has non-banking AI use (asset management, insurance affiliate, tech
platform business) that MRM's remit does not cover.

None of the three is inherently correct. The head reads the
enterprise's actual org design, the CMRO's actual scope, and the
board's actual expectations, and picks the placement that produces
one accountable executive for the AI-specific dimension of every
model-risk conversation. The failure mode is any placement where the
board cannot answer "who is accountable for AI" without asking a
follow-up question.

## Fair-lending and consumer AI — CFPB, Regulation B, and the shape of the head's involvement

Consumer-facing AI in banking runs into two additional supervisory
regimes on top of MRM. The head owns the AI-specific dimensions of
both without owning the compliance function itself.

Regulation B (12 CFR 1002), implementing the Equal Credit
Opportunity Act, requires creditors to provide specific and accurate
statements of the principal reasons for adverse action. CFPB
Circular 2022-03 confirmed that ECOA and Regulation B's adverse-
action notice requirements apply where credit decisions are based
on complex algorithms, including AI/ML systems where the reasoning
is not readily interpretable. CFPB Circular 2023-03 followed on the
proper use of the CFPB's sample forms in that context. The head
coordinates with the Chief Compliance Officer to ensure the AI
system produces adverse-action reasons at model-development time,
not as an after-the-fact reconstruction. The compliance function
owns the Regulation B compliance stance; the head owns the AI-
specific evidence that the reasons are principal and specific.

Anti-discrimination overlay: the Interagency Statement on Fair
Lending, the DOJ / HUD / CFPB pattern-or-practice enforcement
posture, and the OCC's fair-lending examination procedures all read
AI-driven credit decisioning through disparate-impact analysis. The
head coordinates the fair-lending evidence — the disparate-impact
testing methodology, the less-discriminatory alternative analysis,
the disparate-treatment guardrails, the documentation of feature
selection and proxy elimination — with the fair-lending compliance
function. The compliance function fronts the CFPB and DOJ
engagement; the head is the technical author of the fair-lending
record.

<!-- needs-research: confirm current CFPB posture on adverse-action
notice for algorithmic credit decisioning and any post-2023
circulars, guidance, or supervisory highlights that extend Circular
2022-03 and 2023-03. CFPB positioning has been subject to change
through 2024-2026 depending on administration priorities. -->

UDAAP overlay: the Consumer Financial Protection Act's UDAAP
authority reaches AI-driven customer interactions — chatbots, robo-
advisers, personalised offers — where an act or practice is unfair,
deceptive, or abusive. CFPB Circular 2023-03 addressed chatbots
specifically. The head owns the AI-specific fairness and disclosure
evidence; the compliance function owns the UDAAP compliance stance.

## The examination cadence at leadership scope

Large banks under continuous supervision see an examination rhythm
that never fully stops. The head does not run to an examination
schedule; the head runs a standing evidence pipeline that any
horizontal review, targeted examination, or on-site examination
draws from without special preparation. The pipeline produces, on a
rolling basis:

- Current model inventory with AI systems tagged, materiality tier
  assigned, use-case restriction documented.
- Current validation status for every AI system on the MRM cycle,
  with dates of last validation and next scheduled validation.
- Current ongoing-monitoring signal for every deployed AI system —
  performance drift, distribution drift, fairness metrics where
  applicable — with escalation thresholds and the response record
  when thresholds trip.
- Current change-management record for every AI system, including
  version history, retraining events, and the associated re-
  validation decision.
- Current third-party AI attestation trail — foundation model
  provider risk assessments, ongoing monitoring evidence,
  concentration analysis where the enterprise is heavily dependent
  on a single provider.
- Current fair-lending and adverse-action evidence for every
  consumer-facing AI system where Regulation B or ECOA applies.

A horizontal review announced with three weeks' notice does not
change the pipeline; it changes which slice of the pipeline the head
presents. That standing-evidence discipline is the operating
difference between a bank AI program that examines well and one that
does not.

Escalation runs through the sector's own vocabulary. A Matter
Requiring Attention (MRA) from the Federal Reserve or the OCC
triggers a remediation programme with a named executive owner (the
head, or a peer, depending on the MRA's scope), a milestone plan
signed to the exam team, and a closing-evidence package. A Matter
Requiring Immediate Attention (MRIA) triggers audit-committee
briefing (see [[mod-103-board-and-audit-committee-reporting]]
cluster 4) and general-counsel escalation. A formal enforcement
action moves the general counsel and external counsel to the front
seat; the head remains the technical author of the factual record
and the designer of the compliance programme the settlement will
require.

## The head's board-level story

At the audit committee, banking AI governance is a story with three
recurring beats.

1. The AI portfolio is inside the MRM framework, not beside it.
   Every material AI system is in the model inventory, is classified
   at a defensible materiality tier, and is on the validation and
   monitoring cadence appropriate to its tier.
2. The enterprise's regulatory posture across the three US federal
   regulators (Federal Reserve, OCC, FDIC) and, where applicable,
   OSFI, PRA, ECB, EBA, is coherent. The head, the CMRO, and the
   Chief Compliance Officer are aligned on who fronts each
   regulator, who signs each filing, and how AI-specific dimensions
   flow through the sector's escalation ladder.
3. The AI-specific external engagements — the EU AI Act if the
   bank has EU exposure, the US AISI network, the Financial
   Stability Board / FSOC AI workstreams, the AICPA's AI risk
   management framework where the external auditor cites it — are
   coordinated with the MRM function and with the board's ratified
   external-positioning posture (see
   [[mod-106-external-positioning-and-voluntary-codes]]).

An audit committee that gets those three beats consistently, on
each quarter's board pack, does not ask a fourth question — because
the fourth question would be the one the head cannot answer, and
the head has designed the reporting to prevent that question from
arising unprepared.

## Summary

- A bank's AI systems are models under SR 11-7 / OCC 2011-12, and
  the AI governance program lives inside the enterprise's Model
  Risk Management framework, not beside it. Attempting to run a
  parallel AI framework produces a positioning artefact that
  examiners will read as a program-design failure.
- The three US federal instruments the head owns line-by-line are
  SR 11-7 (Federal Reserve, 2011), OCC Bulletin 2011-12 (2011), and
  the 2023 interagency third-party risk guidance (SR 23-4 / OCC
  Bulletin 2023-17 / FDIC FIL-29-2023). The OCC Comptroller's
  Handbook MRM booklet is the on-the-ground examiner reference at
  OCC-supervised banks.
- OSFI E-23 (revised to cover AI/ML) and OSFI B-10 govern Canadian
  federally-regulated FIs. PRA SS1/23 covers UK banks. ECB Guide to
  Internal Models and EBA Guidelines on Internal Governance frame
  the EU-side, with EU AI Act Annex III Credit and Insurance
  categories layered on top for entities in scope.
- The head's placement relative to the CMRO — peer, specialist
  under, or enterprise-wide above the MRM perimeter — is a design
  choice defended to the board; each placement has a supporting
  operating pattern, and the failure mode is any placement where
  the board cannot answer "who is accountable for AI."
- Consumer-facing AI runs into Regulation B / ECOA (CFPB Circulars
  2022-03 and 2023-03), Interagency Fair Lending Statement / OCC
  fair-lending examination procedures, and CFPA UDAAP authority.
  The head owns the AI-specific evidence; the Chief Compliance
  Officer owns the compliance stance.
- The examination cadence at leadership scope is a standing
  evidence pipeline — inventory, validation, monitoring, change
  management, third-party attestation, fair-lending record — that
  is ready for horizontal review, targeted examination, or MRA
  remediation without special preparation.
- The head's board-level story has three beats: AI inside MRM,
  coherent multi-regulator posture, and AI-specific external
  engagements aligned with the board's external-positioning
  ratification. That three-beat rhythm feeds cluster 4 of the
  quarterly board pack in
  [[mod-103-board-and-audit-committee-reporting]] and closes the
  bank-specific dimension of the head's leadership scope.
