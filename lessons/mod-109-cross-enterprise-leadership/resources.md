# Resources for mod-109 — Cross-Enterprise Leadership and CxO Coordination

Primary sources for the twelve CxO adjacencies the module
designs coordination patterns for. Links point to official
standards bodies, regulator publications, professional-
institute publishers, and the primary publications of the
reference frameworks each chapter builds on. The interface
documents, council charter, and escalation ladder the module
produces are only defensible if grounded in primary sources —
a head who cites a trade-press summary of GDPR, the EU AI Act,
NYC LL 144, or an ISO standard is a head who has skipped the
discipline the audit committee will test. `needs-research`
markers below identify specific facts to re-verify against the
primary source before citing at CxO or audit-committee depth;
they are the mechanism by which the module signals uncertainty
rather than guessing at it.

## CISO adjacency — AI security, SOC coordination, red-team routing (chapter 01)

- [CISA / NCSC — Guidelines for Secure AI System
  Development (November 2023)](https://www.cisa.gov/resources-tools/resources/guidelines-secure-ai-system-development)
  — the joint CISA / NCSC guidelines on secure AI system
  development, co-signed by partners from fourteen agencies
  across eighteen countries. Primary source for Surface 1
  (ISMS composition) and Surface 3 (detection engineering).
- [CISA — Deploying AI Systems Securely (April 2024)](https://www.cisa.gov/resources-tools/resources/deploying-ai-systems-securely)
  — the CISA / NSA / FBI joint information sheet on
  deploying AI systems securely, extending the November 2023
  guidelines to the deployment phase. Primary source for
  Surface 4 (incident response) and detection patterns.
- [MITRE ATLAS — Adversarial Threat Landscape for
  Artificial-Intelligence Systems](https://atlas.mitre.org/)
  — the MITRE knowledge base of AI-specific attack
  techniques, tactics, and case studies. The technique-ID
  mapping (AML.T0051 Prompt Injection, AML.T0053 LLM Plugin
  Compromise, etc.) is the finding-template vocabulary for
  Surface 2 (red-team routing).
- [OWASP Top 10 for Large Language Model Applications
  (v1.1, 2023; v2 2025)](https://genai.owasp.org/)
  — the OWASP Generative AI Security Project landing page
  including the LLM Applications & Generative AI Security
  Top 10 (v2, 2025) and the agentic AI security guidance.
  Primary source for the finding-class taxonomy.
- [NIST SP 800-218A — Secure Software Development Practices
  for Generative AI and Dual-Use Foundation Models](https://csrc.nist.gov/pubs/sp/800/218/a/final)
  — the generative-AI extension to NIST SP 800-218 Secure
  Software Development Framework (SSDF). Primary source for
  the SDLC-level composition with the CISO's secure-SDLC
  practice.
- [NIST — Cybersecurity Framework 2.0](https://www.nist.gov/cyberframework)
  — the CSF 2.0 (February 2024) with the GOVERN, IDENTIFY,
  PROTECT, DETECT, RESPOND, RECOVER functions. Parent
  framework the AI-security extension composes into.
- [ISO/IEC 27001:2022 — Information security management
  system](https://www.iso.org/standard/27001)
  — the ISMS standard the CISO operates under; clause 6.1.2
  risk assessment is where the AI risk register composes.
- [ISO/IEC 27002:2022 — Information security controls](https://www.iso.org/standard/75652.html)
  — the controls catalogue the CISO's ISMS applies.
- [ISO/IEC 27005:2022 — Information security risk management](https://www.iso.org/standard/80585.html)
  — the ISO 27005 standard for information-security risk
  management the CISO's risk composition is grounded in.
- [MITRE — ATT&CK](https://attack.mitre.org/)
  — the broader MITRE ATT&CK knowledge base ATLAS composes
  with for the CISO's SOC playbooks.

## CIO / CTO / CDO adjacency — AI platform, model registry, data governance (chapter 02)

- [ISO/IEC 42001:2023 — AI management system](https://www.iso.org/standard/81230.html)
  — the AI management-system standard; clause 8 (operational
  planning and control) is the parent clause the governance-
  runtime specification derives from.
- [NIST AI Risk Management Framework 1.0 (AI 100-1)](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-1.pdf)
  — the AI RMF 1.0 with the GOVERN, MAP, MEASURE, MANAGE
  functions. MAP and MEASURE are the composition points for
  the metadata and evidence contracts.
- [NIST AI Resource Center (AIRC)](https://airc.nist.gov/)
  — the NIST AI RMF Playbook, Profiles, and crosswalks.
- [NIST AI RMF Generative AI Profile (NIST AI 600-1)](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.600-1.pdf)
  — the generative-AI profile adjunct to the AI RMF 1.0.
- [ISO/IEC 38505-1:2017 — Governance of IT — Governance of
  data — Part 1: Application of ISO/IEC 38500 to the
  governance of data](https://www.iso.org/standard/56639.html)
  — the IT data-governance standard the CDO's data-
  governance framework often cites.
- [DAMA International — DAMA-DMBOK 2 (Data Management Body
  of Knowledge, 2nd Edition)](https://www.dama.org/cpages/body-of-knowledge)
  — the data-management-profession reference the CDO's data-
  governance framework typically rests on.
- [MLflow — open-source MLOps / model registry](https://mlflow.org/)
  — representative open-source model-registry stack referenced
  in the AI-platform composition conversation.
- [Kubeflow](https://www.kubeflow.org/) — representative
  open-source ML platform.
- [Google Cloud — Vertex AI Model Registry](https://cloud.google.com/vertex-ai/docs/model-registry/introduction)
  — representative cloud-native model-registry reference.
- [Databricks — Unity Catalog](https://docs.databricks.com/aws/en/data-governance/unity-catalog)
  — representative data-and-model-governance reference.
- [AWS — SageMaker Model Registry](https://docs.aws.amazon.com/sagemaker/latest/dg/model-registry.html)
  — representative cloud-native model-registry reference.

## CPO / DPO adjacency — AIA / DPIA interface, ROPA, cross-jurisdiction privacy (chapter 03)

- [EU — General Data Protection Regulation (Regulation
  (EU) 2016/679)](https://eur-lex.europa.eu/eli/reg/2016/679/oj)
  — the GDPR consolidated text. Article 22 (automated
  decision-making), Article 30 (ROPA), Article 33 (breach
  notification), Article 35 (DPIA), Article 88 (employee data)
  are the specific articles the AIA / DPIA / ROPA interface
  composes against.
- [European Data Protection Board (EDPB) — Guidelines](https://www.edpb.europa.eu/our-work-tools/general-guidance/guidelines-recommendations-best-practices_en)
  — the EDPB's standing guidelines on DPIAs, automated
  decision-making, and employee-data processing.
- [EU — Artificial Intelligence Act (Regulation (EU)
  2024/1689)](https://eur-lex.europa.eu/eli/reg/2024/1689/oj)
  — the EU AI Act consolidated text. Article 27 (fundamental-
  rights impact assessment, FRIA) is the AIA composition
  point.
- [California Privacy Protection Agency (CPPA) — Automated
  Decisionmaking Technology (ADMT) regulations](https://cppa.ca.gov/regulations/)
  — the CPPA's ADMT rulemaking package extending CCPA to
  automated decisionmaking. See needs-research below on the
  current adopted-text status.
- [California Consumer Privacy Act (CCPA) and California
  Privacy Rights Act (CPRA)](https://cppa.ca.gov/regulations/)
  — the California privacy regime the CPPA regulates.
- [India — Digital Personal Data Protection Act, 2023
  (DPDPA)](https://www.meity.gov.in/data-protection-framework)
  — the Indian DPDPA 2023 landing page at the Ministry of
  Electronics and Information Technology.
- [UK Information Commissioner's Office (ICO) — Guidance on
  AI and data protection](https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/artificial-intelligence/)
  — the ICO's AI-and-data-protection guidance, the DPIA
  guidance for AI, and the AI auditing framework.
- [CNIL — Artificial intelligence (France)](https://www.cnil.fr/en/artificial-intelligence)
  — the CNIL's AI landing page including DPIA guidance for
  AI systems.
- [IAPP — Resource Center on AI governance](https://iapp.org/resources/topics/ai-governance/)
  — the IAPP's AI-governance resource landing page the
  CPO / DPO function typically references.

## CRO adjacency — enterprise risk framework, appetite / tolerance / limit (chapter 04)

- [ISO 31000:2018 — Risk management — Guidelines](https://www.iso.org/standard/65694.html)
  — the parent risk-management standard the enterprise risk
  framework typically derives from.
- [ISO/IEC 27005:2022 — Information security risk management](https://www.iso.org/standard/80585.html)
  — the information-security risk-management standard
  adjacent to the CRO's enterprise framework.
- [ISO/IEC 23894:2023 — Artificial intelligence — Guidance
  on risk management](https://www.iso.org/standard/77304.html)
  — the AI-specific risk-management guidance that composes
  into ISO 31000.
- [COSO — Enterprise Risk Management: Integrating with
  Strategy and Performance (2017)](https://www.coso.org/guidance-erm)
  — the COSO ERM framework the CRO's operating model
  typically derives from in US-anchored enterprises.
- [COSO — Compliance Risk Management: Applying the COSO ERM
  Framework (2020)](https://www.coso.org/guidance-crm)
  — the COSO compliance-risk extension.
- [The IIA — Three Lines Model (2020)](https://www.theiia.org/en/content/position-papers/2020/the-iia-three-lines-model/)
  — the Three Lines Model that positions the head's second-
  line function alongside the CRO's parent framework.
- [Basel Committee on Banking Supervision — Operational
  risk](https://www.bis.org/bcbs/publ/d515.htm)
  — the Basel operational-risk framework for banking-sector
  enterprises where the AI risk portfolio composes with
  operational-risk reporting.
- [Federal Reserve — SR 11-7 — Guidance on Model Risk
  Management (April 2011)](https://www.federalreserve.gov/supervisionreg/srletters/sr1107.htm)
  — the SR 11-7 model-risk-management guidance the Head of
  Model Risk Management operates under, cited across the
  banking-sector overlay.

## CAE adjacency — third-line audit, IIA Three Lines, IPPF (chapter 05)

- [The IIA — Three Lines Model (2020)](https://www.theiia.org/en/content/position-papers/2020/the-iia-three-lines-model/)
  — the 2020 Three Lines Model governing the boundary between
  the head's second-line function and the CAE's third-line
  function.
- [The IIA — International Professional Practices Framework
  (IPPF)](https://www.theiia.org/en/standards/what-are-the-standards/)
  — the internal-audit standards the CAE operates against.
  See needs-research below on current edition and transition
  to the Global Internal Audit Standards.
- [The IIA — Global Internal Audit Standards (effective
  January 2025)](https://www.theiia.org/en/standards/2024-standards/global-internal-audit-standards/)
  — the current Global Internal Audit Standards replacing
  the prior IPPF structure.
- [The IIA — Chief Audit Executive resources](https://www.theiia.org/en/leaders-learning/positions/chief-audit-executive/)
  — the CAE-focused landing page for position papers and
  guidance.
- [The IIA — Auditing Artificial Intelligence practice
  guidance](https://www.theiia.org/en/content/guidance/recommended/supplemental/practice-guides/auditing-artificial-intelligence/)
  — the IIA's AI-audit practice guidance the CAE's third-
  line AI audit programme operates against.
- [ISACA — IS Audit and Assurance Standards and Guidelines](https://www.isaca.org/resources/isaca-journal/standards-guidelines-and-tools)
  — the ISACA standards adjacent to the CAE's audit
  discipline, often applied in IT-audit sub-programs.
- [COSO — Internal Control — Integrated Framework (2013)](https://www.coso.org/guidance-on-ic)
  — the internal-control framework the CAE often applies in
  conjunction with the IPPF / Global Internal Audit Standards.

## General Counsel adjacency — regulator interpretation, litigation posture, SAR / MOU / MRA (chapter 06)

- [American Bar Association — Model Rules of Professional
  Conduct](https://www.americanbar.org/groups/professional_responsibility/publications/model_rules_of_professional_conduct/)
  — Rule 2.1 (Advisor) and Rule 2.3 (Evaluation for Use by
  Third Persons) are the primary professional-conduct rules
  governing the GC's delivery of legal opinion versus the
  head's packaging of interpretation.
- [ABA — Model Rules — Rule 2.1 Advisor](https://www.americanbar.org/groups/professional_responsibility/publications/model_rules_of_professional_conduct/rule_2_1_advisor/)
  — the specific rule on independent professional judgement
  in legal advice.
- [Bar Standards Board (UK) — BSB Handbook](https://www.barstandardsboard.org.uk/the-bsb-handbook.html)
  — the UK barrister conduct equivalent.
- [SRA — Solicitors Regulation Authority (UK) — Standards
  and Regulations](https://www.sra.org.uk/solicitors/standards-regulations/)
  — the UK solicitor conduct regime.
- [EU — Artificial Intelligence Act (Regulation (EU)
  2024/1689)](https://eur-lex.europa.eu/eli/reg/2024/1689/oj)
  — the EU AI Act consolidated text. Articles 6, 9, 16, 26,
  27, 50, 55, 72, 73 are the articles the head and GC
  interpret jointly on EU-anchored systems.
- [EU AI Office](https://digital-strategy.ec.europa.eu/en/policies/ai-office)
  — the Commission-anchored Union-level body publishing
  Article-55 GPAI Code of Practice work and implementing /
  delegated acts.
- [NAIC — AI Model Bulletin (December 2023)](https://content.naic.org/sites/default/files/inline-files/2023-12-4%20Model%20Bulletin_Adopted_0.pdf)
  — the NAIC Model Bulletin on the use of AI by insurers.
- [FDA — Good Machine Learning Practice (GMLP) for Medical
  Device Development](https://www.fda.gov/medical-devices/software-medical-device-samd/good-machine-learning-practice-medical-device-development-guiding-principles)
  — the FDA GMLP guiding principles for medical-device AI.
- [NYC Department of Consumer and Worker Protection —
  Local Law 144 of 2021 (Automated Employment Decision
  Tools)](https://www.nyc.gov/site/dca/about/automated-employment-decision-tools.page)
  — NYC LL 144, effective July 2023, requiring bias audits
  for AEDTs.
- [CPPA — Automated Decisionmaking Technology (ADMT) rulemaking](https://cppa.ca.gov/regulations/)
  — the California Privacy Protection Agency's ADMT
  regulatory package.

## CFO adjacency — budget, ROI, capital planning, contingency reserves (chapter 07)

- [US SEC — Final Rule — Cybersecurity Risk Management,
  Strategy, Governance, and Incident Disclosure (July 2023)](https://www.sec.gov/rules/final/2023/33-11216.pdf)
  — the SEC Cybersecurity Disclosure Rule including Item
  1.05 Form 8-K material-cybersecurity-incident disclosure.
  Primary source for the material-event-evaluation surface
  with the CFO.
- [SEC — Form 8-K general instructions](https://www.sec.gov/files/form8-k.pdf)
  — the Form 8-K material-event disclosure form the CFO
  references for AI-incident disclosure determinations.
- [FASB — Accounting Standards Codification](https://www.fasb.org/accounting-standards-codification)
  — the US GAAP standards codification the CFO's financial
  reporting operates under (contingency reserves under ASC
  450).
- [IFRS Foundation — IFRS Standards](https://www.ifrs.org/issued-standards/list-of-standards/)
  — the IFRS standards the CFO's financial reporting operates
  under in international-anchored enterprises (IAS 37 on
  provisions).
- [COSO — Internal Control — Integrated Framework (2013)](https://www.coso.org/guidance-on-ic)
  — the internal-control framework the CFO's finance
  function operates under on SOX-material items.
- [Sarbanes-Oxley Act of 2002](https://www.congress.gov/bill/107th-congress/house-bill/3763)
  — the US SOX legislation requiring material-weakness
  disclosure in internal control over financial reporting.

## CHRO adjacency — AI-in-HR, hiring-tool bias, workforce AI training (chapter 08)

- [NYC Department of Consumer and Worker Protection —
  Automated Employment Decision Tools (Local Law 144)](https://www.nyc.gov/site/dca/about/automated-employment-decision-tools.page)
  — NYC LL 144 landing page with the DCWP's final rules,
  bias-audit guidance, and candidate-notice requirements.
- [US EEOC — The Americans with Disabilities Act and the Use
  of Software, Algorithms, and Artificial Intelligence to
  Assess Job Applicants and Employees (May 2022)](https://www.eeoc.gov/laws/guidance/americans-disabilities-act-and-use-software-algorithms-and-artificial-intelligence)
  — the EEOC's ADA guidance on AI-in-employment tools.
- [US EEOC — Assessing Adverse Impact in Software,
  Algorithms, and Artificial Intelligence Used in Employment
  Selection Procedures Under Title VII of the Civil Rights
  Act of 1964 (May 2023)](https://www.eeoc.gov/laws/guidance/select-issues-assessing-adverse-impact-software-algorithms-and-artificial)
  — the EEOC's Title VII guidance on AI-in-employment
  selection procedures.
- [US EEOC — Artificial Intelligence and Algorithmic
  Fairness Initiative](https://www.eeoc.gov/ai)
  — the EEOC's AI-and-algorithmic-fairness initiative
  landing page.
- [Illinois General Assembly — HB 3773 (Illinois Human
  Rights Act amendments on AI in employment, effective
  January 2026)](https://www.ilga.gov/legislation/BillStatus.asp?DocNum=3773&GAID=17&DocTypeID=HB&SessionID=112&GA=103)
  — Illinois HB 3773 amending the IHRA to address AI
  employment decisions.
- [Colorado General Assembly — SB 24-205 (Colorado Artificial
  Intelligence Act)](https://leg.colorado.gov/bills/sb24-205)
  — Colorado SB 24-205 with its employment applicability.
- [US Department of Labor — Field Assistance Bulletin on AI
  and worker surveillance](https://www.dol.gov/agencies/whd)
  — the US DOL / WHD landing page on labour-standards
  enforcement relevant to AI-in-HR applications.
- [ISO 30414:2018 — Human resource management — Guidelines
  for internal and external human capital reporting](https://www.iso.org/standard/69338.html)
  — the HR reporting standard adjacent to the AI-in-HR
  governance surface.
- [NIST SP 1270 — Towards a Standard for Identifying and
  Managing Bias in Artificial Intelligence (March 2022)](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.1270.pdf)
  — the NIST bias-in-AI reference the bias-audit
  methodology cites.
- [GDPR Article 88 — Processing in the context of employment](https://gdpr-info.eu/art-88-gdpr/)
  — Article 88 empowering member-state law on employee data.
- [SHRM — Society for Human Resource Management](https://www.shrm.org/)
  — the US HR-professional body publishing practice guidance
  on AI-in-HR.

## Chief Compliance Officer adjacency — enterprise policy library, compliance monitoring (chapter 09)

- [US DOJ Criminal Division — Evaluation of Corporate
  Compliance Programs (September 2024 update)](https://www.justice.gov/criminal/criminal-fraud/page/file/937501/download)
  — the DOJ ECCP guidance the CCO's compliance programme is
  typically benchmarked against; the September 2024 update
  specifically addresses the use of new technology including
  AI.
- [US Sentencing Commission — Federal Sentencing Guidelines
  for Organizations (Chapter 8)](https://www.ussc.gov/guidelines/2023-guidelines-manual/2023-chapter-8)
  — the FSGO Chapter 8 effective-compliance-program factors.
- [ISO 37301:2021 — Compliance management systems —
  Requirements with guidance for use](https://www.iso.org/standard/75080.html)
  — the compliance-management-system standard the CCO's
  function often certifies against.
- [ISO 37001:2016 — Anti-bribery management systems](https://www.iso.org/standard/65034.html)
  — the anti-bribery MS standard adjacent to the CCO's
  compliance library.
- [COSO — Compliance Risk Management: Applying the COSO ERM
  Framework (2020)](https://www.coso.org/guidance-crm)
  — the COSO compliance-risk guidance.
- [Society of Corporate Compliance and Ethics (SCCE)](https://www.corporatecompliance.org/)
  — the compliance-professional body publishing practice
  guidance on compliance-program design.

## Chief Communications Officer adjacency — public trust posture, crisis communications (chapter 10)

- [US FTC — Keep your AI claims in check (February 2023)](https://www.ftc.gov/business-guidance/blog/2023/02/keep-your-ai-claims-check)
  — the FTC business-guidance post on substantiating AI
  claims in marketing and public communications.
- [US FTC — AI (and other) companies: Quietly changing your
  terms of service could be unfair or deceptive (February
  2024)](https://www.ftc.gov/business-guidance/blog/2024/02/ai-other-companies-quietly-changing-your-terms-service-could-be-unfair-or-deceptive)
  — the FTC post on terms-of-service changes affecting AI
  claims.
- [US FTC — Operation AI Comply announcements](https://www.ftc.gov/news-events/news/press-releases)
  — FTC enforcement-action press releases relevant to AI
  claims in public communications.
- [US SEC — Final Rule — Cybersecurity Risk Management,
  Strategy, Governance, and Incident Disclosure (July 2023)](https://www.sec.gov/rules/final/2023/33-11216.pdf)
  — the Item 1.05 Form 8-K material-cybersecurity-incident
  disclosure rule the CCO's crisis-communications runbook
  references.
- [NIST — Cybersecurity Framework 2.0](https://www.nist.gov/cyberframework)
  — the CSF 2.0 GOVERN and RESPOND functions on
  communications.
- [IABC — International Association of Business
  Communicators](https://www.iabc.com/)
  — the IABC professional body publishing crisis-
  communications practice.
- [PRSA — Public Relations Society of America — Code of
  Ethics](https://www.prsa.org/about/ethics)
  — the PRSA Code of Ethics the CCO's function operates
  under.
- [ISACA — Communicating audit findings and incidents](https://www.isaca.org/)
  — ISACA practice guidance adjacent to the AI-incident
  communications discipline.

## AI Governance Council — chairing, decision-forcing, dissent-capture (chapter 11)

- [National Association of Parliamentarians — Robert's Rules
  of Order Newly Revised](https://www.parliamentarians.org/robert-s-rules/)
  — the NAP landing page for the parent-parliamentary
  reference many enterprises defer to for formal-vote
  procedure.
- [Robert's Rules of Order Newly Revised, 12th Edition](https://robertsrules.com/)
  — the authoritative edition reference published by Henry M.
  Robert III and the authorship team.
- [Chartered Governance Institute UK & Ireland (CGIUKI,
  formerly ICSA)](https://www.cgi.org.uk/)
  — the CGIUKI (formerly Institute of Chartered Secretaries
  and Administrators) landing page publishing committee-
  chairing and board-secretariat practice guidance.
- [Chartered Governance Institute — Resources on committee
  effectiveness](https://www.cgi.org.uk/knowledge/resources)
  — the CGIUKI resources landing with committee-effectiveness
  practice guidance.
- [ISO/IEC 42001:2023 — AI management system](https://www.iso.org/standard/81230.html)
  — clause 5.3 (organisational roles, responsibilities, and
  authorities) and clause 9.3 (management review) are the
  parent-standard requirements the council operationalises.
- [OECD — Principles of Corporate Governance (2023 revision)](https://www.oecd.org/en/publications/g20-oecd-principles-of-corporate-governance-2023_ed750b30-en.html)
  — the G20 / OECD Principles of Corporate Governance (2023)
  the audit-committee-reporting pathway composes with.
- [The IIA — Governance considerations in internal auditing](https://www.theiia.org/en/content/guidance/)
  — IIA guidance adjacent to governance-committee discipline.
- [Center for Creative Leadership — Research & Insights](https://www.ccl.org/insights/)
  — CCL's research-and-insights landing page for executive-
  committee practice literature.

## Product-conflict management — escalation ladder, negotiation discipline (chapter 12)

- [Fisher and Ury — Getting to Yes: Negotiating Agreement
  Without Giving In (3rd edition, Penguin, 2011)](https://www.pon.harvard.edu/shop/getting-to-yes-negotiating-agreement-without-giving-in/)
  — the Program on Negotiation (Harvard Law School) listing
  for the Fisher / Ury principled-negotiation reference the
  asked-and-answered discipline draws on.
- [Harvard Program on Negotiation — Resources](https://www.pon.harvard.edu/)
  — the PON landing page for additional negotiation-practice
  references.
- [Patterson, Grenny, McMillan, Switzler — Crucial
  Conversations: Tools for Talking When Stakes Are High
  (3rd edition, McGraw-Hill, 2021)](https://cruciallearning.com/crucial-conversations-book/)
  — the Crucial Learning landing page for the authoritative
  reference on high-stakes conversational discipline.
- [Bain & Company — RAPID decision-making framework](https://www.bain.com/insights/rapid-decision-making/)
  — the RAPID (Recommend, Agree, Perform, Input, Decide)
  decision-rights convention Bain publishes.
- [Project Management Institute — RACI matrix guidance](https://www.pmi.org/)
  — the PMI resources on the RACI (Responsible,
  Accountable, Consulted, Informed) decision-rights
  convention.
- [The IIA — Three Lines Model (2020)](https://www.theiia.org/en/content/position-papers/2020/the-iia-three-lines-model/)
  — the Three Lines Model the second-line escalation
  discipline operates under.
- [BSA | The Software Alliance — Framework to Build Trust
  in AI](https://www.bsa.org/policy-filings/bsa-framework-to-build-trust-in-ai)
  — the BSA framework for responsible-AI deployment the
  escalation discipline composes with.
- [OECD AI Principles](https://oecd.ai/en/ai-principles)
  — the OECD AI Principles adopted 2019, updated 2024.
- [OECD — Framework for the Classification of AI Systems](https://oecd.ai/en/classification)
  — the OECD classification framework adjacent to the AI
  Act's risk tiering the escalation ladder references.

## Primary legal and regulatory texts referenced across the module

- [EU — Artificial Intelligence Act (Regulation (EU)
  2024/1689, published OJ 12 July 2024)](https://eur-lex.europa.eu/eli/reg/2024/1689/oj)
  — the EU AI Act consolidated text. Phased application:
  prohibitions from February 2025, GPAI obligations from
  August 2025, high-risk obligations from August 2026. See
  needs-research below on current effective-date status.
- [EU — General Data Protection Regulation (Regulation
  (EU) 2016/679)](https://eur-lex.europa.eu/eli/reg/2016/679/oj)
  — the GDPR consolidated text.
- [UK — Data Protection Act 2018](https://www.legislation.gov.uk/ukpga/2018/12/contents)
  — the UK DPA 2018 (incorporating UK GDPR).
- [India — Digital Personal Data Protection Act, 2023
  (DPDPA)](https://www.meity.gov.in/data-protection-framework)
  — the Indian DPDPA 2023.
- [California — California Consumer Privacy Act (CCPA, as
  amended by CPRA)](https://cppa.ca.gov/)
  — the California CCPA / CPRA regime regulated by the CPPA.
- [US — Civil Rights Act of 1964, Title VII (EEOC-enforced)](https://www.eeoc.gov/statutes/title-vii-civil-rights-act-1964)
  — Title VII of the Civil Rights Act, the parent-statute
  reference for the EEOC guidance on AI in employment.
- [US — Americans with Disabilities Act (ADA)](https://www.ada.gov/)
  — the ADA, the parent-statute reference for the EEOC's
  May 2022 ADA-and-AI guidance.
- [US — Fair Credit Reporting Act (FCRA)](https://www.ftc.gov/legal-library/browse/statutes/fair-credit-reporting-act)
  — the FCRA, the parent-statute reference for background-
  check and other AI applications in employment.

## Related modules in this track

- [mod-101 — Head of AI Governance Role Scope and Leadership
  Shape](../mod-101-role-scope-and-leadership-shape/README.md)
  — the level-ladder architecture (chapter 01), the IIA
  Three Lines positioning (chapter 04), the CxO adjacency
  map (chapter 06), and the engagement-contract discipline
  (chapter 07) this module runs the coordination patterns on
  top of.
- [mod-102 — Running the AI Governance Program](../mod-102-running-the-program/README.md)
  — the AIMS operating calendar, the risk register, the
  inventory, the exception discipline, and the evaluation
  discipline the coordination patterns consume and produce
  into.
- [mod-103 — Board and Audit Committee AI Reporting](../mod-103-board-and-audit-committee-reporting/README.md)
  — the audit-committee reporting cluster Step 5 of the
  escalation ladder escalates into, and the joint-appearance
  cadence the CISO, CRO, CAE, and GC coordinations feed.
- [mod-104 — Direct Regulator Engagement](../mod-104-regulator-engagement/README.md)
  — the regulator-engagement discipline the GC coordination
  (chapter 06) composes with.
- [mod-105 — Enterprise Regulatory Change Management](../mod-105-regulatory-change-management/README.md)
  — the horizon-scanning the GC and CCO coordinations
  consume for interpretation and compliance-library updates.
- [mod-106 — External Positioning and Voluntary Codes](../mod-106-external-positioning-and-voluntary-codes/README.md)
  — the public-trust posture the Chief Communications
  Officer coordination (chapter 10) runs.
- [mod-107 — Program Measurement, Maturity, and ROI
  Reporting](../mod-107-program-measurement-and-maturity/README.md)
  — the KRI / KPI portfolio and the ROI reporting shape the
  CFO coordination (chapter 07) consumes.
- [mod-108 — Leading the AI Governance Function](../mod-108-leading-the-governance-function/README.md)
  — the function-leadership discipline (org shape, hiring,
  coaching, independence balance, CAE coordination, CxO /
  vendor relationships, difficult conversations) this module
  extends outward to CxO peers.
- [mod-110 — Incident Leadership](../mod-110-incident-leadership/README.md)
  — the incident-leadership discipline where every one of
  this module's coordination patterns comes under time
  pressure at once.
- [mod-111 — Sector Program Leadership](../mod-111-sector-program-leadership/README.md)
  — the sector-specialist CxO overlays (Chief Medical
  Officer in health; Head of Model Risk Management in
  banking / insurance) that extend the twelve adjacencies in
  this module.
- [mod-113 — Budget, Vendor P&L, and Investment Case](../mod-113-budget-vendor-p-and-l-and-investment-case/README.md)
  — the CFO coordination (chapter 07) becomes an operating
  budget cycle in mod-113.

<!-- needs-research: verify the current state of the EU AI
Act phased-application schedule at eur-lex.europa.eu
(Regulation (EU) 2024/1689), including the Article 6 high-
risk obligations effective date, the Article 55 GPAI code-of-
practice adoption status, and any Commission implementing or
delegated acts published after the research window, before
citing specific effective dates at CxO depth. -->

<!-- needs-research: verify the current adopted-text status of
the California Privacy Protection Agency (CPPA) Automated
Decisionmaking Technology (ADMT) regulations at cppa.ca.gov,
including the final adopted-text date, operative-date, and
any amendments after the research window. The ADMT package
has evolved through multiple proposed and modified-text
rounds. -->

<!-- needs-research: verify the current effective-date and
rulemaking status of Illinois HB 3773 amending the Illinois
Human Rights Act, at ilga.gov and iDHR.illinois.gov,
including any Illinois Department of Human Rights
implementing rules published after the research window. -->

<!-- needs-research: verify the current effective-date and
rulemaking status of Colorado SB 24-205 (Colorado Artificial
Intelligence Act) at leg.colorado.gov, including any
Attorney-General implementing rules and any amendments
adopted during the Colorado General Assembly's subsequent
sessions. -->

<!-- needs-research: verify the current IIA IPPF and Global
Internal Audit Standards edition and effective date at
theiia.org, including the January 2025 transition from the
prior IPPF edition, before the CAE coordination chapter's
citations are finalised. -->

<!-- needs-research: verify the current published state of
the IIA's Auditing Artificial Intelligence practice guidance
at theiia.org, including any subsequent supplemental guidance
issued after the research window. -->

<!-- needs-research: verify the current published state of
ISO/IEC 42001, ISO/IEC 42005, and ISO/IEC 42006, including
any published amendments or revisions. -->

<!-- needs-research: verify the current September 2024 (or
later) US DOJ Criminal Division Evaluation of Corporate
Compliance Programs guidance at justice.gov, including the
specific AI and emerging-technology provisions and any
subsequent updates after the research window. -->

<!-- needs-research: verify the current state of the SEC
Cybersecurity Disclosure Rule (33-11216) at sec.gov,
including the specific Item 1.05 Form 8-K material-
cybersecurity-incident disclosure requirements and the four-
business-day timing. The rule's application to AI incidents
is interpretive; verify any Division of Corporation Finance
staff guidance published after the research window. -->

<!-- needs-research: verify the current NYC DCWP final rules
on Local Law 144 at nyc.gov/dca, including the bias-audit
methodology requirements and the summary-of-results publication
requirements, and any amendments after the research window. -->

<!-- needs-research: verify the current FDA Good Machine
Learning Practice guidance and any subsequent Software as a
Medical Device (SaMD) AI-specific guidance at fda.gov, before
citing the sector-overlay in the GC coordination chapter. -->

<!-- needs-research: verify the current NAIC AI Model
Bulletin adoption status by state insurance regulators at
naic.org, including the specific states that have adopted,
modified, or declined to adopt the Bulletin after the
December 2023 model publication. -->

<!-- needs-research: verify the current state of the OECD AI
Principles (2019, updated 2024) and the OECD Framework for
the Classification of AI Systems at oecd.ai, including any
subsequent updates or related publications after the research
window. -->

<!-- needs-research: verify jurisdictional differences in the
twelve CxO coordination patterns across the enterprise's
operating jurisdictions. The references cited above are
primarily US-, UK-, and EU-anchored; enterprises operating in
APAC, LATAM, or Middle-East jurisdictions need parallel
primary-source references for the CPO / DPO, CRO, GC, CHRO,
and CCO adjacencies before the coordination patterns are
grounded for those jurisdictions. -->
