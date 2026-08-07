# Insurance — Leading AI Governance Across State DOIs and the NAIC

## Motivation

Banking has a small number of federal supervisors and a shared
enterprise MRM regime. Insurance has neither. There is no federal
insurance regulator in the US — the McCarran-Ferguson Act reserved
insurance regulation to the states — and the enterprise's regulator
count is therefore the number of states it writes in, plus the
District of Columbia and the US territories where it operates, plus
the NAIC as the coordinating body. For a national insurer, that is
50+ regulators applying 50+ jurisdiction-specific variants of every
adopted model law.

That structural reality is the leadership challenge this chapter
opens with. A bank's head of AI governance runs a program that
answers to a handful of prudential and consumer regulators against a
small stack of instruments. An insurer's head of AI governance runs
a program that answers to a state-by-state adopter list against the
NAIC AI Model Bulletin, the state's own AI or algorithmic decisioning
statutes where the state has added them (Colorado is the most
significant example), the state's underlying unfair-trade-practice
and market-conduct statutes, and — for insurers that write in New
York — NYDFS's own circular letter on AI in insurance underwriting
and pricing. The head does not decide "how do we govern AI." The
head decides "how do we govern AI in Colorado, and in California,
and in New York, and in Texas, and in each other state, given that
each state's version of the NAIC bulletin varies from the model text
and each state's underlying statute predates AI by decades."

## Core concept — the two-axis regulatory map

The head maintains a regulatory map organised on two axes: state
(jurisdiction) and instrument-layer (obligation type). Every AI use
case in the enterprise's inventory has a matrix of applicable
regulators derived from the two axes.

### Axis one — jurisdiction

Every state the enterprise writes in is a separate entry in the
regulator inventory. The state's Department of Insurance (or, in a
few states, the Department of Financial Services or Department of
Commerce insurance division) is the primary supervisor. The state's
Attorney General is a parallel supervisor for AI-specific consumer-
protection matters that reach beyond insurance-specific statutes.

The head does not aggregate states into groups except with an
explicit aggregation rule the board can read. "Model-bulletin
adopting states" is an aggregation rule; "the states we write in"
is not.

### Axis two — instrument layer

For each state in the inventory, the head names three instrument
layers.

1. The state's underlying unfair-trade-practice, market-conduct,
   rate-approval, and unfair-discrimination statutes. These predate
   AI by decades and are the anchor obligation surface. AI-specific
   bulletins ride on top; they do not replace.
2. The state's adopted version of the NAIC AI Model Bulletin on the
   Use of Artificial Intelligence Systems by Insurers (adopted at
   the NAIC winter national meeting on 14 December 2023). Adoption
   is on a rolling basis. Where a state has adopted a variant that
   differs from the model text, the head cites the variant, not the
   model.
3. Any state-specific AI or algorithmic decisioning statute or
   regulation. Colorado's Regulation 10-1-1 on Governance and Risk
   Management Framework Requirements for Life Insurers' Use of
   External Consumer Data and Information Sources, Algorithms, and
   Predictive Models is the leading example; New York's Insurance
   Circular Letter No. 7 (2024) is the next; other states have
   state-specific bulletins, guidance, or open rulemakings.

<!-- needs-research: maintain a current list of state DOIs that have
adopted the NAIC AI Model Bulletin (in original or variant form),
that have opened rulemakings extending the bulletin, or that have
declined to act. Adoption is moving through 2025-2026 and the head's
inventory needs a dated source per state, not a paraphrase. Verify
against each state DOI's bulletin publications and the NAIC Big Data
and AI (H) Working Group summaries. -->

<!-- needs-research: verify the current effective status of Colorado
Regulation 10-1-1 (originally effective November 14, 2023) and any
subsequent amendments, including the extensions of scope beyond life
insurance that were consulted through 2024-2025. Confirm against
doi.colorado.gov. -->

## The three foundational instruments the head owns

### The NAIC AI Model Bulletin (adopted 14 December 2023)

