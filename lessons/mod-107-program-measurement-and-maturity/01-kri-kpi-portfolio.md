# The KRI and KPI Portfolio for the Enterprise AI-Governance Program

## Motivation

The board and the audit committee do not experience the head's
program directly. They experience the program through the numbers
that reach them. If the numbers are absent, the program is invisible
and its budget is negotiable. If the numbers are present but
disorganised, the program is legible but not defensible. If the
numbers are present, organised, calibrated, and threshold-triggered
against a written appetite, the program is a *managed* program in
the same sense that credit-risk, market-risk, and operational-risk
programs are managed — and the head can defend it on those terms.

This chapter is how the head assembles that number set. Not one
KPI, not a dashboard the head admires alone, but a *portfolio* of
key risk indicators (KRIs) and key performance indicators (KPIs) —
each with a definition, a source of truth, a target range calibrated
to enterprise appetite, a red-amber-green (RAG) threshold, an owner,
a cadence, and a named committee it reports to. The portfolio is the
running-program's telemetry, and the program-measurement discipline
is the discipline that keeps the telemetry honest.

The failure mode this chapter opens with is not a program without
metrics. It is a program with *many* metrics, none of them anchored
to appetite, several of them redefined between quarters, and none of
them capable of being red at the same time (because if a metric can
never be red, the metric is a status update, not a KRI). Chapter
[[03-annual-maturity-assessment]] carries the maturity plot; this
chapter carries the running-cadence numbers underneath the plot.

## Core concept — the difference between a KPI and a KRI

The head does not confuse the two. Both are numbers on a
dashboard; they answer different questions and they route to
different governance bodies.

- **A KPI (key performance indicator)** measures whether the
  program is delivering on what it committed to deliver. It answers
  *are we operating the program*. KPIs move slowly, live in the
  head's operating cadence, and route to the AI Governance Council
  (see [[mod-102-running-the-program]] chapter 01) and to the
  audit committee's annual programme-effectiveness read.
- **A KRI (key risk indicator)** measures whether the enterprise's
  AI risk exposure is inside appetite. It answers *are we outside
  where the board said we would be*. KRIs move faster, live in the
  risk-committee cadence, and route to the risk committee (see
  [[mod-103-board-and-audit-committee-reporting]] chapter 03) with
  standing lines of escalation into the audit committee when a
  threshold breach touches control-effectiveness.

A single number can be both — control-testing pass rate is a KPI
for the operating program *and* a KRI for control-effectiveness
appetite. When a number is both, the head reports it in both
places, on the same definition, at cadences appropriate to each
committee. Reporting different definitions of the same number to
different committees is the credibility failure the head cannot
walk back.

## The ten-metric portfolio the head defends

The head's portfolio at enterprise scope is not one hundred
metrics. It is a small, defensible set the audit committee can
hold in memory and the head can defend end-to-end. The ten below
are the standing set for a head running an enterprise-scope AI
governance program. Enterprises with sector overlays add sector
metrics (see the sector-metric list later in the chapter); the ten
below are the base.

The metrics are grouped by what they measure: *control health*,
*decision throughput*, *exposure surface*, and *program cost
efficiency*.

### Control-health metrics

**1. Control-testing pass rate.** Of the AI-governance controls
tested in the reporting period, the percentage that passed on first
test. Denominator: controls in the AIMS Annex A control set
([[mod-102-running-the-program]] chapter 04 crosswalk) plus
sector-overlay controls. Numerator: controls that passed the
level-50 architect's evidence review or the third-line CAE's test
without a finding.

This is a KPI (delivery of the operating program) and a KRI
(control-effectiveness appetite). Target range is calibrated to the
enterprise's control-effectiveness appetite, typically expressed as
"green above X%, amber X–Y%, red below Y%". The head does not pick
X and Y from thin air — the CRO's control-effectiveness appetite
band ([[mod-103-board-and-audit-committee-reporting]] chapter 03)
sets X and Y, or the head negotiates them with the CRO before
first publication and locks them for the year.

**2. Exception and waiver load.** The count of active exceptions
and waivers to AI-governance policy, plus the count opened, closed,
and aged past their remediation date in the reporting period.
Denominator context: exceptions per hundred AI systems in scope
(so the metric does not silently move as the inventory grows).

