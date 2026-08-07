# Shape Lessons from Frontier-Lab External Positioning

## Motivation

The frontier AI labs — Anthropic, OpenAI, Google DeepMind, and
adjacent — operate under a specific kind of public scrutiny that
non-frontier enterprises do not yet face at the same intensity.
Every public safety commitment they make is read, cited,
compared against peer commitments, tracked over time for
consistency, and used as the reference point when regulators,
academics, journalists, and civil society write about the
industry. The labs have, in response, built a small set of
distinctive external-positioning artefacts: Anthropic's
Responsible Scaling Policy (RSP), OpenAI's Preparedness
Framework, and Google DeepMind's Frontier Safety Framework
(FSF).

For the head of AI governance at a non-frontier enterprise,
these artefacts are not a template to copy. The frontier-lab
context — model capabilities that are the plausible source of
catastrophic risk, evaluation methodologies that are actively
under development, board-level oversight structures that carry
external commitment on model deployment decisions — is
different enough from the enterprise's own context that direct
transplantation would misfire. But the *shape* of what the
labs have built — the discipline of the artefact, the cadence
of its updates, the way each artefact interacts with the lab's
regulator engagement and its voluntary-code portfolio — is
shape the enterprise can learn from without copying wholesale.

The head who reads the frontier-lab artefacts as *shape
lessons* extracts what the enterprise's equivalent, at
enterprise scale, might look like. The head who reads them as
templates transplants a discipline that does not fit and
produces a public commitment the enterprise cannot honestly
run.

This chapter walks the three frontier-lab artefacts, extracts
the shape lessons the enterprise can apply, and closes with the
enterprise-equivalent posture that is emerging (and where the
enterprise's own posture-authoring discipline should build in
that space).

## The three artefacts, as artefacts

The three artefacts share four durable properties. Understanding
the properties matters more than the specific commitments each
contains, because the specific commitments will continue to
change and the properties will not.

- **Publicly published, with named versions.** Each artefact
  is on the lab's public website, versioned by date, with
  earlier versions retained or referenced. The lab commits
  to the version publicly and updates the version publicly.
- **Committed to a specific update cadence.** Each artefact
  is scheduled for review and update — Anthropic's RSP has
  gone through multiple iterations since the original 2023
  version; OpenAI's Preparedness Framework has been updated
  since its December 2023 release; Google DeepMind's FSF was
  first published in May 2024 with subsequent revisions.
  <!-- needs-research: verify the current published version and
  update cadence of Anthropic's Responsible Scaling Policy
  against anthropic.com; OpenAI's Preparedness Framework
  against openai.com; and Google DeepMind's Frontier Safety
  Framework against deepmind.google. Confirm the specific
  version numbers, publication dates, and any material
  substantive changes across versions before citing at
  audit-committee depth. -->
- **Tied to specific operating disciplines inside the
  organisation.** Each artefact is not just a public statement;
  it commits the organisation to specific evaluation
  procedures, threshold-based deployment gates, and
  escalation processes internally. The public commitment and
  the internal operating discipline are load-bearing on each
  other.
- **Board-level oversight.** Each artefact contemplates a
  role for the organisation's board or a designated
  board-level structure in reviewing or ratifying the
  commitment and its exercise. This is the property most
  directly relevant to the head of AI governance at
  enterprise scale, because it is the property that most
  directly parallels the head's own audit-committee
  reporting cadence
  ([[mod-103-board-and-audit-committee-reporting]]).

The four properties together are what make the artefacts
*credible* — a public statement that is not versioned, not
tied to internal discipline, or not board-overseen is a
statement, not a policy the organisation is willing to be
measured against.

## Anthropic Responsible Scaling Policy — shape lessons

Anthropic first published a Responsible Scaling Policy in
September 2023 and has iterated it in subsequent versions.
<!-- needs-research: verify the current published version of
Anthropic's Responsible Scaling Policy, its current AI Safety
Level (ASL) tier structure, and the specific evaluation
methodology and deployment-commitment discipline the current
version carries, against anthropic.com/responsible-scaling-
policy or the current canonical URL. -->

The load-bearing shape properties of the RSP as of the research
window are the following.

- **Capability-tier framework.** The RSP defines a set of AI
  Safety Level (ASL) tiers, each characterised by capability
  thresholds. As a model's capabilities cross a threshold, the
  next tier's safety commitments come into force.
- **Evaluation-based tier assignment.** Assignment to a tier is
  based on the outcome of specific published evaluations. The
  evaluations are described in the RSP; the results of
  evaluations are used to determine what tier a model has
  reached and therefore what commitments apply.
