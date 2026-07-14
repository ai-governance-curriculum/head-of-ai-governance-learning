# mod-102 — Running the AI Governance Program

**Estimated effort:** 18 hours
**Position on the track:** second module — the operating-discipline
module that takes the level-50 architect's design and turns it into a
running program.

## What this module is for

The head of AI governance at level 60 does not design the operating
system. The `senior-ai-governance-architect` at level 50 did that (see
[[mod-101-role-scope-and-leadership-shape]]). The head *runs* it.

Running it means seven overlapping operating disciplines:

1. Chairing the AI governance council and interfacing to the four
   adjacent committees (audit, enterprise risk, technology,
   executive) with minute-keeping and decision-log discipline the
   certification body will inspect.
2. Running the ISO/IEC 42001 AIMS operating calendar — internal audit
   rounds, management review, risk-treatment plan refresh,
   competence assessments, corrective actions, non-conformity
   closure — with the discipline ISO/IEC 42006 auditors observe.
3. Running the enterprise AI risk register at portfolio cadence —
   appetite tracking, escalation triggers, deviation alarms — under
   ISO 31000 / ISO/IEC 23894 / ISO/IEC 27005 as parent references.
4. Leading the interface to the five external audit relationships —
   the ISO/IEC 42001 certification body, ForHumanity IAAIS auditors,
   BABL AI Algorithm Bias Auditors, sector regulator examiners, and
   the third-line CAE.
5. Running annual and multi-year maturity assessments against the
   NIST AI RMF Playbook, ISO/IEC 42001 AIMS maturity dimensions, and
   the OWASP AI Security & Governance Checklist, and feeding the
   results into board and audit-committee decks.
6. Owning the AI system inventory quality bar — the discipline that
   the inventory is complete, current, and consistent under regulator
   inspection.
7. Owning the AI supply-chain evidence discipline at program scope
   — CycloneDX ML-BOM, SPDX 3.0 AI profile, SLSA attestations,
   Sigstore signatures, and model / system / dataset cards — with
   the completeness bar that stands up to regulator inspection.

This module answers each of the seven, produces the operating
artefacts the head runs the program with, and stages the audit-committee
and board reporting that follows in
[[mod-103-board-and-audit-committee-reporting]].

## Lecture chapters

- [01 — Chairing the AI Governance Council and Adjacent Committee Cadences](01-governance-council-and-minute-discipline.md)
- [02 — The ISO/IEC 42001 AIMS Operating Calendar](02-aims-operating-calendar.md)
- [03 — Running the Enterprise AI Risk Register at Portfolio Cadence](03-portfolio-risk-register-cadence.md)
- [04 — Leading the Third-Party Audit Interface](04-third-party-audit-interface.md)
- [05 — Running Annual and Multi-Year Maturity Assessments](05-maturity-assessment.md)
- [06 — Owning the AI System Inventory Quality Bar](06-ai-system-inventory-quality-bar.md)
- [07 — The AI Supply-Chain Evidence Discipline at Program Scope](07-ai-supply-chain-evidence-discipline.md)

## Exercises

Each exercise produces a running-program artefact the head can carry
into the operating rhythm. Every artefact composes with the artefacts
from [[mod-101-role-scope-and-leadership-shape]] and feeds the reporting
discipline in [[mod-103-board-and-audit-committee-reporting]].

- [exercise-01 — Governance Council Agenda and Minute Discipline](exercises/exercise-01-governance-council-agenda-and-minute-discipline.md)
- [exercise-02 — AIMS Operating Calendar Authoring](exercises/exercise-02-aims-operating-calendar-authoring.md)
- [exercise-03 — Portfolio Risk Register Cadence Drill](exercises/exercise-03-portfolio-risk-register-cadence-drill.md)
- [exercise-04 — Third-Party Audit Interface Runbook](exercises/exercise-04-third-party-audit-interface-runbook.md)
- [exercise-05 — Maturity Assessment Planning Drill](exercises/exercise-05-maturity-assessment-planning-drill.md)
- [exercise-06 — AI Inventory and Supply-Chain Evidence Discipline](exercises/exercise-06-ai-inventory-and-supply-chain-evidence-discipline.md)