Exceptions are inevitable in a maturing program. What is *not*
inevitable is a load that grows without bound, an ageing tail that
never closes, or a concentration of exceptions in a single business
line that signals a systemic control gap. The KRI threshold is on
the aged-past-remediation tail, not on the raw count — a program
with fifty active exceptions and none aged is healthier than a
program with ten active exceptions and eight of them past-due.

**3. Incident MTTR (mean time to remediation).** For AI incidents
logged in the incident register ([[mod-110-incident-leadership]]),
the elapsed time from incident detection to remediation-verified
closure. Reported as median and 90th percentile (never as mean
alone — mean hides tails, and it is the tail that hurts).

Target range is calibrated to the enterprise's operational-risk
appetite for AI. The threshold is a KRI, not a KPI — a rising MTTR
is a signal that the incident-response function is under-resourced
or that the incidents themselves are getting harder, and either
requires committee attention. See [[mod-110-incident-leadership]]
chapter 05 for the incident-response metric shape this feeds into.

### Decision-throughput metrics

**4. Board-report cycle time.** The elapsed calendar days from the
end of the reporting quarter to the date the board pack is
delivered to the board secretariat. Cycle time is a KPI on the
head's own operating discipline — a board pack that lands six weeks
after quarter-end is a pack the board reads as *historical* rather
than *current*.

The target is set by the board secretariat and the audit-committee
chair, not by the head — the head negotiates it and holds to it.
The metric is on the head's own dashboard because the head is the
accountable owner; a slipping cycle time is a signal that either
the pack has grown past what the discipline can carry or the
program-management function underneath the head needs
reinforcement.

**5. Regulator-response latency.** For inbound regulator
correspondence tracked in the regulator-engagement inventory
([[mod-104-regulator-engagement]] chapter 04), the elapsed days
from receipt to head-authorised response. Reported per regulator
and in aggregate.

This is a KRI. A regulator that receives responses inside its
stated timeframe experiences a functional relationship; a
regulator that has to chase is a regulator that is escalating
internally. The threshold is not the regulator's stated deadline —
the threshold is the head's own internal buffer against the
regulator's deadline (typically 5–10 business days earlier),
because a regulator's deadline is a floor, not a target.

**6. AIA turnaround time.** For AI impact assessments (AIAs,
per ISO/IEC 42005 shape, [[mod-102-running-the-program]] chapter
06 adjacent) opened in the reporting period, the elapsed days
from AIA opening to head- or council-authorised closure.

This is a KPI for the operating program *and* a KRI for the
enterprise's ability to onboard new AI systems inside the
appetite envelope. If AIA turnaround is slow, either the AIA
process is under-resourced or the AI system pipeline is
generating cases the process cannot absorb — both are addressable,
neither is addressed by ignoring the metric.

### Exposure-surface metrics

**7. Third-party-vendor tier coverage.** The percentage of
in-scope third-party AI vendors ([[mod-102-running-the-program]]
chapter 07) with completed tier-assignment, completed evidence-
collection at the required tier depth, and standing next-review
date on the calendar. Reported per tier (typically tier 1
critical, tier 2 material, tier 3 general).

The KRI threshold is on tier 1 — a tier 1 vendor without current
evidence is an unmitigated concentration risk. Aggregate coverage
is a KPI (the program is working through the population); tier 1
gap count is a KRI (the enterprise is exposed at the top of the
distribution).

**8. Evidence-completeness rate.** For AI-governance evidence
required at the enterprise's Annex A control set and voluntary-
code commitments ([[mod-106-external-positioning-and-voluntary-codes]]
chapter 01), the percentage of required evidence artefacts that
are current (within their refresh cadence) and retrievable (linked
in the GRC-for-AI stack, not merely nominally produced).

This is the metric a certification-body auditor or a regulator
examiner will press on first. Evidence that exists but cannot be
retrieved inside the auditor's window is evidence that fails the
audit. The metric is a KPI for the operating program and a KRI
for audit and examination readiness.

**9. Maturity progression.** The year-over-year delta on the
enterprise's composite maturity plot ([[03-annual-maturity-assessment]]),
per axis and in composite. Reported annually with a mid-year
read-through against the trajectory line.

Maturity progression is not a fast-moving metric — the annual
cadence is the correct cadence. But the *trajectory adherence*
between annual reads is a legitimate mid-year signal, and a
program that is falling behind its ratified trajectory is a
program the audit committee needs to know is falling behind
before the annual reveal.

