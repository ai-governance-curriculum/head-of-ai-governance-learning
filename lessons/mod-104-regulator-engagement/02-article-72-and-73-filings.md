# Owning the Article 72 and Article 73 Filings at Leadership Scope

## Motivation

The two filing regimes the EU AI Act puts on the enterprise —
post-market monitoring under Article 72 and serious-incident
reporting under Article 73 — are where the running governance
program stops being an internal artefact and becomes an external
one. Everything that happens inside the AIMS is invisible to a
national competent authority until a filing crosses the boundary.
When one does, the authority reads it, forms a view of the
enterprise, and remembers.

That memory is durable. An NCA that reads a first Article 73 filing
as evasive, late, or technically thin does not reset that judgement
at the next quarter. The head of AI governance inherits the tone of
every prior filing when they walk into the next engagement. This is
why the filings are not delegable in signature. The
senior-ai-governance-architect (the paired level-50 role — see
[[mod-101-role-scope-and-leadership-shape]] chapter 04 for the
split) designs and operates the workflow. The head signs the
filing, briefs the board, and stands in front of the NCA. If the
head does not personally own that boundary, the program does not
have leadership scope; it has a workflow.

The rest of this chapter takes the two regimes in turn — Article 72
first because it is continuous, then Article 73 because it is
event-driven — then extracts the seven-question filing-defence
discipline the head runs before signing anything, and finally names
the NCA relationship posture and the boundary with the General
Counsel.

## Core concept: the head signs the filing, does not draft it

The distinction that keeps this chapter honest is the difference
between operating a filing workflow and owning the filing. The
architect owns the workflow: the data pipelines that feed the
post-market monitoring plan, the incident-detection thresholds, the
evidence-gathering runbook, the templated filing forms, the
sign-off routing. Chapter 04 of [[mod-102-running-the-program]]
covers this operating side.

The head owns four things the architect cannot own:

1. The signature on the filing itself. The signature is a personal
   attestation that the head believes the filing is accurate,
   complete, and defensible.
2. The board and audit-committee briefing that accompanies any
   material filing (see [[mod-103-board-and-audit-committee-reporting]]
   cluster 3 — incident and near-miss summary — for the shape).
3. The direct engagement with the NCA once the filing is in — the
   follow-up meeting, the on-site inspection, the written
   information request.
4. The technical position the enterprise takes on what the AI
   system did and what the enterprise did about it. Legal
   interpretation of whether an event meets a statutory definition
   is a General Counsel position; the technical position is the
   head's (chapter 07 of this module extends the boundary).

Everything below rests on that split.

## Article 72 — post-market monitoring at leadership scope

### What Article 72 requires

Article 72 of Regulation (EU) 2024/1689 requires providers of
high-risk AI systems to establish and document a post-market
monitoring system proportionate to the nature of the AI
technologies and the risks of the high-risk AI system. The
monitoring system must actively and systematically collect,
document, and analyse relevant data on the performance of the
high-risk AI system throughout its lifetime, and must enable the
provider to evaluate continuous compliance with the requirements
in Chapter III Section 2 (Articles 8-15). The system is described
in a post-market monitoring plan that forms part of the technical
documentation referred to in Annex IV.
<!-- needs-research: verify exact paragraph structure of Article 72
and the Annex IV reference to the post-market monitoring plan in
Regulation (EU) 2024/1689 -->

The plan is not a policy document. It is an operating specification
that names what data is collected, at what cadence, from what
source, against what performance thresholds, with what escalation
when a threshold is breached, and with what feedback loop back into
the risk-management system under Article 9. An NCA inspecting the
plan expects to see the specification, the evidence that the
specification is being executed, and the evidence that breaches
have driven action.

### The head's role on Article 72

The head is not the plan's author. The architect authors it. The
head owns four accountabilities on top of the plan:

- **Sign-off on the plan itself and on any material revision.** A
  post-market monitoring plan without a named executive signature
  is not a plan an NCA takes seriously. The head signs, dates, and
  files.
- **Annual review of the plan against the current portfolio.** The
  high-risk AI systems in scope one year may be a different set
  from the systems in scope the next. Plans that were proportionate
  when they were written become disproportionate as portfolios
  move. The head schedules and chairs the annual review; the
  architect prepares the delta.
- **Plan evolution as material events occur.** A serious incident
  under Article 73, a near-miss cluster, a regulator finding at a
  peer, a Union-level guidance update from the AI Office, or the
  emergence of a new capability tier in the portfolio each trigger
  an out-of-cycle review of the monitoring plan. The head decides
  whether the trigger warrants a revision.
