# The Audit Committee AI Deep-Dive Shape

## Motivation

The audit committee is not the board. The audit committee is a
delegated committee of the board with a specific mandate — external
auditor oversight, internal audit oversight, financial-reporting
integrity, and (increasingly) enterprise risk and compliance
oversight. Under most listing-standard and regulatory regimes the
audit-committee charter names those responsibilities explicitly.

For the head of AI governance, the audit committee is where the pack
gets *sampled* — where a member with a professional accountancy or
audit background reads the summary and asks the specific follow-up
question, and where an independent third-line finding lands with
management response and committee ratification. The board sees the
program's shape; the audit committee sees whether the shape holds
under sampling.

The IIA Three Lines Model and the IIA International Professional
Practices Framework describe the reference operating model. This
chapter is the head's shape for how the audit committee AI deep-dive
sits inside that model, and what the pack the audit committee sees
looks like as a result.

## Core concept: the audit committee sees the three lines

The head's board pack (chapter 01) presents the *state* of AI risk.
The audit committee's AI deep-dive presents the *assurance* on that
state — evidence that the three lines are each functioning at the
scope the IIA model describes:

- **First line** — the operating owners of AI systems and their
  control operators. Assurance here answers: are the controls the
  policy library requires actually being operated by the
  accountable owners, at the cadence the policy specifies, with
  evidence retained?
- **Second line** — the head of AI governance and adjacent risk /
  compliance functions. Assurance here answers: is the AIMS
  operating as designed; is the risk register maintained at
  cadence; is the appetite framework in force; are non-conformities
  closed; are exceptions bounded and reviewed?
- **Third line** — internal audit under the Chief Audit Executive.
  Assurance here answers, independently: what did the CAE's team
  find on the AI audits in the audit-plan period, what has
  management committed to remediate, and what is the ageing of
  remediation? Third-line independence means the head does *not*
  author or edit the CAE's findings — the head provides management
  response, and the audit committee is the ultimate reader.

The audit-committee AI deep-dive is structured as a first-line
report, then a second-line report, then a third-line report, then a
composite view of external audit and certification-body findings.
The composite view is what the committee acts on.

## The five-cluster audit-committee shape

### Cluster 1 — first-line control effectiveness

The first line owns the controls. The head reports on how the first
line is operating them.

Content:

- **Control operating coverage** — of the AI-specific control
  library the level-50 architect chartered (composed against
  NIST AI RMF, ISO/IEC 42001 Annex A, sector overlays), the
  proportion of controls that were operated at their expected
  cadence in the period, with a tail of controls that were not, and
  the reason for each.
- **Control failure and near-failure** — controls that failed to
  operate as designed, controls where evidence was late or
  incomplete, controls under active remediation. The audit
  committee sees the tail with root-cause categorisation
  (competence, staffing, tooling, process design, policy ambiguity).
- **First-line self-assessment posture** — where first-line owners
  are running a self-assessment (many mature programs do), the
  aggregate posture and the delta from the second-line assessment.
- **Concentration** — first-line control operators who own more
  than a defensible number of controls, systems, or exception
  reviews. Concentration in the first line is a common finding.

### Cluster 2 — second-line coverage and effectiveness

The second line is the head's own function plus adjacent risk and
compliance. This section is the head reporting on the head's own
function, and it is uncomfortable to author well. The audit
committee is specifically watching for over-claim.

Content:

- **AIMS operating discipline** — internal audit rounds executed
  against the ISO/IEC 42001 AIMS calendar, non-conformities raised
  and closed, competence assessments completed and gaps, management
  reviews conducted and outputs. Anything the ISO/IEC 42006
  certification body would sample.
- **Risk-register operating discipline** — updates in period,
  appetite-tracker maintenance, escalation triggers exercised,
  deviations from cadence.
- **Policy and exception discipline** — new policies issued in
  period, policies retired or superseded, exceptions granted /
  aged / expiring / breached.
- **Second-line coverage gaps** — where the second line is
  under-covering (a common tail: emerging capability the policy
  library does not yet address, a jurisdiction with new
  obligations the program has not yet mapped). This section is
  where the head is *most* honest.

### Cluster 3 — third-line audit findings and remediation status

The Chief Audit Executive owns this section. The head does not
author it. The head provides management response and remediation
tracking; the CAE presents the findings and the committee-level
implications.

Content typically comes from the CAE:

- Audits completed in period against the audit plan (the CAE's
  plan is approved by the audit committee; deviations are also
  reported).
- Findings by severity (critical / high / medium / low or the
  IIA-equivalent local categorisation), with number of findings
  by AI-relevant risk category.
- Management response and target remediation dates per finding.
- Ageing of open findings — findings past target date, findings
  where remediation is on hold, findings that were re-opened after
  closure.
