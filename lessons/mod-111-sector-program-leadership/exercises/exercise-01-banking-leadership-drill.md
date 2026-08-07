# exercise-01: Banking Leadership Drill

**Estimated effort:** 4 hours

## Objective

Instantiate the banking-sector leadership shape from chapter 01
against a specific hypothetical (or real, if the exercise is being
worked in-role) bank. The deliverable is the head of AI governance's
operating package for a bank: an AI-inside-MRM control alignment,
a US federal + international overlay statement, a consumer-facing
AI evidence pack, a placement rationale versus the Chief Model
Risk Officer, and a board-level three-beat story.

The deliverable is not a survey of banking AI regulation. It is
the artefact the head signs into on day one, defends at the audit
committee on quarter one, and hands to a successor on quarter
eight.

## Prerequisites

- Chapter [01-banking-mrm-leadership](../01-banking-mrm-leadership.md)
  — read and internalised.
- Chapter 04 of [[mod-104-regulator-engagement]] — the four-part
  sector-regulator engagement pattern the artefacts extend.
- Chapter 04 of [[mod-102-running-the-program]] on running-program
  evidence pipelines the AI-inside-MRM alignment consumes.
- [[mod-103-board-and-audit-committee-reporting]] cluster 4 shape
  the board-level story feeds.
- A specific bank scenario. Options: a US-only regional bank; a
  US-plus-Canada bank with OSFI E-23 exposure; a US-plus-UK bank
  with PRA SS1/23 exposure; a global bank with SSM exposure via
  ECB and EBA. Where any element is hypothetical, hold a working
  assumption and note it.

## Steps

1. **Bank profile one-pager.** Half-page scoping the exercise:
   asset size band, jurisdictional footprint (US federal
   regulators the bank answers to — Federal Reserve, OCC, FDIC;
   Canadian OSFI exposure; UK PRA exposure; EU SSM exposure),
   consumer-facing footprint (retail deposits, credit products,
   wealth management), AI portfolio scale (order-of-magnitude
   count of AI models in production, plus foundation-model
   dependencies), and current placement of the head of AI
   governance in the org (peer of CMRO, specialist under CMRO,
   or enterprise-wide above MRM). The scoping is the scenario
   every subsequent artefact refers to.

2. **AI-inside-MRM control alignment.** For every AI system in
   the scenario's inventory, map to the four SR 11-7 functional
   areas — Development and Implementation, Use, Validation,
   Governance — with the concrete artefact per area. Where an AI
   system does not fit an area (e.g., a foundation-model-based
   productivity assistant that produces no acted-upon
   quantitative estimate), record the exclusion analysis
   defending the treatment. Cite SR 11-7, OCC Bulletin 2011-12,
   and the OCC Comptroller's Handbook MRM booklet at the
   relevant control anchor.

3. **Third-party AI attestation trail.** For every third-party
   AI dependency in the scenario (foundation-model APIs, managed
   ML platforms, model-derived data feeds), map to the SR 23-4
   lifecycle stages — planning, due diligence and third-party
   selection, contract negotiation, ongoing monitoring, and
   termination. Named third-party AI providers get concrete
   entries; unnamed placeholders are called out as
   placeholders. Concentration analysis on the enterprise's
   top-3 foundation-model providers is included.

4. **International overlay statement.** Where the scenario
   includes Canadian, UK, or EU exposure, state the OSFI E-23,
   PRA SS1/23, ECB Guide to Internal Models, and EBA
   GL/2021/05 obligations that apply, and map to the AI-inside-
   MRM controls that satisfy each. Where the EU AI Act's Annex
   III credit-scoring provisions apply, name them.

5. **Consumer-facing AI fair-lending pack.** For any credit-
   decisioning AI in the scenario, produce the Regulation B / ECOA
   evidence pack: adverse-action reason-code generation at
   model-development time, disparate-impact testing methodology,
   less-discriminatory alternative analysis, feature-selection
   and proxy-elimination documentation, and CFPB Circular 2022-03
   / 2023-03 alignment. For any consumer-interaction AI
   (chatbot, robo-advisor, personalised offer engine), produce
   the UDAAP evidence pack: fairness, disclosure, human-
   escalation path.

6. **Placement rationale for the head vs the CMRO.** Author the
   three-way placement analysis (peer, specialist under,
   enterprise-wide above MRM perimeter) against the scenario's
   specifics. Recommend a placement, defend the recommendation
   in a page, and specify the joint operating protocol between
   the head and the CMRO the recommended placement requires.

