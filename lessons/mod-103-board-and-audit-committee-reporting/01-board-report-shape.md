# The Board-Facing AI-Risk Report Shape

## Motivation

The quarterly board pack is where the AI governance program either
looks like a running program or looks like a science project. Boards
do not read the AIMS. Boards do not read the risk register. Boards
read the pack the head of AI governance puts in front of them, and
they form their oversight judgement — the judgement a regulator, a
court, or an incoming director will later interrogate — almost
entirely from what that pack shows.

The pack has to do three things at once. It has to give the board
enough signal that a director who does not read AI research can form
an informed view of where the risk is trending. It has to be
defensible under adversarial reading — a plaintiff's counsel, a
regulator asking "what did the board know and when?", a new director
onboarding from prior minutes. And it has to be *comparable across
quarters*, so trend is visible, not just point-in-time state.

Frontier labs already publish tiered risk frameworks that describe
what their own governing bodies see (Anthropic's Responsible Scaling
Policy, OpenAI's Preparedness Framework, Google DeepMind's Frontier
Safety Framework — chapter 07 discusses these as shape lessons).
Enterprise boards are moving toward comparable shape. The IoD's AI
governance guidance for boards and the NACD's AI-oversight
publications are the reference shapes for that move. This chapter is
the head's shape for the quarterly board pack.

## Core concept: the pack answers three board questions in a fixed order

The board is not asking "what does the AI governance team do?" The
board is asking three questions, and the pack answers them in this
order or it fails:

1. **Has the enterprise's AI risk profile changed since last quarter,
   and is it inside appetite?** If the answer is yes-and-yes, the
   board can move on. If no, the board needs to understand what
   changed and what is being done about it.
2. **Where are we exposed that a director would want to know about?**
   Concentrated third-party dependencies, active regulator
   engagements, near-miss incidents, appetite-edge portfolios,
   pending regulatory change — the specifics that would make a
   director uncomfortable if surfaced first by a journalist or a
   subpoena rather than by the pack.
3. **What decisions is the board being asked to take, or ratify, or
   note?** If nothing, say so explicitly. If something, the ask is
   phrased as a decision — accept / reject / defer with a reason —
   not as a discussion topic.

Every section of the pack maps to one of the three. Sections that
answer none of the three are removed. Sections the board has to hunt
through to find the answer are re-organised.

## The seven-cluster shape

A defensible quarterly board pack for AI risk has seven content
clusters. The exact naming varies by enterprise convention; the
clusters do not.

### Cluster 1 — appetite and portfolio heat map

Two artefacts, one page.

