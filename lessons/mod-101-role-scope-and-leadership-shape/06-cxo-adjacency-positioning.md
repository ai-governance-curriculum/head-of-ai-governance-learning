# CxO Adjacency Positioning — So the Boundary Is Not a Debate Every Quarter

## Motivation

Every quarter that the AI Governance function has to *renegotiate* its
boundaries with the CRO, the CCO, the CPO / DPO, the CAE, the GC, the
CISO, the CIO / CTO / CDO, the Chief Communications Officer, or the
CAIO, the head loses time, credibility, and executive capital. The
boundary should be written down once, ratified by the CEO or the
audit committee, and revisited only on material change.

That written boundary is the CxO adjacency map. It answers, for each
adjacent officer, three questions: **what do they own that we do
not?** — **what do we own that they do not?** — **what do we own
jointly, and who arbitrates?** Three lines per adjacency, one page
per set, ratified once, referenced every time the boundary is
challenged.

This chapter is that map, drawn tightly. It is not exhaustive; every
enterprise's specifics differ. But the *shape* below is defensible
across enterprises, and it lets the head arrive at week one already
in possession of a defensible boundary — not one they have to invent
in argument.

## The nine adjacencies that dominate the head's time

At level 60, nine adjacencies show up in almost every enterprise. In
alphabetical order by title-family, they are the CAE (Chief Audit
Executive), CAIO (Chief AI Officer, where the designation exists),
CCO (Chief Compliance Officer), Chief Communications Officer, CISO
(Chief Information Security Officer), CIO / CTO / CDO
(Chief Information / Technology / Data Officer), CPO / DPO (Chief
Privacy Officer / Data Protection Officer), CRO (Chief Risk Officer),
and GC (General Counsel / CLO). The Head of Model Risk Management
(HoMRM) is included in banking-sector enterprises as a tenth
adjacency; the Chief Medical Officer (CMO) is included in health
system enterprises.

Below, each adjacency gets a three-line boundary. In every case the
head *does not* absorb the other officer's scope; the head defines the
AI-specific extension the other officer needs the head for.

## Chief Risk Officer (CRO)

- **They own:** the enterprise risk framework at parent scope (COSO
  ERM or ISO 31000), the risk appetite framework at enterprise
  scope, the enterprise risk register, and the risk-committee report
  line to the board.
- **We own:** the AI risk taxonomy, the AI-specific appetite
  translation, the AI risk register at portfolio cadence that
  contributes to the enterprise register, and the second-line
  challenge for AI-specific first-line decisions.
- **Jointly, arbitrated by:** the risk committee. The CRO is the
  enterprise risk parent; the head extends into AI. In many
  enterprises the head reports solid-line to CRO (see
  [[07-engagement-contract-authoring]]). Independent audit-committee
  access is preserved regardless of that reporting line.

## Chief Compliance Officer (CCO)

- **They own:** the enterprise compliance program at parent scope,
  the compliance-monitoring function, and the compliance report line
  to the audit committee.
- **We own:** the AI-specific regulatory obligations — EU AI Act,
  sector rules for AI/ML (SR 11-7 with AI extensions, GMLP, NAIC AI
  Model Bulletin, state AI acts, CPPA ADMT, NYC LL 144), voluntary
  codes — with the crosswalk owned by the level-50 architect and the
  operational compliance run by the head's team.
- **Jointly, arbitrated by:** the audit committee or the CEO. The
  boundary is: enterprise-scope compliance belongs to CCO; AI-scope
  compliance belongs to the head; both roles' compliance reports fold
  into the CCO's report to the audit committee.

## Chief Privacy Officer / Data Protection Officer (CPO / DPO)

- **They own:** the enterprise privacy program at parent scope,
  ROPA / Article 30 records, GDPR / CCPA / DPDPA / PIPEDA compliance
  at enterprise scope, and the DPIA methodology.
- **We own:** the AI-specific privacy extension — AI impact
  assessment (ISO/IEC 42005) that interfaces with DPIA where
  personal data is processed, automated-decision-making obligations
  under GDPR Article 22 and CPPA ADMT, and AI-specific privacy risk
  in the AI risk register.
