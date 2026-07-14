# exercise-01: Governance Council Agenda And Minute Discipline

**Estimated effort:** 3 hours

## Objective

Produce a defensible **AI Governance Council operating pack** for the
enterprise you would run (or already run) the council at, consisting
of a standing-agenda template, a minute template, a decision-log
convention, and a worked minute for one full council item. The pack
must be defensible to an ISO/IEC 42001 certification body sampling
under ISO/IEC 42006, to a third-line CAE observer, and to an
audit-committee chair reading the last twelve months of minutes.

The deliverable is not "notes about how we run council." It is the
document set the council actually operates from, plus one worked
example a certification-body auditor could sample.

## Prerequisites

- Chapter [01-governance-council-and-minute-discipline](../01-governance-council-and-minute-discipline.md)
  read and internalised.
- Chapter [01-level-ladder-and-leadership-boundary](../../mod-101-role-scope-and-leadership-shape/01-level-ladder-and-leadership-boundary.md)
  (mod-101) — the level-ladder scope that defines what decisions the
  council takes versus refers up or down.
- Familiarity with the level-50 architect's operating-model RACI (or
  a working assumption of it if you are building the pack for a
  hypothetical enterprise).
- A concrete enterprise in mind, with an assumed sector (banking,
  insurance, health, pharma, public sector, frontier lab, tech
  platform, industrial) and reporting-line configuration (chapter
  07 of mod-101).

## Steps

1. **Council charter one-pager.** Write a one-page council charter
   naming: purpose, decisions the council takes, decisions it does
   not take, voting members and standing attendees, quorum, voting
   convention (consensus / simple majority / head-with-appeal),
   frequency, escalation destinations, secretariat, minute owner,
   and document-retention rules. Every field is specific — no
   "as appropriate" or "as required."
2. **Standing agenda template.** Author the standing agenda
   template following the twelve-item skeleton in chapter 01
   (approvals, actions, AIMS dashboard, risk register, incidents,
   third-party, release escalations, policy exceptions, regulator
   summary, external positioning, standing risks, AOB and forward
   calendar). For each item, specify: expected pre-read, timebox,
   decision or information disposition, and owner. Deviations
   from the twelve-item skeleton are permitted; justify each in one
   line.
3. **Minute template.** Author the minute template following the
   fields in chapter 01 (item ID, title, category, presenting
   owner, pre-read reference, question stated, discussion summary,
   decision, vote record, owner and review trigger, cross-
   references). The template is machine-parseable — every field is
   present per item; a well-formed minute always has every field
   populated.
4. **Decision-log convention.** Specify the decision-log
   convention — how decisions are numbered, how they are cross-
   referenced from the minute to the log, how the log is queried
   ("show me all live policy exceptions with review triggers
   coming due in the next 30 days"), and how errata to approved
   minutes are recorded. The log is a first-class artefact under
   AIMS document control, not a spreadsheet.
5. **Worked minute — one full item.** Draft a minute for one
   council item at the full depth the template requires. Pick a
   scenario at least this complex: a request to grant a 60-day
   exception to a policy, a request to accept a residual risk at
   the edge of appetite, a request to endorse an incident-
   containment action, or a request to sign off on a
   voluntary-code adoption. The minute must be defensible under
   sampling — a reader six months later can tell what was decided,
   by whom, on what evidence, and when it will be revisited.
6. **Escalation choreography table.** Author a table listing the
   council's escalation destinations (audit committee, enterprise
   risk committee, technology committee, executive committee AI
   standing item, GC, CAE) with, per destination: the ask type,
   the loop-close mechanism, the standing-cadence at which the
   destination sees the escalation. See chapter 01 on
   loop-close discipline.
7. **CAE-interface note.** Write a half-page note describing how
   the council's operation preserves third-line independence: what
   the head does and does not do with respect to the CAE's scope,
   how sideways written requests are recorded, and how draft
   third-line findings return to the council for management
   response without violating independence. See chapter 04.

## Deliverables

- `council-operating-pack.pdf` (or `.md` collection) — one document
  containing the charter, standing agenda, minute template, and
  decision-log convention as first-class sections. Ready to circulate
  to the audit committee for ratification.
- `worked-minute-example.md` — the worked minute at full depth for
  one item.
- `escalation-choreography.md` (or CSV) — the destinations,
  ask types, loop-closes, and cadences.
- `cae-interface-note.md` — the half-page third-line independence
  note.

## Acceptance criteria

- The charter names *specific* decisions the council takes and does
  not take. Generic language ("as appropriate," "as required") is
  disqualifying.
- The standing agenda has twelve items (or explicit-justified
  deviations) with pre-read, timebox, disposition, and owner per
  item.
- The minute template covers every field named in chapter 01.
- The worked minute is defensible under a sampling read six months
  later — a reader can reconstruct what was decided, by whom, on
  what evidence, and when it revisits.
- The decision-log convention supports at least three canonical
  queries (live exceptions, upcoming review triggers, decisions
  in the last quarter by category).
- The escalation choreography has a loop-close mechanism per
  destination — not just an ask.
- The CAE-interface note preserves independence while enabling
  coordination on access; both are named.

## Stretch goals

- Draft the two-year minute retention and archival policy that
  composes with the AIMS document-control policy — how minutes are
  locked, how errata are appended, how retention windows are
  determined per record class.
- Draft the specific mechanism by which a dissent from a voting
  member is captured and preserved in the minutes such that
  subsequent audits can trace the dissent to the record. Include a
  worked dissent example.
- Author the pack in a way that is directly importable into the
  GRC-for-AI platform the level-50 architect selected (Credo AI,
  Holistic AI, ModelOp, Monitaur, ServiceNow AI Control Tower, IBM
  watsonx.governance, or the actual platform). Structured
  formatting (YAML front matter, controlled vocabulary tags)
  counts.
- Circulate the pack to a peer at another head-of-role or at
  audit-committee-chair level and incorporate one round of critique.

## Notes and starter guidance

- The charter is the audit-committee-ratifiable version of the
  council. If you would not be comfortable submitting your draft
  to the audit committee for ratification, revise it.
- Chapter 01's chairing behaviour section — state the question,
  close the question — is the load-bearing habit the pack
  enforces. If your minute template does not surface the *question
  stated*, the pack under-enforces the discipline.
- Resist the urge to make the standing agenda expand under time
  pressure. Councils that meet for four hours because everyone's
  topic gets added are working groups. The timebox is the
  discipline.
- Test the pack by sampling: pick any three minutes you have
  drafted (or would draft) and ask yourself whether an
  ISO/IEC 42006 auditor could infer top-management commitment,
  management-review coverage, and continual improvement from
  them alone. If not, the pack is under-authored.
