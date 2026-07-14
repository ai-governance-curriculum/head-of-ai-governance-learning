# Engagement Contracts With Level 50 Below and Level 70 Above

## Motivation

The level ladder scope (chapter 01) and the CxO adjacency map (chapter
06) tell the head *what is inside their box*. The engagement contract
tells the head *how the traffic flows across the box's two most
important edges*: downward to the level-50 architect and upward to the
level-70 CAIO (or the CIO / CTO / CDO / CFO / CEO cluster where no
CAIO exists).

Without these two contracts in writing, three predictable pathologies
develop:

- The head re-authors what the architect owes, because the deliverable
  boundary was never named.
- The head absorbs what the CAIO owes, because the escalation
  boundary was never named.
- The head defers what belongs to the head, because the accountability
  boundary was never named.

The two contracts prevent all three. They are short — one to three
pages each — signed by the head and the counterparty, and ratified
by the audit committee (for the downward contract) and the CEO (for
the upward contract).

This chapter is how to write both.

## The contract shape

Both contracts have the same structure, adapted from an operating-
model RACI plus a service-level agreement plus an escalation table.
The four sections are:

- **Consume** — what the head consumes *from* the counterparty
  (downward) or delivers *to* the counterparty (upward).
- **Deliver** — what the head delivers *to* the counterparty
  (downward) or consumes *from* the counterparty (upward).
- **Defer** — what the head explicitly does not do, sending it to
  the counterparty for authorship.
- **Escalate** — when and how the boundary is redrawn, and by whom.

Each section is a bulleted list of concrete deliverables. Vague
verbs ("collaborate on," "partner around") are prohibited; every
line is a nameable artefact with a cadence.

## Downward contract — head to level-50 architect

The downward contract is between the head and the senior AI
governance / risk architect at level 50. The architect is the head's
primary supplier of the twelve architectural deliverables enumerated
in chapter 01. This contract makes the supply relationship explicit.

### Consume — what the head consumes from the architect

Twelve architectural deliverables, on a documented cadence:

- **Control library.** Consumed at first-approval, updated on
  material regulatory change or annual review, whichever comes
  first. Delivered as a machine-readable catalogue (JSON, OSCAL, or
  equivalent), not a spreadsheet.
- **Policy taxonomy.** Consumed at first-approval, updated on the
  annual policy review cycle. Delivered as the parent policy plus
  sub-policies, standards, procedures, work instructions, with
  ownership matrix.
- **Cross-jurisdiction crosswalk.** Consumed at first-approval,
  updated at least quarterly and on material regulatory change.
  Delivered as the machine-readable map from EU AI Act obligations
  → NIST AI RMF categories → ISO/IEC 42001 controls → sector rule →
  enterprise control ID.
- **ISO/IEC 42001 AIMS scope.** Consumed at first-approval and at
  each ISO/IEC 42006 audit body inspection. Delivered as the Statement
  of Applicability, scope statement, interface to ISMS.
- **Risk taxonomy and appetite framework.** Consumed at first-
  approval and annually. Delivered as taxonomy plus appetite plus
  tolerance-limit definitions, aligned to ISO 31000 and ISO/IEC
  23894.
- **Assurance architecture.** Consumed at first-approval and on
  material change. Delivered as the release-assurance methodology
  document, gating criteria, and interface to level-35 evaluation
  engineering.
- **Evidence architecture.** Consumed at first-approval and on
  material change. Delivered as the machine-readable evidence store
  design plus interfaces to OSCAL, CycloneDX ML-BOM, SPDX 3.0 AI,
  model cards, system cards, dataset cards, SLSA.
- **Third-party program design.** Consumed at first-approval and
  annually. Delivered as tiering criteria, questionnaire library,
  evidence-request pack, continuous-monitoring pattern.
- **Post-market surveillance architecture.** Consumed at first-
  approval and on EU AI Act Chapter VII updates. Delivered as the
  Article 72 monitoring design and Article 73 reporting workflow.
- **GRC-for-AI reference architecture.** Consumed at first-approval
  and on vendor selection changes. Delivered as the integration
  design against the chosen platform (Credo AI, Holistic AI,
  ModelOp, Monitaur, ServiceNow AI Control Tower, IBM
  watsonx.governance, or equivalent).
