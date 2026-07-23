# The Enterprise Change-Management Plan Shape

## Motivation

The interpretation workflow of chapter 02 ends when the level-50
architect has the interpreted, prioritised obligation in hand and
begins updating the crosswalk and control library. That is where an
architectural design cycle takes over — outside the scope of the
head's operating discipline. But the design cycle is not what
lands change in the enterprise. What lands change is the
*enterprise change-management plan* that the head personally
authors, sponsors, and defends, sitting alongside the architect's
crosswalk update and translating it into the operating moves the
enterprise makes across every function, every business line, and
every regulator-facing artefact.

The failure mode this chapter closes is characteristic and, once
seen, embarrassing. The architect updates the crosswalk. The
policy taxonomy is regenerated. The control library reflects the
new obligation. Someone at level 15 issues an internal
announcement. And nine months later, the regulator finds the
enterprise has not actually done the thing. Product still routes
around the new step because nobody trained them. Procurement
signed a new supplier contract without the new clauses because
nobody told them the clause library had shifted. HR did not
refresh training. Communications was blindsided by a journalist
who read the same regulation the enterprise did. The board saw
"AI regulatory change management: on track" every quarter and
learns about the miss from the trade press. The architectural
update was real; the operating landing never happened.

The change-management plan is the head's insurance against that
outcome. It is the artefact that turns the crosswalk delta into
operating reality, with an accountable owner per lane, a cadence
per lane, and a defensible finish line per lane. It is not a
project plan (though it borrows discipline from project
management); it is not a risk assessment (though it feeds one); it
is not a communications plan (though it contains one). It is the
head-of-AI-governance instrument that makes regulator-facing
promises land inside the enterprise.

The reference frames are ISO/IEC 42001 clause 8.1 (operational
planning and control of the AIMS), clause 8.3 (AI system impact
assessment), and clause 10 (improvement — nonconformity and
corrective action), together with ISO 9001-lineage change control
in the QMS the enterprise operates. The plan is the head's own
document, but it presses against these clauses so that a
certification body under ISO/IEC 42006 recognises it as AIMS
evidence when the enterprise is audited.

## Core concept — the seven-lane plan

Every enterprise change-management plan the head authors has the
same seven lanes. Missing a lane is how the failure modes above
occur.

- **Lane 1 — Governance authority.** Who inside the enterprise is
  formally authorised to make the change happen, at what
  committee, with what documented decision.
- **Lane 2 — Communications cadence.** Who says what to whom, in
  what sequence, on what channels — CEO letter, function letter,
  team-level runbook update, external posture (Communications
  owns externally).
- **Lane 3 — Training refresh.** What training is updated, for
  which populations, on what timeline, with what completion
  discipline.
- **Lane 4 — Exception window.** Which prior exception-and-waiver
  records are affected, how the exception is closed or renewed,
  what the transition posture is for systems that cannot make the
  deadline.
- **Lane 5 — Board and audit-committee reporting.** How the
  change appears in the quarterly board pack cluster
  ([[mod-103-board-and-audit-committee-reporting]] chapter 01)
  and the audit-committee deep-dive cluster (chapter 02 of that
  module).
- **Lane 6 — Regulator-facing notification.** Where the change
  requires or invites communication back to the regulator — a
  filing under a specific article, a status update in a
  supervisory dialogue, a public-consultation submission.
- **Lane 7 — Third-party and supply-chain.** How the change is
  propagated to material suppliers of the enterprise's AI
  program — model vendors, GRC-for-AI tooling, evaluation
  services, notified bodies.

The rest of this chapter walks each lane in turn. The plan itself
is a document the head signs — the sign-out is not a bureaucratic
detail; it is what makes lane 1 real.

## Lane 1 — governance authority

The plan does not exist until it has a named authorising decision.
The failure mode here is subtle: the enterprise operates from a
document that circulates by email, is agreed by acclamation, and
lacks a decision record anyone can point to. The regulator, in an
examination, asks "when did the enterprise decide to make this
change, and who decided?" — and the enterprise cannot answer with
a date and a committee.

The head takes the interpreted obligation and the level-50
architect's proposed crosswalk delta to a formally chartered
committee — typically the AI governance council
([[mod-102-running-the-program]] chapter 01) or, for enterprise-
scale changes, the risk committee or executive committee. The
committee minutes record:

- The obligation and its citation.
- The GC opinion reference (the opinion itself remains privileged;
  the record notes its existence and its author).
- The proposed change and its scope.
- The decision — approved, deferred, modified — with reasoning.
- The authorised authority to execute (this is the head, unless
  the head has delegated).

The record is the authorising decision. Without it, later lanes
have no ground to stand on and later audit questions have no
answer.

