# Running the Enterprise AI Risk Register at Portfolio Cadence

## Motivation

A risk register that is *authored* — with named risks, taxonomy tags,
appetite thresholds, and treatment plans — is not the same as one that
is *running*. A running risk register moves. Risks are opened, tagged,
tracked against appetite, escalated when they deviate, treated,
re-scored, and closed with root cause. New risks arrive by intake
channels — incident reports, near-misses, red-team results,
horizon-scan output from the level-50 architect, regulator
correspondence, third-party notifications, and the AI system inventory
change log — and land in a triage discipline that decides in-scope,
severity, initial score, and owner within a bounded window.

The head of AI governance owns the *operating discipline* of the risk
register at portfolio cadence. The level-50 architect designed the
taxonomy — the risk categories, the scoring model, the appetite-
setting framework, the escalation trigger definitions. The head runs
the register so that at any moment the enterprise can answer: which AI
risks are inside appetite, which are outside appetite, which are
approaching threshold, which have owners with due-dated treatments,
and how the aggregate portfolio is trending.

This chapter is how to run the register in that shape, using ISO 31000,
ISO/IEC 23894, and ISO/IEC 27005 as parent references.

## Core concept: three parent standards, one operating discipline

Three ISO standards, in composition, define the shape of a defensible
enterprise risk-management discipline for AI:

- **ISO 31000:2018 — Risk management guidelines.** The enterprise-
  agnostic parent. Defines the risk-management process (scope-context-
  criteria; assessment via identification, analysis, and evaluation;
  treatment; monitoring and review; recording and reporting;
  communication and consultation).
- **ISO/IEC 23894:2023 — Guidance on AI risk management.** ISO 31000
  applied to AI. Adds AI-specific risk sources — data quality,
  algorithmic bias, model brittleness, human-AI interaction failure,
  emergent behaviour, and so on — and AI-lifecycle-specific
  considerations. Non-certifiable guidance.
- **ISO/IEC 27005:2022 — Information security risk management.** The
  ISMS-specific risk-management guidance under ISO/IEC 27001. Where
  AI risk touches information security (a substantial fraction — data
  poisoning, model theft, prompt injection, training-data exposure,
  supply-chain compromise), the AI risk register composes with the
  ISMS risk register under 27005's scoring conventions.

None of the three is a mandatory framework in most jurisdictions.
Together, they set the vocabulary the head uses to argue why the
register operates the way it does. If a regulator, auditor, or
board challenges the register's shape, the answer starts with these
three standards and specialises down to the enterprise's taxonomy.

## Reading the taxonomy the architect delivered

The level-50 architect delivered the enterprise AI risk taxonomy (see
[[mod-101-role-scope-and-leadership-shape]] chapter 01). The head
does not re-author it. The head reads it so accurately that every
risk on the register can be defended against the taxonomy in the
council. Concretely, the head must be able to name — for any risk on
the register — the following without looking:

- **Category.** Which top-level taxonomy category the risk sits in
  (a defensible taxonomy typically has categories including but not
  limited to: safety, security, privacy, fairness and non-
  discrimination, robustness and reliability, transparency and
  explainability, human oversight, environmental impact, third-party
  dependency, regulatory compliance, financial, reputational,
  operational).
- **Subcategory.** The specific subcategory beneath the parent,
  keyed to the taxonomy document control.
- **Systems affected.** The AI-system inventory records (chapter 06)
  the risk touches.
- **Regulatory nexus.** Whether any specific regulatory obligation
  is implicated (EU AI Act article, sector rule, data-protection
  obligation).
- **Appetite band.** Whether the risk sits inside, at, or outside
  the appetite threshold for its category.

If the head cannot answer those five for any risk in under thirty
seconds, either the register is stale, the taxonomy is opaque, or the
head has not internalised the architect's design. All three are
solvable; none is acceptable indefinitely.

## Appetite tracking as an operating discipline

