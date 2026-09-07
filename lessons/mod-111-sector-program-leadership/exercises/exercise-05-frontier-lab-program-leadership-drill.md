# exercise-05: Frontier Lab Program Leadership Drill

**Estimated effort:** 4 hours

## Objective

Instantiate the frontier-lab leadership shape from chapter 06
against a specific frontier-lab scenario. The deliverable is the
head's operating package for a lab that runs a published safety
framework (RSP, Preparedness Framework, FSF, or an equivalent):
a capability-threshold operationalisation plan, a mitigation-
standard implementation map, a governance-body operating record,
a White House / AISI / Frontier Model Forum external-engagement
map, a public-transparency cadence, and a board-and-Safety-and-
Security-Committee three-beat story.

The deliverable is not a survey of frontier-lab AI policy. It is
the operating record the head signs into so that the lab's
published commitments are credibly executed rather than credibly
declared.

## Prerequisites

- Chapter [06-frontier-lab-rsp-preparedness-fsf-leadership](../06-frontier-lab-rsp-preparedness-fsf-leadership.md)
  — read and internalised.
- Chapter 04 of [[mod-104-regulator-engagement]] — the regulator-
  engagement pattern the AISI and White House engagement extends
  (even though neither is a regulator in the conventional sense).
- [[mod-106-external-positioning-and-voluntary-codes]] chapters 02
  and 03 — the external-positioning portfolio and the voluntary-
  code discipline the RSP / Preparedness / FSF publication commits
  the lab to.
- [[mod-110-incident-leadership]] chapter 05 (post-incident
  learning cycle) and chapter 07 (calibration from public incident
  data) — the incident-summary publication commitments the safety
  framework carries.
- [[mod-103-board-and-audit-committee-reporting]] cluster 4 and
  any Safety-and-Security-Committee-adjacent cluster.
- A specific frontier-lab scenario. Options:
  - **Anthropic-shaped scenario.** A lab with a published
    Responsible Scaling Policy naming ASL tiers, a Responsible
    Scaling Officer role, and a public commitment cadence.
  - **OpenAI-shaped scenario.** A lab with a published
    Preparedness Framework naming Preparedness Levels, a
    Preparedness team, a Safety Advisory Group, and a Board's
    Safety and Security Committee.
  - **DeepMind-shaped scenario.** A lab with a published Frontier
    Safety Framework naming Critical Capability Levels and
    governance structures inside the DeepMind and Google AI
    Principles framework.
  - **New-entrant-shaped scenario.** A lab whose safety framework
    is under development, joining the Frontier Model Forum
    membership pathway, negotiating first-time AISI evaluation
    access, and preparing initial Seoul Commitment adherence.

## Steps

1. **Lab profile one-pager.** Half-page scoping: enterprise
   structure (independent lab, subsidiary of a hyperscaler,
   university-spinout), current safety framework and its
   published version, current governance body naming (RSO,
   Preparedness Committee, FSF Committee, or under-development
   equivalent), current model portfolio scale (deployed base
   models, deployed frontier models, in-training frontier
   models), and current commitment portfolio (White House
   Voluntary Commitments, Seoul Commitments, other public
   pledges). Note every commitment as either signed, considered-
   and-declined, or under-consideration.

2. **Capability-threshold operationalisation plan.** For each
   named capability threshold in the lab's safety framework —
   Critical Capability Levels, Preparedness Levels, or the
   sector's equivalent — author the evaluation plan the head
   runs. Per threshold, name:
   - The evaluation methodology (internal evaluations, external
     evaluations, red-team engagements, government-institute
     evaluations).
   - The evaluation cadence (every base-model release, every
     post-training modification of relevance, every deployment-
     configuration change, on a calendar-driven cadence
     independent of releases).
   - The determination body (the RSO / Preparedness Committee /
     FSF Committee), the head's role on that body, and the
     record of dissents.
   - The uncertainty-preservation practice — how the
     determination captures uncertainty rather than resolving
     it into binary crossed / not-crossed.
   Cite the specific published framework language for each
   threshold, or a `<!-- needs-research: -->` flag if the
   current published version is uncertain.

