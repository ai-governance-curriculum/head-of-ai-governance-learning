# exercise-03: Portfolio Risk Register Cadence Drill

**Estimated effort:** 3 hours

## Objective

Produce a **portfolio AI risk register operating handbook** and run a
worked **twelve-month cadence drill** at portfolio scope. The
deliverable is not a register — the level-50 architect designed the
schema. The deliverable is the *operating discipline* the head runs on
top of the schema: appetite thresholds, deviation alarms, escalation
triggers, monthly and quarterly cadences, and a worked drill that
walks the register through a twelve-month period including at least
one appetite deviation, one incident-driven intake, one escalation to
the audit committee, and one closure with root cause.

## Prerequisites

- Chapter [03-portfolio-risk-register-cadence](../03-portfolio-risk-register-cadence.md)
  read and internalised.
- Familiarity with ISO 31000, ISO/IEC 23894, and ISO/IEC 27005 (at
  the read-the-vocabulary level — you should be able to name the
  risk-management process steps and where AI-specific and
  information-security-specific risks compose).
- The level-50 architect's AI risk taxonomy (real or assumed). If
  assumed, name at least eight taxonomy categories at the top level
  and record them.
- The council pack from exercise 01 (or a draft) because the
  monthly cadence composes with the council standing agenda.

## Steps

1. **Appetite framework.** Author the enterprise's AI risk
   appetite framework: for each of your eight-plus taxonomy
   categories, name the quantitative threshold (or the
   documented qualitative substitute), the approaching-appetite
   alarm level, the deviation alarm level, the breach level, the
   measurement cadence, and the first-line owner. Every threshold
   must be operable — not "moderate risk" but "no more than N
   tier-1 systems with an open finding older than 30 days," or
   equivalent. See chapter 03's example on the fairness category
   for shape.
2. **Register row schema.** Adopt (do not reinvent) the row
   schema from chapter 03 (Risk ID, title, category, description,
   inherent score, treatments, residual score, appetite band,
   owner, second-line challenge, next review, escalation triggers,
   regulatory nexus, linked evidence). Add any sector-specific
   fields your enterprise requires.
3. **Escalation-trigger catalogue.** Author the catalogue of
   escalation triggers — pre-agreed conditions under which a row
   moves out of council scope. At minimum, cover the five
   triggers in chapter 03 (appetite breach, cross-CxO impact,
   regulatory nexus threshold, sponsor-level ambiguity, ageing
   at the edge of appetite). Add any sector-specific triggers.
   Each trigger has: measurable condition, destination body, ask,
   timeframe, and loop-close.
4. **Monthly and quarterly cadences.** Author the operating
   cadence for the register: what happens at continuous intake
   (48-hour triage window), what happens at the monthly council
   review (chapter 01), and what happens at the quarterly
   portfolio deep-dive. For each, name the pre-read, participants,
   decision-set expected, and minute template.
5. **Twelve-month worked drill.** Author a twelve-month narrative
   drill in which the register operates through a realistic
   twelve-month period. The drill must include, at minimum:
   - Two new register rows opened via distinct intake channels
     (e.g., an incident and a horizon scan).
   - One category rolling from inside-appetite → approaching-
     appetite → at-appetite, with the corresponding trigger
     firing.
   - One escalation to the audit committee under a documented
     trigger, with the committee's response and the head's
     follow-through.
   - One risk closure with a documented root cause and a
     control-library-gap referral to the level-50 architect.
   - One retired risk (no longer applicable to the enterprise's
     current AI portfolio).
   - One appetite-threshold adjustment ratified at the annual
     review.
   The drill's monthly council reviews cross-reference to the
   council pack from exercise 01.
6. **Composition with the parent enterprise risk register.**
   Write a half-page note describing how AI risks of enterprise-
   material size are upserted into the parent enterprise risk
   register (under the CRO), how AI risks with information-security
   dimensions cross-reference the ISMS register (under the CISO),
   and how AI risks with privacy dimensions cross-reference the
   privacy register (under the CPO / DPO). Name the specific
   translation-layer artefacts.