- **Jointly, arbitrated by:** an explicit interface document,
  written and signed. The AIA-DPIA interface is one of the most
  contested boundaries in the field; the head who does not have this
  interface in writing will lose every quarter arguing it. Typical
  pattern: DPO is the accountable executive for DPIA; head is the
  accountable executive for AIA; the two are co-signed for any AI
  system that processes personal data.

## Chief Audit Executive (CAE)

- **They own:** third-line internal audit under IIA IPPF; audit
  independence; audit plan authorship; audit-committee report line.
- **We own:** second-line function; no involvement in third-line
  audit planning; provision of evidence access to third line.
- **Jointly, arbitrated by:** the audit committee. The CAE and the
  head are peers. Neither reports to the other. Joint audit-committee
  appearance annually, at minimum. See
  [[04-three-lines-at-leadership-scope]] on the invariants.

## General Counsel / Chief Legal Officer (GC / CLO)

- **They own:** legal opinions on regulatory interpretation,
  litigation posture, subject-access-request (SAR) management,
  Memoranda of Understanding (MOU) and Mutual Recognition
  Arrangements (MRA), attorney-client privilege on incident
  investigations, and enforcement-defence strategy.
- **We own:** engagement with regulators on operational matters
  (Article 72, Article 73, sector exam coordination),
  operational obligations under regulation, and the compliance
  operating discipline. The head files with regulators; the GC
  advises on legal exposure.
- **Jointly, arbitrated by:** the CEO. The critical distinction is
  *engaging* a regulator (head) versus *delivering a legal opinion*
  (GC). Any regulator interaction where legal privilege attaches
  becomes GC-led; any operational interaction is head-led. Both are
  briefed on the other's activity.

## Chief Information Security Officer (CISO)

- **They own:** enterprise cybersecurity under CSF 2.0 or equivalent,
  ISMS under ISO/IEC 27001, security operations, DFIR, and the
  security report line.
- **We own:** the AI-specific extension of cybersecurity — prompt
  injection, model extraction, adversarial-ML, training-data
  poisoning, jailbreak-driven downstream harm, and the joint
  interface with SOC on AI-signal detection. The head does not run
  the SOC.
- **Jointly, arbitrated by:** CSF 2.0 composition and the CISA / NCSC
  Guidelines for Secure AI System Development (2023). The CISO's
  runbook has the head's AI-specific extensions; the head's runbook
  respects the CISO's SOC ownership. Joint report to the audit
  committee for any AI-security incident.

## CIO / CTO / CDO

- **They own:** the enterprise data platform, AI platform, model
  registry, MLOps discipline, and the technology delivery
  accountability for AI systems. The CDO owns the data
  governance parent framework.
- **We own:** the AI system inventory quality bar at second-line
  scope; the model-and-system-card evidence discipline; the release-
  assurance sign-off at second-line scope; and the AI-specific
  extension to data governance for training and evaluation data.
- **Jointly, arbitrated by:** the AI governance council (chaired by
  head with CIO / CTO / CDO members) and, on escalation, the CAIO or
  CEO. The head does not build the model registry; the head requires
  it to feed the AIMS evidence store, and the interface is designed
  jointly with the level-50 architect.

## Chief Communications Officer (CCO — Communications)

- **They own:** enterprise communications strategy, crisis
  communications runbook, media relations, and the public-trust
  posture at enterprise scope.
- **We own:** the *content* of AI-specific communications — what to
  say about an AI incident, what a voluntary-code sign-on obligates,
  how to handle a regulator's public statement about the
  enterprise's AI — with the Communications officer owning the
  *channel* and *cadence*.
- **Jointly, arbitrated by:** the CEO. In a crisis, the head is on
  the incident bridge and briefs the Communications officer; the
  Communications officer briefs the CEO and the public. Never
  reverse.

## Chief AI Officer (CAIO)

- **They own:** AI strategy, AI portfolio P&L, external positioning
  at CEO / board-seat scope, enterprise-wide AI budget envelope. See
  chapter 01 and [[07-engagement-contract-authoring]].
