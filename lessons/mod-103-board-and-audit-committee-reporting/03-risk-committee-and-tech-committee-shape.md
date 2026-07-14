# The Risk-Committee (or Technology-Committee) AI Shape

## Motivation

Not every enterprise has a risk committee. Not every risk committee
has AI in scope. Enterprises with a mature enterprise-risk-
management function under a Chief Risk Officer typically do route
AI to the risk committee at board level. Enterprises without that
structure — or where the risk committee's scope is limited to
financial or operational risk — often route AI to a
technology-committee (or its equivalent, sometimes called a science
and technology committee, an innovation and technology committee, or
a digital committee) instead. Some enterprises route to both.

The head of AI governance does not choose the routing. The board
does, in the committee charters. The head's job is to author the
right shape of AI-risk pack for whichever committee the routing
lands at, and to be able to defend the same content in front of
whichever board committee is asking.

This chapter is the head's shape for the risk-committee (or
technology-committee) AI-risk deep-dive, layered onto the parent
frameworks that already govern enterprise risk — COSO ERM in most
US enterprises, ISO 31000 in most international enterprises, and
ISO/IEC 23894 as the AI-specific overlay.

## Core concept: the risk committee tunes appetite, the technology committee tunes deployment

The two committees have different centres of gravity, and the pack
respects the difference:

- The **risk committee** is about *appetite calibration*. It ratifies
  the enterprise's AI risk appetite, adjudicates escalations that
  test the appetite, and confirms that the second line is
  operating the appetite framework at portfolio scope. Its pack is
  weighted toward risk taxonomy, appetite statements, deviation
  analysis, and the interplay of AI risk with the parent risk
  categories (operational, technology, credit, market, insurance,
  patient-safety, cyber, legal, reputational).
- The **technology committee** is about *deployment posture*. It
  ratifies capability tiers and the pre-committed responses per
  tier, considers stop-shipping triggers and their exercise,
  reviews build-versus-buy and platform investment decisions, and
  looks at the AI supply chain from an operational-resilience
  angle. Its pack is weighted toward capability tiers, deployment
  gates, evaluation posture, and platform-and-vendor architecture.

Enterprises route AI to whichever of these has scope. Where both
have scope, the pack is authored once and split — the risk-committee
version emphasises the first bullet, the technology-committee
version emphasises the second — and the underlying evidence is
identical. The head does not maintain two truths.

## Parent frameworks the pack layers onto

The risk-committee pack does not invent a risk framework. It layers
AI-specific content onto whichever enterprise risk framework the
CRO has already established.

- **COSO Enterprise Risk Management — Integrating with Strategy and
  Performance (2017)** — the dominant framework in US enterprises.
  Its five components (governance and culture; strategy and
  objective-setting; performance; review and revision; information,
  communication, and reporting) frame the risk-committee's
  standing agenda. AI risk fits into the "performance" and "review
  and revision" components most naturally; the pack is authored so
  the committee can read it without re-mapping.
- **ISO 31000:2018** — the international guidelines-style parent
  framework. Its risk-management process (scope, context, criteria
  → identification → analysis → evaluation → treatment →
  monitoring → recording and reporting → communication and
  consultation) is the sequence the committee will assume the head
  is running against. The pack shows the sequence explicitly for
  AI at portfolio scope.
- **ISO/IEC 23894:2023** — AI-specific risk management guidance
  that specialises ISO 31000. This is the standard the head cites
  when the committee asks *why* the AI-risk process differs from
  the enterprise-risk process in specific places.

The committee is not being asked to endorse a new framework. It is
being asked to see that the AI overlay composes with the framework
already in force.

## The five-cluster risk-committee shape

### Cluster 1 — portfolio appetite calibration

The centrepiece. The committee is being asked to ratify (or adjust)
the AI risk appetite for the coming period.

- **Named appetite statements** — the current appetite statements
  the head runs the register against, expressed in the form the
  CRO's framework prescribes (qualitative bands, quantitative
  thresholds, tolerance intervals, or a mix). Each statement is
  cross-referenced to the risk category it constrains.
- **Position vs. appetite per statement** — the current portfolio
  position, prior-period position, distance from threshold. The
  same portfolio heat map that appears in the board pack, but at
  full resolution and with the underlying data tables.
- **Deviations from appetite in period** — where the portfolio
  exceeded appetite, temporarily or persistently, what triggered
  the deviation, what compensating actions were taken, and whether
  the appetite statement itself needs adjustment.
- **Committee decision requested** — ratify existing appetite;
  adjust a specific statement with rationale; add a new statement
  covering a category the current framework does not adequately
  address (a common ask for emerging capability areas).

### Cluster 2 — capability-tier posture and escalations

The committee sees the current capability tiers and the escalation
posture.

- **Capability tiers in force** — the tier framework the program
  operates (built to align with the level-50 architect's operating
  model and, for enterprises drawing on frontier-lab shape,
  patterned on the tiered frameworks discussed in chapter 07).
  For each tier: what qualifies a system for the tier, what
  pre-committed responses attach to the tier, what evaluation
  cadence applies, what deployment gates apply.
- **Systems in each tier** — the count and the tier-migration
  events in period (systems that moved up a tier as capability
  grew or new evidence emerged, systems that moved down after
  narrowing scope, systems newly onboarded).
- **Escalations in period** — where a system's evaluation or
  incident triggered escalation across tier boundaries, what the
  escalation path did, what the outcome was.
