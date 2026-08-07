# Frontier Lab — Leading an RSP, Preparedness, or FSF Program

## Motivation

The head of AI governance at a frontier lab operates against a
public policy commitment structure that is unlike anything in
banking, insurance, healthcare, pharma, public sector, or critical
infrastructure. The commitments are not regulator-imposed. They are
lab-adopted and lab-published. Anthropic's Responsible Scaling
Policy (RSP), OpenAI's Preparedness Framework, and Google DeepMind's
Frontier Safety Framework (FSF) are voluntary public policies that
the lab has committed itself to and that regulators, governments,
and civil society read as the labs' articulated safety architecture.
The Frontier Model Forum operates as the member-lab coordination
body around these commitments.

That policy structure is what makes the leadership problem
distinctive. In every other sector, the head executes governance
built around externally imposed obligations. At a frontier lab, the
head executes governance built around obligations the lab publicly
committed itself to — the RSP, the Preparedness Framework, or the
FSF, plus the White House Voluntary Commitments (July 2023) and the
Seoul Frontier AI Safety Commitments (May 2024) the lab has signed
onto — and the lab's credibility depends on the visible integrity of
that execution.

<!-- needs-research: verify the current status and version of the
Anthropic RSP, OpenAI Preparedness Framework, and Google DeepMind
Frontier Safety Framework as of the current date; each has been
revised at least once since initial publication. Confirm against
anthropic.com, openai.com, and deepmind.google. -->

<!-- needs-research: verify current White House Voluntary
Commitments status (multiple companies signed in July 2023 and
September 2023 rounds; subsequent policy has evolved) and Seoul
Commitments status (signed at May 2024 AI Seoul Summit). Confirm
against whitehouse.gov and gov.uk. -->

## Core concept — the RSP / Preparedness / FSF as the enterprise safety architecture

Each frontier lab's public safety framework has a common architectural
shape, even where the specifics differ by lab.

1. **Capability threshold definitions.** Named thresholds — Critical
   Capability Levels in the RSP; Preparedness Levels in OpenAI's
   framework; Critical Capability Levels in DeepMind's FSF — that
   describe capabilities of concern with sufficient precision to be
   evaluated against.
2. **Evaluation methodology.** How the lab evaluates whether a
   model reaches or crosses a threshold, including internal
   evaluations, external evaluations, and (in some versions) pre-
   deployment evaluation access for third parties including
   government-sponsored AI safety institutes.
3. **Mitigation commitments.** Safeguards the lab commits to if a
   threshold is crossed — security, deployment, and safety
   controls that must be in place before further development or
   deployment. In the RSP language, these are ASL (AI Safety
   Levels) with corresponding standards; in Preparedness, similar
   tiered mitigations; in FSF, similar.
4. **Governance mechanics.** Who inside the lab makes the
   determination that a threshold is crossed, who authorises
   continued development or deployment, how the board is engaged,
   and how disagreements between the safety function and product
   or research are resolved.
5. **Publication commitments.** What the lab commits to publish —
   updated policies, capability evaluation results, incident
   summaries, threshold crossings — and on what cadence.

The head of AI governance runs the program that operationalises all
five layers. That program has technical, organisational, and
external-communications dimensions the head is accountable for.

## The head's operating architecture

### The capability threshold operationalisation program

Capability thresholds only mean something if the lab can, on
demand, evaluate a model against them. The head runs the program
that produces that evaluation capability. Practically:

- The evaluation team runs threshold-relevant evaluations against
  every model that could plausibly reach a threshold, at a
  cadence appropriate to model development. New base models are
  evaluated. Post-training modifications that could increase
  capabilities are evaluated. Deployment configurations are
  evaluated.
- Evaluation methodology is documented in enough detail to be
  reproducible by external evaluators.
- Evaluation results are reviewed against the lab's threshold
  definitions by a designated body — commonly a Responsible Scaling
  Officer, a Preparedness Committee, an FSF Committee, or an
  equivalent function. The head is on that body or reports directly
  to it, depending on lab-specific structure.
- Uncertainty in threshold determination is preserved and
  reported. A binary crossed / not crossed determination that
  papers over model-behaviour uncertainty is a governance failure
  in itself.

### Mitigation-standard implementation

For each threshold and each mitigation level, the head runs
implementation of the corresponding security, deployment, and
safety standards. Practically:

- Security standards (typically escalating with capability
  threshold) touch model weights protection, insider threat
  posture, infrastructure security, and access control. The head
  coordinates with the CISO; the CISO owns implementation.
- Deployment standards touch what the model is allowed to be
  deployed for, in what modalities, with what monitoring, with
  what use-case restrictions, and with what human oversight. The
  head coordinates with product and deployment engineering.
- Safety standards touch model-behaviour red teaming, misuse
  monitoring, alignment training, and safeguards embedded in the
  model itself. The head coordinates with safety research.

The head is not the person who implements any single standard. The
head is the person who owns the integrated view — is every required
standard for the applicable threshold in place, or is it not — and
signs into the accountable executive tier that decides "may this
model be further developed or deployed given the current
mitigation status."

### Governance mechanics — the RSO / Preparedness / FSF Committee model

Each lab operationalises threshold determinations and deployment
decisions through a named body. Anthropic's RSP names a Responsible
Scaling Officer. OpenAI's Preparedness Framework names a
Preparedness team and Safety Advisory Group. DeepMind's FSF operates
through governance structures inside the DeepMind and Google AI
Principles framework.

<!-- needs-research: verify the current named governance structures
in each of Anthropic's RSP (Responsible Scaling Officer role and
current version's governance structure), OpenAI's Preparedness
Framework (Preparedness team, Safety Advisory Group, board's Safety
and Security Committee), and Google DeepMind's FSF as of current
publication versions. -->

The head's operating role in this structure is either the executive
running the body's day-to-day work, the executive presenting to the
body, or the executive chairing the body — depending on the lab's
specific design. In every case, the head is accountable for the
body's operating record: the decisions made, the evidence
supporting them, the dissents recorded, and the outputs published.

### Publication and transparency

The lab's public commitments include publication of updated safety
policies, capability threshold crossings, mitigation-standard
attestations, and (in some cases) incident summaries. The head owns
the publication pipeline: what is published, when, to what standard
of technical accuracy, with what audit-committee ratification, and
with what response plan for the external reactions publication
draws.

External positioning discipline from
[[mod-106-external-positioning-and-voluntary-codes]] applies at
elevated intensity. Every publication is a public commitment. The
credibility cost of an under-delivered commitment is durable; the
credibility cost of a walked-back commitment is durable.

## White House engagement

Frontier labs engage the White House directly, at the Office of
Science and Technology Policy (OSTP), the National Security
Council, and — for foreign policy dimensions — the State Department.
Engagement channels include:

- The Voluntary Commitments the lab signed onto. Adherence to the
  commitments is public-facing and interpreted by the
  administration through periodic engagements.
- Ad hoc briefings on capability developments the administration
  is interested in — offensive cyber, biosecurity, election
  integrity, national security.
- Presidential and Cabinet-level events where the lab's CEO or
  senior leadership appears.

The head coordinates with the lab's policy function on the AI-
specific technical substance of White House engagement. The policy
function fronts the political-relationship channel; the head
provides technical accuracy.

<!-- needs-research: verify current White House organisational
structure for AI policy (OSTP, NSC AI Policy Coordinator, or
equivalent) given executive-branch changes through 2025-2026. -->

## US AISI and UK AISI evaluation-access negotiation

The US AI Safety Institute and the UK AI Safety Institute conduct
pre-deployment evaluations of frontier models. Access to models for
evaluation is negotiated between each lab and each institute, on
terms that address:

- What the institute may evaluate the model for (which capabilities,
  which risk categories).
- Under what security and confidentiality constraints access is
  provided (unreleased model versions require unreleased-model
  handling).
- What evaluation results are shared with the lab, at what stage,
  and with what response cycle.
- What evaluation results may be published, by whom, on what
  timeline, and after what internal review.
- What the institute's role is in the lab's own threshold
  determination — evaluation results as input to the lab's decision;
  the lab retains the decision authority.

The head is inside the negotiation as the enterprise's technical
counterpart. Legal fronts the contractual dimensions; the head
fronts the technical and program-integration dimensions.

<!-- needs-research: verify current organisational status, sponsoring
department, and evaluation-access practice of the US AISI (at NIST)
given administration changes post-EO 14179, and of the UK AISI
including any renaming. Confirm against nist.gov/aisi and gov.uk. -->

## Frontier Model Forum and industry-body chair roles