- **A portfolio heat map** — the AI system inventory summarised
  against the risk taxonomy the level-50 architect chartered
  (safety / security / privacy / fairness / IP / robustness /
  transparency / accountability, or the local taxonomy) with cell
  colour showing the aggregated risk position and cell count showing
  the number of systems in that cell. The board learns
  concentration ("we have twelve customer-facing GenAI systems all
  at amber on privacy") not just headline counts.
- **A portfolio appetite tracker** — for each named appetite
  statement (from mod-102 chapter 03 — the enterprise AI risk
  register), the current position, prior-quarter position, and the
  distance to threshold. If a statement is *at* threshold or
  *breached*, it is highlighted and referenced to a specific
  decision item in cluster 7.

Heat maps are visual shorthand and they lie by aggregation. The
board pack accompanies every heat map with a two-sentence "what has
moved since last quarter" caption. Without the caption the heat map
is decoration.

### Cluster 2 — KRI dashboard

A single page of key risk indicators, each with:

- Definition (one line — what this indicator measures).
- Current value and prior-three-quarter trend (spark line or short
  table).
- Threshold (green / amber / red bands agreed with the CRO under
  the parent enterprise risk framework — COSO ERM in most US
  enterprises, ISO 31000 elsewhere).
- Movement commentary if amber or red.

Typical AI-KRIs the head reports (the specific list is the head's to
tune with the CRO):

- Number of AI systems in inventory by capability tier.
- Number of policy exceptions live, aged, and expiring in period.
- Incident and near-miss count in period by severity.
- Third-party vendor status by tier (in-good-standing, remediating,
  suspended).
- Time-to-close on third-line audit findings by severity.
- Regulator correspondence volume and open-item aging.
- Model-monitoring drift and performance-degradation alarms in
  period.
- Evaluations conducted in period against expected cadence.

The dashboard does not tell the board what to do. It tells the board
what is moving. Decisions live in cluster 7.

### Cluster 3 — incident and near-miss summary

The board sees every incident that would be reportable under the
serious-incident regime that applies to the enterprise (EU AI Act
Article 73 for EU-market high-risk deployments, sector regulator
regimes elsewhere — see [[mod-110-incident-leadership]] for the
incident-leadership discipline). The board also sees near-misses at
a threshold agreed in advance with the audit committee.

Per incident, the summary is at most half a page:

- Incident ID, dates (occurred, detected, contained, closed).
- AI system(s) involved and risk taxonomy category.
- One-paragraph factual summary — what happened, no attribution
  of blame, no analysis.
- Regulatory reportability status (reported, in-report-preparation,
  determined non-reportable with rationale).
- Containment and remediation status.
- Board-level implications — reputational, financial, regulatory,
  operational — and any board decision requested.

Incidents that would surface first through a journalist or subpoena
if not in the pack are the exact incidents the pack exists to
surface.

### Cluster 4 — regulator engagement summary

A one-page-per-jurisdiction summary of active regulator
engagements. The General Counsel (or the chief compliance officer,
depending on reporting-line — see [[mod-101-role-scope-and-leadership-shape]]
chapter 06) owns the content of this cluster; the head coordinates
authoring and sign-off (chapter 04 of this module covers the CxO
sign-off flow).

Per engagement, the fields:

- Regulator, jurisdiction, and legal instrument at play (EU AI Act
  Article 26 / Article 72 / Article 73; sector regulator citation;
  consumer-protection agency citation; etc.).
- Nature of the engagement (proactive notification, information
  request, examination, formal action, consent order compliance,
  routine reporting).
- Enterprise counterpart named (who at the enterprise is the
  regulator's contact).
- Status and next-action-by-date.
- Board-decision needed (typically none; occasionally: authorise
  external counsel spend, authorise a settlement position,
  authorise a public disclosure).

Where the pack lists no active engagement in a jurisdiction the
enterprise operates in and the regulator is active in AI, that fact
itself is worth noting.

### Cluster 5 — third-party vendor and AI supply chain status

The board sees concentration and change. Not every vendor.

- **Concentration** — top vendors by AI-system dependency, top
  foundation-model providers by inference volume or by number of
  downstream systems, top data-labelling / evaluation providers by
  spend or by number of dependent systems. Concentration is the
  systemic-risk signal boards need.
- **Change since last quarter** — vendors added, vendors moved
  between tiers, vendors suspended or terminated, contractual
  disputes (with GC coordination).
- **Attestation posture** — the proportion of AI-relevant vendors
  with current SOC 2 Type 2 / ISO 27001 / ISO 42001 / relevant
  sector attestations, and the tail of vendors without.

See [[mod-102-running-the-program]] chapter 07 (AI supply-chain
evidence discipline) for the operating side of this cluster.

### Cluster 6 — regulatory change and program-maturity update

Two adjacent updates, half a page each.

- **Regulatory change in period** — new obligations that came into
  force, obligations coming into force in the next reporting window,
  material guidance updates from named regulators (EU AI Office,
  NIST AISI, sector regulators, ICO / CNIL / other DPAs, etc.).
  Each item is annotated with the enterprise's assessed exposure and
  the current program response. See
  [[mod-105-regulatory-change-management]] for the operating
  discipline.
- **Program maturity update** — the point-in-time position on the
  reference maturity plot the program tracks against (NIST AI RMF
  Playbook maturity dimensions, ISO/IEC 42001 AIMS maturity, OWASP
  AI Security & Governance Checklist coverage — see
  [[mod-107-program-measurement-and-maturity]]). The board sees
  trajectory, not detail.

### Cluster 7 — board decisions requested

The last cluster is the ask. Every item is written as a decision:

- Item title and one-sentence context.
- Specific decision requested (approve / accept / ratify / note),
  with wording the board can adopt verbatim.
- Owner accountable for execution if approved.
- Review or reporting-back trigger.
- Dissent-capture mechanism (the standing convention the board
  minutes use, referenced by the pack for clarity).

If there are no board decisions requested this quarter, the cluster
says so and lists what the board will be asked to decide next
quarter. Empty asks are visible; ambiguous asks are hidden asks and
they generate audit findings.

## Cadence, comparability, and archive

The pack is quarterly at primary cadence with a monthly written
delta between formal quarters (a one-page written update sent to
the audit-committee chair and the risk-committee chair; the delta
is captured in the pack archive but not tabled). This is a common
shape; heavily-regulated enterprises run monthly primary cadence.

Comparability across quarters is a property of the pack, not of any
individual quarter. That means:

- Section headings do not change quarter to quarter without a
  formally-tabled rationale.
- KRI definitions do not change without a formally-tabled rationale
  and a restated prior-quarter comparator.
- Heat map cell definitions do not change without a formally-tabled
  rationale.
- Archived packs are locked and version-controlled; amendments are
  errata, not edits.

Boards notice when the shape moves under them. A pack that changes
its KRI list every quarter is a pack that has stopped being an
oversight instrument and has become a positioning instrument. The
head does not let that happen.

## The one thing to hold in the pack — appetite

If the head has to compress the pack to one sentence, that sentence
is: *the enterprise's AI risk position, expressed against the
board-ratified appetite, moved this way this quarter, for these
reasons, and here is what has been done about it.* Every cluster is
in service of that sentence. Every KRI, heat-map cell, incident
summary, regulator engagement update, and third-party status point
either substantiates the sentence or clarifies it. Clusters that do
neither are cut.

## Reference shapes to consult, not to copy

The IoD's AI-governance guidance for boards and the NACD's AI
Oversight publications are the closest thing the discipline has to
board-consensus references for what boards should be asking about
AI. They are shape references, not templates — every enterprise
tunes to its sector, its regulator profile, its portfolio, and its
board composition. Chapters 02 (audit committee) and 03 (risk /
technology committee) of this module extend the shape to the
committees that receive deeper cuts.

The frontier-lab tiered-risk frameworks — Anthropic's Responsible
Scaling Policy, OpenAI's Preparedness Framework, Google DeepMind's
Frontier Safety Framework — are useful shape references even for
enterprises that are not frontier labs. Chapter 07 draws out which
shape lessons transfer. The short version: the discipline of naming
capability tiers, naming pre-committed responses at each tier, and
naming stop-shipping triggers with owners is the discipline
enterprise boards will increasingly expect.

## Summary

- The board pack answers three questions in order: has risk moved
  and is it inside appetite; where are we exposed that a director
  would want to know; what decisions are requested.
- Seven content clusters — heat map and appetite tracker, KRI
  dashboard, incident and near-miss summary, regulator engagement
  summary, third-party and supply-chain status, regulatory change
  and maturity update, decisions requested.
- Quarterly primary cadence with monthly written deltas; every
  archived pack is locked and comparable across quarters.
- Every heat map has a "what moved" caption; every KRI has a trend;
  every incident has reportability status; every ask is a specific
  decision.
- IoD and NACD publications are shape references, not templates;
  frontier-lab tiered-risk frameworks (Anthropic RSP, OpenAI
  Preparedness, Google DeepMind FSF) are useful shape lessons for
  where enterprise expectations are heading (chapter 07).