- **We own:** the second-line function; the AI risk register; the
  regulator interface; the AIMS operating discipline; the AI
  governance function budget as a line inside the CAIO's envelope
  (or negotiated directly with CFO where no CAIO exists).
- **Jointly, arbitrated by:** the CEO or, in some enterprises, the
  board. Where the CAIO designation exists, the head typically
  reports to or matrixes with the CAIO. Independent audit-committee
  access remains an invariant.

## Sector-specific adjacencies

Two sector-specific adjacencies matter enough to name explicitly:

- **Head of Model Risk Management (HoMRM), banking.** In a banking
  enterprise the head coordinates with the HoMRM on SR 11-7 / OCC
  2011-12 / SR 23-4 / OSFI E-23 model risk. In some enterprises the
  head *is* the HoMRM (AI/ML extension of MRM); in others they are
  peers. Boundary: HoMRM owns all model risk (credit, market,
  operational, AI/ML) under SR 11-7; head owns the AI/ML extension
  and the parts of AI risk that fall outside the classical
  model-risk envelope (fairness, transparency, human oversight,
  agentic risk). Jointly-arbitrated by the CRO.
- **Chief Medical Officer (CMO), health system.** In a health system
  the head coordinates with the CMO on clinical governance of AI-
  enabled clinical decision support and SaMD (Software as a Medical
  Device). Boundary: CMO owns clinical decision authority and the
  medical-staff bylaws; head owns the AI-specific extension of
  governance around SaMD (FDA GMLP, PCCP) and the clinical-AI risk
  register. Jointly-arbitrated by the CEO and the medical-staff
  executive committee. See [[mod-111-sector-program-leadership]].

## The three failure patterns to prevent

Three failure patterns in adjacency management are worth naming so
the head can spot them early.

- **Turf war.** Two officers each claim the same scope; the audit
  committee sees two contradictory reports. Prevented by written,
  ratified boundaries and by joint reports on shared boundaries.
- **Silent abdication.** No officer claims a scope; the risk falls
  through the cracks. Common at the head / CISO boundary on
  AI-specific security. Prevented by explicit joint-signoff on
  AI-security controls and by an AI risk register line that catches
  anything falling into the gap.
- **Silent expansion.** One officer quietly extends into another's
  scope over a quarter, and the boundary shifts without ratification.
  Prevented by an annual boundary-review conversation in the audit
  committee, with both officers present.

## Example — a one-page ratified boundary sheet

An audit-committee-ratified one-page boundary sheet, for each
adjacency, lists:

- **Adjacent officer** (title, name).
- **They own** (three bullets).
- **We own** (three bullets).
- **Joint** (one to three bullets).
- **Arbitrated by** (named body — audit committee / risk committee /
  CEO / board).
- **Review cadence** (annual / on material change).
- **Signature date and next review** (dates).

Nine sheets (plus sector-specific), ratified in one audit committee
sitting, revisited annually. That is what a defensible CxO adjacency
map looks like at level 60.

## Summary

- Nine CxO adjacencies — CAE, CAIO, CCO (Compliance), Chief
  Communications, CISO, CIO / CTO / CDO, CPO / DPO, CRO, GC —
  dominate the head's boundary-management time. Sector-specific
  adjacencies (HoMRM, CMO) add a tenth.
- For each adjacency, the head writes a three-line boundary — they
  own / we own / joint — plus the arbitration body and review
  cadence, and gets it ratified once by the audit committee or the
  CEO.
- The head *engages* regulators; the GC delivers *legal opinions*.
  The head extends the CISO's CSF into AI; the CISO runs the SOC.
  The head runs the AIMS; the CIO / CTO / CDO run the AI platform.
  The head coordinates with the CAE; the CAE owns third-line audit
  independence.
- Turf war, silent abdication, and silent expansion are the three
  failure patterns. Prevented by written boundaries, joint sign-off
  on shared scope, and an annual boundary review.
- A ratified boundary sheet — nine to eleven pages, one per
  adjacency — is the artefact this chapter maps to. Exercise 5 in
  this module asks the learner to draft one.