- **Deployment-and-training commitments per tier.** Each tier
  carries specific commitments — on the security posture
  around the model, on the deployment restrictions, on the
  training-continuation posture, and on the disclosure
  posture.
- **Commitment to iterate.** The RSP explicitly commits
  Anthropic to update the policy as the field and the
  organisation learn more, and to publish those updates.

The shape lessons the head extracts, applicable to the
enterprise's own context whether frontier or not:

- A *tier-based framework* is a defensible way to relate a
  system's capability or risk profile to the specific
  commitments the enterprise is willing to make. The
  enterprise's tiers do not have to be capability tiers —
  they can be risk-classification tiers (Annex III versus
  non-Annex III under the AI Act, systemic-risk versus non-
  systemic-risk under Article 55, or the enterprise's own
  internal-risk taxonomy). What matters is that the tiers are
  *published*, *bounded*, and *evaluated against*.
- *Evaluation-based tier assignment* forces the enterprise to
  own the evaluation methodology. The enterprise cannot claim
  a system is at tier T without having evaluated to tier T.
  The head's operating parallel is the AIMS internal audit
  discipline ([[mod-102-running-the-program]] chapter 05) that
  produces the evaluation the tier assignment rests on.
- *Commitments per tier* means the enterprise can commit
  differently to different system classes without either
  under-committing across the whole portfolio (the failure
  mode of a single low commitment applied to everything) or
  over-committing across the whole portfolio (the failure
  mode of a single high commitment applied to everything).
  The head who has struggled with an all-or-nothing
  voluntary-code commitment recognises this as a resolution
  pattern.
- *Commitment to iterate* is what turns a one-time public
  statement into a durable policy the enterprise revises
  publicly. Chapter 03's annual public-trust plan is the
  operating parallel: the head's own external posture is
  planned, not left as a static statement.

## OpenAI Preparedness Framework — shape lessons

OpenAI published a Preparedness Framework in December 2023 and
has iterated it since.
<!-- needs-research: verify the current published version of
OpenAI's Preparedness Framework, the current risk-category
structure (biosecurity, cybersecurity, autonomy, and adjacent),
the current risk-level definitions (typically low / medium /
high / critical), the current pre-mitigation and post-
mitigation evaluation discipline, and the current governance
structure (Safety Advisory Group and Board-level oversight)
against openai.com/safety or the current canonical URL. -->

The load-bearing shape properties of the Preparedness Framework
as of the research window are the following.

- **Risk-category structure.** The framework organises risks
  into a small number of categories (biosecurity risk,
  cybersecurity risk, autonomy risk, and other model-driven
  risks), each with its own evaluation approach.
- **Risk-level scoring per category.** Each category is scored
  on a defined scale (low / medium / high / critical or
  equivalent), with the scoring driven by specific
  evaluations. Both pre-mitigation and post-mitigation scores
  are contemplated.
- **Threshold-based deployment gating.** Deployment and
  training-continuation decisions are gated on the post-
  mitigation score. Above defined thresholds, deployment or
  further training triggers specific commitments (additional
  mitigations, additional review, escalation to defined
  governance structures).
- **Defined governance structures.** The framework identifies
  specific internal governance structures — a Safety Advisory
  Group and Board-level oversight — with defined roles in the
  deployment-decision process.

The shape lessons the head extracts:

- *Risk-category structure* is a resolution move that keeps
  the enterprise from treating "AI risk" as a single
  undifferentiated construct. The head's own AI risk register
  ([[mod-102-running-the-program]] chapter 03) benefits from
  the same discipline: risks named by category, evaluated by
  category, and mitigated by category, rather than a monolithic
  risk score for each system.
- *Pre-mitigation and post-mitigation scoring* is what makes
  the enterprise's mitigation work visible. A system that
  scores high pre-mitigation and low post-mitigation
  demonstrates the mitigations are load-bearing; a system
  that scores low pre-mitigation and low post-mitigation
  demonstrates the risk is low intrinsically. The distinction
  matters for regulator conversations and for the enterprise's
  own understanding of where its mitigation investment goes.