The Model Bulletin frames AI-specific expectations against the NAIC
Model Unfair Trade Practices Act, the Model Unfair Claims Settlement
Practices Act, and existing market-conduct examination authority.
The head reads the bulletin as five substantive expectations that
each state's adopting version applies to the enterprise:

1. A written AI Systems Program (AIS Program) that governs the
   development, acquisition, use, and monitoring of AI systems
   throughout their lifecycle.
2. Governance structure with senior leadership accountability, risk
   assessment against enterprise objectives, and documented policies
   and procedures.
3. Risk-management controls addressing data governance,
   transparency, third-party AI acquisition, and testing and
   validation.
4. Internal audit or independent evaluation of the AIS Program.
5. Documentation demonstrating compliance and availability for
   state-DOI examination.

The head runs the enterprise AI Systems Program as the direct
answer to items 1-5. Where a specific state's adopted variant adds
requirements — enhanced disclosure, specified fairness testing,
additional documentation, notification triggers — the head layers
the state-specific requirement on top of the enterprise AIS Program
rather than running a separate state-specific program.

### Colorado Regulation 10-1-1

Colorado's Regulation 10-1-1 sits under Section 10-3-1104.9, C.R.S.
(unfair discrimination in insurance based on external consumer data
and information sources or algorithms and predictive models). The
regulation, originally directed at life insurers, requires a
documented governance and risk-management framework covering
external consumer data, algorithms, and predictive models, and
requires ongoing testing for unfairly discriminatory outcomes. The
head reads Regulation 10-1-1 as the current best-articulated state-
level standard for what "unfair discrimination through algorithms"
means operationally, and treats the framework as the maturity
benchmark for the enterprise's AIS Program even in states that have
not adopted an equivalent instrument.

<!-- needs-research: verify the current scope of Colorado Regulation
10-1-1 including whether it has been extended to lines of business
beyond life insurance through 2024-2026 rulemaking. Confirm against
doi.colorado.gov and Colorado Division of Insurance regulatory
alerts. -->

### NYDFS Insurance Circular Letter No. 7 (2024)

NYDFS's Circular Letter No. 7 (11 July 2024) sets NYDFS's
expectations for insurers writing in New York on the use of AI
systems and external consumer data and information sources in
underwriting and pricing. The circular's requirements — governance
and risk management, fairness and disparate-impact testing, third-
party AI provider oversight, disclosure — track the NAIC bulletin's
architecture but are enforceable as NYDFS's own supervisory
expectations from the date of issue. For an insurer writing in New
York, the head treats the NYDFS circular as an operating obligation
alongside the state's adopted NAIC bulletin variant, whichever is
more stringent per topic.

## External actuarial coordination — AI-driven pricing and underwriting

Every material AI system used in pricing or underwriting has an
actuarial dimension. The state DOI expects an appointed actuary or a
consulting actuary to have signed off on rate structure, pricing
methodology, and unfair-discrimination testing where the state
requires it. The head coordinates with the enterprise's Chief
Actuary and, for retained external actuarial firms, with the lead
consulting actuary, on four points:

1. The AI system's role in the pricing or underwriting decision is
   described in the actuarial memorandum in language a state DOI
   actuary reviewer can follow. "Machine learning model produces
   rating factor" is not sufficient; the memorandum specifies input
   features, model class, calibration methodology, and post-hoc
   monotonicity or clustering adjustments the actuary made to
   produce a filable structure.
2. Disparate-impact and unfair-discrimination testing is executed to
   a methodology that satisfies the state's expectations. In
   Colorado, this is Regulation 10-1-1's documented testing
   methodology. In states where the bulletin has been adopted
   without specific testing methodology, the enterprise's testing
   methodology is defensible against the NAIC bulletin's fairness
   expectation.
3. The rate filing or form filing that supports the AI-driven
   product includes the AI-specific documentation the state expects
   under its adopted bulletin. The Chief Actuary owns the filing
   itself; the head owns the AI-specific technical content that
   goes into the filing.