For material changes — those affecting a substantial share of the
AI system inventory or crossing a threshold set in the enterprise's
risk appetite ([[mod-103-board-and-audit-committee-reporting]]
chapter 03) — the authorising decision includes an audit-committee
briefing. The head does not need audit-committee approval for
every regulatory change; the head does need the audit-committee
chair aware, so that when the pack lands, the material change is
not the first the chair hears of it.

## Lane 2 — communications cadence

Communications is where the plan most obviously interacts with
functions the head does not directly own. The Chief Communications
Officer owns external communication about the enterprise. HR
owns internal announcements to employees. The head owns *the
regulatory-change-specific overlay* — the substantive content that
makes those announcements say the right thing.

The cadence has four staged waves.

### Wave A — internal alignment

Before any external or broad-internal move, the head aligns the
CxO peers (chapter 05 of this module covers the coordination
pattern in detail). This is not "gain consensus"; it is "surface
disagreement early enough to resolve without disrupting later
waves". The wave A artefact is a briefing memo the head
circulates to the AI governance council and to the CxO peers:
CISO, CIO / CTO / CDO, CPO / DPO, CRO, CAE, GC, CFO, CHRO, CCO,
and (where present) CAIO. The memo states the change, the timing,
and the ask of each function.

### Wave B — enterprise-scale internal announcement

Where the change is enterprise-scale, the CEO (or CAIO or the head,
depending on enterprise structure) issues a signed internal
communication announcing the change. The letter says three things:
what is changing, why, and what the enterprise's posture is on
readiness. It is short — one page for the CEO's signature. It does
not contain implementation detail; it establishes the executive
posture that later waves refer back to.