3. **Mitigation-standard implementation map.** For each named
   mitigation standard (ASL security standards, Preparedness
   mitigations, FSF mitigations), author the implementation
   status map. Per standard, name:
   - The specific security, deployment, and safety controls the
     standard requires at the applicable threshold posture.
   - The named counterpart function (CISO for weights-protection
     and insider-threat controls; product and deployment
     engineering for deployment controls; safety research for
     model-behaviour controls).
   - The implementation status (implemented; partially
     implemented with a milestone plan; not yet implemented with
     a milestone plan and dependency chain).
   - The escalation posture if a threshold moves and the current
     mitigation posture cannot be brought into compliance ahead
     of the move (development pause; deployment pause;
     scope-limited deployment; other).
   The head does not implement any single control; the head owns
   the integrated implementation-status view.

4. **Governance-body operating record.** Author the RSO /
   Preparedness Committee / FSF Committee operating record: chair
   (name the function; individual if publicly known), required
   members, meeting cadence, agenda ownership, decision recording,
   dissent-recording practice, and escalation to the board's
   Safety and Security Committee (or equivalent). Include the
   specific decision types the body owns (threshold determination;
   mitigation-standard sufficiency determination; deployment
   authorisation; framework revision) and the specific decision
   types the body does not own (product roadmap; research
   direction; commercial strategy).

5. **White House engagement map.** For each White House channel
   the enterprise engages (OSTP, NSC AI policy coordinator or
   equivalent, State Department for foreign-policy dimensions),
   name: the enterprise counterpart who fronts the channel
   (typically the policy function), the head's technical-substance
   contribution, the standing-engagement cadence, and the ad-hoc
   engagement pattern (capability-development briefings, safety-
   incident briefings, response to presidential- or Cabinet-level
   requests). Where the enterprise has signed the Voluntary
   Commitments, name each commitment and cite the enterprise's
   living evidence of adherence.

6. **US AISI / UK AISI evaluation-access negotiation record.**
   For each institute the enterprise has (or is negotiating)
   evaluation-access with, author the negotiated-terms record:
   scope (which capabilities and risk categories may be
   evaluated), security constraints (unreleased-model handling,
   NDA / classification treatment), results-sharing cadence
   (stage-gated, calendar-driven), publication policy (what may
   be published, by whom, on what timeline, after what internal
   review), and decision-authority preservation (evaluation
   results as input, not as substitute for the lab's own
   threshold determination). Name the legal counsel who fronts
   contractual terms and the head as the technical-and-program-
   integration counterpart.

7. **Frontier Model Forum and adjacent industry-body portfolio.**
   Author the industry-body engagement portfolio. Per body —
   Frontier Model Forum, Partnership on AI, MLCommons AI Safety,
   IEEE AI standards, ISO/IEC JTC 1/SC 42, sector-specific
   consortia — name: signed / considered-and-declined / under-
   consideration status per
   [[mod-106-external-positioning-and-voluntary-codes]]; chair or
   officer roles the enterprise holds, with the external-
   positioning committee's ratified scope; working-group
   participation and cross-body consistency (a public position in
   one body reconciled with public positions in others).

8. **Public-transparency cadence.** Author the annual publication
   calendar: safety-framework updates (RSP / Preparedness / FSF
   version updates with change logs), capability-threshold
   publications (as thresholds are approached, reached, or
   crossed and as security and competitive considerations allow),
   incident-summary publications (as the framework's publication
   threshold is met), and model system-cards for each major model
   release. Per publication, name the owner, the internal-review
   cycle, the audit-committee (or Safety and Security Committee)
   ratification step, and the response plan for the external
   reactions publication draws.

9. **Board-and-Safety-and-Security-Committee three-beat story.**
   Author the standing narrative in the three-beat structure from
   chapter 06: safety framework executed as published; external-
   engagement posture coherent; incident and near-miss history
   complete and defensible. The narrative is drop-in ready for
   the Safety and Security Committee (or the equivalent primary
   body) and reconciles with the Audit Committee's compliance-
   substance cluster.

## Deliverables

- `lab-profile.md` — the one-page scenario scoping and commitment
  portfolio.
- `capability-threshold-operationalisation.md` — the per-threshold
  evaluation plan.
- `mitigation-standard-implementation-map.md` — the per-standard
  implementation status with named counterparts and milestone
  plans.
- `governance-body-operating-record.md` — the RSO / Preparedness /
  FSF Committee charter, cadence, and decision-recording
  practice.
- `white-house-engagement-map.md` — the OSTP / NSC / State
  channel map and Voluntary Commitments adherence record.
- `aisi-evaluation-access-record.md` — the US AISI and UK AISI
  negotiated-terms record.
- `industry-body-portfolio.md` — the Frontier Model Forum and
  adjacent-body engagement portfolio.
- `public-transparency-cadence.md` — the annual publication
  calendar with owners and review steps.