7. **Examination-readiness evidence pipeline map.** Name the
   pipeline that produces, on a rolling basis, the six evidence
   streams from chapter 01: current model inventory with AI
   tags, current validation status, current monitoring signal,
   current change-management record, current third-party AI
   attestation trail, and current fair-lending evidence for
   consumer-facing AI. Per stream, name the owner and the
   refresh cadence.

8. **Board-level three-beat story.** Author the audit-committee
   quarterly narrative in the three-beat structure from chapter 01:
   AI inside MRM; multi-regulator posture coherent; AI-specific
   external engagements aligned to ratified external-positioning
   posture. The narrative is drop-in ready for cluster 4 of the
   board pack in [[mod-103-board-and-audit-committee-reporting]].

## Deliverables

- `bank-profile.md` — the one-page scenario scoping.
- `ai-inside-mrm-alignment.md` — the AI-to-SR-11-7 mapping, one
  entry per AI system with concrete artefacts named per SR 11-7
  functional area.
- `third-party-ai-attestation.md` — the SR 23-4 lifecycle mapping
  per named third-party AI provider, plus concentration
  analysis.
- `international-overlay.md` — the OSFI E-23 / PRA SS1/23 / ECB /
  EBA overlay statement as applicable.
- `fair-lending-and-udaap-pack.md` — the Regulation B / UDAAP
  evidence pack for consumer-facing AI.
- `placement-rationale.md` — the head-vs-CMRO placement analysis
  and joint operating protocol.
- `examination-readiness-pipeline.md` — the standing evidence
  pipeline map.
- `board-three-beat-story.md` — the audit-committee narrative.

## Acceptance criteria

- Every AI system in the scenario inventory has a defensible
  treatment under SR 11-7 — either mapped into a functional area
  or excluded with reasoning.
- Every third-party AI provider has a concrete SR 23-4 lifecycle
  status. Placeholder "vendor TBD" entries are called out
  explicitly; the exercise does not accept unspecified
  dependencies.
- Where international overlays apply, they cite the specific
  instrument (OSFI E-23, PRA SS1/23 by number, ECB Guide to
  Internal Models, EBA/GL/2021/05).
- Consumer-facing AI evidence packs cite the specific CFPB
  circular (2022-03, 2023-03) and the specific Regulation B
  provisions attaching.
- The placement rationale names the specific enterprise geography
  it responds to and specifies the joint operating protocol,
  not merely the placement letter.
- The examination-readiness pipeline names owners and cadences,
  not generic "TBD."
- The board-level three-beat story is drop-in ready — a director
  can read it without asking a follow-up question.
- Where an instrument's status is uncertain (interagency GenAI
  Q&A; current Fed / OCC positioning on foundation-model
  treatment), a `<!-- needs-research: ... -->` flag is recorded
  rather than a guess.

## Stretch goals

- Add a rate-of-change dimension: what would the artefact change
  if the enterprise moved from Placement A (peer of CMRO) to
  Placement B (specialist under CMRO), or if a US-only bank
  acquired a UK subsidiary bringing SS1/23 into scope. The
  head's own succession planning depends on knowing which
  artefacts are placement-sensitive and which are placement-
  invariant.
- Author the MRA-response pre-decision: what is the head's
  posture if the next examination cycle produces an AI-scope
  Matter Requiring Attention on validation independence,
  monitoring adequacy, or third-party AI oversight? Pre-decide
  before the pressure arrives.
- Circulate the placement rationale and the joint operating
  protocol to a peer at CMRO level (real or role-played) and
  incorporate one round of critique.

## Notes and starter guidance

- The most common failure mode is running an AI framework
  outside the MRM perimeter. Every draft that positions AI
  governance as a parallel discipline to MRM fails the exercise.
  If the enterprise's actual org has AI positioned separately,
  the exercise's job is to design the AI-to-MRM interface, not
  to defend the separation.
- The SR 23-4 lifecycle mapping is the exercise's single most
  overlooked area. Third-party AI is where the current
  supervisory attention lives; a bank with a defensible SR 11-7
  package and a weak SR 23-4 package will attract MRA activity
  on the third-party side.
- The placement recommendation depends on the enterprise. There
  is no globally correct answer. The exercise tests whether the
  reasoning is complete, whether the joint operating protocol
  survives personnel change, and whether the board could ratify
  the choice.
- The examination-readiness pipeline is not the artefact you
  build for an announced examination. It is the artefact that
  is running before any announcement. If the pipeline requires
  announcement-triggered work, redesign it.
- The board three-beat story is a narrative artefact. Practise
  writing it in prose the audit committee reads in three to five
  minutes. Length is not the goal; density and directness are.
