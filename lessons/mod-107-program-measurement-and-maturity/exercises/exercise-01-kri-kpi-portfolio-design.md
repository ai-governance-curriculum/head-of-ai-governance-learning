# exercise-01: KRI / KPI Portfolio Design

**Estimated effort:** 3 hours

## Objective

Author the enterprise **KRI/KPI portfolio** for the AI-governance
program at enterprise scope — the ten-metric base plus the
sector overlays applicable to the enterprise, each with a
one-page metric-definition sheet under document control. The
deliverable is the artefact the head presents to the CRO for
threshold ratification, the artefact the level-15 analyst runs
production against monthly, the artefact the audit committee
sees at the annual programme-effectiveness read, and the
artefact the third-line CAE tests when the CAE's audit plan
reaches the AI-governance function.

The portfolio has to survive three stress tests. First, the CRO
challenges a threshold — the head has to show the appetite-
reference derivation on the definition sheet, not from memory.
Second, the audit committee asks "how do you compare with peers
on this metric" — the definition sheet has to make the peer
comparison possible without redefinition. Third, a new level-50
architect joins the head's team six months in and inherits the
portfolio — the sheets have to allow the new architect to
maintain the metric without re-negotiating the definition with
the CRO or the finance business partner.

The portfolio is not a dashboard. It is the discipline that
turns numbers into signals the enterprise's governance forums
can act on.

## Prerequisites

- Chapter [01-kri-kpi-portfolio](../01-kri-kpi-portfolio.md) —
  the ten-metric portfolio, the KRI-vs-KPI distinction, the
  threshold discipline, and the metric-definition sheet
  contents — read and internalised.
- Chapter [02-authoring-the-maturity-model](../02-authoring-the-maturity-model.md)
  for the maturity-progression metric (metric 9) that the
  portfolio references; chapter
  [05-program-cost-management](../05-program-cost-management.md)
  for the cost-per-AI-system-governed metric (metric 10).
- [[mod-102-running-the-program]] chapter 02 (AIMS operating
  calendar) for the cadences the portfolio rides on; chapter
  03 (risk register) for the source of most exposure metrics;
  chapter 04 (regulatory crosswalk) for the control set metric
  1 is defined against; chapter 06 (AI system inventory) for
  the denominator of metric 10; chapter 07 (supply-chain
  evidence) for metric 7.
- [[mod-103-board-and-audit-committee-reporting]] chapter 03
  (risk appetite) for the framework KRI thresholds derive from.
- [[mod-104-regulator-engagement]] chapter 04 (regulator
  inventory) for metric 5.
- [[mod-108-leading-the-governance-function]] for the team
  structure that carries the ownership map — the head owns
  definition, level-15 analyst owns production, level-50
  architect owns interpretation.
- [[mod-110-incident-leadership]] for the incident register
  that carries metric 3 (MTTR).
- A concrete enterprise in mind — sector (banking, insurance,
  health / medical device, pharma, public sector, frontier lab,
  tech platform, industrial), jurisdictional footprint, AI
  system portfolio scope, and the running-program artefacts
  the portfolio's sources reference. The sector overlays
  applicable depend on this context; make it explicit.

## Steps

1. **Enterprise context one-pager.** Author the half-page
   context the portfolio operates against: sector,
   jurisdictional footprint (EU, US federal, US states, Canada,
   UK, APAC, other), AI system portfolio scope (Annex III
   categories where relevant, GPAI provider or deployer scope,
   frontier-model scope), current CRO's risk-appetite
   framework at a high level (the specific appetite bands the
   enterprise runs against), and the operating owner
   assumption for the team (level-50 senior AI-governance
   architect and level-15 analyst at minimum; document the
   assumption if the enterprise has a different structure).
   Every subsequent artefact refers back to this one-pager.