- **Defensibility to an inspection.** The head has to be able to
  walk an NCA inspector through the plan, the operating evidence,
  and the change log without needing the architect in the room to
  answer. If the head cannot do this on any given high-risk system
  in the portfolio, the head is signing filings they do not
  understand.

### Peer coordination on Article 72

Article 72 monitoring touches every functional peer with an
adjacent oversight interest. The head coordinates the map; the
architect operates the joins.

- **Product and engineering** produce the raw performance data —
  accuracy, drift, latency, availability, human-oversight
  intervention rate, user complaint volume, adverse-event reports.
- **The CISO** covers cyber-adjacent monitoring: authentication
  anomalies, prompt-injection detection, model-serving compromise
  indicators. Where cyber monitoring overlaps with AI-system
  monitoring, the head names the joint owner and the escalation
  path in the plan itself.
- **The DPO** covers privacy-adjacent monitoring: subject-rights
  request volume against AI-driven decisions, data-quality signals
  that affect fairness, cross-border transfer posture where
  monitoring data itself is personal data.
- **General Counsel** reviews the plan for interpretive gotchas
  before it is filed or provided to an NCA — wording that commits
  the enterprise to positions it did not intend, wording that
  admits facts contested in litigation, wording that narrows or
  broadens statutory definitions unhelpfully.
- **The CRO** integrates the post-market monitoring output into the
  enterprise risk register (see [[mod-102-running-the-program]]
  chapter 03) so that trends from Article 72 monitoring surface at
  the enterprise-risk cadence, not only inside the AIMS.

The head is the one person in the room whose job title makes them
accountable for the plan as a whole. That is why the signature is
theirs.

## Article 73 — serious-incident reporting at leadership scope

### What Article 73 requires

Article 73 of Regulation (EU) 2024/1689 requires providers of
high-risk AI systems placed on the Union market to report any
serious incident to the market-surveillance authorities of the
Member States where the incident occurred. The report is made to
the national competent authority (or the authorities where more
than one Member State is affected — the coordination discipline
sits under Chapter VII, covered in chapter 01 of this module).
<!-- needs-research: verify that Article 73(1) frames the recipient
as the market-surveillance authorities of the Member States where
the incident occurred, in Regulation (EU) 2024/1689 -->

A serious incident is defined in Article 3(49) as an incident or
malfunctioning of an AI system that directly or indirectly leads
to any of the following: the death of a person or serious harm to
a person's health; a serious and irreversible disruption of the
management or operation of critical infrastructure; an infringement
of obligations under Union law intended to protect fundamental
rights; or serious harm to property or the environment.
<!-- needs-research: verify the exact wording of Article 3(49) and
that the four categories are as listed, in Regulation (EU)
2024/1689 -->

### The reporting timelines

Article 73 stacks three timelines. The head has to know all three
without looking them up, because incident triage decisions turn on
which timeline applies.

- **General rule — Article 73(2).** The provider reports the
  serious incident immediately after the provider has established
  a causal link between the AI system and the serious incident or
  the reasonable likelihood of such a link, and in any event not
  later than 15 days after the provider (or, where applicable, the
  deployer) becomes aware of the serious incident.
  <!-- needs-research: verify the exact 15-day formulation and the
  "immediately after establishing causal link or reasonable
  likelihood" phrasing in Article 73(2) of Regulation (EU)
  2024/1689 -->
- **Widespread infringement or serious-and-irreversible
  fundamental-rights breach — Article 73(3).** A shorter timeline
  applies — reporting immediately and no later than 2 days after
  becoming aware.
  <!-- needs-research: verify the 2-day timeline and the exact
  triggering categories in Article 73(3) of Regulation (EU)
  2024/1689 -->
- **Death of a person — Article 73(4).** A different short
  timeline applies — no later than 10 days after becoming aware.
  <!-- needs-research: verify the 10-day timeline and the
  triggering category for death of a person in Article 73(4) of
  Regulation (EU) 2024/1689 -->

The head who cannot recite the three timelines in the moment cannot
run the sign-off meeting when an incident lands. The architect
should preload the timeline on every incident triage packet, but
the head is the one whose recollection matters when the packet is
missing a detail and a decision has to be made in the room.

### The head's role on Article 73

The head owns four accountabilities on Article 73:

- **The signature on the filing itself.** The head signs the
  filing to the NCA. If the head is unavailable, the pre-nominated
  delegate signs; the delegate name is on file with the NCA in
  advance, not chosen in the moment.
