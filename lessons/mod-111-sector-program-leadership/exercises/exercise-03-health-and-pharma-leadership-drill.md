# exercise-03: Health and Pharma Leadership Drill

**Estimated effort:** 5 hours

## Objective

Instantiate the health-system and pharmaceutical leadership shapes
from chapters 03 and 04 against either a health-system scenario, a
pharmaceutical-company scenario, or a combined integrated-health-
enterprise scenario. The deliverable is the head's operating
package: for a health system, the four-layer stack (device / PHI /
clinical / state-medical), the clinical-governance committee
interface, the HIPAA / BAA discipline, and the accreditation-
readiness posture; for a pharma company, the FDA / EMA / MHRA /
PMDA regulatory-submission overlay, the GxP interface, the
pharmacovigilance-AI validation, and the inspection-readiness
posture; for a combined enterprise, both.

The exercise is longer than most because health and pharma are
covered by two chapters and the operating packages are
substantively different. Working both in one pass builds the
skill of running an integrated-health-enterprise governance program.

## Prerequisites

- Chapter [03-health-system-fda-hhs-leadership](../03-health-system-fda-hhs-leadership.md)
  and chapter [04-pharmaceutical-fda-mhra-ema-pmda-leadership](../04-pharmaceutical-fda-mhra-ema-pmda-leadership.md)
  — both read and internalised.
- Chapter 04 of [[mod-104-regulator-engagement]] — the sector-
  regulator engagement pattern.
- [[mod-110-incident-leadership]] chapter on health-incident
  handling (HIPAA breach; adverse-event MDR; pharmacovigilance
  ICSR) — the AI-triggered incident dimension of both scenarios.
- [[mod-103-board-and-audit-committee-reporting]] cluster 4 and
  the Quality Committee cluster (health system) or R&D / Science
  and Technology Committee cluster (pharma).
- A specific scenario. Options:
  - **Health system.** Integrated health system with a research
    arm and an owned health plan; 200-hospital chain; regional
    health system with a device-development spinout.
  - **Pharma.** Top-20 originator with AI in early discovery,
    trials, PV, and manufacturing; biotech with AI-driven trial
    design; pharma with a companion-diagnostic device pipeline.
  - **Combined integrated-health-enterprise.** A health system
    that has invested in developing regulated devices, or a
    pharma with a healthcare-delivery affiliate.

## Steps

### Health-system track (if scenario applies)

1. **Health-system profile one-pager.** Half-page scoping: system
   size, jurisdictional footprint (states of operation), payer
   affiliations, research posture, device-development posture,
   and existing clinical-governance structure (Chief Medical
   Officer, Chief Medical Informatics Officer, medical staff
   committee structure).

2. **Four-layer stack per AI system.** For every clinical AI in
   the inventory, map to the four layers from chapter 03:
   device (FDA classification analysis; SaMD / non-device;
   CDS-exemption if applicable), PHI (HIPAA
   applicability, BAA scope, breach-notification posture),
   clinical (medical-staff committee review and approval
   status), state-medical (per state — California SB 1120 and
   AB 3030 fit if operating in California; other state statutes
   as applicable).

3. **Clinical-governance committee interface.** Author the
   operating agreement between the head and the clinical AI
   committee (chaired by the CMIO or a Vice-Chief-of-Staff for
   Informatics). Specify what the head brings to committee
   (technical characterisation; regulatory status; HIPAA posture;
   monitoring plan; escalation path), what the committee
   decides, and how disagreements are resolved.

4. **HIPAA and BAA discipline.** Author the BAA-terms standard for
   third-party AI vendors that process PHI: model-training
   restrictions, prompt-data handling, audit rights, breach
   notification terms. Include the AI-specific breach-notification
   pattern analysis — prompt-injection, foundation-model
   provider incidents, RAG-system PHI leakage, training-data
   regurgitation — with the response readiness per pattern.