- *Threshold-based deployment gating* is a variant of the
  enterprise's release-gate discipline
  ([[mod-102-running-the-program]] chapter 04's operating
  crosswalk and chapter 05's internal audit). The frontier-
  lab version is more explicit about the gate being *at the
  policy level*, not just in operational sign-off. The head
  who has struggled with release gates that are enforced
  inconsistently across teams recognises the value of
  raising the gate to policy-and-public-commitment level.
- *Defined governance structures* — a named advisory body and
  named board-level oversight — is the artefact the head
  most directly maps to the enterprise's own AI governance
  council and audit-committee cadence. The frontier-lab shape
  is a stronger version of the same structure, made public.

## Google DeepMind Frontier Safety Framework — shape lessons

Google DeepMind published a Frontier Safety Framework in May
2024 and has iterated it since.
<!-- needs-research: verify the current published version of
Google DeepMind's Frontier Safety Framework, the current
Critical Capability Level (CCL) structure, the current
evaluation methodology, the current mitigation and disclosure
commitments per CCL, and the current cross-organisational
governance structure (including any coordination with Google
and Alphabet governance) against deepmind.google or the
current canonical URL. -->

The load-bearing shape properties of the FSF as of the research
window are the following.

- **Critical Capability Level (CCL) framework.** The FSF
  identifies specific capability thresholds ("Critical
  Capability Levels") in defined risk categories
  (autonomy, biosecurity, cybersecurity, and adjacent), with
  each CCL characterised by specific capabilities the
  organisation commits to detecting and to responding to.
- **Evaluation cadence.** The FSF commits DeepMind to
  evaluate its most capable models against the CCLs on a
  defined cadence and at defined trigger points (before
  external deployment, at material capability jumps, and
  during training-run continuation decisions).
- **Response protocols per CCL.** For each CCL, the FSF
  specifies the response — additional mitigations, external
  disclosure, coordination with governments, pausing of
  further capability increase pending safety work.
- **Coordination with Google and Alphabet governance.** The
  FSF is a DeepMind artefact but is embedded in the broader
  Google and Alphabet governance structures; the artefact
  contemplates coordination with the parent organisation's
  own AI-governance and risk-management functions.

The shape lessons the head extracts:

- The *CCL framework* parallels Anthropic's ASL and OpenAI's
  category-and-level structure: the shared shape is a
  *pre-declared capability or risk boundary* the enterprise
  commits to detecting and to responding to. The enterprise's
  equivalent, at non-frontier scale, is a pre-declared
  operating-boundary framework — the risk-appetite statements
  from [[mod-103-board-and-audit-committee-reporting]] chapter
  03 turned into operating-boundary triggers with defined
  responses.
- The *cross-organisational coordination* is the shape
  lesson most directly applicable to enterprises embedded in
  larger corporate parents (subsidiaries, business units of
  diversified enterprises, spun-off AI functions). The head
  whose enterprise is a business unit of a larger corporate
  parent draws on the FSF shape for how the enterprise's own
  AI-governance framework coordinates with the parent's
  overall governance without either duplicating it or being
  invisible to it.
- The *response-protocol per level* discipline —
  "when we detect capability C, we do X, Y, and Z" — is
  operationally tighter than "we monitor and respond
  appropriately". The head who writes response protocols at
  the level of specificity the FSF uses forces the
  enterprise to have decided *before the trigger fires* what
  the response actually is.

## What the three artefacts collectively teach

Across the three artefacts, the common shape lessons the head
of AI governance at enterprise scale extracts are five.

- **A public policy is a durable artefact, not a statement.**
  The frontier labs treat their safety artefacts as
  policies — versioned, updated, published — not as public
  statements. The enterprise's equivalent public postures
  (voluntary-code sign-ons, position papers, public
  transparency reports) should be treated with the same
  discipline.
- **Tiering keeps commitments proportionate.** All three
  frameworks use some form of tiering (ASL, risk levels,
  CCLs) to keep commitments proportionate to what triggered
  them. The enterprise benefits from the same discipline —
  the AI Act's high-risk / limited-risk / minimal-risk
  classification, or the enterprise's own risk taxonomy, is
  a natural place to apply the pattern.
- **Evaluation-based triggers demand evaluation methodology.**
  A commitment that says "when we detect X we do Y" only
  works if the enterprise has an X-detection methodology.
  Frontier labs invest heavily in evaluation methodology
  because their commitments make them dependent on it. The
  enterprise's own commitments should be made dependent on
  evaluation the enterprise can actually run.
- **Board-level oversight makes the policy real.** All three
  frameworks bring a board-level structure into the
  commitment. The enterprise's audit-committee cadence
  ([[mod-103-board-and-audit-committee-reporting]]) is the
  parallel; the head who wants an external commitment to be
  operationally load-bearing routes the commitment through
  the committee.
- **Iteration in public is a strength, not a weakness.** The
  frontier labs revise their policies publicly and treat
  revision as evidence of learning, not as evidence of
  earlier failure. The enterprise's public postures benefit
  from the same posture: version, revise, and publish the
  revision as continued engagement with the substance.

## The enterprise-equivalent posture

The enterprise's own equivalent to the RSP / Preparedness
Framework / FSF is not yet a settled shape at non-frontier
scale as of the research window. The industry is early. A
handful of non-frontier enterprises publish AI transparency
reports, some publish AI governance overviews, some publish
policy positions on specific topics. None yet publishes a
single artefact with all four properties the frontier labs'
artefacts share.

The head's opportunity — and the head's obligation, at
sufficient enterprise scale — is to build toward that
enterprise-equivalent artefact deliberately. The building
blocks are already in the head's operating discipline: the
voluntary-code portfolio (chapter 01), the standards-body
participation record (chapter 02), the public-trust posture
(chapter 03), the RFI / RFP response discipline (chapter 04),
the audit-committee cadence
([[mod-103-board-and-audit-committee-reporting]]), and the
program-measurement KRI portfolio
([[mod-107-program-measurement-and-maturity]] chapter 01).

The composition of these into a single enterprise-equivalent
public artefact — a versioned, cadence-committed, operating-
disciplined, board-overseen public commitment framework — is
the head's forward-looking work. The exact form will vary by
enterprise (an AIMS-anchored transparency report, an AI-
governance policy pack on the enterprise's own AI-governance
channel, a set of commitments cross-referenced to voluntary
codes and standards, or some combination), but the properties
the artefact needs to have — the four load-bearing properties
the frontier labs demonstrate — are already clear.

The head who is aware of the shape the frontier labs have
built, and of the shape the enterprise's own equivalent will
need, is a head positioned to build the equivalent
deliberately rather than reactively. When a regulator or a
customer eventually asks "where is the enterprise's
equivalent to the frontier labs' safety frameworks", the
answer the head wants ready is a specific artefact the
enterprise has been building toward, not a scramble to
assemble one after the question lands.

## What the head does not confuse

Three category errors the head does not make:

- The frontier-lab artefacts are not templates. Direct
  transplantation of an ASL framework to a non-frontier
  enterprise's system portfolio produces a framework that
  does not fit the enterprise's actual capability shape and
  costs credibility. The shape is transferable; the specifics
  are not.
- Publishing an enterprise-equivalent artefact is not a
  marketing exercise. The artefact commits the enterprise to
  the operating discipline the artefact describes. The
  chapter-01 sign-on discipline applies at least as tightly
  to the enterprise's own public commitments as it does to
  a peer body's voluntary code.
- The frontier labs are not always right about their own
  framework choices. The frontier labs iterate their
  frameworks partly because earlier versions had elements
  that did not work at scale. The head reads the shape
  lessons as *shape*, not as endorsement of every specific
  choice the labs have made.

## Summary

- The frontier labs — Anthropic (RSP), OpenAI (Preparedness
  Framework), Google DeepMind (FSF) — have built distinctive
  external-positioning artefacts that share four durable
  properties: publicly published with named versions,
  committed to a specific update cadence, tied to specific
  internal operating disciplines, and board-overseen.
- The shape lessons transferable to non-frontier enterprise
  scale: a public policy is a durable artefact not a
  statement; tiering keeps commitments proportionate;
  evaluation-based triggers demand evaluation methodology;
  board-level oversight makes the policy real; and iteration
  in public is a strength.
- Anthropic's RSP contributes the shape lesson of a
  capability-tier framework tied to evaluation-based tier
  assignment and per-tier commitments.
- OpenAI's Preparedness Framework contributes the shape
  lesson of risk-category structure, pre-mitigation and
  post-mitigation scoring, threshold-based deployment
  gating, and defined governance structures.
- Google DeepMind's FSF contributes the shape lesson of
  Critical Capability Level thresholds tied to defined
  response protocols and cross-organisational governance
  coordination.
- Direct transplantation of frontier-lab framework specifics
  to non-frontier enterprises misfires; the shape is
  transferable, the specifics are not.
- The enterprise-equivalent artefact is emerging, not yet
  settled at non-frontier scale. The head's forward-looking
  work is to compose the building blocks — voluntary-code
  portfolio, standards-body participation, public-trust
  posture, RFI / RFP discipline, audit-committee cadence,
  program-measurement KRIs — into a single versioned,
  cadence-committed, operating-disciplined, board-overseen
  public commitment framework.
- The head who builds toward the enterprise-equivalent
  deliberately is positioned to answer the "where is your
  equivalent" question when regulators, customers, and
  investors eventually ask; the head who does not is
  positioned to scramble.