- **The board and audit-committee briefing.** Every Article 73
  filing is briefed to the board through the incident cluster in
  [[mod-103-board-and-audit-committee-reporting]]. Material
  filings trigger an out-of-cycle briefing to the audit-committee
  chair and the risk-committee chair before the next scheduled
  board sitting.
- **Direct engagement with the NCA.** The head takes the follow-up
  call, attends the follow-up meeting, hosts the on-site
  inspection if one is called. The head does not delegate the
  NCA-facing seat to the architect. The NCA is a peer counterpart
  of the head; treating it as an architect-level counterpart is a
  positioning error the head does not recover from cheaply.
- **Incident-leadership face.** The head is the enterprise's
  visible incident-leadership presence internally as well —
  chairing the incident bridge, briefing the CEO, coordinating
  with Comms and Government Affairs. See
  [[mod-110-incident-leadership]] for the incident-leadership
  discipline the filing rides on top of.

### Peer coordination on Article 73

Serious-incident reporting is the most coordination-heavy filing
the head signs. The peer map is dense because the incident cuts
across every governance function at once.

- **The architect** operated the incident-response workflow that
  produced the evidence in the filing — timeline reconstruction,
  root-cause analysis, containment record, remediation record. The
  architect is the head's technical brief-holder during NCA
  engagement.
- **General Counsel** reviewed the filing for privilege posture,
  for interpretive gotchas on whether the event meets Article
  3(49), and for litigation-adjacent wording. GC also owns the
  interface with any parallel breach-notification regimes (GDPR
  Article 33 where personal data is implicated; sector regulator
  incident-notification obligations).
- **Comms** briefed on external posture — press-response readiness,
  customer-communication drafts, holding statements, employee
  communications. Comms does not draft what goes to the NCA; Comms
  aligns everything else with what does.
- **Government Affairs** coordinated the political relationships —
  Member State political contacts, EU institutional contacts,
  awareness of any parallel policy sensitivity that shapes how the
  filing will be received.
- **The CISO** covered cyber-adjacent evidence — logs, integrity
  attestations, chain-of-custody for artefacts.
- **The DPO** covered privacy-adjacent evidence — where the
  incident touches personal data, where subject-rights obligations
  are triggered in parallel, where the incident interacts with
  cross-border transfer posture.
- **The CRO** updated the enterprise-risk position — an Article 73
  event nearly always moves the enterprise risk register and
  usually moves at least one appetite statement (chapter 03 of
  [[mod-102-running-the-program]]).

The head does not do any of that work. The head runs the room in
which that work converges into a filing.

## The seven-question filing-defence discipline

Before the head signs an Article 72 revision or an Article 73
filing, the head walks through seven questions with the architect
and the immediate peer set. If the head cannot answer any one of
them clearly, the filing does not go out. The discipline is not a
template to fill in; it is the internal test the head applies.

1. **What happened, factually, in one paragraph?** No jargon, no
   framing, no attribution of blame. A paragraph a plaintiff's
   counsel or a journalist could read and not find weasel words in.
2. **When did we become aware, and how did we date that?** The
   Article 73 timelines run from the moment of awareness. The
   enterprise has to have a defensible position on when awareness
   was established and on the evidence for that date — logs, ticket
   timestamps, incident-bridge minutes, escalation records.
3. **Have we established causal link or reasonable likelihood?**
   Article 73(2) uses both phrases. The head has to be clear which
   the enterprise is asserting and what evidence supports the
   assertion. Filing under "reasonable likelihood" without a
   defensible technical rationale invites the NCA to press.
4. **What have we done to contain and remediate?** Containment is
   what stopped the harm continuing; remediation is what addresses
   the root cause. The head names both and names when each was
   completed or when each is expected to complete.
5. **Who is affected, and have they been notified?** Individuals,
   customer organisations, downstream deployers, integration
   partners, regulators in adjacent jurisdictions. Notification
   status is on the filing or is explicitly noted as pending with a
   named date.
6. **What is our current view of root cause, and what is the
   evidence?** A filing can be honest that root cause is still
   under investigation, but the head has to have a current view and
   name it. Silence on root cause reads as evasion.
7. **What corrective action are we committing to, by when?** The
   NCA reads corrective action as the enterprise's forward
   commitment. Vague commitments invite follow-up. Specific
   commitments with dates invite follow-up on the dates — which is
   the exposure the head wants, because it is manageable.

The seven questions are the head's discipline for Article 73. They
also apply to Article 72 plan revisions, in a lighter form: what
does the revised plan monitor that the prior plan did not, why does
that change now, what triggered the change, and what is the head
committing the enterprise to going forward.