- **Operating model.** Consumed at first-approval and annually.
  Delivered as RACI, cadence catalogue, escalation paths, first-line
  embed pattern.
- **Sector blueprints.** Consumed at first-approval and on sector
  regulatory change. Delivered as the sector-specific overlay for
  the enterprise's sectors.

### Deliver — what the head delivers to the architect

- **Regulatory-change signal.** New or material regulation the
  architect must fold into the crosswalk, with a target update date
  and the head's assessment of urgency.
- **Operating-fitness feedback.** Findings from the AIMS operating
  discipline — where the architecture is not operable, where the
  control library has gaps, where the evidence architecture is
  incomplete — with severity and requested resolution.
- **Regulator-engagement signal.** What regulators are asking for
  that the architect's design must adapt to (for example, an EU AI
  Office GPAI Code of Practice update).
- **Incident lessons-learned signal.** From the incident logbook,
  the architectural implications of what went wrong so the level-50
  design incorporates the lesson.
- **Sponsorship at CxO scope.** The head brings the architect's
  work into the CIO / CTO / CDO / CRO / GC conversations so the
  architect does not have to secure sponsorship personally for
  every design decision.

### Defer — what the head does not do

- Authoring the control library, policy taxonomy, crosswalk, AIMS
  scope, risk taxonomy, assurance architecture, evidence
  architecture, third-party program design, post-market surveillance
  architecture, GRC-for-AI reference architecture, operating model,
  or sector blueprints. If the head is drafting any of these, the
  contract has failed and the head must escalate to fix it.
- Executing methodology at level 35 (evaluation engineering) or
  level 25 (risk engineering) or level 15 (analyst legwork). Those
  are staffed and coached, not personally taken over.

### Escalate — when the boundary is redrawn

- On a material change to the architect's scope (a new deliverable
  becomes necessary — for example, a new sector blueprint), the
  head and architect co-propose to the CAE and the audit committee
  a scope update.
- On a persistent under-delivery from the architect (two consecutive
  quarters of missed cadence), the head escalates to the architect's
  reporting manager and, if unresolved, to the audit committee.
- On a persistent scope-drift attempt (the head being asked to
  re-author), the head escalates to the CAIO / CEO with the
  architect present.

### Signature and cadence

The downward contract is signed by the head and the architect,
ratified by the audit committee, reviewed annually, and versioned
in the AIMS document control.

## Upward contract — head to level-70 CAIO (or the equivalent cluster)

The upward contract is between the head and either the CAIO (where
the designation exists) or the officers who split the CAIO scope
(CEO, CIO / CTO / CDO, CFO) where it does not. The purpose is to
make explicit what the head delivers upward, what the head consumes
downward from the level-70 position, and where the head does not
absorb scope that does not belong.

### Consume — what the head consumes from level 70

- **AI strategy alignment.** The enterprise AI strategy, portfolio
  priorities, and technology-family selection, from which the head
  derives the governance function's forward calendar. Delivered
  annually at strategy season, with material-change updates.
- **Enterprise AI budget envelope.** The top-line envelope inside
  which the AI governance function budget is one line. Delivered
  annually at budget season.
- **External positioning direction.** The enterprise's public voice
  on AI, from which the head derives what the head can and cannot
  say publicly.
- **Escalation-and-appeal decisions.** When the AI governance
  council escalates a decision (stop-shipping, appetite breach,
  regulator-material issue), the level-70 position is the appeal
  body and produces the decision.

### Deliver — what the head delivers to level 70

- **Second-line coverage report.** Quarterly. Status of the
  seven-item second-line envelope from
  [[04-three-lines-at-leadership-scope]].
- **AI risk register at portfolio cadence.** Monthly at director
  level; quarterly at board level.
- **Regulator-engagement summary.** Monthly. Open matters, exams,
  filings, material changes.
- **Incident summary.** As they occur (any Sev 1 within 24 hours;
  Sev 2 within 72 hours) plus a rolling monthly digest.
- **Voluntary-code and standards-body posture recommendations.**
  Ahead of each sign-on decision (EU AI Office GPAI Code of
  Practice, G7 Hiroshima Code, White House Voluntary AI Commitments,
  Frontier Model Forum, Partnership on AI, MLCommons AI Safety, US
  AISI Consortium).
- **Function budget and vendor P&L.** Annually at budget season;
  quarterly at management review.