The head drafts the letter; the CEO or CAIO's office refines and
sends it. Coordination with Communications is not optional — the
letter tone must be consistent with the enterprise's external
posture (Communications' job) and must not create a legal
disclosure obligation the enterprise is not ready for (GC's
review). Wave B without CEO signature is not enterprise-scale.

### Wave C — function-and-team-level rollout

Each function that owns an affected lane — product, engineering,
sales, procurement, HR, sector-facing regulatory relations —
issues its own function-level communication and updates its own
team-level runbooks. The head does not draft these; the head
supplies the substance and reviews the drafts. The point of wave C
is that the change reaches the daily work of the people who
actually operate the AI systems.

Wave C has the most execution risk in the whole plan. The head's
discipline: review-not-write, on a fixed timeline, with a
completion register the head can point at. Function heads who
miss the timeline are surfaced at wave D or at the next AI
governance council.

### Wave D — external posture confirmation

Communications finalises the external posture — the position the
enterprise takes if a journalist asks, if a customer asks, if a
prospect RFP touches on the obligation. The head supplies the
substance. GC reviews for exposure. Communications signs. Where a
proactive statement is appropriate — a blog post, an ISO/IEC 42001
public statement update, an entry in an ESG or trust-centre
disclosure — Communications drafts, the head reviews for accuracy,
GC reviews for exposure, the CEO or CAIO signs when the tier
warrants.

The external posture is not the enterprise "announcing compliance".
The head does not make compliance claims; the enterprise's
external claims about compliance belong to Communications and GC
jointly, with the head as substance owner. The head who lets
"we are fully compliant with X" appear in a blog post without
being able to point to the evidence has made a program-level
mistake that a regulator can and will use in later supervision.

## Lane 3 — training refresh

Every regulatory change of material scope drives a training
refresh — for the AI-governance function (owned by the head), for
the first-line operators of affected systems, and for the general
employee population where the change touches acceptable-use
policies.

The refresh has three tiers.

- **Tier 1 — function refresh.** The AI-governance function is
  briefed on the interpretation, the crosswalk update, and the
  operating change. This happens in the function's regular staff
  meeting or in a called session — no external LMS record needed,
  but a minute-record entry is kept.
- **Tier 2 — first-line role-based refresh.** Product managers,
  data scientists, ML engineers, evaluators, procurement
  specialists, sales engineers on regulated deals — each
  role-based population that operates the affected systems
  receives a role-specific update. This tier requires LMS record-
  keeping so completion can be audited. The head sets the
  completion SLA (typically 30 to 60 days from wave C).
- **Tier 3 — enterprise-wide policy refresh.** Where the change
  affects an acceptable-use policy (AI acceptable use, third-
  party model use, prompt-injection hygiene, data-handling in AI
  contexts), the enterprise's mandatory training programme
  incorporates the change on its next quarterly refresh. The
  head coordinates with HR / Learning & Development on curriculum
  update.

For each tier, the head cares about three attributes: content
accuracy (the head signs off), timing (owned by the head or by HR
under a service-level agreement), and completion evidence (owned
by HR or L&D; audited by the head against the SLA).

Training refresh is one of the lanes most often let slide when
the enterprise is under compliance-date pressure. The head who
lets tier 2 slip is buying an operational failure inside 90 days.

## Lane 4 — exception window

Every mature governance program carries exceptions — systems that
operate outside standard controls under a documented, dated,
committee-approved waiver
([[mod-102-running-the-program]] chapter 03 covers the exception
discipline). A regulatory change rearranges the exception
landscape.

Three things happen in lane 4.

- **Existing exceptions are re-scored.** The head instructs the
  desk to review every open exception against the new obligation.
  Some exceptions become invalid (the exception was against a
  control the new obligation replaces); some become more
  material (the underlying risk grew); some are unaffected. The
  re-scoring is captured in the exception register.
- **A transition-window posture is authored.** Some affected
  systems cannot achieve the new obligation by the compliance
  date without disrupting operations. The head authors a
  transition-window posture: which systems get how long,
  contingent on what interim safeguards, escalated through what
  committee. The transition-window posture is board-visible
  ([[mod-103-board-and-audit-committee-reporting]] chapter 04 on
  CxO sign-off flow).
- **A new-exception moratorium is considered.** For material
  changes, the head may impose a temporary moratorium on new
  exceptions in the affected control area, to prevent the plan
  from being undermined by exception creep during rollout. The
  moratorium is time-boxed and lifted after the plan reaches
  steady state.

Exceptions are a program-discipline signal. A regulator inspecting
the enterprise reads the exception register as a proxy for how
seriously the enterprise takes its own controls. A change-
management plan that ignores exceptions produces a rollout that
looks complete on paper and is riddled with exception-covered
holes in operation.

## Lane 5 — board and audit-committee reporting

The change appears in the quarterly board pack the head produces
under [[mod-103-board-and-audit-committee-reporting]]. Lane 5's
work is coordinating with the pack cadence.

- **Regulator-engagement summary cluster** — the change is
  reflected here if it involved a regulator interaction (a
  filing, a consultation submission, an examination outcome).
- **Regulatory-change tracking cluster** — the change is
  reflected here regardless, with its status (interpretation
  done, plan approved, rollout in progress, complete).
- **Portfolio risk-appetite cluster** — if the change shifted an
  appetite tolerance, the shift is called out.
- **KRI dashboard** — if the change added or reshaped a KRI, the
  new metric is introduced with a baseline.

For material changes, the audit committee receives a deep-dive
briefing at the quarter where the change is finalised, so the
committee has heard the substance directly rather than only via
the board summary. The head owns the deep-dive; GC and the level-
50 architect co-brief where their contribution is material.

## Lane 6 — regulator-facing notification

Some regulatory changes require or invite the enterprise to
communicate back to the regulator. Lane 6 catches those and
sequences them.

- **Required filings.** Where a new obligation requires the
  enterprise to file a statement, register a system, or lodge a
  post-market monitoring update, lane 6 owns the filing timeline
  and the artefact production. The filing goes through the
  regulator-engagement discipline
  ([[mod-104-regulator-engagement]] chapters 02 and 05).
- **Supervisory-dialogue updates.** Where the enterprise is in
  ongoing supervisory dialogue with a regulator on a related
  matter, the change is reported as part of the next update. The
  head signals the update in advance if the change is material.
- **Public-consultation participation.** Where the regulator is
  consulting on interpretive guidance or on adjacent regulation,
  the enterprise participates through the consultation
  discipline ([[mod-104-regulator-engagement]] chapter 06).
- **Voluntary transparency communications.** Where the enterprise
  chooses to communicate proactively (a public statement about
  its readiness posture, a joint-industry statement, a customer-
  facing FAQ), lane 6 coordinates with lane 2 wave D and with
  GC.

Lane 6 also names what the enterprise does *not* communicate to
the regulator during the change window — internal drafting
disagreements, tentative interpretations, transition-window
extensions the enterprise has not yet operationalised. The
discipline is that the enterprise communicates to regulators from
a settled position, not from a work-in-progress.

## Lane 7 — third-party and supply-chain propagation

AI programs run on suppliers. A change that the enterprise absorbs
without propagating to suppliers is a change that will fail at
the supplier boundary — a model provider that does not honour a
new data-handling clause, a GRC-for-AI tool that does not surface
the new obligation in its dashboard, a notified body that
sequences its assessment against an outdated version of the AIMS.

Lane 7 does four things.

- **Contract audits.** Procurement, coordinated with GC and the
  head, audits material AI-supplier contracts against the new
  obligation. Where the contract already covers the obligation
  (via a well-drafted regulatory-change clause), no action.
  Where it does not, procurement opens contract-amendment
  negotiations on a timeline aligned to the compliance date.
- **New-contract template updates.** The enterprise's model
  contract templates for AI suppliers are updated to reflect the
  new obligation. This work is one-shot and pays back on every
  subsequent procurement.
- **Supplier communications.** Material suppliers receive a
  formal communication naming the change, its effective date, and
  the enterprise's expectation of the supplier's own readiness.
  This is not "asking suppliers to comply" — legally the supplier
  is either in scope of the obligation or not — it is expressing
  the enterprise's expectation of how the supplier's product will
  behave.
- **Post-change supplier verification.** After the compliance
  date, procurement, coordinated with the desk owner from
  chapter 02, verifies that material suppliers have moved. This
  is an ongoing supplier-performance function
  ([[mod-102-running-the-program]] chapter 04 covers the third-
  party audit interface).

Lane 7 depends on the AI supplier inventory the level-50 architect
maintains and the head governs
([[mod-102-running-the-program]] chapters 06 and 07). Without
that inventory, lane 7 is a scramble every time.

## The plan document itself

The seven lanes are the shape. The plan document that ties them
together is a specific artefact the head signs. It has a fixed
outline the head reuses across regulatory changes:

- Change identifier, regulator, obligation citation, effective
  date, authorising decision reference.
- One-page executive summary — what, why, when, key risks.
- Lane-by-lane detail — for each of the seven lanes: named owner,
  key milestones, SLA, evidence-of-completion definition.
- Interdependencies — where lane N's completion depends on lane
  M's output.
- Escalation triggers — the specific conditions under which the
  plan is escalated to the AI governance council, to the audit
  committee, or to the CEO.
- Sign-out — the head's signature, the CxO sign-out where
  material (typically CIO / CTO for engineering-carried lanes,
  CHRO for training-carried lanes, CCO for external-facing
  lanes, GC for regulator-facing lanes).

The plan is versioned. Changes to the plan (extended timelines,
retired lanes, added lanes) are logged with reasoning. A plan
that never changed during rollout is either a very small change or
a plan the enterprise did not actually operate from.

## What the plan does not do

Three disciplines belong to adjacent modules and the plan
coordinates with, but does not replace, them.

- **Detailed engineering execution planning** — engineering
  leaders own the sprint plans, the release calendars, the
  test-strategy adjustments that turn the crosswalk delta into
  code. The change-management plan tracks their completion; it
  does not enumerate their tasks.
- **Legal opinion iteration** — GC's opinion (chapter 02 step 3)
  is not re-authored in the plan. If GC needs to revise the
  opinion mid-rollout, that revision is a separate GC artefact
  the plan references.
- **Enterprise risk-register updates** — the plan feeds the
  enterprise AI risk register ([[mod-102-running-the-program]]
  chapter 03) but does not replace it. Risk-register changes
  belong to that discipline, referenced by the plan where
  material.

## The one-sentence summary

The change-management plan is the seven-lane artefact — governance
authority, communications, training, exceptions, board reporting,
regulator notification, supply-chain propagation — that the head
signs, the AI governance council approves, and the enterprise
operates from to turn an interpreted obligation into landed
change; without it, the crosswalk update is architectural
paperwork and the miss is coming.

## Summary

- The interpretation workflow ends with the architect updating
  the crosswalk; the change-management plan is what turns the
  crosswalk update into operating reality across the enterprise.
- Seven lanes, all named, always present: governance authority,
  communications cadence, training refresh, exception window,
  board and audit-committee reporting, regulator-facing
  notification, third-party and supply-chain propagation.
- Governance authority is a formal committee record — decision,
  reasoning, authorised authority — without which the later
  lanes cannot be defended in audit.
- Communications is a four-wave cadence (internal alignment, CEO
  letter, function rollout, external posture) with Communications
  owning externally, HR owning internally, and the head owning
  the substance.
- Training refresh has three tiers (function, role-based, all-
  employee) with completion SLAs the head enforces.
- Exception discipline re-scores existing exceptions, authors a
  transition-window posture, and may impose a new-exception
  moratorium during rollout.
- Board reporting reflects the change across the pack clusters
  and includes an audit-committee deep-dive for material
  changes.
- Regulator-facing notification catches required filings,
  supervisory-dialogue updates, public consultations, and
  proactive transparency communications — always from a settled
  position, never work-in-progress.
- Supply-chain propagation is contract audits + template
  updates + supplier communications + post-change verification;
  it depends on the AI-supplier inventory the head governs.
- The plan document has a fixed outline, is signed by the head
  (and CxO peers per lane), is versioned, and is the artefact
  the enterprise actually operates from — not the interpretation
  memo, not the crosswalk delta.