## The relationship discipline with the NCA

A filing is not a one-shot event. It opens an engagement. The head
who treats a filing as a form to submit and forget has misread the
regulatory posture the AI Act creates. The head who treats the
filing as the opening move of a durable engagement with the NCA
has read it correctly.

Concretely, after any Article 73 filing the head expects:

- A written information request within a small number of weeks,
  asking for supporting documentation not included in the initial
  filing.
- A follow-up meeting request, usually by video, occasionally in
  person, to walk through the enterprise's account of the event.
- An on-site inspection request in the more serious cases,
  scheduled with reasonable notice, coordinated by the architect
  and hosted by the head.
- A follow-up letter closing the matter, or opening a formal
  investigation, or requiring a corrective-action plan against a
  fixed timeline.

The head prepares the enterprise for that sequence in advance. The
architect maintains the evidence repository so that information
requests can be answered within the requested window without a
scramble. GC maintains the privilege log so that responses do not
inadvertently waive protections. Government Affairs monitors the
political weather for any signal that the NCA's posture is
hardening or softening. The head runs the schedule of engagement
touchpoints as an active portfolio, not a reactive queue.

Chapter 05 of this module extends this into the durable NCA
relationship posture — the periodic proactive briefings, the
attendance at regulator-hosted convenings, the pre-clearance of
significant enterprise moves before they become filings. For the
purposes of this chapter, the load-bearing point is that Article 72
and Article 73 are what open the relationship. Everything else
builds on how the first filings land.

## The General Counsel boundary

The head takes the technical position. GC takes the legal position.
The two are related but not the same, and the difference matters
most under filing pressure.

The technical position covers what the AI system did, what data
the enterprise had about it, what evidence supports the account of
events, what containment and remediation were undertaken, and what
the corrective-action commitment is going forward. The head speaks
on all of that, in front of the NCA, without needing GC in the
room.

The legal position covers whether an event meets the Article 3(49)
definition of serious incident, whether a specific report is
legally required under a specific paragraph of Article 73, how the
filing interacts with parallel obligations (GDPR Article 33,
sector-regulator incident regimes, US state-level obligations),
what is protected by privilege, and what litigation posture the
enterprise is taking. GC speaks on all of that.

The failure mode the head avoids is drifting into legal
interpretation under time pressure — asserting that an event does
or does not meet Article 3(49) without GC's concurrence, agreeing
to statutory characterisations in an NCA meeting without a legal
check. The reverse failure — GC drifting into technical assertion
about what the system did — is equally corrosive to the
relationship and is GC's discipline to hold, not the head's.

Chapter 07 of this module extends this boundary in detail —
including the pre-agreed handoff protocol, the joint-briefing
convention, and how the two positions are integrated into a single
filing without one collapsing into the other. For this chapter the
head holds one rule: on the technical account, the head speaks; on
the legal characterisation, GC speaks; the head does not
freelance across the line under pressure.

## Summary

- The head personally owns the Article 72 post-market monitoring
  filing and the Article 73 serious-incident filing at leadership
  scope. The architect designs and operates the workflow; the head
  signs, briefs the board, and engages the NCA.
- Article 72 requires a documented post-market monitoring plan
  proportionate to the risk of the high-risk AI system, actively
  collecting and analysing performance data across the system's
  lifetime, with feedback into the risk-management system under
  Article 9.
- Article 73 stacks three timelines — the Article 73(2) general
  rule of 15 days from awareness, the Article 73(3) shorter rule
  for widespread infringement or serious-and-irreversible
  fundamental-rights breach, and the Article 73(4) shorter rule
  for death of a person. The head has to know all three without
  looking them up.
- The seven-question filing-defence discipline is the head's
  internal test before signing: what happened; when we became
  aware; causal link or reasonable likelihood; containment and
  remediation; who is affected and notified; root-cause view and
  evidence; corrective-action commitment with dates.
- A filing opens an engagement, not a form-submission event. The
  head prepares the enterprise for the follow-up information
  requests, follow-up meetings, and possible on-site inspections
  that Article 73 filings routinely trigger.
- The head takes the technical position (what the system did, what
  we knew, what we did about it); GC takes the legal position
  (does the event meet Article 3(49), is a specific report
  required, privilege, litigation posture). Chapter 07 extends
  this boundary.
- Peer coordination is dense — architect, product, engineering,
  CISO, DPO, GC, Comms, Government Affairs, CRO — and the head
  runs the convergence rather than doing any of the underlying
  work.