- **Multi-year investment case.** Every 24 months at strategy
  season, plus on demand for CFO / board decisions.
- **Board pack contribution.** The AI-risk section, ISO/IEC 38507-
  shaped, quarterly.

### Defer — what the head does not do

- Authoring AI *strategy*, AI portfolio P&L, or the enterprise-wide
  AI budget envelope. The head *co-produces* by providing the
  governance shape and risk envelope. The head does not sign the
  strategy document as the accountable executive.
- Speaking at CEO / board-seat scope externally. The head speaks at
  the head-of-role scope (ISO/IEC JTC 1/SC 42 chair, IAPP AIGP
  body-of-knowledge committee, Frontier Model Forum working group).
  The CAIO or the CEO speaks at CEO / board-seat scope.
- Managing the enterprise-wide AI budget. The head manages the
  governance function line and negotiates the AI-observability,
  AI-runtime security, GRC-for-AI, and assurance vendor P&Ls inside
  that line.

### Escalate — when the boundary is redrawn

- On a strategy pivot that changes the risk envelope (for example,
  entering the EU market with a high-risk AI system for the first
  time), the head requests a boundary review with the CAIO.
- On a CEO-scope external statement about AI that the head
  disagrees with as a governance matter, the head requests an audit-
  committee session with the CAIO / CEO present.
- On a persistent under-consumption of the head's risk register
  signal by the CAIO (two consecutive quarters of the CAIO not
  acting on flagged material risk), the head escalates to the audit
  committee.

### Signature and cadence

The upward contract is signed by the head and the CAIO (or the
functional equivalent cluster), ratified by the CEO, reviewed
annually, and referenced in both the head's and the CAIO's
charters. Where no CAIO exists, the upward contract is signed by
the CEO and the head, and lists the CIO / CTO / CDO / CFO
delegations for the CAIO's four scopes.

## The two configurations of the upward contract

**Configuration A — CAIO exists.** The upward contract is a single
document between the head and the CAIO, ratified by the CEO.
Independent audit-committee access is preserved regardless of
reporting line.

**Configuration B — no CAIO.** The upward contract is a set of
delegations across the CEO / CIO / CTO / CDO / CFO. The head
negotiates each fragment separately and asks the CEO to ratify the
composite. This configuration is more work to maintain but not
inherently worse; some enterprises consciously choose not to have a
CAIO and want the head negotiating each conversation directly. The
critical invariant is that *someone at CEO / board-seat scope* is
the appeal body — otherwise the head has no upward escalation and
the second-line function loses independence.

## What is *not* in either contract

- **Regulator engagement operating detail.** The head is the
  regulator interface; details of engagements are not delegated up.
- **AIMS internal audit findings.** These stay in the AIMS
  operating cycle and land in the quarterly management-review
  record, not in the upward contract.
- **Adjacency arbitration.** That is in the CxO adjacency map from
  chapter 06, not here.
- **Function personnel decisions.** Those are between the head and
  CHRO, not part of the CAIO / architect contracts.

## Example — a two-page downward contract table of contents

A concrete example of the downward contract's table of contents:

1. Parties, dates, ratification.
2. Consume (the twelve deliverables and their cadences).
3. Deliver (five upward signals and their cadences).
4. Defer (the enumerated list of what the head does not author).
5. Escalate (the three escalation triggers).
6. Signatures (head, architect, CAE observing, audit-committee chair).
7. Next review date.
8. Version history and AIMS document control ID.

Two pages. Signed. Referenced. When the boundary is challenged, the
head reaches for this document, not for a fresh argument.

## Summary

- Two engagement contracts — downward to the level-50 architect and
  upward to the level-70 CAIO (or functional-equivalent cluster) —
  are the artefacts that turn the level ladder scope from a diagram
  into an operating discipline.
- Each contract has the same four-section shape — Consume, Deliver,
  Defer, Escalate — and lists concrete deliverables with cadences,
  not vague verbs.
- The downward contract is signed by the head and the architect,
  ratified by the audit committee, reviewed annually. The upward
  contract is signed by the head and the CAIO (or functional
  equivalent) and ratified by the CEO, reviewed annually.
- Independent audit-committee access remains the invariant under any
  configuration of the upward contract.
- Exercise 6 in this module asks the learner to author both
  contracts for their target enterprise as a first-week-of-role
  deliverable.