5. **Accreditation-readiness posture.** For the enterprise's
   accreditation body (TJC, DNV, or equivalent), map the AI
   portfolio to the applicable accreditation standards. Where
   the next survey window is known, name the AI-specific
   evidence the survey team will inspect.

6. **Health-system board narrative.** Author the Quality
   Committee and Audit Committee slices per chapter 03.

### Pharma track (if scenario applies)

1. **Pharma profile one-pager.** Half-page scoping: therapeutic
   areas, geographic marketing-authorisation footprint (FDA,
   EMA, MHRA, PMDA, Health Canada, and others), pipeline stage
   distribution, manufacturing footprint, and existing
   Regulatory Affairs / Quality structure.

2. **Regulatory-submission AI overlay.** For each in-flight or
   planned regulatory submission (IND / IMPD / CTA and NDA / BLA
   / MAA), name every AI system material to the submission and
   author the AI-specific documentation the submission carries.
   Cite FDA CDER's January 2025 draft guidance framework
   (verified for current status), EMA's September 2024
   reflection paper, and MHRA's positioning. Where scientific
   advice engagements have aligned expectations, document them.

3. **Pharmacovigilance AI validation.** For each AI system in
   the PV pipeline (case processing, signal detection, NLP over
   literature or real-world data), author the validation
   package the QPPV can rely on: validation methodology,
   independence-of-test-data-from-training-data record, ongoing
   monitoring, and audit-trail for regulator inspection.

4. **GMP-regulated manufacturing AI.** For each AI system in
   GMP-regulated manufacturing, author the CSV / CSA treatment
   per GAMP 5 Second Edition, the ALCOA+ data-integrity
   attestation, 21 CFR Part 11 compliance, and change-control
   integration with the site QMS.

5. **Inspector-engagement stance.** For each site subject to
   FDA, EMA, MHRA, or PMDA inspection, name the AI-specific
   inspection response preparation: pre-inspection review, host-
   function briefing, standing-by protocol, and post-inspection
   observation response.

6. **Three-function operating protocol — Regulatory Affairs,
   Quality, head of AI governance.** Author the written protocol
   naming who owns what at each regulated event; signature by
   all three.

7. **Pharma board narrative.** Author the Audit Committee slice
   and the R&D / Science and Technology Committee slice per
   chapter 04.

### Combined-enterprise integration (if scenario applies)

If the scenario is a combined integrated-health-enterprise, add:

- A cross-track coordination protocol naming how the health-
  system CMO and pharma Chief Medical Officer (or Chief
  Scientific Officer) interact where the enterprise both
  develops a device and operates the clinical setting the
  device is used in.
- A group-level board narrative that reconciles the health-
  system Quality Committee content and the pharma R&D
  Committee content into a coherent group Audit Committee view.

## Deliverables

### Health-system track

- `health-system-profile.md`
- `four-layer-stack.md` (or `.csv`) — one row per AI system with
  the four layers filled in.
- `clinical-committee-interface.md` — the operating agreement.
- `hipaa-baa-discipline.md` — the BAA-terms standard plus AI-
  triggered breach pattern analysis.
- `accreditation-readiness.md` — the accreditation-standards
  map.
- `board-narrative-quality-audit.md` — the Quality Committee
  and Audit Committee narratives.

### Pharma track

- `pharma-profile.md`
- `regulatory-submission-overlay.md` — the AI-specific overlay
  per in-flight / planned submission.
- `pv-ai-validation-package.md` — the PV AI validation
  packages, one per PV AI system.
- `gmp-manufacturing-ai-package.md` — the CSV / CSA / ALCOA+ /
  Part 11 / change-control package per manufacturing AI.
- `inspector-engagement-plan.md`
- `three-function-protocol.md` — RA / Quality / head.
- `board-narrative-audit-rnd.md` — the Audit and R&D committee
  narratives.

### Combined-enterprise integration (if applicable)

- `combined-enterprise-coordination-protocol.md`
- `group-board-narrative.md`

