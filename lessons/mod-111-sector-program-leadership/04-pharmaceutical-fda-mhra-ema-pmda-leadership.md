# Pharmaceutical — Leading AI Governance Across FDA, MHRA, EMA, PMDA, and the GxP Interface

## Motivation

A pharmaceutical company answers to more national regulators than
almost any other kind of enterprise. A drug marketed in the US, the
UK, the EU, Japan, Canada, and a set of major emerging markets is
reviewed by FDA, MHRA, EMA (working with the national competent
authorities in the EU member states plus the European Commission),
PMDA (working with Japan's Ministry of Health, Labour and Welfare),
Health Canada, and each additional market's regulator, on
overlapping but non-identical timelines. AI systems used in drug
development, clinical trials, pharmacovigilance, and manufacturing
enter each regulator's review at whichever submission or inspection
touchpoint the AI system attaches to. GxP obligations — Good
Laboratory Practice, Good Clinical Practice, Good Manufacturing
Practice, Good Pharmacovigilance Practice, Good Distribution
Practice — carry regulatory expectations that predate AI by
decades and now apply to AI systems used in each domain.

The head of AI governance at a pharmaceutical company does not run
a regulator engagement program organised around AI. The head runs
an AI-specific overlay on the pharma regulatory-submission and GxP
lifecycle that the enterprise's Regulatory Affairs and Quality
functions already operate. The chapter maps how the overlay works,
where the head's leadership is decisive, and how the head
coordinates submission cadence across the four principal regulators
without becoming the person who submits.

## Core concept — AI attaches to the regulatory event, not to a standalone regime

Pharma AI regulation is not (yet) a body of AI-specific statute. It
is a set of regulator statements — draft guidance documents,
reflection papers, discussion papers, and inspection Q&A — that
attach to the enterprise's use of AI at specific regulated events:
an IND filing, an NDA or BLA submission, an inspection, an aggregate
safety report, a marketing-authorisation variation, a manufacturing
change. The head reads AI regulation in pharma through the lens of
the events, not through a taxonomy of AI systems.

The current landscape has four principal regulator-issued
instruments framing that lens.

### FDA — AI in drug development (May 2023 discussion paper and January 2025 draft guidance)

FDA CDER and CBER jointly issued the discussion paper Using
Artificial Intelligence and Machine Learning in the Development of
Drug and Biological Products in May 2023. The paper opened public
dialogue on FDA's framing of AI/ML across the drug development
lifecycle: drug discovery, non-clinical research, clinical research,
manufacturing, and postmarketing safety surveillance.

FDA CDER issued the draft guidance Considerations for the Use of
Artificial Intelligence to Support Regulatory Decision-Making for
Drug and Biological Products in January 2025. The draft guidance
introduces a risk-based framework — model influence, decision
consequence — that FDA uses to calibrate the level of evidence it
expects on an AI model used in a regulatory submission.

<!-- needs-research: verify current status of FDA CDER's January
2025 draft guidance Considerations for the Use of Artificial
Intelligence to Support Regulatory Decision-Making for Drug and
Biological Products; the guidance may have moved from draft to
final since publication. Confirm against fda.gov guidance-documents
search. -->

FDA CDER's Office of Study Integrity and Surveillance and the
Bioresearch Monitoring (BIMO) programme have inspection authority
over AI systems used in GCP-regulated clinical research. The head
reads FDA's inspection posture as expecting the AI system's
development, validation, and use to be traceable to source data on
demand.

### EMA — Reflection paper (September 2024)

EMA published the Reflection Paper on the Use of Artificial
Intelligence in the Medicinal Product Lifecycle in September 2024
after a 2023 public consultation on the draft. The reflection paper
sets EMA's framing of AI in drug discovery, non-clinical
development, clinical trials, precision medicine, product
information, manufacturing, and post-authorisation activities.

The reflection paper does not create binding obligations. It
communicates EMA's expectations to marketing-authorisation
applicants and existing marketing-authorisation holders, and
signals the CHMP's readiness to raise AI-specific questions in
scientific advice, in marketing-authorisation review, and in post-
authorisation inspection.

<!-- needs-research: verify EMA reflection paper publication date
(September 2024 based on public record) and any subsequent
consultation outputs, follow-on guidance, or CHMP scientific advice
outputs that extend the reflection paper. Confirm against ema.europa.eu. -->

### MHRA — AI as a Medical Device programme and the AI in Medicines regulatory sandbox (AI-Airlock)

MHRA operates the Software and AI as a Medical Device change
programme (formally launched 2021) and the AI-Airlock, a regulatory
sandbox for AI as a Medical Device. Where the enterprise develops
a device-adjacent AI product (a companion diagnostic, a decision-
support tool paired with a medicinal product), the MHRA device path
and the medicinal product path intersect. The head coordinates with
Regulatory Affairs on both paths.

For medicinal products, the MHRA follows the EMA reflection paper
framework post-Brexit while retaining independent supervisory
authority. MHRA has issued statements on the use of AI in clinical
trial applications and in pharmacovigilance.

<!-- needs-research: verify MHRA AI-Airlock current status and any
published sandbox outputs or lessons-learned reports that inform
the head's engagement posture. Confirm against gov.uk/mhra. -->

### PMDA — evolving guidance and the Sakigake designation environment

Japan's Pharmaceuticals and Medical Devices Agency operates its own
review timelines and Sakigake designation environment for
innovative products. PMDA has issued guidance on AI-driven medical
device software and is developing its posture on AI in drug
development. Japanese Ministry of Health, Labour and Welfare
communications on AI in healthcare set the policy context PMDA
operates within.

<!-- needs-research: identify current PMDA and MHLW guidance
specifically addressing AI in drug development, drug submission,
and pharmacovigilance. PMDA has published on AI-enabled medical
devices; identify AI-specific guidance touching medicinal products.
Confirm against pmda.go.jp. -->

## Regulatory-submission leadership on AI-enabled clinical trials

The head's submission-leadership work is concentrated at the trial-
design stage and at the submission-authoring stage.

### Trial-design stage

Where the enterprise uses AI in trial design — patient identification
and stratification, synthetic control arms, endpoint prediction,
adaptive trial designs driven by AI/ML, digital biomarkers derived
from AI models on wearable data — the trial protocol carries AI-
specific documentation. Regulator scientific advice (FDA Type C
meetings, EMA scientific advice, MHRA scientific advice) is the
preferred vehicle to align regulator expectations before the
protocol is finalised.

The head does not chair scientific advice engagements (Regulatory
Affairs does, working with Clinical Development). The head prepares
the AI-specific technical briefing materials that Regulatory
Affairs presents.

### Submission-authoring stage

The IND / IMPD / Clinical Trial Application submission carries the
AI-specific documentation the trial-design agreement requires.
Every AI system material to the trial's conduct or the trial's
interpretation appears in the submission with:

- A description of the AI system's purpose in the trial.
- The AI system's development and validation record.
- The data provenance and governance record.
- The independence of test data from training data (a GMLP
  principle FDA and MHRA share).
- The change-control approach across the trial's duration.
- The plan for handling AI-system failure modes and the
  contingency if the AI system is withdrawn mid-trial.

At the marketing-authorisation submission (NDA, BLA, MAA), the AI-
specific documentation is refreshed to reflect the final AI system
version used in the pivotal evidence, and any AI system that will be
used post-authorisation (in labelling, in dosing algorithms, in
post-market pharmacovigilance) is documented in the appropriate
Common Technical Document (CTD) module.

## Pharmacovigilance and AI

Good Pharmacovigilance Practice under EU Regulation 726/2004 and
FDA post-market safety surveillance under 21 CFR 314.80 both require
the enterprise to collect, evaluate, and report adverse events. AI
systems increasingly participate in that pipeline: automated
adverse-event case processing, signal detection algorithms on
adverse-event databases, natural-language processing over medical
literature and social media, and predictive models on real-world
data for signal validation.

The head's leadership on PV AI is threefold.

1. Every AI system in the PV pipeline is validated to a standard
   the qualified person for pharmacovigilance (QPPV) can rely on.
   The QPPV signs pharmacovigilance master files and periodic
   safety update reports; the head does not, but the head is
   accountable that AI-produced content in the PV pipeline meets
   the reliability standard.
2. AI-driven signal detection and validation is defensible against
   the CIOMS Working Group VIII methodological standards on
   signal management and the ICH E2E post-approval safety data
   management principles. The head coordinates with the PV function
   on the methodology and the audit trail.
3. Any AI system that touches individual case safety reporting
   (ICSR) is validated and monitored against regulator-specific
   ICSR requirements (FAERS, EudraVigilance, Vigibase). The head
   coordinates with PV IT on the technical dimensions and with
   Regulatory Affairs on inspection readiness.

<!-- needs-research: verify current CIOMS Working Group outputs on
AI in pharmacovigilance and any AI-specific updates to ICH E2E, E2F,
or E2D that the head's PV posture needs to reflect. Confirm against
cioms.ch and ich.org. -->

## AI in GMP-regulated manufacturing

AI systems in pharmaceutical manufacturing — process control,
predictive maintenance, batch-release decisioning, quality-
inspection computer vision — attach to Good Manufacturing Practice
regulation. FDA under 21 CFR Parts 210, 211, 600, and 610; EMA
under EudraLex Volume 4; MHRA and PMDA under aligned national
frameworks; ICH Q7 through Q13 as the international harmonisation
layer.

The head coordinates with the Quality function on:

1. Computer System Validation (CSV) or Computer Software Assurance
   (CSA) treatment of the AI system, aligned to GAMP 5 Second
   Edition as the industry practice reference.
2. Data integrity per ALCOA+ principles and 21 CFR Part 11
   compliance for electronic records and electronic signatures.
3. Change control under the site's quality management system for
   AI-model updates, retraining events, and rollout of new
   versions.
4. Inspection readiness for FDA, EMA, MHRA, and PMDA GMP
   inspections that examine the AI system's role in the process.

The head does not own GMP compliance (the Quality function and the
Qualified Person, in the EU sense, do). The head owns the AI-
specific dimensions the QP and the head of Quality rely on when
they certify batches or defend the process at inspection.

<!-- needs-research: verify current GAMP 5 Second Edition status and
any ISPE Guide updates specifically addressing AI/ML validation.
Confirm against ispe.org. -->

## Inspector engagement

Regulatory inspectors from FDA (through OMPT and OII), EMA (through
national competent authorities), MHRA (through its inspectorate),
and PMDA arrive on inspection cycles that predate any AI-specific
consideration. The head does not front inspections; the site head,
the Quality function, the QP, or the QPPV does, depending on the
inspection type (GCP, GLP, GMP, GVP, GDP).

The head prepares the AI-specific inspection response the way the
head prepares FDA submissions: pre-inspection review of AI systems
in scope, briefing to the inspection-hosting function on the AI
system's technical dimensions, standing-by during the inspection to
answer AI-specific technical questions if invited, and post-
inspection review of any AI-specific inspectional observation (Form
FDA 483 item, EU inspection deficiency, MHRA inspection
observation). Where an inspection triggers a warning letter (FDA)
or a Statement of Non-Compliance (EU), the head is inside the
response team.

## Regulatory-submission cadence coordination

The head coordinates AI-specific submission content across the
four regulators without owning the submissions themselves. The
coordination discipline is:

1. A single AI-specific documentation package is authored to the
   most stringent regulator's expectations, and the same package is
   used across all regulators, with regulator-specific formatting
   handled by Regulatory Affairs. Authoring divergent AI-specific
   content per regulator invites divergent regulator questions and
   compounds review load.
2. Scientific advice engagements across FDA, EMA, MHRA, and PMDA
   are sequenced so that later engagements build on earlier
   ones. Where an FDA Type C meeting has produced alignment on an
   AI-specific point, the EMA scientific advice submission
   references the FDA alignment; where a divergence emerges, the
   head is inside the divergence-resolution.
3. The submission cadence — expected filing dates, expected first
   response, expected marketing authorisation — is on a shared
   view across Regulatory Affairs, the head, and Clinical
   Development. Any AI-specific update to the submission package
   between filings across regulators (an updated model version, an
   updated validation, an updated post-market plan) is versioned
   and reflected across all in-flight submissions.

## The head's relationship with Regulatory Affairs and Quality

At a pharma company, Regulatory Affairs and Quality are the two
functions the head must operate through. Regulatory Affairs owns
submissions and regulator relationships; Quality owns GMP,
inspections, and the batch record. Neither is the head's function.

The head reports either to the Chief Medical Officer, the Chief
Scientific Officer, the Chief Compliance Officer, or (in some
enterprises) the Chief Digital / Data Officer. The head does not
report to Regulatory Affairs — the head's independence from the
submission-authoring function is a governance value the enterprise
protects.

The three-function operating protocol — Regulatory Affairs, Quality,
head of AI governance — is written down and ratified. It names
which function owns what at each regulated event, how AI-specific
content flows between them, how disagreements are resolved, and how
the three collectively defend the enterprise's AI use at
inspection.

## The head's board-level story at a pharma company

At the board — usually a Board of Directors with an Audit Committee
and either a separate R&D Committee or a Science and Technology
Committee — the AI governance story has three beats.

1. Every AI system used in a regulated context has a defensible
   regulatory-status characterisation against the FDA CDER draft
   guidance framework, the EMA reflection paper framework, the
   MHRA framework, and the PMDA framework. Where scientific advice
   has aligned expectations with regulators, the alignment is
   documented.
2. GxP-regulated AI systems are validated and controlled to the
   applicable GxP standard, and inspection readiness is current
   across FDA, EMA, MHRA, and PMDA sites.
3. Pharmacovigilance AI is defensible against ICH and CIOMS
   standards; PV master file references AI-driven components
   accurately; QPPV can rely on AI-produced signals and cases.

That story feeds the Audit Committee cluster 4 (regulator
engagement) and the R&D or Science and Technology Committee's own
oversight of AI in drug development.

## Summary

- Pharma AI attaches to regulated events — IND filings, marketing-
  authorisation submissions, GxP inspections, aggregate safety
  reports, manufacturing changes — rather than to a standalone AI
  regime. The head runs an AI-specific overlay on the pharma
  regulatory-submission and GxP lifecycle.
- The four principal regulator instruments framing the current
  landscape are FDA CDER's May 2023 discussion paper and January
  2025 draft guidance on AI in regulatory decision-making, EMA's
  September 2024 reflection paper, MHRA's Software and AI as a
  Medical Device programme (plus AI-Airlock sandbox), and PMDA /
  MHLW guidance in evolution.
- AI in clinical trials is addressed at the trial-design stage
  through regulator scientific advice, then documented in the IND
  / IMPD / CTA and refreshed at the marketing-authorisation
  submission.
- Pharmacovigilance AI is validated to a standard the QPPV can
  rely on and defensible against CIOMS Working Group standards and
  ICH E2 series principles.
- GMP-regulated AI systems in manufacturing are validated per
  GAMP 5 Second Edition, data-integrity-compliant per ALCOA+ and
  21 CFR Part 11, change-controlled, and inspection-ready across
  FDA, EMA, MHRA, and PMDA sites.
- Inspector engagement is fronted by the site head, Quality, QP,
  or QPPV depending on inspection type. The head prepares the
  AI-specific response, briefs the hosting function, and stands by
  for technical questions.
- The three-function operating protocol — Regulatory Affairs,
  Quality, head of AI governance — is written down, ratified, and
  defends the enterprise from a split answer at inspection.
- The board-level story has three beats: defensible AI-system
  regulatory status per regulator; GxP-controlled and inspection-
  ready manufacturing AI; PV-defensible AI-driven safety pipeline.
  Feeds cluster 4 of the Audit Committee pack in
  [[mod-103-board-and-audit-committee-reporting]] and the R&D /
  Science-and-Technology Committee's AI oversight.