4. The ongoing monitoring feedback loop — actual-vs-expected loss
   experience, actual pricing outcomes vs projected, actual
   disparate-impact metrics vs prior testing — reaches both the
   actuary (for reserving and reserving-adequacy purposes) and the
   AIS Program (for ongoing-monitoring purposes). The two functions
   are looking at the same underlying data with different
   objectives, and a mismatch between the two views is a supervisory
   risk the head anticipates.

American Academy of Actuaries practice notes and the Actuarial
Standards Board's Actuarial Standards of Practice — particularly ASOP
No. 12 (Risk Classification) and ASOP No. 56 (Modeling) — set the
external professional standard the actuary works to. The head reads
both, understands what the actuary must certify to, and does not
place the actuary in a position where certifying requires a
representation the AI evidence does not support.

<!-- needs-research: verify the current issued status of Actuarial
Standards of Practice specifically addressing AI/ML models in
insurance, including any updates to ASOP No. 56 (Modeling) or new
ASOPs on algorithmic fairness. The ASB has active exposure drafts;
confirm current status against actuarialstandardsboard.org. -->

## Consumer-facing AI obligations in insurance

Beyond pricing and underwriting, the head owns the AI-specific
dimensions of two consumer-facing surfaces the state DOI supervises.

1. Claims handling. AI-driven claims triage, claim severity
   prediction, and fraud-detection systems attach to the state's
   Unfair Claims Settlement Practices Act. The NAIC bulletin
   applies. A denial or reduction driven materially by an AI system
   needs to be defensible against the state's fair-claims-handling
   standard, and the head owns the AI-specific evidence supporting
   the defence.