- **Stop-shipping triggers exercised** — where a pre-committed
  stop-shipping trigger fired (an evaluation failed, a serious
  incident occurred, a regulator opened an action, a supply-chain
  event withdrew a dependency), the response, the current status.
  Stop-shipping is disruptive; the committee sees each instance
  with root cause and forward-look.

Chapter 07 (frontier-lab tiered frameworks as shape lessons)
develops the tier discipline further.

### Cluster 3 — parent-risk composition

Where AI risk interacts with the parent risk taxonomy the committee
already governs. This is the cluster that makes the risk committee
see AI as an *overlay* rather than an *addition*.

For each parent risk category the enterprise runs (typical set:
operational, technology, cyber, model, credit, market, insurance,
patient-safety, legal, compliance, reputational), the pack shows:

- The AI-specific contribution to that category in period.
- Cross-category interactions AI has introduced (e.g. a
  third-party AI dependency introduces a concentrated technology-
  risk exposure that also creates an operational-risk exposure if
  the dependency fails).
- Whether the parent category's appetite has been affected.

For financial services enterprises the composition with
model-risk-management under Federal Reserve SR 11-7 (or the local
equivalent — OCC Bulletin 2011-12, OSFI Guideline E-23, EBA and
ECB model risk guidance in Europe) is particularly load-bearing.
The pack shows explicitly how AI systems are treated under the MRM
framework and where the AI governance program supplements versus
overlaps with model-risk management.

### Cluster 4 — treatment and monitoring at portfolio scope

The ISO 31000 sequence made visible.

- **Risk treatment in period** — treatments applied (avoid,
  transfer, mitigate, accept) at portfolio scope, and the
  aggregate effect on the appetite position.
- **Monitoring signal** — the KRIs the head runs against (a
  richer version of the board KRI dashboard), the trend, and any
  alarm the committee should note.
- **Continual improvement** — non-conformities and their closure,
  corrective action outcomes, management-review outputs that
  affect the risk framework.

### Cluster 5 — technology-committee-specific: build/buy, platform, and resilience

Where the routing is to a technology committee (or where the
technology committee shares scope with the risk committee), an
additional cluster.

- **Build/buy posture** — investment decisions in period on
  AI platforms (GRC-for-AI, evaluation tooling, monitoring
  tooling, model-serving infrastructure), platform-consolidation
  or split decisions, in-house versus vendor for specific
  capabilities.
- **Vendor and foundation-model concentration** — the concentration
  view from the board pack, extended with the operational
  implication and the resilience commentary.
- **Operational resilience** — for regulated enterprises, the
  composition with operational-resilience regulation (UK PRA / FCA
  operational-resilience regime; EU DORA for financial services;
  sector-specific business-continuity regimes) and how AI
  dependencies are treated as important business services.

## Cadence

Risk-committee cadence is typically quarterly, aligned with the
audit-committee cadence and the enterprise's risk-committee
schedule. Technology-committee cadence varies more; some enterprises
run it quarterly, some semi-annually, some on-demand around
significant technology initiatives.

Whichever cadence applies, the appetite-calibration exercise (cluster
1) is at least annual and is a specific board-committee agenda item
with named decisions and a written ratification.

## What the risk committee is watching for

Risk-committee members bring risk-management fluency. They are
watching for:

- Whether appetite statements are *specific enough to be measured
  against*. Vague appetite statements are the leading indicator of
  a program with no real appetite discipline.
- Whether deviations are surfaced honestly and treated, or
  quietly renamed and buried in a subcategory.
- Whether the parent-risk composition holds — whether AI is being
  treated as a new bolt-on category rather than an overlay on
  existing operational, technology, model, and cyber risk (a
  common failure mode).
- Whether capability tiers are *pre-committed* — the committee is
  looking for the discipline that the response at a tier was
  agreed *before* the escalation, not composed *after*.
- Whether stop-shipping triggers exist at all, and whether they
  have ever been exercised. A program that has never exercised a
  stop-shipping trigger under any circumstance is a program whose
  stop-shipping triggers are not real.

The head's pack is authored to make each of these visible.

## When routing changes

Reporting-line changes at enterprise scope are common (see
[[mod-101-role-scope-and-leadership-shape]] chapter 06 on CxO
positioning). When AI's routing moves — from risk committee to
technology committee, or the reverse, or from either to a newly
constituted AI committee — the head:

- Ratifies the new routing in writing with the board secretary or
  general counsel so the audit trail is clear.
- Retains parallel authoring of the deprecated committee's pack
  until the transition is minute-approved by both committees.
- Preserves the underlying evidence in the AIMS document control
  so any committee can request the same evidence at any time.

Routing changes are governance events. They are not the head's
choice to freelance around.

## Summary

- The risk committee tunes AI risk appetite at portfolio scope;
  the technology committee tunes deployment posture, capability
  tiers, and platform architecture. Some enterprises route AI to
  both; the head authors one truth and splits the emphasis.
- The pack layers onto the parent risk framework in force — COSO
  ERM, ISO 31000, ISO/IEC 23894 as the AI overlay — and shows
  the AI process as an overlay, not an addition.
- Five clusters: portfolio appetite calibration; capability-tier
  posture and escalations (including stop-shipping triggers);
  parent-risk composition (particularly with model-risk regimes
  in financial services); treatment and monitoring at portfolio
  scope; technology-committee-specific build/buy and resilience
  content.
- The committee is watching for measurable appetite statements,
  honest deviation reporting, parent-risk composition, pre-
  committed capability-tier responses, and stop-shipping triggers
  that have ever fired.
- When routing changes, the head ratifies the change with the
  board secretary in writing and preserves parallel authoring
  through the transition.