### Cost-efficiency metrics

**10. Cost-per-AI-system-governed.** Total AI-governance program
cost (see [[05-program-cost-management]]) divided by the count of
AI systems in the enterprise inventory
([[mod-102-running-the-program]] chapter 06). Reported per
inventory scope (production systems only; production plus pre-
production; and total including sunset systems still under
oversight).

This is the CFO's headline efficiency metric. It is a KPI on
program cost discipline — a rising cost-per-system without a
corresponding rise in coverage or maturity signals inefficiency
the CFO will surface. The head reports it, defends it, and
explains the drivers when it moves. The metric composes with
the ROI reporting shape in [[04-roi-reporting-to-cfo]].

## Calibrating the target ranges to appetite

A KRI without a threshold is a status update. The threshold is
what turns a number into a signal. Two disciplines govern how the
head sets thresholds.

First, **thresholds derive from appetite, not from the metric's
history**. The temptation is to set the amber threshold at "one
standard deviation off the trailing-twelve-month mean" and call
that calibrated. That threshold answers "is this metric unusual"
— which is not the question the risk committee is asking. The
risk committee is asking "is this metric outside the exposure the
board tolerates". The appetite framework
([[mod-103-board-and-audit-committee-reporting]] chapter 03) is
what defines the tolerated exposure; the threshold is where the
appetite meets the metric.

For a metric where the appetite is not yet articulated, the head
does not invent it. The head runs the metric at "measured, no
threshold" for one to two reporting cycles, then convenes the CRO
and takes the calibration decision with the CRO's authority. A
threshold set without CRO ratification is a threshold the CRO can
challenge at the risk committee, and the head loses the argument
in the room.

Second, **thresholds are asymmetric across the RAG bands**.
Green-to-amber is the trigger for management attention. Amber-to-
red is the trigger for committee attention. A metric that
oscillates between green and amber week over week is either a
noisy metric (the threshold is too tight) or a program that is
genuinely on the border (the threshold is right and the program
needs work); the head diagnoses which. A metric that flashes red
should be genuinely rare — if red is routine, the threshold is
mis-calibrated, or the appetite itself is the wrong appetite and
the CRO needs to re-open the appetite conversation.

## The metric-definition sheet — one per portfolio metric

Every metric in the portfolio has a one-page definition sheet.
The sheet is the head's contract with the CRO, the audit
committee, and the third-line CAE about what the metric measures
and how it behaves. Without the sheet, the metric drifts across
quarters and the head cannot defend a moving number.

The definition sheet has, at minimum:

- **Metric name and short code.** The name is the label on the
  dashboard; the short code is the reference used in minutes.
- **What it measures, in one sentence.** If the sentence cannot
  fit, the metric is composite and should be split.
- **Numerator and denominator specification.** Explicit. "Number
  of controls" is not a specification; "number of controls in the
  Annex A set enumerated in the AIMS statement of applicability,
  version N.M" is.
- **Source of truth.** The system, table, or register the number
  comes from. Numbers computed by hand in a spreadsheet by the
  head's analyst are numbers the head cannot audit.
- **Cadence.** Monthly, quarterly, per-incident, annual. The
  cadence lines up with the committee cadence it reports to.
- **Owner.** A named role, not a team. The level-50 architect
  owns most metric definitions; the level-15 analyst owns
  most metric production.
- **RAG thresholds.** Green range, amber range, red range, with
  the appetite reference each threshold derives from.
- **Escalation on breach.** What happens when the metric enters
  amber. What happens when the metric enters red. Which committee
  is notified, on what timeline, by whom. The escalation is
  written down *before* the breach; scrambling to define the
  escalation during the breach is the credibility failure the
  discipline is designed to prevent.
- **Known limitations.** Every metric has failure modes — a
  numerator that under-counts, a denominator that lags, a source
  system that is quarter-lag. The head names them so the audit
  committee reads the number correctly.
- **Version and last-review date.** Metrics evolve. The
  version-controlled sheet is the record of the evolution.

The metric-definition sheet lives in the same document-control
system as the AIMS scope statement and the risk-appetite framework
— it is a governance artefact, not the head's private notes.

## Sector overlays — additional metrics per regime

The ten-metric base extends with sector overlays where the
enterprise operates in a regulated sector. The sector metrics do
not replace the base; they add to it, with the same definition-
sheet discipline.

