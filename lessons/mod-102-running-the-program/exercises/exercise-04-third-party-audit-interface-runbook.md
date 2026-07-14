# exercise-04: Third-Party Audit Interface Runbook

**Estimated effort:** 3 hours

## Objective

Author a **third-party audit interface runbook** covering the five
external audit relationships the head owns: ISO/IEC 42001 certification
body (accredited under ISO/IEC 42006), ForHumanity IAAIS auditor,
BABL AI Algorithm Bias Auditor, sector regulator examiner, and
third-line internal audit (under the CAE). The runbook must be
defensible when a certification body samples it under ISO/IEC 42006's
own audit-quality expectations, and must preserve third-line
independence under the IIA Three Lines Model.

## Prerequisites

- Chapter [04-third-party-audit-interface](../04-third-party-audit-interface.md)
  read and internalised.
- Chapter [02-aims-operating-calendar](../02-aims-operating-calendar.md)
  — the calendar's anchor 9 (certification-body engagement window)
  composes with this runbook.
- Chapter [04-three-lines-at-leadership-scope](../../mod-101-role-scope-and-leadership-shape/04-three-lines-at-leadership-scope.md)
  (mod-101) — the third-line independence discipline the runbook
  preserves.
- Assumed enterprise from the prior exercises, with an assumed
  sector so the sector-regulator examiner section is specific.

## Steps

1. **Five-relationship matrix.** Author a matrix of the five
   external audit relationships with columns for: mandate,
   accreditation or authority, scope, independence posture,
   evidence-package expectations, sampling access mechanism,
   reporting-line into the enterprise, and cadence. Do not
   collapse any two relationships; the runbook fails when the
   head treats them as one.
2. **Evidence-bundle assembly convention.** Document the
   convention for assembling an audit-ready evidence bundle from
   the level-50 architect's evidence architecture. Cover: which
   documents constitute the AIMS statement of applicability
   package; how the control-mapping table is generated; how
   per-control evidence is exported (OSCAL, ML-BOM, model /
   system / dataset cards); how management-review minutes and
   internal-audit reports are staged; how the risk-register and
   inventory extracts are frozen for the visit; how third-party
   evidence for sampled vendors is included.
3. **Sampling-access administration.** Author the sampling-
   access procedure: how auditor accounts are provisioned, how
   read-only access is enforced, how live-view sessions are
   escorted and logged, how interview scheduling and note-taking
   work, how the head enforces un-tampered access. Include the
   specific control that prevents curation of the sampling
   population.
4. **Exit-meeting discipline.** Author the exit-meeting
   discipline note: the head's behaviour, what is said, what is
   not said, how factual clarifications are captured on the
   record, how substantive disagreement is queued for the
   auditor's dispute process. Include a specific script (three to
   five sentences) the head uses to open and close the exit
   meeting.
5. **Finding triage and remediation-plan template.** Author the
   finding-triage classification (major non-conformity, minor
   non-conformity, observation, matter-requiring-attention,
   third-line-audit rating) and the remediation-plan template
   (finding reference, root cause, corrective action, containment
   action, owner, target date, effectiveness review, council and
   audit-committee visibility).
6. **Audit-committee reporting shape.** Author the audit-committee
   pack section that reports external and third-line audit
   findings under the fixed shape: summary, findings by class,
   trend, systemic themes, management response, remediation
   status, ask of the committee. Include a worked example
   applying the shape to one sampled audit (real or realistic).
7. **Four-audit coordination calendar.** Author a twelve-month
   coordination calendar showing when each of the five
   relationships is expected to visit, what preparation windows
   overlap, and how sampling coverage is coordinated across the
   four external audits without compromising independence.
8. **Third-line independence note.** Write a half-page note on
   how the runbook preserves CAE independence: what the head
   does and does not do with respect to CAE scope; how sideways
   written requests are recorded (see chapter 01 on
   loop-closes); how draft third-line findings return to the
   council for management response without violating
   independence.

## Deliverables

- `five-relationship-matrix.md` — the matrix as authored.
- `evidence-bundle-convention.md` — the assembly convention.
- `sampling-access-procedure.md` — the access procedure.
- `exit-meeting-discipline.md` — the exit-meeting note with
  script.
- `finding-triage-and-remediation-template.md` — the
  classification and template.
- `audit-committee-reporting-shape.md` — the pack section with
  a worked example.
- `four-audit-coordination-calendar.md` — the twelve-month
  coordination calendar.
- `third-line-independence-note.md` — the half-page note.

## Acceptance criteria

- The five-relationship matrix has every column for every
  relationship; no collapsed rows.
- The evidence-bundle convention names specific canonical formats
  (OSCAL, CycloneDX ML-BOM, SPDX AI, SLSA attestations,
  Sigstore-verifiable signatures, model / system / dataset cards);
  no folder-of-screenshots pattern.
- The sampling-access procedure names the specific control that
  prevents curation of the sampling population and the specific
  logging mechanism that makes tampering detectable after the
  fact.
- The exit-meeting script is three to five sentences and
  demonstrates the "state the question / close the question"
  discipline from chapter 01.
- The finding-triage classification is exhaustive across the five
  relationships' finding vocabularies.
- The remediation-plan template includes root cause,
  effectiveness review, and audit-committee visibility.
- The audit-committee reporting shape's worked example produces a
  brief that the head could present at the audit committee's next
  meeting without further edits.
- The four-audit coordination calendar names sampling-coverage
  coordination without conflating it with substance-coordination.
- The third-line independence note names both what the head must
  not do (direct scope, attend first-line interviews, edit
  drafts) and what the head should do (formal written requests,
  un-tampered access, factual-clarification response, management
  response at the audit committee).

## Stretch goals

- Draft the ISO/IEC 42006 sampling-quality expectations at the
  auditor's own quality-management level (as they inspect the
  head's discipline, an ISO/IEC 42006-accredited certification
  body is inspected by their accreditation body — UKAS, ANAB,
  DAkkS — and their sampling quality is one of the things
  inspected). Show how you would prepare for a joint
  accreditation-body observation of the certification body
  auditing you.
- Extend the sector-regulator section for your assumed sector
  with the actual examination-cycle expectations (SR 15-19 and
  SR 20-4 in banking; state insurance-department AI examination
  cycles; FDA GMLP post-market-surveillance examination
  patterns; OMB M-25-21 federal-agency examination expectations;
  RSP / PF / FSF external validation for frontier labs).
- Draft the two-week "certification body arrival playbook"
  — day-by-day preparation, day-of arrival protocol, exit
  protocol, and thirty-day post-visit close-out plan.
- Draft the specific integration with the AIMS document-control
  policy for post-visit remediation evidence — how corrective
  actions are versioned, retained, and re-presented at the next
  surveillance visit.

## Notes and starter guidance

- The single most common runbook failure is treating the five
  relationships as one. Force yourself to write each column of
  the matrix distinctly. If two rows share language, one of them
  is under-authored.
- The exit-meeting script is small but load-bearing. The head's
  behaviour in the first two minutes of the exit meeting
  determines whether the auditor perceives the enterprise as
  cooperative-but-professional, or defensive, or capitulating.
  Draft it, read it aloud, revise.
- The four-audit coordination is where under-coordination hurts
  the most in operation. Draft the calendar assuming realistic
  cadence overlap (certification-body surveillance in one month,
  regulator examination the next, third-line audit in the
  quarter after) and identify the coordination points the head
  owns.
- Third-line independence is a legally-load-bearing invariant in
  many jurisdictions. If your independence note is vague on any
  specific point, revise. Chapter 04 lists the specific must-not
  and should items.