- `board-and-ssc-three-beat-story.md` — the standing narrative
  for the Safety and Security Committee and Audit Committee.

## Acceptance criteria

- Every threshold in the lab's published safety framework has a
  concrete evaluation plan. Category labels ("we evaluate for
  cyber capabilities") without cadence, methodology, and
  determination-body naming fail the exercise.
- Every mitigation standard has a named counterpart function
  and an implementation status. "In progress" without a
  milestone plan and a dependency chain does not count as an
  implementation status.
- The governance-body operating record names the specific
  decisions the body owns and the specific decisions it does
  not own. Bodies whose scope is not decision-typed fail on
  accountability at incident.
- White House engagement is per channel, not aggregated. If the
  enterprise engages only OSTP, that is the record; if the
  enterprise engages OSTP, NSC, and State, each is a separate
  entry with a separate counterpart and cadence.
- AISI evaluation-access records include all five terms — scope,
  security constraints, results-sharing, publication, decision-
  authority preservation — per institute. Missing terms are
  flagged for negotiation, not left unspecified.
- Industry-body portfolio uses the signed / considered-and-
  declined / under-consideration discipline from
  [[mod-106-external-positioning-and-voluntary-codes]] and cites
  external-positioning-committee ratification for every chair
  or officer role.
- Public-transparency cadence is per publication with owner and
  review step. "Annual updates" as a category note fails; each
  scheduled publication is a named artefact with a scheduled
  window and an owner.
- The three-beat story is drop-in ready to the Safety and
  Security Committee's standing pack and reconciles with the
  Audit Committee's compliance-substance cluster.
- Uncertain framework status (RSP / Preparedness / FSF current
  published version; specific commitment adherence; specific
  AISI negotiation stage; Frontier Model Forum current
  membership and executive director) carries a
  `<!-- needs-research: -->` flag rather than a guess.

## Stretch goals

- Rehearse a capability-threshold-crossing decision meeting. The
  evaluation team returns results that a specific model is close
  to a Critical Capability Level. Author the decision meeting
  shape: participants, standing agenda, evidence expected,
  decision-authority resolution, dissent-capture, external-
  communications trigger, board-notification trigger. Include
  the counterfactual — what if the same evidence had returned
  more equivocal results?
- Rehearse a public-transparency schedule slip. The annual RSP
  / Preparedness / FSF update is late by one calendar quarter.
  Author the failure-mode analysis (what caused the slip), the
  external-communications posture (does the lab acknowledge the
  slip, and how), and the internal remediation plan (what
  changes so the next annual update does not slip).
- Circulate the capability-threshold operationalisation plan and
  the mitigation-standard implementation map to a peer at another
  frontier lab (through the Frontier Model Forum working-group
  channel or through direct executive contact) and incorporate
  one round of critique.
- Author the enterprise's stance for a scenario where a
  government (US or UK) requests pre-deployment evaluation access
  on terms materially outside the negotiated framework — the
  head's escalation posture, the legal counsel's contractual
  posture, and the CEO's public-comms posture.

## Notes and starter guidance

- The single most common failure mode is treating the safety
  framework as a compliance artefact rather than an operating
  program. Designs that produce framework documentation without
  an evaluation cadence, a mitigation-implementation status, or
  a governance-body operating record fail the exercise. Every
  published commitment must have a living operating counterpart.
- The RSO / Preparedness Committee / FSF Committee governance
  body is the accountability spine of the whole framework. If
  the body's decision-recording is thin, the framework is
  effectively unenforceable and every downstream commitment is
  weakened. Rehearse the body's decision-typing before you
  rehearse anything else.
- Public transparency is a program the head operates, not a
  publication event the head prepares for. Designs that treat
  publications as one-off preparations rather than as calendared
  operating outputs miss the sector's shape.
- AISI evaluation-access negotiation is joint work with legal
  counsel. The head does not front the contractual dimensions,
  and the legal counsel does not front the technical
  dimensions. Designs that put the head or the legal counsel in
  the wrong seat fail on operating fit.
- The Frontier Model Forum is the industry-body surface the
  sector expects the enterprise to engage. Non-participation is
  a defensible choice but must be a considered-and-declined
  choice recorded in the external-positioning portfolio, not an
  absence.
- Uncertain framework status is a live-issue item. RSPs,
  Preparedness Frameworks, and FSFs move on the labs' own
  publication cycles, sometimes annually. The exercise expects
  `<!-- needs-research: -->` flags on any item where current
  published version is uncertain.