- **Banking (US and Canada).** Model-risk-management (MRM) metrics
  under Federal Reserve SR 11-7 and OCC 2011-12 (US), OSFI E-23
  (Canada) — model-inventory coverage, effective-challenge
  completion rate, model-performance-monitoring exception rate,
  and time-to-retire on models flagged for decommissioning. The
  enterprise's MRM function usually owns these; the head
  coordinates on AI-specific models and on the AI-adjacent overlay
  (see [[mod-111-sector-program-leadership]]).
- **Insurance (US).** State-DOI AI-model-bulletin-adoption
  coverage per state the enterprise operates in, and, where the
  Colorado Division of Insurance Regulation 10-1-1 applies, the
  bias-testing frequency and remediation-close rate the regulation
  requires. See [[mod-105-regulatory-change-management]] chapter
  07 for the regulation shape.
- **Health / medical device.** For enterprises with AI/ML as
  software as a medical device (SaMD) surface, FDA Good Machine
  Learning Practice (GMLP) coverage, predetermined change control
  plan (PCCP) adherence, and post-market performance-monitoring
  currency metrics. See the FDA AI/ML SaMD programme reference.
- **Public sector (US federal).** OMB M-25-21 governance
  requirements produce agency-specific metrics — impact-assessment
  completion, minimum-practice coverage, and public-inventory
  currency — that federal agencies and federal contractors track
  in parallel to the base ten.
- **EU AI Act — provider or deployer scope.** Article 26 (deployer)
  and Article 16 (provider) obligation-coverage metrics — post-
  market monitoring plan currency, serious-incident reporting
  latency against Article 73 windows, fundamental-rights impact
  assessment (FRIA) completion for public-sector or bank-scoped
  Annex III systems.
- **GPAI provider scope.** For enterprises within GPAI provider
  scope, the additional metrics associated with the EU AI Office
  General-Purpose AI Code of Practice signatory commitments where
  the enterprise is a signatory ([[mod-106-external-positioning-and-voluntary-codes]]
  chapter 01), including systemic-risk-assessment currency and
  transparency-report cadence adherence.

The overlays add specificity, not volume. The head resists the
pull to add every reference to the portfolio; a metric that does
not have a committee that reads it is a metric that is not worth
producing.

## Who owns what — the metric ownership map

Ownership across the portfolio is not "the head owns everything".
The head owns the portfolio *definition* and the *appetite
calibration*; specific metrics have specific owners.

- **Metric definition and threshold calibration.** Head, with CRO
  ratification.
- **Metric production and evidence for the number.** Level-15
  analyst on the head's team ([[mod-108-leading-the-governance-function]]),
  drawing from the source-of-truth systems. The analyst does not
  compute the metric in a spreadsheet from lookup; the analyst
  runs the pipeline that produces the metric, and the number is
  reproducible by any second analyst working from the same
  pipeline.
- **Metric interpretation and drafted commentary.** Level-50
  senior AI-governance architect. The narrative around the
  number — what the number means, what it does not mean, what
  moved it, what the outlook is — is the architect's craft, not
  the analyst's.
- **Metric escalation on breach.** Head, personally. The head
  does not delegate the "we are red" conversation with the risk
  committee or the audit committee. See [[06-difficult-measurement-conversations]].
- **Metric audit and independent validation.** Third-line CAE, at
  the CAE's discretion and on the CAE's audit-plan cycle. The
  head does not assure their own numbers; the CAE does, or an
  external assurance provider does.

Ownership is on the metric-definition sheet. A metric without a
named owner in each of the five roles above is a metric the head
has not stood up yet.

## Anti-patterns the head does not permit

Three anti-patterns the head names and refuses to run.

**The vanity dashboard.** Fifty metrics, all green, updated
weekly, presented at the AI Governance Council with pride and
never discussed. The dashboard flatters the head and teaches the
council nothing. The remedy is the ten-metric discipline —
pressed against appetite, threshold-triggered, and small enough
that every metric is discussed at every cadence.

**The redefinition-under-fire pattern.** A metric goes red; the
head returns the next quarter with a "refined definition" that
puts the metric back to green. The audit committee will notice.
Once the pattern is noticed, every metric the head reports is
suspect. The remedy is the version-controlled definition sheet
and the discipline that a redefinition mid-year requires audit-
committee-chair sign-off with a written rationale — not
"clarification".