Risk appetite is where enterprise risk-management theory most often
collides with operating reality. A written appetite statement that
says "the enterprise accepts moderate AI risk" is not appetite; it is
decoration. Appetite is operable when each taxonomy category has:

- A **quantitative threshold** where possible (e.g. "no more than N
  material fairness incidents per year"; "no more than 5% of tier-1
  AI systems with an open non-conformity older than 90 days"; "no
  more than X% cumulative model drift on any regulated system without
  re-validation").
- A **qualitative threshold** where quantitative measurement is not
  feasible (e.g. "no deployment of high-risk-by-EU-AI-Act-classifiction
  systems without a completed impact assessment approved by the
  council").
- A **deviation-alarm** — the level at which the register
  automatically flags a deviation-from-appetite for council review,
  typically expressed as a percentage of the threshold (e.g.
  approaching-appetite at 75%, deviation at 100%, breach at 120%).
- A **cadence of measurement** — the frequency at which the metric
  is refreshed, so that appetite tracking is a live signal, not an
  annual reconciliation.
- An **owner** — the first-line executive whose delivery keeps the
  metric inside appetite.

The head owns the discipline that appetite thresholds are set (with
council ratification), measured (through the GRC platform or the
control-evidence store), and refreshed (through the annual objectives
cycle in chapter 02). Appetite thresholds are not set once and
forgotten; they are revisited as the enterprise's AI portfolio, the
regulatory landscape, and the enterprise's tolerance for risk shift.

## The register's shape — every row is decision-supporting

A row on the enterprise AI risk register is not a paragraph of
description. It is a decision-supporting record with fields the
council can act on in seconds. A defensible row contains:

- **Risk ID** — monotonic, per taxonomy category.
- **Title** — one line, verb-oriented (what could happen), not
  noun-oriented (what the topic is).
- **Category and subcategory** — from the architect's taxonomy.
- **Description** — three to five lines: the risk scenario, the
  systems affected, the plausible trigger, the plausible consequence.
- **Inherent score** — the raw likelihood-and-impact score before
  treatment.
- **Applied treatments** — the specific controls, mitigations, or
  compensating measures currently in place.
- **Residual score** — the post-treatment score.
- **Appetite band** — inside / approaching / at / outside / breach.
- **Owner (first-line)** — the accountable first-line executive.
- **Second-line challenge** — the head's or a delegate's independent
  view of the score, treatment adequacy, and appetite position.
- **Next review** — the date the register revisits the row.
- **Escalation triggers** — specific events that would move the row
  out of council scope and into audit-committee or executive-committee
  scope (chapter 01).
- **Regulatory nexus** — as above.
- **Linked evidence** — pointers to the AIMS document-control
  evidence supporting the score.

A register whose rows do not carry those fields is a description
document, not a decision instrument. The GRC-for-AI platform the
architect selected (Credo AI, Holistic AI, ModelOp, Monitaur,
ServiceNow AI Control Tower, IBM watsonx.governance, or equivalent)
implements the schema; the head enforces the discipline that the
schema is populated to the same depth for every row.

## Portfolio-cadence rhythms

The head runs the register at three distinct cadences layered on top
of each other.

- **Continuous intake.** New risks arrive by the intake channels
  above (incident, near-miss, red-team, horizon scan, regulator
  correspondence, third-party notification, inventory change). A
  first-line risk analyst or GRC operator triages within a bounded
  window (48 hours is typical for material items). Triage produces:
  initial category, initial score, initial owner, and a next-council
  decision on acceptance.
- **Monthly council review.** The AI governance council reviews the
  register at every meeting (chapter 01). The review is *not* a
  full walk-through of every row; it is targeted at: new risks
  since last meeting, appetite deviations and approaches, escalation
  triggers hit, standing risks the council chose to revisit, and
  closed risks with root cause.
- **Quarterly portfolio deep-dive.** Once a quarter the council
  spends a full session on portfolio patterns — where the aggregate
  is trending, which categories are widening, which sectors of the
  AI portfolio are producing disproportionate risk, whether the
  taxonomy needs adjustment (a request the head takes to the
  level-50 architect), and whether the appetite thresholds
  themselves are still calibrated.

The audit committee sees the portfolio deep-dive on its own quarterly
cadence (chapter 01 and [[mod-103-board-and-audit-committee-reporting]]),
usually the meeting after the council's deep-dive so the council view
is settled.

## Escalation triggers — the trip-wires that move a row out of council scope

Escalation triggers are the pre-agreed conditions under which a risk
row moves out of the council's own decision authority. Setting them
in advance — rather than negotiating them under pressure at the
moment of a live incident — is what separates a governing body from
a working group at moments of crisis.

Typical triggers the head must have in writing:

- **Appetite breach.** A residual score that crosses the outside-
  appetite threshold triggers a mandatory audit-committee brief
  within a fixed window (a week is typical for material items) and
  a written response from the accountable first-line executive.
- **Cross-CxO impact.** A risk whose materialisation would touch
  multiple CxO scopes (CRO, CFO, CPO, CISO, GC, CCO) escalates
  sideways to the enterprise risk committee.
- **Regulatory nexus threshold.** A risk with a plausible regulatory
  reporting nexus (EU AI Act Article 73 serious incident, GDPR
  Article 33 personal-data breach, sector-specific reporting
  obligations) escalates immediately to the GC and to whichever body
  the enterprise's regulator-engagement runbook nominates. See
  [[mod-104-regulator-engagement]] and [[mod-110-incident-leadership]].
- **Sponsor-level ambiguity.** A risk without an accountable first-
  line owner at the required scope (typically SVP or above for
  material items) is itself an escalation; the head is not the
  fallback owner.
- **Ageing threshold.** A risk that has been *approaching-appetite*
  for two consecutive council cycles without treatment progress
  auto-escalates to the audit committee. This defends against the
  soft failure mode where a risk simply lives at the edge of
  appetite indefinitely.

Each trigger is documented, each is measurable, each is auditable
after the fact. The head does not decide in the moment whether an
escalation is warranted; the trigger decides.

## Root-cause discipline on closed risks

Closed risks are as diagnostic as open ones. When a row is closed
— because the risk materialised and was managed, because the risk
was successfully treated below appetite, or because the risk was
retired as no longer relevant — the closure entry captures:

- The closure reason.
- The root cause (using the taxonomy the architect specified — a
  common shape is a modified Ishikawa or "5-whys" against the AI
  risk taxonomy).
- Any control-library gap the closure exposes.
- Any policy or procedure change the closure implies.
- Any similar risks elsewhere in the portfolio that may share the
  root cause.

Closures without root-cause data are debt against the continual-
improvement cycle (chapter 02, anchor 10). The head reviews closure
data annually and feeds patterns into the architect for taxonomy
and control-library adjustment.

## Composition with the enterprise risk register

The AI risk register is not the enterprise's only risk register.
There is a parent enterprise risk register under the CRO, an
information-security risk register under the CISO / ISMS owner, a
privacy risk register under the CPO / DPO, a model-risk register
under the model-risk-management function in banking, and often
sector-specific registers (medical device, insurance, safety-of-life).

The head's job is not to consolidate all of them into one. The head's
job is to ensure that:

- Every AI risk of enterprise-material size is *upserted* into the
  parent enterprise risk register with a taxonomy tag identifying it
  as AI-origin. Materiality thresholds are defined by the CRO's
  framework.
- Every AI risk with an information-security dimension is either
  represented in the ISMS register or has a documented cross-
  reference (chapter 02 on AIMS-ISMS composition).
- Every AI risk with a privacy dimension is either represented in
  the privacy register or has a documented cross-reference.
- The AI risk register's taxonomy composes with the enterprise
  parent taxonomy — a translation layer is documented and owned by
  the level-50 architect.

This composition is a common failure point. A registered AI risk with
no linked enterprise-risk row, or with a linked row that scores
differently under the parent taxonomy, is exactly the inconsistency a
third-line audit will find. The head prevents it by owning the
composition discipline, not by trying to unify the registers.

## Example — an appetite deviation, worked through

The register carries a risk `AIR-FAI-004` (fairness — disparate impact
on protected-class subgroups in a credit-decisioning model). Category:
fairness. Subcategory: disparate impact. Systems affected: `AIS-CRED-
017` (unsecured lending model, tier 1).

Appetite for the fairness category is: no more than N high-risk
tier-1 systems with an unresolved disparate-impact finding older than
30 days. Approaching-appetite trigger: 75% of N. Deviation trigger:
100% of N. Breach: 120% of N.

The register update, run monthly, finds three tier-1 systems now
carrying unresolved disparate-impact findings, up from one last
month. The category rolls up to approaching-appetite. The
council-review pack for the next monthly meeting flags the trigger.

The council reviews. Discussion surfaces: two of the three findings
are on the same model family, sharing a training-data feature the
level-25 risk engineers are working on remediating; the third is on
an unrelated model with an independent root cause. The council
decides: accept the approaching-appetite band for the coming cycle,
require the first-line owner of the credit-decisioning portfolio to
present a treatment plan at the next meeting, and refer the
common-root-cause pattern to the level-50 architect for control-
library review.

Two months later a fourth finding arrives on the same model family.
The category rolls to at-appetite. The escalation trigger for
audit-committee brief within a week fires. The head schedules the
brief; the pack references the earlier council decisions and shows
the treatment-plan progress. The audit committee ratifies the head's
recommendation to accept the appetite deviation for one further cycle
with a specific committee-defined trigger to force stop-shipping if
a fifth finding materialises.

Every step of that sequence — the trigger firing, the escalation, the
committee brief, the ratified deviation, the stop-shipping condition —
is captured in the register, in the council minutes, and in the
audit-committee minutes, cross-referenced, and available to a
regulator or a certification-body auditor. That is the operating
discipline.

## Common failure modes

Three failure modes the head must defend against.

- **Register that only grows.** Risks are added, few are closed, none
  are retired. The register becomes a warehouse; portfolio-level
  signal is lost. The head enforces closure discipline and periodic
  retirement review.
- **Score without evidence.** Rows carry inherent and residual
  scores with no linked evidence supporting the score. Under
  certification-body sampling this reads as arbitrary. Every score
  must be traceable to the underlying measurement or attestation.
- **Appetite that never triggers.** Appetite thresholds set high
  enough that no realistic scenario ever breaches them are decorative.
  A register that has not fired an appetite trigger in a year is
  probably calibrated wrong; the annual appetite review addresses
  this.

Each failure mode is a leading indicator of a governance failure at
the audit committee or at the certification body. The head watches
for all three.

## Summary

- The AI risk register composes ISO 31000, ISO/IEC 23894, and
  ISO/IEC 27005 into an operating discipline the head runs at
  portfolio cadence; the level-50 architect designed the taxonomy.
- Appetite is operable when every taxonomy category has a
  quantitative threshold (or a documented qualitative substitute), a
  deviation alarm, a measurement cadence, and a first-line owner.
- Every register row is decision-supporting — Risk ID, title,
  category, description, inherent score, treatments, residual
  score, appetite band, owner, second-line challenge, review date,
  escalation triggers, regulatory nexus, linked evidence.
- Three rhythms overlap — continuous intake, monthly council
  review, quarterly portfolio deep-dive; the audit committee sees
  the deep-dive on its own quarterly cadence.
- Escalation triggers are pre-agreed and mechanical — appetite
  breach, cross-CxO impact, regulatory nexus, sponsor-level
  ambiguity, ageing at the edge of appetite — so that a running
  incident does not become a negotiation.
- Closures capture root cause; patterns feed the level-50 architect
  for taxonomy and control-library adjustment; unresolved patterns
  feed the year-end continual-improvement cycle (chapter 02).
- The AI register composes with the enterprise risk, ISMS, and
  privacy registers under a documented translation the head
  enforces; unification is not the head's job.
