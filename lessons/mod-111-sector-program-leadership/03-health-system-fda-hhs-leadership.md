# Health System — Leading AI Governance Across FDA, HHS OCR, State Medical-AI Statutes, and Hospital Accreditors

## Motivation

A hospital, health system, or integrated payer-provider is not
regulated as a technology company. It is regulated as a healthcare
delivery organisation, and its AI systems inherit that regulatory
identity whether or not the AI systems' builders think of it that
way. The FDA supervises Software as a Medical Device (SaMD) —
including AI/ML-enabled SaMD — under the Federal Food, Drug, and
Cosmetic Act. HHS Office for Civil Rights (OCR) supervises PHI
handling under HIPAA and the HITECH Act. State medical boards
supervise medical practice, and state legislatures have begun
regulating specific AI-in-medicine uses (California and Texas are
among the leading examples). The Joint Commission (TJC), DNV
Healthcare, and other accreditation bodies inspect against
accreditation standards that increasingly touch AI-driven clinical
tools. Above the clinical layer sits the enterprise's Chief Medical
Officer (CMO) and the medical staff, whose governance authority over
clinical practice — including AI-augmented clinical practice — is
codified in medical-staff bylaws and, at academic medical centres,
in the affiliation agreement with the school.

The head of AI governance at a health system runs a program that
sits at the intersection of all of that. This chapter is the
leadership map: what each regulator wants, where clinical governance
begins and technology governance ends, and how the head owns AI
policy without owning clinical judgment.

## Core concept — the four-layer supervisory stack for a health-system AI

Every AI system a health system deploys sits inside a stack the head
maps explicitly.

1. **Device layer.** Is the AI system a medical device under 21 USC
   § 321(h)? If yes, FDA regulates it as SaMD (or as a component of a
   traditional device where embedded), and the pre-market and post-
   market obligations attach. If the system is developed in-house by
   the health system for its own use, FDA's enforcement discretion
   for laboratory-developed tests and similar exemptions may apply,
   but the head defends the classification, not the assumption.
2. **PHI layer.** Does the AI system process protected health
   information under HIPAA? Almost every clinical AI does. HHS OCR
   supervises the enterprise as a covered entity or a business
   associate (or both), and the AI system's data flows,
   authorisations, and security controls are inside the HIPAA
   Privacy Rule, Security Rule, and Breach Notification Rule
   perimeter.
3. **Clinical layer.** Is the AI system used in clinical decisioning
   — diagnosis, treatment recommendation, risk stratification,
   patient triage? If yes, it is subject to medical-staff oversight
   through the CMO and, at accredited institutions, to accreditation
   standards on clinical decision support.
4. **State-medical layer.** Does the AI system's use interact with a
   state's medical-AI statute, medical-board rule, or consumer-
   protection statute? California's SB 1120 (Physicians Make
   Decisions Act, 2024), New York's medical-AI provisions, Texas's
   emerging medical-AI legislation, and other state statutes attach
   here.

An AI system may sit inside all four layers simultaneously (an
image-based diagnostic AI operating on radiology PHI under medical-
staff supervision in California is inside all four). Every layer's
regulator is a separate entry in the head's regulator inventory.

## FDA — GMLP and the PCCP submission

### Good Machine Learning Practice guiding principles (October 2021)

FDA, jointly with Health Canada and the UK MHRA, published Good
Machine Learning Practice for Medical Device Development: Guiding
Principles in October 2021. The ten guiding principles frame the
lifecycle expectations for AI/ML-enabled medical device software:
multidisciplinary expertise leveraged throughout the total product
lifecycle, good software engineering practices and security
practices, clinical study participants and data sets representative
of the intended patient population, training data sets independent
of test sets, selected reference standards based on best available
methods, model design tailored to the available data, focus placed
on the performance of the human-AI team, testing demonstrating device
performance during clinically relevant conditions, users provided
clear and essential information, and deployed models monitored for
performance with re-training risks managed. The head reads the ten
principles as the operating framework for FDA-facing AI submissions
and as the language the FDA reviewer will use in the review dialogue.

### Predetermined Change Control Plans (PCCP)