2. **Metric-definition sheet template.** Author the one-page
   template every metric-definition sheet uses. Required
   fields, from chapter 01: metric name and short code; what
   it measures in one sentence; numerator and denominator
   specification; source of truth; cadence; owner (definition,
   production, interpretation, escalation, audit — five
   distinct roles); RAG thresholds with appetite reference per
   threshold; escalation on breach; known limitations; version
   and last-review date. The template is the shared contract
   with the finance business partner, the CRO, and the CAE —
   every sheet uses the same fields so the audit committee's
   read is consistent.

3. **Author the ten base sheets.** For each of the ten
   metrics chapter 01 names — control-testing pass rate,
   exception and waiver load, incident MTTR, board-report
   cycle time, regulator-response latency, AIA turnaround
   time, third-party-vendor tier coverage, evidence-
   completeness rate, maturity progression, cost-per-AI-
   system-governed — author the definition sheet using the
   template. For each:
   - Specify the numerator and denominator explicitly against
     the enterprise's own systems of record (do not write
     "number of controls" without naming the control-set
     version and the source system).
   - Specify the RAG thresholds against the enterprise's
     appetite framework. Where a threshold is a candidate
     that the head will negotiate with the CRO, mark it as
     "candidate, pending CRO ratification" — do not present
     an unratified threshold as final.
   - Name the source of truth (the system, table, or register
     the number comes from). Numbers computed by hand in a
     spreadsheet fail the discipline.
   - Name the five owners for the metric — definition, production,
     interpretation, escalation, audit — as roles, not people.
   - Specify the escalation on breach: which committee is
     notified, on what timeline, by whom. The escalation is
     written down before the breach.
   - Name known limitations — every metric has failure modes,
     and the sheet surfaces them so the audit committee reads
     the number correctly.

4. **Sector overlays.** For each sector overlay applicable to
   the enterprise's context (banking / insurance / health-and-
   medical-device / public sector / EU AI Act provider or
   deployer / GPAI provider scope / frontier lab, per the
   enterprise context one-pager), add the metrics chapter 01
   names for that overlay. Author the definition sheet for each
   overlay metric with the same template. Where the enterprise
   is not in scope for an overlay, note the fact explicitly in
   the portfolio README so an incoming head does not spend time
   looking for the overlay sheets.

5. **The threshold-calibration workbook.** Author the specific
   workbook the head takes to the CRO for threshold
   ratification. For each metric with a KRI threshold, the
   workbook has:
   - The candidate green, amber, and red bands.
   - The appetite reference (the CRO's appetite framework
     clause the threshold maps to).
   - The historical data — where available — showing where the
     metric has run over the trailing twelve months and what
     the proposed bands would have flagged.
   - The proposed escalation triggers per band.
   - The head's recommendation and rationale.
   The workbook is one working session with the CRO, not a
   sequence of emails. The head convenes; the CRO ratifies;
   the ratified thresholds go onto the definition sheets and
   the workbook goes into document control as the record of
   the calibration decision.

6. **The KRI-vs-KPI matrix.** Author the one-page matrix
   showing, for each of the ten metrics (and each overlay
   metric), which committee reads it as a KPI, which committee
   reads it as a KRI, and — where a metric is both — what the
   reporting cadence is to each committee. The matrix is what
   the head reviews at the AIMS operating calendar cycle to
   confirm every metric has a downstream committee, and it is
   what the level-15 analyst uses to schedule production runs.
   A metric with no downstream committee is a metric the head
   is producing for the head's benefit alone; the matrix
   surfaces the discipline break.

7. **Ownership map.** Author the ownership map naming, per
   metric, the specific role holding each of the five
   ownership positions (definition, production, interpretation,
   escalation, audit). Where the head is the escalation owner
   personally, name the head as personally escalating — the
   discipline is that the head does not delegate the "we are
   red" conversation. Where the third-line CAE is the audit
   owner, note the CAE's engagement depth (evidence assurance,
   methodology assurance, full audit) as it applies to the
   metric.