2. Marketing and distribution. AI-driven quote personalisation,
   agent-facing recommendation systems, and consumer-facing chatbots
   attach to the state's unfair-trade-practice authority. The FTC
   Section 5 layer (FTC Section 5 applies to insurance where the
   FTC's authority reaches, which varies by state and by product)
   and state Attorney General consumer-protection authority sit
   alongside.

Neither surface is exclusively the head's — the Chief Compliance
Officer, the Chief Claims Officer, and the Chief Marketing Officer
front their respective functions — but each surface has an AI-
specific dimension the head is accountable for.

## State-DOI examination cadence and the head's response capacity

State-DOI market-conduct examinations run on a rhythm that varies by
state — every three to five years is common, event-driven is
frequent for large or troubled writers. Rate-filing review is
continuous for lines of business the state approves prior to use.
Data calls are event-driven or annual depending on the state and
the topic.

The head's response capacity is designed around the cadence. For
market-conduct examinations, the head runs an evidence pipeline that
can be reconstituted on notice — a state that examines the enterprise
every fourth year expects the enterprise to reconstruct the
intervening years' evidence when asked. Reconstruction requires the
underlying artefacts (the actual model versions in production during
each year, the actual monitoring metrics for each year, the actual
disparate-impact test results the enterprise ran and acted on) to
have been captured contemporaneously. The head does not build
evidence to answer a specific examination; the head captures evidence
continuously so any examination can be answered from the archive.

Escalation runs through the state's sector-specific vocabulary.
Deficiencies noted in the examination report trigger response
letters. Formal enforcement actions from the state DOI take the form
of consent orders, market-conduct action plans, or, in serious
cases, licence conditions or licence suspension. Rate-filing
disapprovals require the enterprise to withdraw and refile with the
AI-specific documentation the state has specified. Consumer
complaints filed with the state DOI (the NAIC's Complaint Index is a
public indicator the head monitors) drive examination priorities.

At the multi-state coordinated examination level, the NAIC's
Market Analysis Working Group and Market Actions Working Group
coordinate examination activity across states for large multi-state
writers. Where the enterprise is targeted for a coordinated
examination, the head owns the AI-specific coordination across every
state's participating team.

## The head's relationship with the enterprise's Chief Actuary and Chief Underwriting Officer

The head of AI governance at an insurer sits inside a triangle with
the Chief Actuary and the Chief Underwriting Officer. Each of the
three has a distinct accountability the other two rely on.

- The Chief Actuary certifies rate structures and reserving, signs
  actuarial memoranda, and answers to state DOI actuary reviewers.
- The Chief Underwriting Officer owns underwriting judgment
  (including AI-augmented judgment), owns the underwriting workflow
  the AI system participates in, and answers to state DOI examiners
  on underwriting practice.
- The head of AI governance owns the AI-specific dimensions — model
  documentation, validation, disparate-impact testing, monitoring,
  documentation for state examination — that both the actuary and
  the CUO rely on to sign their respective certifications and
  defend their respective judgments.

The three functions are governed by a joint operating protocol,
written down, that names who owns what at each stage of the AI-in-
pricing lifecycle: model development, actuarial calibration,
underwriting deployment, rate filing, ongoing monitoring, and
retirement. The protocol is signed by all three and ratified at the
audit-committee level. Its purpose is to prevent the state DOI from
receiving a split answer at examination where the actuary's memo,
the CUO's underwriting manual, and the AIS Program documentation
each imply a different version of what the AI system does and why.

## The head's board-level story

At the audit committee, insurance AI governance is a story with
three recurring beats.

1. The AIS Program is running to a standard defensible against the
   NAIC bulletin baseline, the state-specific overlays where they
   apply (Colorado, New York, and any other state whose overlay is
   more stringent than the model), and the underlying unfair-trade-
   practice and market-conduct authority in every state the
   enterprise writes in.
2. The pricing and underwriting AI portfolio is coordinated across
   the head, the Chief Actuary, and the Chief Underwriting Officer,
   with a written protocol the board can read and a rate-filing
   record the board can inspect.
3. The state-DOI regulatory posture is coherent per state, coherent
   in aggregate across the state footprint, and directly tied to the
   regulator inventory the head maintains (see
   [[mod-104-regulator-engagement]] chapter 04). Where a state has
   opened an examination or issued a data call, the board sees the
   status; where a rate filing has been disapproved or a market-
   conduct action plan is in force, the board sees the milestone.

## Summary

- Insurance is regulated state-by-state, and the head's regulatory
  map has two axes: jurisdiction (per-state) and instrument-layer
  (underlying state statute, NAIC AI Model Bulletin as adopted,
  state-specific AI or algorithmic decisioning instrument).
- The three foundational instruments the head owns are the NAIC AI
  Model Bulletin (adopted 14 December 2023), Colorado Regulation
  10-1-1 (originally effective 14 November 2023), and NYDFS
  Insurance Circular Letter No. 7 (11 July 2024). Each rides on
  top of underlying non-AI-specific statutes.
- The enterprise AI Systems Program (AIS Program) is the direct
  answer to the NAIC bulletin's five substantive expectations —
  governance, written program, risk-management controls,
  independent evaluation, and documentation — with state-specific
  overlays layered on top.
- External actuarial coordination is a first-class dimension of
  the head's role. The head and the Chief Actuary jointly own the
  AI-specific technical content of actuarial memoranda and rate
  filings against the ASOP standards.
- Consumer-facing AI in insurance — pricing, underwriting, claims
  handling, marketing — attaches to the state's unfair-trade-
  practice and unfair-claims-settlement authority; the head owns
  the AI-specific evidence supporting the defence at each surface.
- The examination cadence runs on state-DOI market-conduct cycles
  that vary by state; the head's response capacity is a
  reconstitutable evidence pipeline captured continuously, not an
  examination-triggered evidence build.
- The head, Chief Actuary, and Chief Underwriting Officer operate
  under a written joint operating protocol that prevents the state
  DOI from receiving a split answer at examination.
- The board-level story has three beats: AIS Program defensible
  against the NAIC baseline plus state overlays; pricing and
  underwriting coordinated across head, Chief Actuary, and CUO;
  state-DOI posture coherent per state and in aggregate, feeding
  cluster 4 of the quarterly board pack in
  [[mod-103-board-and-audit-committee-reporting]].