FDA released the draft guidance on Marketing Submission
Recommendations for a Predetermined Change Control Plan for
Artificial Intelligence-Enabled Device Software Functions in April
2023.

<!-- needs-research: verify whether the FDA PCCP guidance for AI/ML-
enabled device software functions has moved from draft to final
status since April 2023, and update citation accordingly. The
guidance-status change is exactly the kind of item the head's
regulatory-change inventory must be current on. Confirm against
fda.gov guidance-documents search. -->

A PCCP is a pre-authorised description of the changes an AI/ML-
enabled device software function may make to itself post-market
without triggering a new marketing submission. The PCCP has three
components: a Description of Modifications (what will change), a
Modification Protocol (how the changes will be developed, verified,
and validated), and an Impact Assessment (what the changes mean for
safety and effectiveness).

The head of AI governance owns the submission-leadership dimension
of PCCP:

1. Deciding which of the enterprise's AI-enabled devices are
   candidates for a PCCP (the answer is "the ones where post-market
   learning is a design intent, not the ones where the model is
   frozen at release").
2. Coordinating with Regulatory Affairs on the PCCP's structure
   and content — Regulatory Affairs fronts the submission channel,
   the head owns the AI-specific technical content that fills the
   modification protocol.
3. Standing behind the PCCP's monitoring commitments post-market.
   The PCCP is a promise to FDA about how the enterprise will
   monitor and control changes; the head signs into the operational
   pipeline that delivers on the promise.

### 510(k), De Novo, PMA — the submission pathway question

Independent of PCCP, every FDA-regulated AI/ML SaMD needs a
submission pathway: 510(k) (substantial equivalence to a predicate),
De Novo (novel low-to-moderate risk device without a predicate), or
PMA (premarket approval, for Class III high-risk devices). The
pathway determines the evidence expectation, the submission timeline,
and the post-market obligations. The head does not choose the
pathway (Regulatory Affairs does, against 21 CFR Part 807 or Part
814 requirements), but the head is the technical author of the AI-
specific dimensions of whichever pathway is chosen.

The FDA's Digital Health Center of Excellence and its Software
Precertification (Pre-Cert) Program work stream inform the FDA's
posture on SaMD submissions. The head follows the Digital Health
Center's public communications, workshops, and pilot outputs the
way a banking head follows Federal Reserve speeches.

### Post-market surveillance — MDR and adverse-event reporting

Post-market, the head owns the AI-specific dimension of the Medical
Device Reporting (MDR) system under 21 CFR Part 803 — the mandatory
reporting of device-related deaths, serious injuries, and
malfunctions. AI-driven false negatives, false positives that led to
harm, and material performance degradations against labelled
indications for use each trigger the MDR analysis. The head does
not decide reportability (Regulatory Affairs does), but the head is
the technical author of the AI-specific dimensions of every MDR
analysis and every reportable event.

## Clinical governance interface with the Chief Medical Officer

FDA regulates the device. The medical staff regulates its use.
Those are two different regulatory regimes, and the head navigates
the boundary between them without either violating clinical
judgment prerogatives or ceding technology governance.

The CMO owns clinical practice. Medical staff bylaws — reviewed at
accredited institutions by the accreditation body — codify who may
order what, whose orders count as clinical decisions, and how new
clinical tools are introduced. An AI clinical decision support (CDS)
system entering the clinical workflow does so through the CMO's
governance channel: typically a medical staff clinical AI committee,
or a subgroup of the existing pharmacy and therapeutics or CDS
committee. The head is a standing member of that committee, but the
head does not chair it. The chair is a clinician, usually the CMIO
(Chief Medical Informatics Officer) or a Vice-Chief-of-Staff for
Informatics.

The head's contribution to the clinical AI committee is:

- The AI system's technical characterisation: what it does, how it
  was developed and validated, what the vendor's evidence looks
  like, what the enterprise's independent evaluation shows.
- The FDA regulatory status: cleared, approved, De Novo-authorised,
  or non-device (the last is common for CDS that meets 21st Century
  Cures Act CDS exemption criteria; the head still evaluates
  whether it qualifies).
- The HIPAA and data-handling posture.
- The proposed monitoring plan post-deployment.
- The escalation path if the AI system produces clinically
  concerning behaviour.

The CMO or the committee decides whether the AI system enters the
clinical workflow, on what indications, with what training
requirements for the clinicians who will use it, and with what
review cadence. The head implements the technology-side controls
the decision requires, but the head does not decide clinical
adoption. That distinction preserves both the CMO's authority and
the head's independence at the technology governance layer.

## HHS OCR — HIPAA breach notification for AI-triggered PHI events

HHS OCR enforces HIPAA and HITECH. Every AI system that processes
PHI is inside the Privacy Rule (45 CFR Part 164 Subpart E), the
Security Rule (Subpart C), and the Breach Notification Rule (Subpart
D). The head owns two AI-specific dimensions of the OCR posture.

First, business-associate agreements with third-party AI vendors.
Every foundation-model API provider, every cloud-hosted ML platform,
every AI-enabled clinical tool vendor whose services process PHI on
the enterprise's behalf is a business associate. The BAA carries
the standard HIPAA-required terms plus AI-specific overlays: what
the vendor may do with the PHI for model training or improvement
(the head's default answer is "nothing"), how the vendor handles
prompt data that may contain PHI, what audit rights the enterprise
retains, what breach-notification terms bind the vendor. Contract
review is Procurement plus General Counsel's function; the head
owns the AI-specific terms.

Second, breach notification for AI-triggered PHI events. A breach
of PHI triggers the 60-day notification obligation under 45 CFR §
164.400 et seq. AI-specific breach patterns include: prompt-injection
attacks that cause an AI system to disclose PHI to unauthorised
third parties, foundation-model provider incidents where the enterprise's
PHI-containing prompts were retained beyond contract, retrieval-
augmented generation systems that surface a patient's PHI to a
user without authorisation, training-data leakage where a fine-tuned
model regurgitates training PHI at inference. Each pattern is
covered by the standard HIPAA breach analysis: was PHI acquired,
accessed, used, or disclosed in a manner not permitted; does the
low-probability-of-compromise analysis under 45 CFR § 164.402(2)
apply; is notification to affected individuals, the Secretary, and
(for breaches of 500 or more individuals) the media required.

The head does not make the breach determination (the HIPAA privacy
officer does, in consultation with General Counsel), but the head
is the technical author of the AI-specific facts the breach
analysis rests on. In a serious AI-triggered PHI event, the head
also stands next to the CIO and CISO in the incident-response tier
(see [[mod-110-incident-leadership]]).

<!-- needs-research: identify current HHS OCR guidance specifically
addressing AI systems processing PHI, including any updates to the
OCR bulletin on online tracking technologies as it applies to AI-
driven analytics, any post-2023 rulemaking on the HIPAA Security
Rule's application to AI, and any resolution agreements with AI-
specific facts. Confirm against hhs.gov/hipaa. -->

## State medical-AI regulation

California SB 1120, the Physicians Make Decisions Act, was signed
in September 2024. It requires health insurers and health plans in
California to ensure that AI, algorithm, or other software tools
used to inform medical necessity decisions are used consistent with
specific requirements — including individualised patient information
review, non-discrimination, and human physician oversight.

California AB 3030 (2024) requires health facilities, clinics,
physician's offices, and group practices that use generative AI to
generate written or verbal patient communications pertaining to
patient clinical information to include specified disclaimers and
directions.

<!-- needs-research: verify effective dates and current implementing
guidance for California SB 1120 and AB 3030; the statutes were
signed in 2024 with staged effective dates through 2025-2026.
Confirm against California Department of Managed Health Care and
California Department of Insurance guidance. -->

New York's medical-AI provisions and Texas's medical-AI provisions
are moving on parallel tracks. Other state legislatures have
introduced medical-AI bills; state medical boards have issued
statements on physician use of AI in clinical practice.

The head maintains a per-state map for state medical-AI statutes
that mirrors the per-state map for state DOI adoption of the NAIC
bulletin in insurance (see chapter 02): where the enterprise
operates, what statute applies, what obligation attaches, and who
inside the enterprise owns each obligation.

## Hospital accreditation — TJC and DNV

The Joint Commission and DNV Healthcare are the two dominant
accreditation bodies for US hospitals. Accreditation is voluntary in
name but functionally required — Medicare and Medicaid
reimbursement conditions on hospital participation typically
reference deemed status under an approved accreditation programme,
and payer contracts frequently require accreditation.

Both accreditors have expanded standards to touch AI-driven
clinical decision support, information management, and patient
safety over the last several years. TJC's standards under the
Information Management (IM), Provision of Care (PC), and Leadership
(LD) chapters, and DNV's standards under similar categories, apply
to how the enterprise governs AI-driven clinical tools, how the
enterprise trains staff on their use, and how the enterprise
monitors for patient-safety implications.

<!-- needs-research: identify the specific TJC and DNV Healthcare
standards that most directly address AI-driven clinical decision
support, including any AI-specific standards added through 2024-
2026. TJC has been publishing on AI governance; confirm current
standard citations against jointcommission.org. -->

The head coordinates with the enterprise's accreditation-readiness
lead (typically inside the CMO or CNO office) on the AI-specific
evidence that supports the accreditation survey, and stands in the
survey when AI-specific standards are examined.

## The head's board-level story at a health system

At a health-system board — usually a governing board with a Quality
Committee and either a separate Audit Committee or a combined
Quality-and-Compliance Committee — the AI governance story has
three beats.

1. Every AI system in clinical use has a defensible regulatory
   status (FDA classification, PCCP if applicable, CDS-exemption
   analysis where it applies) and a defensible clinical-governance
   status (medical-staff committee review, approval, monitoring,
   escalation path). The board can inspect the register.
2. The HIPAA posture across the AI portfolio is coherent — BAAs are
   in place with AI vendors on terms that reflect AI-specific
   risks, breach-response readiness is tested, and any AI-triggered
   PHI event has been reported through the standard HIPAA process.
3. The state-medical-AI compliance posture (California SB 1120 and
   AB 3030 where applicable, other states as their statutes come
   into force, medical-board expectations in states where the board
   has published guidance) is coherent, and the accreditation
   posture (TJC or DNV standards touching AI, next survey window)
   is on track.

## Summary

- A health-system AI sits inside a four-layer stack: device
  (FDA / SaMD), PHI (HIPAA / HHS OCR), clinical (CMO and medical
  staff governance), and state-medical (state statutes and medical-
  board rules). The head maps every AI system in the inventory
  against the four layers explicitly.
- FDA regulates the device: GMLP guiding principles (October 2021,
  joint with Health Canada and MHRA), PCCP guidance (draft April
  2023, status to verify), 510(k) / De Novo / PMA submission
  pathways, and post-market MDR obligations. The head is the
  technical author; Regulatory Affairs fronts the channel.
- Clinical governance sits with the CMO and the medical staff,
  typically through a clinical AI committee chaired by a clinician
  (often the CMIO). The head is a standing member and contributes
  technical characterisation, regulatory status, HIPAA posture,
  monitoring plan, and escalation path — but does not decide
  clinical adoption.
- HHS OCR enforces HIPAA. Every AI system processing PHI is in the
  Privacy, Security, and Breach Notification Rule perimeter. The
  head owns AI-specific business-associate agreement terms and the
  technical facts underlying breach-notification analysis for AI-
  triggered PHI events.
- State medical-AI statutes — California SB 1120 (Physicians Make
  Decisions Act, September 2024) and California AB 3030 (2024) are
  leading examples — are mapped per state. Hospital accreditors
  (TJC, DNV Healthcare) inspect AI-related standards under
  Information Management, Provision of Care, and Leadership
  categories.
- The board-level story has three beats: defensible regulatory
  and clinical-governance status per AI system; coherent HIPAA
  posture with AI-appropriate BAA terms; coherent state-medical-AI
  and accreditation posture. That story feeds cluster 4 of the
  quarterly board pack in [[mod-103-board-and-audit-committee-reporting]],
  with the Quality Committee also receiving the clinical-governance
  dimensions in its own cluster.