8. **The metric-review discipline.** Author the short
   discipline for annual metric review — when the portfolio is
   revisited (typically the annual maturity-assessment cycle,
   see chapter [03-annual-maturity-assessment](../03-annual-maturity-assessment.md)),
   who convenes the review, what triggers a mid-year
   redefinition (only material events — a regulatory change,
   an incident-driven insight, a CRO-initiated appetite
   change — not a red metric), and how a redefinition is
   ratified. The discipline is the defence against
   redefinition-under-fire.

9. **The failure-mode audit.** Author a short section — one
   paragraph per failure mode — naming how the portfolio
   detects and recovers from each of these failure modes:
   - A metric's source of truth is retired or restructured and
     the pipeline breaks silently.
   - A metric's threshold is red for two consecutive quarters
     without recovery, and no CRO-initiated re-calibration
     conversation has opened.
   - A metric owned by a role that is vacated or restructured
     out of existence, with no replacement owner named.
   - A metric that is neither a KRI nor a KPI to any downstream
     committee — a legacy metric that has drifted out of scope.
   - A composite metric that is green while a component metric
     is red, with the composite reported at the committee and
     the component buried in an appendix.

## Deliverables

- `enterprise-context.md` — the half-page context one-pager.
- `metric-definition-template.md` — the one-page template
  every metric-definition sheet uses.
- `metrics/metric-01-control-testing-pass-rate.md` through
  `metrics/metric-10-cost-per-ai-system-governed.md` — the ten
  base metric-definition sheets.
- `metrics/overlay-<sector>-<metric>.md` — sector-overlay
  metric-definition sheets, per enterprise context.
- `threshold-calibration-workbook.md` — the workbook the head
  takes to the CRO for threshold ratification.
- `kri-kpi-matrix.md` — the one-page KRI-vs-KPI matrix per
  metric and per committee.
- `ownership-map.md` — the five-role ownership map per metric.
- `metric-review-discipline.md` — the annual metric-review
  discipline and the redefinition ratification procedure.
- `failure-mode-audit.md` — the five failure-mode
  detection-and-recovery paragraphs.

## Acceptance criteria

- Every metric-definition sheet has every required field
  populated — no `TBD` fields, no "to be determined at
  quarterly review" fields. A sheet with an incomplete field
  fails the discipline.
- Every KRI threshold has an appetite reference. A threshold
  set from the metric's historical range without an appetite
  reference fails the criterion — the chapter is explicit that
  thresholds derive from appetite, not from history.
- Every metric has a named source of truth that is not a
  spreadsheet on the head's laptop. A source-of-truth field
  reading "manual" fails the criterion.
- Every metric has the five ownership roles populated (definition,
  production, interpretation, escalation, audit), and the
  escalation role is a specific role (head or a specifically
  named delegate), not "the team".
- Every metric has a downstream committee identified on the
  KRI-vs-KPI matrix. A metric with no downstream committee is
  a metric the exercise flags as a discipline break — either
  the metric moves off the portfolio or a downstream committee
  is identified.
- The threshold-calibration workbook is genuinely a workbook
  the head could take to the CRO in one working session. A
  workbook that is a set of paragraphs without candidate
  bands, historical data, and specific asks per metric fails
  the criterion.
- The failure-mode audit names, for each of the five failure
  modes, at least one specific detection signal and one
  specific recovery action.
- Any factual claim about a specific regulator's enforcement
  approach, a specific sector-body publication, or a specific
  peer's KPI practice carries a
  `<!-- needs-research: verify [specific fact] against
  [official source] -->` marker where the fact is not
  independently verifiable. No practice is guessed.

## Stretch goals

- Extend the portfolio with a **three-year forward look** —
  which metrics the head expects to add to the portfolio over
  the next three years as regulations evolve (EU AI Act GPAI
  Article 55 obligation metrics as they crystallise; sector-
  specific metrics as state adoption of the NAIC AI Model
  Bulletin expands; frontier-lab capability-tier metrics for
  enterprises with frontier-model surface). Each candidate
  metric named with the horizon-scanning source (per
  [[mod-105-regulatory-change-management]] chapter 01) and
  the expected first-published date.
