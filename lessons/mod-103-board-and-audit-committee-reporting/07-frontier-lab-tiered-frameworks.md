# Frontier-Lab Tiered Risk Frameworks as Shape Lessons

## Motivation

Enterprise boards do not read Anthropic's Responsible Scaling
Policy, OpenAI's Preparedness Framework, or Google DeepMind's
Frontier Safety Framework. They read what the head of AI governance
puts in front of them (chapter 01). But the frontier labs *have*
published tiered risk frameworks that describe what their own
governing bodies see — the frameworks are the frontier labs'
answer to the same question the enterprise head is answering, in
a context where the risks and the technical maturity have both
been pushed further than most enterprises need to go.

The shapes are worth studying not because enterprises are frontier
labs (most are not) but because the frameworks encode design moves
that transfer. The tiered-risk discipline — pre-committing
responses to capability thresholds *before* the thresholds are
crossed — is exactly the discipline the risk committee (chapter
03) wants to see the enterprise operating. Enterprise boards will
increasingly ask for it. The head who has already thought
about how to adapt the shape is the head who has the answer ready.

This chapter is a short reading of the three published frameworks,
the design moves they share, and how the enterprise head adapts
the moves to a non-frontier-lab context.

## Core concept: tiers, pre-committed responses, and stop-shipping triggers

Across the three frameworks the common structure is:

- **A tier ladder** — a small number of named capability tiers,
  each defined by concrete threshold criteria (evaluation
  results, capability benchmarks, deployment scope, risk profile).
  Systems are assigned to tiers by evidence, not by intention.
- **Pre-committed responses per tier** — for each tier, a written
  set of responses the lab has committed to in advance. These
  cover access controls, deployment gates, evaluation cadences,
  external assurance, security posture, publication policy, and
  in the highest tiers, mandatory holds pending mitigation.
- **Stop-shipping (or stop-development) triggers** — explicit
  triggers that halt deployment (and in some frameworks halt
  development) if the response infrastructure for the next tier
  is not yet in place when a system reaches the tier threshold.
  The triggers are named, the authorising body is named, and the
  triggers are pre-committed *before* any specific system tests
  them.

The load-bearing move is pre-commitment. A response committed after
the threshold is crossed is a negotiation; a response committed
before is a policy. Governing bodies — frontier-lab boards or
long-term-benefit trusts, or enterprise boards — are looking for
the second, not the first.

## Reading the three frameworks briefly

Each of the three labs publishes and periodically updates its
framework. What follows is the *shape* to read for; the head
should read the current versions directly (linked in
[resources.md](resources.md)) rather than relying on a summary.

### Anthropic — Responsible Scaling Policy (RSP)

Anthropic's RSP defines a ladder of AI Safety Levels (ASL). Each
level has entry criteria (based on evaluations of dangerous
capabilities in categories including CBRN, autonomy, cyber, and
model-weight-security-adjacent risks) and required safeguards
(security, deployment, and process). Progression is governed by a
Capability Report / Safeguards Report process, with attestation and
board (long-term-benefit trust) visibility.

The transferable shape moves:

- Named capability thresholds tied to *evaluation results*, not to
  narrative estimates.
- Required safeguards *pre-committed* per tier, so the lab knows
  what infrastructure must be in place before crossing.
- Explicit process for what happens if evaluations show a
  threshold is crossed and the required safeguards are not yet in
  place (a pause / restrictive-deployment posture).
- Governing-body attestation as part of tier transitions.

### OpenAI — Preparedness Framework

OpenAI's Preparedness Framework describes tracked risk categories
(biological / chemical, cyber, self-improvement / autonomy,
persuasion, and other emerging categories in updated versions),
each with capability levels and deployment thresholds. The
framework describes Preparedness scorecards, a Safety Advisory
Group that reviews evidence, and executive- and board-level
governance of the highest-risk decisions.

The transferable shape moves:

- Multiple parallel risk categories rather than a single ladder,
  each with its own thresholds and required mitigations. Systems
  can be at different tiers on different categories.
- Named review body (Safety Advisory Group) as an internal
  second-line-like function with independence from the product
  organisation.
- Escalation posture to executives and to the board for
  highest-risk deployment decisions.

### Google DeepMind — Frontier Safety Framework (FSF)

Google DeepMind's FSF describes Critical Capability Levels (CCLs)
in specified risk domains, with associated evaluations, mitigations,
and response protocols. Updated versions extend to additional
domains and articulate the interaction between evaluations,
mitigations, and deployment / holding decisions.

The transferable shape moves:

- Explicit *Critical Capability Levels* — the thresholds at which
  a specified capability warrants a specified response.
- Evaluations *designed against the CCLs* rather than against
  benchmarks-of-convenience, so the evaluation-to-response chain
  is auditable.
- A mitigations palette (security-, deployment-, and access-
  focused mitigations) that pairs to each CCL.

## The design moves that transfer to enterprise scope

Enterprise systems are typically not at frontier-lab capability
thresholds. That does not mean the design moves do not transfer.
The moves are:

### Move 1 — the tier ladder is *evidence-defined*, not aspirational

Enterprises often draft capability-tier definitions that read like
strategy statements ("Tier 1 systems are our highest-impact AI
deployments"). Boards and regulators cannot audit that. The
transferable move is to define each tier by *concrete criteria a
third party could reproduce*: named deployment scope, named
risk categories, named data classes, named evaluation results,
named third-party dependencies. A system's tier assignment is a
record that can be defended by evidence.

### Move 2 — responses per tier are *pre-committed*

For each tier the enterprise commits, in writing, in advance, to
the responses that attach: the evaluation cadence, the impact-
assessment depth, the deployment gates, the external assurance
posture, the access controls, the monitoring intensity, the
incident-reporting sensitivity. Pre-commitment means the response
exists as policy before any specific system is assigned to the
tier.

The board and audit committee see the pre-commitment. The response
that arrives on the day is the response the policy prescribed,
not the response the head negotiated after the fact.

### Move 3 — stop-shipping triggers are named, authorised, and *have fired*

A stop-shipping trigger that has never fired is one the enterprise
should not claim as a control. The transferable discipline is:

- Triggers are named — specific evaluations, specific incident
  patterns, specific regulator actions, specific supply-chain
  events.
- Authorisation to fire is named — the release-assurance function
  (level 35 architect's function in most enterprise stacks), the
  head of AI governance, the AI Governance Council, or a
  combination with a documented decision tree.
- Firing is expected to happen occasionally. A pattern of
  never-fired triggers is a pattern of triggers with thresholds
  that are too permissive or of a monitoring posture that is not
  detecting.

### Move 4 — the tier framework is *reviewed and updated*

Capability moves faster than the tier framework. The transferable
move is that the tier framework itself is a *living* document with
a named review cadence (annual at minimum, with event-driven
interim reviews when a new capability class or regulator regime
emerges), a named review authority (typically the AI Governance
Council or the risk committee), and version control.

### Move 5 — the governing body sees the framework in force

The pack the risk committee (chapter 03) sees includes:

- The tier framework in force.
- Systems in each tier and tier-migration events in period.
- Stop-shipping triggers exercised in period.
- Framework updates proposed or ratified.

This is exactly the discipline chapter 03's cluster 2 (capability-
tier posture and escalations) describes. The tier framework and
the pack are two views of the same governance artefact.

## What does *not* transfer

The frontier-lab frameworks address risks — mis-aligned autonomous
capability, dangerous-capability enablement at global scale, model-
weight exfiltration to state-level adversaries — that most
enterprises are not deploying systems capable of. Copying the
frontier-lab risk categories verbatim into an enterprise's
appetite framework is a category error. The transferable content
is the *shape*, not the *risk taxonomy*.

Enterprise heads adapt by:

- Using the enterprise's own risk taxonomy (fairness, privacy,
  safety in the enterprise's operating sense, IP, security,
  robustness, transparency, accountability, sector-specific
  categories) as the categories the tier ladder operates over.
- Sizing capability thresholds to the enterprise's deployment
  scope. Tier 1 in an enterprise using AI in customer credit
  decisioning is not the same as Tier 1 in a frontier lab
  training foundation models.
- Naming pre-committed responses that fit enterprise operating
  reality — human-in-the-loop escalation, deployment scope
  restriction, external attestation, sector-regulator
  notification — rather than the responses that fit frontier-lab
  operating reality (compute-cluster access restriction,
  publication holds, weight-security hardening).

## Reading the frameworks over time

The three frameworks update. Anthropic has iterated the RSP through
multiple published revisions; OpenAI has updated the Preparedness
Framework as new risk categories and capability levels have
emerged; Google DeepMind has extended the FSF across successive
versions. Between-version deltas are themselves informative —
they show what the labs learned from operating the earlier
version, which is exactly the meta-question the enterprise head is
asking about its own framework.

Reading these frameworks quarterly, and reading the delta
commentary the labs publish when they update, is a cheap way for
the head to stay current on how the shape is evolving. The head
does *not* import specific responses without adaptation, but the
shape signal is worth having in the room when the risk committee
tunes the enterprise's own framework.

## Summary

- Anthropic's RSP, OpenAI's Preparedness Framework, and Google
  DeepMind's FSF are the published examples of tiered risk
  frameworks a governing body oversees; they are shape
  references, not templates.
- The design moves that transfer to enterprise scope are:
  evidence-defined tiers; pre-committed responses per tier; named,
  authorised, ever-fired stop-shipping triggers; a living
  framework with a named review authority; and the governing
  body seeing the framework in force each cycle.
- The risk categories and specific thresholds do *not* transfer —
  enterprises adapt to their own taxonomy, deployment scope, and
  operating reality.
- The frameworks update; reading the between-version deltas is
  the cheap way for the head to stay current on how the shape is
  evolving.
- Enterprise boards are moving toward comparable shape. The head
  who has adapted the design moves in advance is the head with
  the answer ready when the risk committee asks.