**The composite-only report.** A single "AI governance health"
number aggregating the ten. Composites are readable but they
launder red metrics into amber and amber metrics into green. The
head reports the ten, individually, with the composite as a
summary read *after* the individual metrics are on the page. The
board and audit committee read composites; they only trust the
composite when they can see the numbers underneath it.

## Composition with adjacent modules

The portfolio composes with the running program and the reporting
disciplines the head has already built.

- The **operating calendar** in [[mod-102-running-the-program]]
  chapter 02 is the calendar the portfolio's cadences ride on.
  Metric-production runs are calendar events, not ad hoc requests.
- The **risk register** in [[mod-102-running-the-program]] chapter
  03 is the source-of-truth for exposure metrics 7 (vendor tier
  coverage) and 8 (evidence completeness), and it feeds the
  incident-count and appetite-breach signals that inform metric 3
  (MTTR) and the KRI escalations more broadly.
- The **audit-committee reporting cluster** in [[mod-103-board-and-audit-committee-reporting]]
  is the destination for the KPI subset of the portfolio, at the
  cadence chapter 03 fixes.
- The **risk-appetite framework** in [[mod-103-board-and-audit-committee-reporting]]
  chapter 03 is the definitive reference for KRI thresholds —
  the head does not set a threshold that departs from the CRO's
  appetite framework without the CRO in the room.
- The **regulator-engagement inventory** in [[mod-104-regulator-engagement]]
  chapter 04 is the source for metric 5 (regulator-response
  latency).
- The **regulatory-change register** in [[mod-105-regulatory-change-management]]
  chapter 01 is the source for the metric that feeds
  [[03-annual-maturity-assessment]] on the pace of the enterprise's
  regulatory-alignment work — used at annual maturity depth, not
  at quarterly KRI depth.
- The **voluntary-code register** in [[mod-106-external-positioning-and-voluntary-codes]]
  chapter 01 is where evidence-completeness rate (metric 8) picks
  up the signatory-commitment obligations.
- The **incident register** in [[mod-110-incident-leadership]]
  is the source for MTTR (metric 3) and for the incident-volume
  and severity-trend signals the KRI escalations reference.

The portfolio is not built in isolation. Each metric points to a
specific artefact in another chapter as its source, and each
metric feeds a specific committee reporting cycle. Metrics that
do not compose with the running program are metrics the head is
running for the head's benefit alone; the discipline is that
every metric has a source upstream and a committee downstream.

## Summary

- The head runs a *portfolio* of KRIs and KPIs, not a dashboard —
  ten base metrics at enterprise scope, with sector overlays as
  applicable, each with a one-page definition sheet under document
  control.
- KPIs answer "is the program operating" and route to the AI
  Governance Council and the audit committee's programme-
  effectiveness read; KRIs answer "is the exposure inside
  appetite" and route to the risk committee. A single number can
  be both, reported in both places on the same definition.
- The ten base metrics: control-testing pass rate, exception and
  waiver load, incident MTTR, board-report cycle time, regulator-
  response latency, AIA turnaround time, third-party-vendor tier
  coverage, evidence-completeness rate, maturity progression, and
  cost-per-AI-system-governed.
- Thresholds derive from the CRO's appetite framework, not from
  the metric's own history. Every KRI threshold is CRO-ratified
  before first publication and locked for the year absent a
  written re-calibration.
- Every metric has an owner in each of five roles — definition
  (head), production (level-15 analyst), interpretation (level-50
  architect), escalation on breach (head personally), and audit
  (third-line CAE).
- Three anti-patterns the head refuses to run: the vanity
  dashboard, redefinition-under-fire, and composite-only
  reporting.
- The portfolio composes with the operating calendar, the risk
  register, the reporting clusters, the appetite framework, the
  regulator inventory, and the incident register. Every metric
  has an upstream source and a downstream committee.
- Chapter [[02-authoring-the-maturity-model]] turns to the
  maturity model that the maturity-progression metric (metric 9)
  measures against; chapter [[03-annual-maturity-assessment]]
  turns to the assessment shape that produces the annual maturity
  read; chapter [[04-roi-reporting-to-cfo]] turns to the ROI
  reporting that composes with cost-per-system (metric 10); and
  chapter [[06-difficult-measurement-conversations]] rehearses
  the conversations the head owns when a KPI or KRI is red.