- Author the **audit-committee briefing pack** for the annual
  programme-effectiveness read on the portfolio. The pack is
  a two-to-three-page summary that a committee director can
  read in ten minutes and act on: the ten base metrics with
  RAG status, year-over-year trend, threshold breaches during
  the year, correctives in flight, and the forward look. Use
  the pack shape convention from
  [[mod-103-board-and-audit-committee-reporting]] chapter 01.
- Draft the **metric-breach after-action review template** —
  the short review the head runs after each KRI threshold
  breach (whether the breach was recovered, unrecovered, or
  ambiguous). The review captures what the metric flagged,
  what the response was, what the recovery timing was, and
  what would have detected the breach earlier. Reviews feed
  the annual portfolio review.
- Extend the ownership map with the **head-and-CRO joint
  operating agreement** on threshold calibration — how the
  head and the CRO run the annual threshold-review conversation,
  what the CRO's specific accountability is (ratifying
  thresholds and holding them for the year), what the head's
  specific accountability is (bringing candidate thresholds
  supported by appetite reference and historical data), and
  how disagreement is resolved.
- Draft the **third-line CAE engagement note** — the specific
  scope of engagement the head recommends to the CAE for the
  first assurance cycle on the portfolio. The note is what the
  head hands to the CAE at the first working session; it
  frames the engagement without dictating it (CAE
  independence is preserved), and it identifies the specific
  metrics where evidence-assurance depth is warranted, where
  methodology-assurance depth is warranted, and where full-
  audit depth would be premature.

## Notes and starter guidance

The most common first-cut failure of the portfolio is the head
who authors "aspirational" definition sheets — sheets that
describe how the metric *ought* to be produced rather than how
it is produced now. Aspirational sheets fail on the first
audit, because the source of truth field names a system that
does not yet produce the number. Start from what the enterprise
can actually produce today, with the level-15 analyst working
against the systems the enterprise actually has; where a metric
requires a source of truth the enterprise does not yet have,
name the source and the specific investment required to build
it, and mark the metric as "planned Q3" or similar. A sheet
that describes a metric the enterprise cannot actually produce
is a sheet the audit committee will discover the enterprise
cannot produce, and the head loses the credibility that would
have carried the discipline.

The second common failure is the head who authors thresholds
without the CRO in the room. A KRI threshold ratified by the
head alone is a threshold the CRO will challenge at the risk
committee, and the head loses the argument in the room. Do the
threshold-calibration workbook as a genuine working session with
the CRO — schedule it, walk through it, ratify per metric, and
minute the ratification. The workbook then becomes the audit-
committee evidence that the thresholds are appetite-anchored.

On the KRI-vs-KPI matrix — the temptation is to make every
metric both, because "everything is a signal to somebody". A
metric that is both KRI and KPI at every committee is a metric
that reports to no one specifically. Force the matrix into
specificity: for each metric, name the committee that reads it
as a KRI (typically one committee — usually the risk
committee) and the committee that reads it as a KPI
(typically one committee — usually the AI Governance Council or
the audit committee's programme-effectiveness read).

On the ownership map — resist naming the same person or the
same role for every metric. A portfolio where the head is the
escalation owner for every metric is defensible; a portfolio
where the head is the interpretation owner for every metric is
not — that is the level-50 architect's craft, and the head who
does the interpretation personally is the head who has not built
the team.

On the failure-mode audit — pick the failures the head has
actually seen (or has seen in a peer's program), not
hypothetical failures. The audit is stronger when it names
concrete detection signals from actual experience.

The portfolio is a living artefact. Version it, date it, review
it annually at the maturity-assessment cycle, update the
threshold-calibration workbook when the CRO revises the
appetite framework, and update the definition sheets when a
source of truth is restructured. A portfolio that has not been
touched in a year is a portfolio that no longer reflects the
discipline it claims to describe.