The Frontier Model Forum (FMF) is the industry body founded by
Anthropic, Google, Microsoft, and OpenAI in July 2023 as a member
organisation of frontier AI developers. The FMF's stated remit
includes advancing AI safety research, identifying best practices,
supporting cross-industry information sharing, and coordinating
with governments and civil society on safety.

The head's engagement with the FMF has three dimensions.

1. The lab's own membership responsibilities — participating in
   working groups, contributing to shared publications, sharing
   safety-relevant information under agreed protocols.
2. Chair or officer roles the lab holds within the FMF. If the head
   or a designee holds a chair or officer role, the enterprise's
   external-positioning committee (see
   [[mod-106-external-positioning-and-voluntary-codes]]) has
   ratified the role, and the head operates against the ratified
   scope.
3. Adjacent industry bodies — Partnership on AI, MLCommons, IEEE
   working groups, ISO/IEC JTC 1/SC 42, industry-specific consortia
   — the lab engages with. The engagement portfolio is coherent
   with the FMF membership and with the lab's own public
   commitments.

<!-- needs-research: verify current Frontier Model Forum membership
(founding members plus any subsequent additions), current executive
director, current work streams, and any publicly released outputs.
Confirm against frontiermodelforum.org. -->

## The public-transparency cadence

Beyond regulator engagement, the head owns a public-transparency
cadence that other sectors do not run at this intensity.

- **Annual updates to the safety framework.** RSP versions,
  Preparedness Framework versions, FSF versions are published with
  a stated change log and rationale.
- **Capability-threshold publications.** Where the lab has
  developed or tested capabilities the safety framework flagged as
  relevant, the lab publishes what it can consistent with security
  and competitive considerations.
- **Incident-summary publications.** Where a safety-relevant
  incident has occurred, the lab publishes an incident summary
  consistent with the framework's commitments. Incident
  leadership discipline from [[mod-110-incident-leadership]]
  applies.
- **Model system-cards and evaluation results.** Each major model
  release carries a system card documenting capabilities,
  limitations, evaluations run, and safety-relevant findings.

The transparency cadence is a program the head operates, on a
calendar the audit committee or the board's safety and security
committee ratifies, with the discipline that a missed publication
is a credibility event the enterprise treats as a program failure.

## The head's board-level story at a frontier lab

At the board — often with a dedicated Safety and Security Committee
in addition to an Audit Committee — the AI governance story has
three beats.

1. The safety framework (RSP / Preparedness / FSF) is being
   executed as published. Capability evaluations are current;
   mitigation standards for the current threshold posture are in
   place; the governance body has met on its stated cadence; no
   commitment has quietly slipped.
2. External-engagement posture is coherent. Voluntary Commitments
   and Seoul Commitments are being lived up to; White House and
   AISI relationships are current; FMF and adjacent industry-body
   participation is on track; the public-transparency cadence is
   met.
3. Incident and near-miss history is complete and defensible.
   Incidents that met the framework's publication threshold have
   been published; incidents below the threshold have been logged
   and analysed; the audit committee has visibility into the
   pattern.

## Summary

- Frontier lab AI governance is built around a lab-published
  safety framework (Anthropic RSP, OpenAI Preparedness Framework,
  Google DeepMind FSF) that names capability thresholds,
  evaluation methodology, mitigation standards, governance
  mechanics, and publication commitments — plus the White House
  Voluntary Commitments (July / September 2023) and Seoul
  Commitments (May 2024) the lab has signed onto.
- The head operationalises all five framework layers: capability
  threshold evaluation, mitigation-standard implementation,
  governance mechanics (RSO / Preparedness Committee / FSF
  Committee), and publication.
- White House engagement runs through OSTP and NSC channels with
  the lab's policy function fronting; the head contributes
  technical substance.
- US AISI and UK AISI evaluation-access is negotiated per lab, per
  institute, on terms addressing scope, security, results-sharing,
  publication, and decision-authority.
- Frontier Model Forum membership and chair or officer roles are
  ratified through the external-positioning discipline in
  [[mod-106-external-positioning-and-voluntary-codes]] and
  operated to the ratified scope.
- Public-transparency cadence — annual framework updates,
  capability-threshold publications, incident-summary publications,
  model system-cards — is a program the head operates, on a
  calendar the board ratifies, treating any missed publication as
  a credibility event.
- Board-level story has three beats: framework executed as
  published; external-engagement posture coherent; incident and
  near-miss history complete and defensible.