- Any qualified or adverse opinion the CAE has issued on an
  AI-relevant audit, with the committee's decision path.

Third-line independence is the *only* thing the audit committee
cares about here beyond the substance of the findings. The head's
job in this cluster is to make it *easy* for the CAE to present
without editorial interference — see chapter 04 on CxO sign-off
flow, which explicitly names the CAE ownership boundary.

### Cluster 4 — external audit and certification-body findings

Adjacent to the third line but distinct. The enterprise may be
subject to:

- ISO/IEC 42001 certification-body audit under ISO/IEC 42006.
- Financial-statement external audit findings that touch AI
  systems used in financial reporting (model risk in valuation,
  provisioning, fraud detection).
- Sector regulator examination findings (banking supervisors,
  insurance supervisors, health regulators, transport safety
  authorities, communications regulators, competition authorities,
  data-protection authorities).
- Voluntary third-party attestation results (ForHumanity IAAIS,
  BABL AI, IEEE CertifAIEd — see
  [[mod-102-running-the-program]] chapter 04 for the third-party
  audit interface).
- Customer or B2B contractual assurance requests (large-enterprise
  buyers now conduct their own AI vendor assurance).

Content per external interaction:

- Auditor / examiner and the scope of the review.
- Findings and severity.
- Management response and remediation ownership.
- Ageing and status.
- Any regulatory or contractual consequence pending on remediation.

### Cluster 5 — composite assurance view and committee decisions

The prior four clusters are inputs. The composite view is what the
committee acts on.

- **Aggregate assurance posture** — a one-page composite of how the
  head, the CAE, and the external auditors read the aggregate AI
  risk posture. Where the three views agree, that is signal; where
  they disagree, that is a red flag the committee explicitly
  discusses.
- **Convergence and divergence commentary** — where first, second,
  and third lines see the same picture, and where they do not. A
  program where all three lines *always* agree is a program where
  independence is at risk.
- **Committee decisions requested** — audit-plan approvals, CAE
  scope-of-work approvals for the coming period, remediation-
  extension approvals, ratification of management response to
  qualified opinions, escalations to the board.

## Cadence

Quarterly primary cadence, aligned with the audit-committee
calendar (financial-quarter cadence in most enterprises). The
audit-plan and CAE scope-of-work approvals are typically annual
and land at a specific point in the cycle. Findings ageing is
month-over-month and the committee expects the ageing view to be
current, not backdated.

Between quarters the head keeps the audit-committee chair in the
loop through short written notes — new findings above a severity
threshold, incidents with audit implications, regulator engagement
developments — on the same shape as the board delta note but
directed at the audit-committee chair.

## What the audit committee is watching for

The audit-committee members do not know AI. They know audit and
risk. They are watching for the same signals they watch for on any
program:

- Whether the second line's self-report is consistent with the
  third line's independent view. Divergence — and the head's
  reaction to divergence — is signal.
- Whether findings age. Aging findings are the strongest signal
  of a program in trouble.
- Whether exceptions accumulate. A program with a growing
  exception population is a program where policy is drifting away
  from operating reality.
- Whether root cause is analysed. Findings without root cause
  come back.
- Whether the tail of controls that did not operate is small,
  stable, and honestly reported. A tail that is silently getting
  smaller is a tail that has been redefined.

The head's pack is authored to make each of these visible without
the committee having to hunt for them.

## Coordination with the CAE

The CAE is independent under the IIA framework. Independence is
preserved by process, not by intention. Specifically:

- The head does not review, edit, or seek to influence third-line
  finding language before it reaches the committee.
- The head does provide *management response* — the head's function
  is management for the AIMS scope — and that response is part of
  the pack.
- Where the head wants a topic considered for third-line coverage,
  the head sends a written request to the CAE (referenced in
  [[mod-102-running-the-program]] chapter 01) and that written
  request is itself an audit-committee-visible artefact.
- Where the CAE's finding surfaces a divergence with second-line
  view, the head *says so* in management response and offers the
  committee both views, rather than trying to unify the position.

The audit committee's confidence in the AI program is a function of
how visibly this discipline is held.

## Summary

- The audit committee sees the assurance layer over the risk
  picture the board sees — the three lines each reporting on their
  own scope, then the composite view.
- Five clusters: first-line control effectiveness; second-line
  coverage and effectiveness (including honest under-coverage
  reporting); third-line audit findings and remediation
  (CAE-owned); external audit and certification-body findings;
  composite view and committee decisions.
- Third-line independence is preserved by process — the head does
  not edit CAE findings, does provide management response, uses
  written requests for scope suggestions, and surfaces divergence
  rather than unifying.
- The committee is watching for divergence, aging findings,
  exception drift, missing root-cause analysis, and tail
  redefinition; the pack surfaces each without hunting.
- Cadence is quarterly with short written between-quarter notes to
  the audit-committee chair on significant developments.
