# Resources for mod-102 — Running the AI Governance Program

Primary sources for the topics in this module. All links point to
official standards bodies, government publishers, or the professional
associations that maintain the standard. Avoid secondary summaries
when authoring the artefacts described in the exercises — a head of
role who quotes primary sources at the audit committee is a head of
role the audit committee ratifies.

## ISO/IEC 42001 AIMS and adjacent standards

- [ISO/IEC 42001:2023 — AI management system](https://www.iso.org/standard/81230.html)
  — the AIMS standard. Clauses 4–10 (Context, Leadership, Planning,
  Support, Operation, Performance evaluation, Improvement) plus
  Annex A controls anchor chapters 01, 02, and 05.
- [ISO/IEC 42005:2025 — AI system impact assessment](https://www.iso.org/standard/44545.html)
  — the impact-assessment standard the inventory cross-references
  in chapter 06.
- [ISO/IEC 42006:2025 — Requirements for bodies providing audit and
  certification of AI management systems](https://www.iso.org/standard/44546.html)
  — the AIMS certification / audit body standard the head prepares
  for in chapters 02 and 04.
- [ISO/IEC 23894:2023 — Guidance on AI risk management](https://www.iso.org/standard/77304.html)
  — AI-specific risk-management guidance the register in chapter 03
  is built against.
- [ISO/IEC 27001:2022 — Information security management systems](https://www.iso.org/standard/82875.html)
  — the ISMS standard the AIMS calendar composes with (chapter 02).
- [ISO/IEC 27005:2022 — Guidance on managing information security
  risks](https://www.iso.org/standard/80585.html) — the ISMS-side
  risk parent that composes with ISO/IEC 23894 in chapter 03.
- [ISO/IEC 27036 — Cybersecurity — Supplier relationships](https://www.iso.org/standard/59648.html)
  — the third-party supplier-relationship standard referenced from
  chapter 07's AI-vendor tiering.
- [ISO 31000:2018 — Risk management guidelines](https://www.iso.org/standard/65694.html)
  — the parent enterprise-risk framework in chapter 03.
- [ISO/IEC 17021-1:2015 — Conformity assessment — Requirements for
  bodies providing audit and certification of management systems](https://www.iso.org/standard/61651.html)
  — the parent standard ISO/IEC 42006 specialises for AI management
  systems.
- [ISO/IEC Directives, Part 1 — Consolidated ISO Supplement (Annex
  SL / Harmonised Structure)](https://www.iso.org/directives-and-policies.html)
  — the Harmonised Structure that gives ISO/IEC 42001 and ISO/IEC
  27001 their shared clause layout referenced in chapter 02.

## ISO/IEC 38507 and the governance family (board and council posture)

- [ISO/IEC 38507:2022 — Governance implications of the use of
  artificial intelligence by organizations](https://www.iso.org/standard/56641.html)
  — the board-facing standard referenced from chapter 01 on council
  chairing and from [[mod-103-board-and-audit-committee-reporting]]
  for the five-cluster board pack.
- [ISO/IEC 38500:2015 — Governance of IT for the organization](https://www.iso.org/standard/62816.html)
  — the parent evaluate → direct → monitor framework 38507
  specialises for AI.

## NIST AI RMF, Playbook, and CSF 2.0

- [NIST AI Risk Management Framework 1.0 (AI 100-1)](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-1.pdf)
  — the foundational framework document, January 2023.
- [NIST AI RMF Playbook](https://airc.nist.gov/AI_RMF_Knowledge_Base/Playbook)
  — subcategory-level actions used as the leadership-shape maturity
  reference in chapter 05.
- [NIST AI RMF Generative AI Profile (AI 600-1)](https://airc.nist.gov/AI_RMF_Knowledge_Base/AI_RMF/Uses/GenAI-Profile)
  — the GenAI overlay, July 2024.
- [NIST AI Resource Center (AIRC)](https://airc.nist.gov/) — the
  landing site for crosswalks, profile documents, and Playbook
  updates.
- [NIST Cybersecurity Framework 2.0](https://www.nist.gov/cyberframework)
  — the CSF 2.0 landing page; the GOVERN function and GV.SC
  supply-chain-risk-management category anchor chapter 07.
- [CISA / NCSC Guidelines for Secure AI System Development (2023)](https://www.cisa.gov/resources-tools/resources/guidelines-secure-ai-system-development)
  — the joint AI-security guidance referenced from chapter 07 for
  supply-chain-of-AI expectations.

## OWASP AI security and governance references

- [OWASP AI Security and Governance Checklist](https://owasp.org/www-project-ai-security-and-privacy-guide/)
  — the technical-control reference used as the third maturity axis
  in chapter 05.
- [OWASP Top 10 for LLM Applications](https://genai.owasp.org/)
  — the LLM Top 10 landing site; composes with the Checklist where
  the enterprise operates LLM-based systems.
- [OWASP Machine Learning Security Top 10](https://owasp.org/www-project-machine-learning-security-top-10/)
  — the classical-ML security top 10 that composes with the
  Checklist for non-LLM AI systems.

## AI supply-chain evidence architecture (chapter 07)

- [CycloneDX ML-BOM (Machine Learning Bill of Materials)](https://cyclonedx.org/capabilities/mlbom/)
  — the ML-BOM extension to CycloneDX.
- [CycloneDX specification](https://cyclonedx.org/specification/)
  — the parent CycloneDX SBOM specification.
- [SPDX 3.0 (Software Package Data Exchange)](https://spdx.dev/)
  — the SPDX 3.0 landing page including the AI profile.
- [SPDX AI Profile specification (SPDX 3.0)](https://spdx.github.io/spdx-spec/)
  — the SPDX 3.0 specification; the AI profile is defined in
  Chapter 12 of the SPDX 3.0 model documentation.
- [SLSA — Supply-chain Levels for Software Artifacts](https://slsa.dev/)
  — the SLSA framework with build-integrity levels 1 through 4
  referenced in chapter 07.
- [Sigstore](https://www.sigstore.dev/) — the signing infrastructure
  (cosign, Fulcio, Rekor transparency log) referenced in chapter 07.
- [in-toto attestation framework](https://in-toto.io/) — the
  attestation format SLSA builds on, useful when authoring the
  attestation schema.
- [OSCAL — Open Security Controls Assessment Language (NIST)](https://pages.nist.gov/OSCAL/)
  — the machine-readable controls-and-assessment format used in
  chapters 06 and 07 for inventory and evidence export.

## Model, system, and dataset cards

- [Model Cards for Model Reporting (Mitchell et al. 2019)](https://arxiv.org/abs/1810.03993)
  — the model-cards paper referenced across evidence architecture
  discussion in chapter 07.
- [Datasheets for Datasets (Gebru et al. 2018 / 2021)](https://arxiv.org/abs/1803.09010)
  — the datasheets paper the dataset-card practice descends from.
- [Data Cards (Pushkarna et al. 2022)](https://arxiv.org/abs/2204.01075)
  — the Data Cards paper from Google Research; the productionised
  form of dataset-card practice.
- [OpenAI system-cards landing page (via research index)](https://openai.com/research/)
  — the research index where OpenAI's system cards for GPT-4,
  GPT-4o, DALL·E 3, and later frontier releases are published.
- [Meta Llama system-cards (via the Llama landing site)](https://ai.meta.com/llama/)
  — where Meta publishes the Llama-family model and system cards.

## Frontier-lab governance-posture disclosures (context for chapters 04 and 05)

- [Anthropic Responsible Scaling Policy (RSP)](https://www.anthropic.com/rsp)
  — the RSP as published by Anthropic; a frontier-lab governance-
  posture disclosure the head references in third-party AI vendor
  tiering.
- [OpenAI Preparedness Framework](https://openai.com/safety/preparedness/)
  — the OpenAI framework governing capability-elicitation and
  release decisions.
- [Google DeepMind Frontier Safety Framework](https://deepmind.google/discover/blog/introducing-the-frontier-safety-framework/)
  — Google DeepMind's frontier framework, useful as a maturity
  benchmark for frontier-lab-adjacent enterprises in chapter 05.
- [Frontier Model Forum](https://www.frontiermodel.org/) — the
  frontier-lab industry body providing peer-disclosure norms
  chapter 05 references.

## Third-party audit ecosystem (chapter 04)

- [ForHumanity Independent Audit of AI Systems (IAAIS)](https://forhumanity.center/independent-audit-of-ai-systems/)
  — the IAAIS certification programme; ForHumanity auditors are one
  of the five external audit relationships in chapter 04.
- [BABL AI — Algorithm Bias Auditor Certification](https://babl.ai/)
  — BABL AI's landing site; the Algorithm Bias Auditor certification
  is the reference for the bias-audit relationship in chapter 04.
- [IIA Three Lines Model (2020)](https://www.theiia.org/en/content/position-papers/2020/the-iia-three-lines-model/)
  — the 2020 update to the earlier Three Lines of Defense model;
  the parent independence discipline for the CAE interface in
  chapters 01 and 04.
- [IIA International Professional Practices Framework (IPPF)](https://www.theiia.org/en/standards/what-are-the-standards/)
  — the professional standards for internal audit; particularly
  relevant to the CAE / head interface in chapter 04.
- [International Accreditation Forum (IAF) — MD 5 Duration of QMS
  and EMS Audits and other mandatory documents](https://iaf.nu/en/iaf-documents/)
  — the accreditation-body mandatory documents that constrain
  certification bodies' own sampling; referenced from chapter 04's
  ISO/IEC 42006 accreditation posture.
- [ANAB (ANSI National Accreditation Board)](https://anab.ansi.org/)
  — one of the US accreditation bodies for ISO/IEC 42001
  certification bodies.
- [UKAS (United Kingdom Accreditation Service)](https://www.ukas.com/)
  — the UK accreditation body.
- [DAkkS (Deutsche Akkreditierungsstelle)](https://www.dakks.de/en/home_en.html)
  — the German accreditation body.

## EU AI Act, EU AI governance apparatus, and Article 60 / 72 / 73

- [Regulation (EU) 2024/1689 — the EU AI Act](https://eur-lex.europa.eu/eli/reg/2024/1689/oj)
  — the consolidated text. Chapters III (high-risk) and V (GPAI)
  drive chapters 06 and 07 in this module; Chapter VII (Articles
  64–70) drives regulator-engagement work in
  [[mod-104-regulator-engagement]]; Article 60 covers registration;
  Articles 72 and 73 cover post-market monitoring and serious-
  incident reporting.
- [European AI Office](https://digital-strategy.ec.europa.eu/en/policies/ai-office)
  — the EU AI Office landing page.
- [European Artificial Intelligence Board](https://digital-strategy.ec.europa.eu/en/policies/ai-board)
  — the EU AI Board landing page.
- [EU AI Act Article 60 — EU database of high-risk AI systems (text
  via EUR-Lex)](https://eur-lex.europa.eu/eli/reg/2024/1689/oj) —
  Article 60 sits inside the consolidated text linked above; it is
  the registration obligation chapter 06's Article 60 section is
  built against.
- [EU AI Office — GPAI Code of Practice](https://digital-strategy.ec.europa.eu/en/policies/ai-code-practice)
  — the GPAI Code of Practice for signatories, referenced from
  chapter 05's voluntary-code maturity composition and from
  [[mod-106-external-positioning-and-voluntary-codes]].

## US AI governance apparatus

- [US AI Safety Institute (AISI)](https://www.nist.gov/aisi) — NIST
  AISI landing page.
- [AISI Consortium (AISIC)](https://www.nist.gov/aisi/artificial-intelligence-safety-institute-consortium-aisic)
  — the consortium page.
- [OMB M-25-21 — Accelerating Federal Use of AI through Innovation,
  Governance, and Public Trust](https://www.whitehouse.gov/wp-content/uploads/2025/04/M-25-21-Accelerating-Federal-Use-of-AI-through-Innovation-Governance-and-Public-Trust.pdf)
  — the federal Chief AI Officer designation, AI Governance Board,
  and use-case inventory expectations referenced in chapters 05 and
  06.
- [OMB M-24-10 — Advancing Governance, Innovation, and Risk
  Management for Agency Use of AI](https://www.whitehouse.gov/wp-content/uploads/2024/03/M-24-10-Advancing-Governance-Innovation-and-Risk-Management-for-Agency-Use-of-Artificial-Intelligence.pdf)
  — predecessor memorandum with governance detail retained as
  background.

## Sector-specific model-risk and supervisory references

- [Federal Reserve SR 11-7 — Guidance on Model Risk Management](https://www.federalreserve.gov/supervisionreg/srletters/sr1107.htm)
  — the foundational US MRM reference. The tiering conventions in
  chapters 03, 05, and 06 compose with SR 11-7 in banking.
- [OCC Bulletin 2011-12 — Sound Practices for Model Risk
  Management](https://www.occ.gov/news-issuances/bulletins/2011/bulletin-2011-12.html)
  — the OCC's parallel MRM guidance.
- [Federal Reserve SR 23-4 — Interagency Guidance on Third-Party
  Relationships](https://www.federalreserve.gov/supervisionreg/srletters/SR2304.htm)
  — third-party risk guidance referenced in chapter 07 for the
  AI-vendor tiering parent framework.
- [Federal Reserve SR 15-19 — Federal Reserve Supervisory Assessment
  of Capital Planning and Positions](https://www.federalreserve.gov/supervisionreg/srletters/sr1519.htm)
  — the parent supervisory-assessment framework referenced from
  chapter 04's sector-regulator examiner section.
- [OSFI Guideline E-23 — Model Risk Management](https://www.osfi-bsif.gc.ca/en/guidance/guidance-library/model-risk-management-guideline-e-23)
  — Canadian federally-regulated financial institutions MRM
  guidance.
- [NAIC Model Bulletin on the Use of Artificial Intelligence Systems
  by Insurers](https://content.naic.org/sites/default/files/inline-files/2023-12-4%20Model%20Bulletin_Adopted_0.pdf)
  — the NAIC AI Model Bulletin adopted in December 2023; the
  state-by-state adoption is the reference for the insurance-sector
  maturity composition in chapter 05.
- [FDA Good Machine Learning Practice (GMLP) — Guiding Principles
  for AI/ML-Based Medical Devices](https://www.fda.gov/medical-devices/software-medical-device-samd/good-machine-learning-practice-medical-device-development-guiding-principles)
  — the FDA GMLP page; the medical-device maturity composition
  reference in chapter 05 and the post-market surveillance reference
  in chapter 06.
- [FDA Predetermined Change Control Plan (PCCP) — Guidance for
  AI/ML-Based Medical Devices](https://www.fda.gov/regulatory-information/search-fda-guidance-documents/marketing-submission-recommendations-predetermined-change-control-plan-artificial)
  — the PCCP guidance referenced in chapter 05.

## Governance and enterprise-risk parent references (context for chapters 01 and 03)

- [COSO Enterprise Risk Management — Integrating with Strategy and
  Performance (2017)](https://www.coso.org/enterprise-risk-management)
  — the parent enterprise-risk framework in most US enterprises;
  the enterprise risk register in chapter 03 usually reports up
  under COSO ERM.
- [COSO Internal Control — Integrated Framework (2013)](https://www.coso.org/internal-control)
  — the parent internal-control framework relevant to the
  three-lines discipline in chapter 04.

## Related modules in this track

- [mod-101 — Head of AI Governance Role Scope and Leadership Shape](../mod-101-role-scope-and-leadership-shape/README.md)
  — the level-50 architect's design outputs the head consumes here.
- [mod-103 — Board, Audit Committee, and Risk Committee AI
  Reporting](../mod-103-board-and-audit-committee-reporting/README.md)
  — where the maturity plot, council minutes, register escalations,
  audit findings, and inventory metrics land as board and
  audit-committee reporting.
- [mod-104 — Regulator Engagement](../mod-104-regulator-engagement/README.md)
  — where sector-regulator examiner engagement (chapter 04) is
  extended to full regulator-relationship management.
- [mod-106 — External Positioning and Voluntary Codes](../mod-106-external-positioning-and-voluntary-codes/README.md)
  — where the voluntary-code maturity commitments in chapter 05 are
  authored and defended.
- [mod-107 — Program Measurement, Maturity, and ROI Reporting](../mod-107-program-measurement-and-maturity/README.md)
  — where the maturity plot in chapter 05 is extended into full
  program-measurement and ROI reporting.
- [mod-110 — Incident Leadership](../mod-110-incident-leadership/README.md)
  — where the shadow-discovery incident triage referenced in
  chapter 06 lives.
- [mod-113 — Budget, Vendor, P&L, and Investment Case](../mod-113-budget-vendor-p-and-l-and-investment-case/README.md)
  — where the cost-of-move table from exercise 05 lands in the
  annual budget cycle.

<!-- needs-research: verify SPDX AI Profile section reference — the
SPDX 3.0 specification is the parent; the AI profile is defined
within it, and the chapter number may shift with spec revisions.
Confirm the current chapter for the AI profile when citing at audit-
committee depth. -->

<!-- needs-research: verify the OpenAI Preparedness Framework and
Google DeepMind Frontier Safety Framework URLs above resolve — both
frameworks have been revised since first publication and the
landing URLs shift with each revision. -->