7. **Closure discipline template.** Author the closure template
   for register rows: closure reason, root cause (using the
   architect's taxonomy for root-cause classification), any
   control-library gap the closure exposes, any policy or
   procedure change the closure implies, and any similar-risk
   pattern the closure suggests in the portfolio.

## Deliverables

- `ai-risk-appetite-framework.md` — the appetite framework with
  per-category thresholds, alarms, and owners.
- `register-row-schema.md` — the adopted row schema (with any
  sector-specific extensions).
- `escalation-trigger-catalogue.md` — the trigger catalogue with
  measurable conditions and destinations.
- `register-operating-cadence.md` — the intake, monthly, and
  quarterly cadences with pre-reads and expected decisions.
- `twelve-month-drill.md` (or `.pdf`) — the worked twelve-month
  narrative drill with monthly council references and audit-
  committee brief attachments.
- `parent-register-composition.md` — the half-page composition
  note.
- `closure-discipline-template.md` — the closure template with a
  worked example from the drill.

## Acceptance criteria

- Every taxonomy category in the appetite framework has an
  operable threshold, an approaching-appetite alarm, a deviation
  alarm, a breach threshold, a measurement cadence, and a named
  first-line owner.
- The escalation-trigger catalogue covers at least the five
  triggers named in chapter 03, each with a measurable condition,
  destination, ask, timeframe, and loop-close.
- The twelve-month drill executes at least the six required
  events (two new rows, one appetite roll-up, one escalation, one
  closure with root cause, one retirement, one threshold
  adjustment).
- The audit-committee escalation in the drill produces a defensible
  brief pack — summary, trigger reference, current position,
  proposed disposition, ask of the committee — traceable back to
  the council decisions that preceded it.
- The closure template captures root cause, control-library-gap
  referral, policy implication, and similar-risk pattern; the
  worked example demonstrates each.
- The parent-register composition note names the CRO, CISO, and
  CPO / DPO registers explicitly and describes the translation
  layer, not a promise to build one.

## Stretch goals

- Author the register in machine-readable YAML or JSON so a
  GRC-for-AI platform can import it directly, with controlled
  vocabulary tags aligned to the level-50 architect's taxonomy.
- Add a sector-specific example category and appetite framework
  (e.g., algorithmic bias in credit decisioning for banking;
  clinical-decision-support drift for health; fair-claims-adjudication
  monitoring for insurance; content-classifier drift for a public-
  sector deployment; frontier-capability-elicitation drift for a
  frontier lab).
- Draft the annual appetite-review pack — the artefact the head
  brings to the council and the audit committee to ratify the
  next year's thresholds. Show at least one uncomfortable
  proposed change (e.g., tightening a threshold in a business
  unit under P&L pressure) and how you would defend it.
- Draft the monthly-dashboard visualisation the council reviews
  under item 4 of the standing agenda (chapter 01), showing at
  least: new-since-last, appetite deviations, approaching-
  appetite, escalations fired, closures with root cause.

## Notes and starter guidance

- The single hardest thing about this exercise is writing operable
  appetite thresholds. It is very tempting to leave them as
  narrative ("we accept moderate fairness risk"). Force yourself
  to specific measurable statements even if they are wrong on the
  first pass. Chapter 03's fairness example is the shape.
- The twelve-month drill is where the pack becomes real. If the
  drill executes cleanly it means the appetite framework, the
  escalation triggers, and the cadence are internally
  consistent. If it does not, revise those artefacts, not the
  drill.
- The audit-committee escalation is the moment the pack is
  stress-tested from above. If you cannot write a defensible
  audit-committee brief for the escalation event you drilled,
  the escalation triggers or the register data are under-authored.
- The closure discipline is where continual improvement lives.
  A closure with no root cause is not a closure; it is a
  deletion. Every closure in the drill has a defensible root
  cause.