## Learning objectives (from the plan)

- Consume the senior-ai-governance-architect (level 50) operating
  design and translate it into a running program — chair the AI
  governance council, run the adjacent committee cadences (audit,
  risk, technology, executive), own the minute-keeping and
  decision-log discipline.
- Own the ISO/IEC 42001 AIMS operating calendar — internal audit
  rounds, management-review cadence, risk-treatment plan refresh,
  competence assessments, corrective-action follow-through,
  non-conformity closure — with the discipline a certification body
  will inspect under ISO/IEC 42006.
- Run the enterprise AI risk register at portfolio cadence —
  appetite tracking, escalation triggers, deviation-from-appetite
  alarms — using ISO 31000 / ISO/IEC 23894 / ISO/IEC 27005 as parent
  references and consuming the risk taxonomy the architect designed.
- Lead the third-party-audit interface — ISO/IEC 42001 certification
  body, ForHumanity IAAIS auditor, BABL AI Algorithm Bias Auditor,
  sector regulator examiner, third-line internal audit — evidence
  packaging, sampling access, remediation plans, audit-committee
  reporting on findings.
- Run annual and multi-year maturity assessments against NIST AI RMF
  Playbook maturity dimensions, ISO/IEC 42001 maturity dimensions,
  and OWASP AI Security & Governance Checklist coverage; feed
  maturity reporting into board and audit-committee decks.
- Own the AI system inventory quality bar — the architect designed
  the schema; the head owns the operating discipline that the
  inventory is complete, current, and defensible under regulator
  inspection.
- Own the AI supply-chain evidence discipline at program scope —
  CycloneDX ML-BOM + SPDX AI + SLSA + Sigstore + model / system /
  dataset cards — with the completeness bar that stands up to
  regulator inspection; coordinate with
  `senior-ai-governance-architect` (level 50) on schema changes.

## Structure

- `01-…md` … `07-…md`: lecture chapters (this module).
- `exercises/`: six exercise prompts.
- `labs/`: long-form hands-on labs (module cycle authors these
  separately; see `labs/README.md`).
- `quizzes/`: knowledge checks (module cycle authors these
  separately).
- `resources.md`: curated primary-source references cited across
  the chapters.

## How to work through this module

The module is designed to be worked linearly. Chapter 01 sets the
governing-body discipline that every other chapter's outputs feed
into. Chapters 02 and 03 build the two central operating rhythms
(AIMS calendar and portfolio risk register) the head runs day-to-day.
Chapter 04 is the external-audit interface that inspects the outputs
of chapters 02 and 03. Chapter 05 is the maturity-assessment cadence
that reads across all four. Chapters 06 and 07 are the data
disciplines — inventory and supply-chain evidence — that the previous
chapters rely on and that any inspection surfaces first.

Exercises follow the same order. Exercises 1 and 2 (council and
AIMS calendar) are prerequisites for exercise 4 (external audit
runbook) because the runbook consumes both. Exercise 6 (inventory
and supply-chain evidence) can be worked in parallel with the
others but must be complete before the runbook is defensible.

By the end of the module, a working head-of-role has produced:

- A one-page governance-council charter and standing-agenda template
  with a minute-discipline exemplar.
- An annual AIMS operating calendar with named owners, evidence
  retention, and management-review inputs and outputs.
- A portfolio risk-register operating handbook with appetite
  thresholds, escalation triggers, and a worked deviation drill.
- A third-party-audit interface runbook covering all five external
  audit relationships and the ISO/IEC 42006 sampling discipline.
- A two-year maturity trajectory across the three references (NIST
  AI RMF Playbook, ISO/IEC 42001 AIMS, OWASP AI Security &
  Governance Checklist) with cost-of-move and audit-committee ask.
- An AI system inventory operating handbook and an AI supply-chain
  evidence completeness bar with per-tier expectations for CycloneDX
  ML-BOM, SPDX 3.0 AI, SLSA, Sigstore, and model / system / dataset
  cards.

These artefacts are the substrate the rest of the track builds on.
Every subsequent module — board reporting, regulator engagement,
regulatory change management, incident leadership, function
leadership, sector programs, budget — assumes them as running
inputs.