## Acceptance criteria

### Common

- Every AI system in scope has a defensible regulatory-status
  characterisation with the specific instrument cited (FDA
  GMLP; PCCP guidance; CDER draft; EMA reflection paper; MHRA;
  PMDA; state medical-AI statute; HIPAA rule and subsection).
- The board narratives are drop-in ready to the relevant
  committee's cluster.
- Uncertain instrument status (PCCP guidance draft-vs-final;
  CDER guidance final status; California SB 1120 / AB 3030
  effective dates; other state medical-AI statute status;
  current PMDA / MHLW positioning; TJC / DNV AI-specific
  standards) carries a `<!-- needs-research: -->` flag rather
  than a guess.

### Health-system track

- The four-layer stack is complete: every clinical AI has an
  entry in each of the four layers with concrete detail, not a
  category label.
- The clinical-committee interface names the committee chair
  (function, not name if hypothetical) and the head's standing-
  member role.
- The HIPAA / BAA discipline includes AI-specific vendor terms
  (training-data restriction, prompt-data handling, audit
  rights) and an AI-triggered breach pattern analysis.
- The accreditation-readiness posture identifies the applicable
  accreditor and the standards touching AI.

### Pharma track

- The regulatory-submission AI overlay is per submission and per
  regulator, not aggregated.
- The PV AI validation is per PV AI system, not one blanket
  document.
- The GMP AI package cites GAMP 5 Second Edition, ALCOA+, 21 CFR
  Part 11, and the site's QMS change control.
- The three-function protocol is signed by Regulatory Affairs,
  Quality, and the head, and ratified at the audit-committee
  tier.

## Stretch goals

- **Health system.** Add an AI-triggered PHI breach response
  walk-through: prompt-injection incident, foundation-model
  provider incident, or RAG PHI leakage. Author the breach-
  analysis walk-through against 45 CFR § 164.402 (breach
  definition), § 164.404 (individual notification), § 164.406
  (media notification for 500+), § 164.408 (Secretary
  notification). Coordinate with the [[mod-110-incident-leadership]]
  chapter on the incident-leadership dimensions.
- **Pharma.** Add a scientific-advice engagement walk-through:
  the enterprise seeks FDA Type C alignment on AI in trial-
  design and then EMA scientific advice on the same package.
  Author the briefing materials the head prepares for
  Regulatory Affairs to present, plus the cross-regulator
  alignment analysis.
- **Combined enterprise.** Rehearse the FDA / EMA inspection
  where the same AI system is used in the pharma's manufacturing
  and the health system's clinical operations. Who fronts, who
  is copied, and how does the enterprise avoid a split answer
  at inspection?

## Notes and starter guidance

- The four-layer stack in health-system work is the single most
  important discipline; without it, the head is answering to
  one regulator at a time rather than to the four the AI system
  actually attaches to.
- The clinical AI committee interface is a peer-fronting
  discipline. The head does not chair the committee; the head
  contributes technical substance and is a standing member.
  Designs that put the head in the chair usually fail on the
  medical-staff-authority axis.
- In pharma, the head is never the person who submits, never
  the person who inspects with, and never the person who
  signs the QP release. The head produces AI-specific technical
  content that Regulatory Affairs, Quality, and the QP rely on.
  A pharma-track design that puts the head in front-line
  regulator-facing positions on non-AI regulated events fails
  the exercise.
- The three-function protocol in pharma prevents split answers
  at inspection. The three-function protocol in the health
  system does the same at accreditation survey. Both are
  necessary; neither is optional.
- Uncertain regulator status is a live issue in both sectors.
  The FDA CDER guidance progression, the EMA reflection paper's
  follow-on, the PMDA / MHLW positioning, the state medical-AI
  statute effective dates, and the accreditor AI-standard
  updates all move on cycles inside the working horizon. The
  exercise expects `<!-- needs-research: -->` flags, not
  guesses.
