# The AI-Observability Vendor P&L — Coordinated with the Level-35 Evaluator

## Motivation

The AI-observability category sits at the operational-monitoring
boundary between the AI runtime — production models, deployed
pipelines, LLM endpoints, agentic systems — and the governance
function's evidence store. The head of AI governance does not
own operational monitoring; the AI/ML platform team owns the
runtime, and the level-35 `ai-evaluation-engineer` owns the
tooling requirements and the operational discipline that turns
raw observability signal into the release-assurance and drift-
detection workflows the enterprise runs against. What the head
owns is the *budget line* and the *P&L* underneath the
observability stack, because the observability stack is what
feeds the KRI portfolio ([[mod-107-program-measurement-and-
maturity]] chapter 01) and the AIMS metric surface
([[mod-102-running-the-program]]) that the audit committee reads
as the enterprise's ambient-risk signal on production AI.

The head who abdicates observability spend to the ML platform
team is a head who has ceded control over the evidence surface
the audit committee scrutinises. When drift on a high-impact
production model goes undetected because the observability
platform was scoped for developer ergonomics rather than for
audit-committee-facing signal, the head owns the failure. When
the vendor contract renews at a materially higher rate because
the per-prediction pricing curve was never modelled against
production growth, the head owns the invoice surprise. When the
KRI feed to the audit committee is fragile because the
observability stack is an open-source library with no supported
enterprise tier, the head owns the resulting audit-committee
moment.

This chapter is how the head runs the observability vendor P&L
without stepping on the level-35 evaluator's operational
authority. The chapter is smaller in scope than the GRC-for-AI
P&L in chapter [03 — The GRC-for-AI Vendor P&L at CxO Scope](03-grc-for-ai-vendor-pnl.md)
— fewer named vendors, typically smaller contract envelopes, a
more sharply defined technical coordination surface — but the
discipline is the same shape: the head owns the commercial and
audit-committee-facing case; the level-35 practitioner owns the
technical requirements; the two compose.

## The observability category map

The head does not need to be a monitoring-tool expert. The head
does need enough ambient literacy on the category to run the
commercial case, negotiate renewals, and defend the vendor line
at CFO scope. The level-35 evaluator carries the deep technical
read.

### The named AI-observability vendors

**Fiddler AI.** Enterprise ML observability, monitoring, and
explainability platform positioned toward the production-AI
observability surface for classical ML and, increasingly, for
LLM/GenAI applications.
<!-- needs-research: verify Fiddler's current product scope, LLM/GenAI-observability feature set, and enterprise-tier positioning against the vendor's own public materials at the time of authoring the P&L. -->

**Arthur AI.** Model observability and monitoring, historically
anchored in classical-ML performance and fairness monitoring
and expanding into LLM/GenAI observability with a distinct
LLM-focused product surface.
<!-- needs-research: verify Arthur AI's current product portfolio boundary between classical-ML monitoring and its LLM/GenAI-monitoring offering; check current positioning statement and pricing metric. -->

**WhyLabs.** Data-and-ML observability with a strong open-source
heritage — the WhyLogs open-source library — and a managed
platform tier for enterprise deployments.
<!-- needs-research: verify WhyLabs' current OSS-vs-managed-tier boundary, the specific capabilities gated to the managed platform, and the pricing metric for the managed tier. -->

**Evidently.** Open-source-first ML and LLM evaluation and
monitoring, with an enterprise tier that layers managed
capabilities on top of the open-source library.
<!-- needs-research: verify Evidently's current OSS-vs-enterprise-tier boundary and the specific enterprise-only features relevant to KRI-feeding use cases. -->

The head reads these four as the named category. The vendor set
is not exhaustive — the category is fluid, entrants and
adjacent-category players regularly move into observability
scope — and the head reserves the right to add a named entrant
after a substantive briefing.

### Adjacent categories the head watches

The observability category does not sit in isolation. Three
adjacent categories overlap enough that the head cannot make a
consolidation decision without reading them.

**Hyperscaler-native observability.** Amazon SageMaker Model
Monitor, Azure Machine Learning monitoring, Google Vertex AI
monitoring. Enterprises deep in one hyperscaler often have
first-party monitoring available at incremental cost against
the hyperscaler contract; the head reads this as a genuine
option, not as a substitute-for-the-specialist decision made
implicitly.
<!-- needs-research: verify current feature scope of Amazon SageMaker Model Monitor, Azure ML monitoring, and Google Vertex AI monitoring; confirm feature-parity gaps and any LLM-observability positioning inside the hyperscaler-native offerings. -->

**MLOps-platform-native monitoring.** Databricks Lakehouse
Monitoring, Weights & Biases, Neptune, Comet, MLflow enterprise
distributions. Where the enterprise has already selected an
MLOps platform, that platform typically ships a monitoring
surface — sometimes competitive with the specialist vendors,
sometimes materially thinner; the head reads the specific
platform's current scope before assuming coverage.
<!-- needs-research: verify current monitoring capabilities inside Databricks, Weights & Biases, Neptune, Comet, and MLflow enterprise distributions; note any gaps against typical enterprise KRI-feeding requirements. -->

**The LLM-evaluation overlay.** Arize AI, LangSmith, Braintrust,
HumanLoop, Confident-AI, Patronus AI, and adjacent. These
vendors sit at the intersection of observability and evaluation
for LLM/GenAI applications; some overlap the pure observability
scope, some sit distinctly at the evaluation-harness scope. The
head does not treat the LLM-eval overlay as a full substitute
for classical-ML observability, and does not treat classical-ML
observability as a full substitute for the LLM-eval overlay.
<!-- needs-research: verify current product boundaries between Arize, LangSmith, Braintrust, HumanLoop, Confident-AI, and Patronus; check whether each positions as observability, evaluation, or both, and note which surface the level-35 evaluator would treat as load-bearing. -->

The head reads these three adjacencies because the
consolidation-or-expansion decision later in this chapter turns
on them. A head who treats the specialist observability vendors
as the only option pays for coverage the enterprise may already
have; a head who assumes the hyperscaler-native or MLOps-
platform-native monitoring is sufficient pays with an audit-
committee moment when the KRI feed breaks.

## Coordination with the level-35 evaluator

The load-bearing distinctive of this chapter — the thing that
separates the observability P&L from the GRC-for-AI P&L in
chapter [03 — The GRC-for-AI Vendor P&L at CxO Scope](03-grc-for-ai-vendor-pnl.md)
— is the coordination discipline the head runs with the level-
35 `ai-evaluation-engineer`. The GRC-for-AI platform is chosen
largely on head-of-function requirements; the observability
platform is chosen largely on level-35-evaluator requirements
with the head owning the commercial and audit-committee-facing
frame around them.

### The scope split

The head and the level-35 evaluator each own a distinct scope,
and the scope split is explicit rather than negotiated case by
case.

- **The head owns the P&L.** Contract-envelope shape, multi-year
  cost trajectory, renewal negotiation posture, escalation
  authority to the CFO and CIO, consolidation-or-expansion
  decision, board-facing defence of the observability line, and
  continuity planning against vendor lock-in.
- **The level-35 evaluator owns the tooling requirements.** The
  metric coverage the platform has to produce (data drift,
  prediction drift, concept drift, fairness-metric surface,
  calibration monitoring, output-quality metrics for LLMs,
  hallucination-and-groundedness signal, prompt-injection
  detection where relevant, evaluation-harness integration
  surface, alerting shape, on-call-integration surface), the
  vendor selection short-list from a technical fit standpoint,
  and the operational read on whether the platform is
  performing against those requirements.

The scope split works because the two questions the head and the
evaluator answer are distinct. The head answers "is this the
right commercial deal for the enterprise across the term, and
is this the right vendor for the audit-committee-facing evidence
surface?" The evaluator answers "does this platform produce the
signal our production-AI portfolio needs, and does it integrate
with the evaluation harness and the on-call rotation cleanly?"
Confusing the two questions produces both worse commercial
outcomes and worse operational outcomes.

### The consolidation the head runs

The evaluator's technical requirements are authored in the
evaluator's own artefact — typically a functional-and-non-
functional requirements document with metric coverage, latency
targets, retention targets, integration-surface targets, and
alerting-shape targets. The head does not re-author these. What
the head does is *consolidate* the requirements into a vendor-
selection or renewal case that reads at CFO scope.

The consolidation shape:

- **The functional envelope.** A one-page summary of what the
  observability platform must produce, sourced from the
  evaluator's requirements document but authored in language
  the CFO and the CIO can read. Not "P95 latency on drift-metric
  compute under X ms" — instead, "the platform produces the
  drift signal fast enough that the enterprise's on-call
  rotation can act within the enterprise's incident-response
  SLA."
- **The commercial envelope.** The total cost of ownership over
  the contract term — licence, data-egress, storage, integration
  labour, professional services, plus the ambient cost of the
  team members who operate the platform. Authored at the same
  fidelity as the GRC-for-AI TCO in chapter [03](03-grc-for-ai-vendor-pnl.md).
- **The audit-committee frame.** A short read on why the chosen
  platform is defensible as the source of the KRI feed the audit
  committee reads — the platform's own certifications where
  they apply, the platform's SLA commitments, the platform's
  incident-history posture, and the enterprise's continuity
  plan against the platform.

The consolidation is what the head presents at the vendor-
selection meeting, the renewal meeting, and — if the case
warrants it — the audit-committee update. The evaluator's
technical requirements sit underneath as the load-bearing
detail; the consolidation is the head's authoring on top.

### The vendor-satisfaction pulse the two co-run

The vendor-satisfaction pulse for the observability vendor —
analogous to the pulse chapter [[mod-108-leading-the-governance-
function]] chapter 06 describes for the GRC-for-AI vendor —
runs at quarterly cadence, and the head and the evaluator co-
run it. The split is explicit.

- **The evaluator surfaces operational friction.** Are drift
  metrics computing correctly against the production model
  behaviour? Is the alerting shape producing actionable signal
  or noise? Is the integration surface with the enterprise's
  MLOps platform stable? Are new-model onboarding workflows
  reasonable? Are LLM-observability capabilities keeping pace
  with the enterprise's GenAI portfolio growth? Is the vendor's
  product roadmap addressing the gaps the enterprise has
  flagged? The evaluator does not soften the read to be
  diplomatic.
- **The head surfaces P&L friction.** Is the invoice tracking
  the model? Are per-prediction charges growing on the pricing
  curve the head expected, or is there a materially different
  usage-growth pattern? Are storage costs on the retention
  policy the head signed, or has retention drifted upward
  ambiently? Are professional-services engagements landing
  inside the envelope or over? Are contract terms — SLA credits,
  renewal caps, data-portability commitments — being honoured?

The two reads feed a single consolidated pulse the head takes
to the quarterly vendor account review. The evaluator is
present in the account review; the head runs it. The vendor
sees both the operational read and the commercial read in one
meeting rather than in two disjointed channels.

### The escalation authority

The escalation authority sits with the head, not with the
evaluator. This is explicit.

- **The evaluator does not open CFO-scope escalations.** If the
  vendor is materially underperforming — repeated outages during
  audit-committee cycles, roadmap items slipping past the
  commitments the enterprise contracted against, support
  responsiveness degrading below SLA — the evaluator surfaces
  the pattern to the head, and the head opens the escalation
  through the ladder described later in this chapter. The
  evaluator does not go around the head to the CFO; the head
  does not permit that shape.
- **The head does not open technical-support tickets.** When
  the platform's metric computation is producing an anomalous
  signal, when an integration endpoint has broken, when a model
  onboarding is stalling on a product-configuration issue, the
  head does not open the ticket. The evaluator opens the
  ticket, works the vendor's technical support, and — if the
  ticket goes unresolved at severity — escalates to the head.

Clear scope keeps both sides functional. The evaluator who runs
CFO-scope escalations degrades the head's standing (see the
anti-pattern later in this chapter). The head who opens
technical support tickets degrades the head's own operating
tempo and blurs a scope the vendor's account team then reads
as ambiguous.

## What the observability P&L covers

The head's authoring for the observability vendor P&L covers a
specific set of cost categories. Each category has its own
dynamics; the head reads each distinctly rather than under a
generic "licence spend" umbrella.

### Base licence — the pricing-metric question

Observability vendors do not price on a single common metric.
The pricing metric matters because the enterprise's usage shape
determines which metric produces the cheaper deal and which
metric produces the surprise invoice.

- **Per-model licensing** — predictable if the enterprise's
  model portfolio grows slowly; punishing if the enterprise
  runs many small models against a portfolio-sprawl pattern.
- **Per-prediction (or per-inference) licensing** — efficient
  for low-volume, high-value inference; punishing for high-
  volume, low-margin inference workloads. The head models the
  growth curve of production inference before signing this
  pricing metric.
- **Per-data-volume licensing** — the vendor charges by the
  volume of features, prediction logs, or events ingested.
  Common for data-and-ML observability tiers; the head models
  data-ingestion growth against the retention policy.
- **Per-seat or per-user licensing** — less common in pure
  observability, more common at the LLM-eval overlay boundary.

The head reads each candidate vendor's specific pricing metric,
models it against the enterprise's production-AI trajectory
over the contract term, and produces a defensible three-year
cost envelope. A head who signs on year-one pricing without
modelling year-three usage growth is a head who owns the year-
three renewal surprise.

### Data-egress and data-plane costs

Most named observability vendors run as SaaS. Enterprise
prediction logs, feature values, and evaluation artefacts leave
the enterprise network and land in the vendor's platform. The
head models the data-plane cost — either the vendor's own
data-plane charges where they apply, or the enterprise's own
egress costs from the enterprise's cloud footprint to the
vendor's platform. Some vendors offer private-deployment or
in-VPC deployment options that materially change the data-plane
economics; the private-deployment tier is typically more
expensive at licence level and cheaper at data-plane level, and
the arithmetic against the enterprise's specific volume and
data-residency posture matters.

### Storage costs — the retention question

Observability platforms store historical prediction logs,
evaluation-run archives, drift-computation results, and — for
LLM applications — prompt/response traces. Storage grows with
retention policy, and retention policy is not a free choice —
it is set by the enterprise's evidence-retention obligations
under regulation, by internal audit's lookback requirements,
and by the audit committee's tolerance for gaps in the evidence
surface. The head reads the retention policy, models storage
growth against production-AI growth, and does not let retention
drift upward without an explicit decision. Retention that
starts at ninety days and drifts to two years across three
contract cycles because "nobody decided to prune" is a storage
line the head has effectively authored by not authoring.

### Integration labour and professional services

The observability platform integrates with the enterprise's
model-serving infrastructure, feature store, MLOps platform,
evaluation harness, and — increasingly — the enterprise's GenAI
gateway. Integration is not free; the head models the labour —
engineering time from the ML platform team, the level-35
evaluator's time on integration validation, and the vendor's
own professional-services envelope where the enterprise chooses
vendor-led integration. Integration labour is typically front-
loaded in year one and tapers, but a vendor that ships breaking
API changes at each major release re-imposes it each time; the
head reads the vendor's release discipline as part of the P&L.

The professional-services envelope for advanced use cases —
bespoke fairness metrics, custom drift-detection logic, sector-
specific regulatory reporting shapes, LLM-eval workflows tuned
to the enterprise's harness pattern — is a distinct line item
with its own scoping discipline. Professional services that
expand ambiently without a change order signed against them are
costs the head has effectively agreed by not disagreeing.

### Open-source-plus-enterprise-support arithmetic

Evidently and WhyLabs specifically — and, at the LLM-eval
overlay boundary, several other vendors — have significant
open-source library heritage. The enterprise can, in principle,
run the open-source library without the enterprise tier. The
head does not treat this as free, and has an explicit decision
on the boundary rather than letting the ML platform team decide
implicitly by pulling the OSS library. Three postures:

- **OSS-only.** Zero licence. The ML platform team maintains
  the library integration, tracks upstream releases, and
  absorbs the ambient risk that upstream community support may
  shift or that enterprise-grade features (SSO, RBAC, audit
  logging, enterprise-scoped SLAs) are absent.
- **OSS-plus-enterprise-tier.** The enterprise runs the OSS
  library and pays for the vendor's enterprise tier for the
  managed platform, enterprise-grade features, and SLA-backed
  support.
- **Enterprise-tier-only.** The enterprise runs the vendor's
  platform without engaging the OSS library.

Where the observability platform feeds the KRI surface the
audit committee reads, the head takes an explicit position on
whether the OSS-only posture is defensible for that specific
feed, or whether the audit-committee-facing surface warrants
the enterprise-tier support.

## Renewal-and-escalation discipline

The observability vendor renewal follows the same shape as
the GRC-for-AI renewal in chapter [03](03-grc-for-ai-vendor-pnl.md),
scaled to the smaller category. Fewer vendors, typically smaller
contract envelopes, but the same shape.

### Renewal preparation

The head begins renewal preparation six months before the
contract-end date, not one month before. Renewal preparation:

- **Refresh the P&L across the term.** The head, working with
  the enterprise's finance business partner, refreshes the
  actual cost across the current term against the modelled
  cost, and identifies the deltas — where the invoice ran
  higher than modelled, where lower, and why.
- **Refresh the evaluator's technical read.** The level-35
  evaluator refreshes the fitness-for-purpose read — is the
  platform still delivering against the requirements, what has
  slipped, what has improved, what new requirements have
  emerged that the platform does or does not address.
- **Refresh the alternative-vendor awareness.** The head takes
  at least one substantive briefing from a credible alternative
  vendor and, where the LLM-eval overlay is materially relevant,
  from at least one adjacent-category vendor. Not to threaten
  the incumbent — to have a genuine read on what the
  alternatives now look like.
- **Refresh the consolidation-or-expansion posture.** The head
  reads whether the enterprise is on the right side of the
  consolidation-or-expansion decision (see below) or whether
  the renewal is the moment to change posture.

### The escalation ladder

When the observability vendor is materially underperforming —
repeated missed SLA on platform availability, metric-computation
errors that produce false-positive or false-negative KRI signal,
professional-services engagements running materially over,
roadmap items the enterprise depended on slipping past their
commitments — the head escalates through a defined ladder. Same
shape as the GRC-for-AI ladder, at smaller scale.

- **First escalation: the account executive.** The head, at the
  next quarterly account review, names the escalation
  explicitly and requests a specific remediation with a
  specific date. The evaluator is present to substantiate the
  technical detail.
- **Second escalation: the vendor's CxO sponsor.** If the first
  escalation does not produce a substantive response in the
  agreed window, the head raises directly with the vendor's
  executive sponsor. The head names the pattern rather than the
  incident, and asks for CxO-scope engagement.
- **Third escalation: the enterprise's CFO and CIO.** If the
  second escalation does not produce substantive change, the
  head engages internally — a material-underperformance case
  that either invokes contract remedies (SLA credits, contract
  restructuring, early termination clauses where they apply) or
  begins the replacement-vendor evaluation.
- **Fourth escalation: replacement.** The nuclear option.
  Exercised rarely — the observability category has real
  switching cost from a data-history perspective, and the head
  does not open replacement lightly. When exercised, the
  replacement is authored as a formal project with the level-
  35 evaluator running the technical migration and the head
  running the commercial and audit-committee-facing frame.

### The switching-cost read

The head reads switching cost honestly. The observability
platform holds historical prediction logs, drift-computation
history, and evaluation-run archives that are load-bearing for
trending analysis, for regulator-facing evidence, and for the
KRI portfolio's own trend signal. A migration mid-cycle loses
the trend continuity unless the head has authored the data-
portability discipline into the contract.

The head does not open replacement without a data-portability
plan. Where the incumbent vendor's contract does not guarantee
portable export in a documented format, the head raises the
portability gap explicitly at the next renewal — either the
vendor commits to portability, or the head begins the
alternate-vendor evaluation at that renewal cycle rather than
mid-term.

## Consolidation-or-expansion decision

The head runs the consolidation-or-expansion decision on the
observability portfolio at least annually, and materially at
each renewal. Three postures.

**Consolidate on a single observability vendor.** One vendor
across classical-ML and LLM/GenAI observability. Advantages:
simpler operational surface, easier evidence-store integration,
one vendor account to run at CxO scope, one KRI-feed path to
defend at audit-committee scope. Disadvantages: higher single-
vendor risk (the vendor's outage becomes the enterprise's KRI-
feed outage), potentially thinner feature coverage where the
vendor is stronger in one sub-category than another, and weaker
commercial leverage at renewal. The head reads consolidation as
the default posture for enterprises whose production-AI
portfolio is dominated by one model shape and where the chosen
vendor has substantive coverage of that shape.

**Best-of-breed across sub-categories.** One vendor for
classical-ML observability, one for LLM-eval overlay, and —
where the head has chosen it — one for OSS-plus-enterprise-tier
foundations. Advantages: best coverage in each sub-category, no
single-vendor risk on the KRI feed. Disadvantages: more complex
operational surface, more integration labour, more contracts to
run, and the level-35 evaluator's operational discipline is
materially load-bearing — a best-of-breed posture the evaluator
cannot operate collapses into a de facto consolidation on
whichever vendor the team can operate. The head does not adopt
best-of-breed on a "diversify vendor risk" argument alone — the
operational cost is real.

**Hyperscaler-native plus specialty overlay.** The enterprise
runs hyperscaler-native monitoring for classical-ML — SageMaker
Model Monitor if AWS-heavy, Azure ML monitoring if Azure-heavy,
Vertex AI monitoring if GCP-heavy — and layers a specialty
vendor for LLM-eval or for the audit-committee-facing KRI feed.
The hyperscaler-native monitoring runs against the existing
hyperscaler contract with limited incremental spend and no
separate data-egress; the specialty overlay covers the sub-
category where the hyperscaler-native option is materially
thin. Trade-off: two tools to operate, two evidence surfaces to
reconcile, and feature-parity gaps against the specialty vendors
in areas the head has to read explicitly.
<!-- needs-research: verify the current feature-parity gap between hyperscaler-native monitoring (SageMaker Model Monitor, Azure ML monitoring, Vertex AI monitoring) and the specialty observability vendors on the specific dimensions typical enterprise KRI feeds depend on. -->
The head reads this posture as the commercially-driven option
for enterprises deep in one hyperscaler with a large classical-
ML portfolio, and revisits it at each renewal — the
hyperscaler-native scope moves quickly, and the arithmetic
against the specialty vendors shifts each cycle.

The consolidation-or-expansion decision is not authored once
and left. It is authored at renewal, revisited when the
enterprise's production-AI portfolio shifts materially, and
tested against the enterprise's audit-committee-facing signal
requirements.

## Anti-patterns the head does not permit

**The "observability is an ML platform team decision"
abdication.** The head has never opened the observability P&L
in a substantive way. The ML platform team selected the
observability vendor on developer-ergonomics grounds — the tool
the platform team's engineers preferred to work with — and the
head inherited a KRI-feed surface that the audit committee
reads. When the vendor has a material outage during the audit-
committee cycle, or when the vendor's roadmap misses a
requirement the KRI feed depends on, the head owns the failure
without ever having owned the selection. The remedy is the
scope split described earlier — the head owns the P&L and the
audit-committee frame, the level-35 evaluator owns the tooling
requirements, both are present in the vendor selection.

**The double-monitoring pattern.** The enterprise runs
hyperscaler-native monitoring on the classical-ML portfolio and
a specialty observability vendor with materially overlapping
scope. Nobody has taken the consolidation decision — the
hyperscaler-native tool was set up by the ML platform team
before the specialty vendor was procured, and neither was
retired when the other was adopted. The enterprise pays for
overlapping coverage; the evidence surface is fragmented across
two tools; the KRI feed to the audit committee is stitched
together operationally rather than authored cleanly. The remedy
is the consolidation-or-expansion decision the head runs at
each renewal and revisits when the portfolio shifts.

**The under-scoped SaaS-egress pattern.** The head signed the
observability contract at year-one prediction volumes without
modelling the data-egress cost curve against year-two and
year-three production growth. Year-two invoices arrive
materially over the modelled envelope; year-three invoices are
worse. The head negotiates a mid-term amendment from a weak
position — the vendor holds the incumbency, the switching cost
is high, and the head is in front of the CFO explaining a
budget line that has slipped. The remedy is the data-plane
modelling discipline described earlier — the head models the
pricing metric against the multi-year growth curve, not against
the year-one baseline.

**The OSS-and-enterprise-tier confusion.** The enterprise is
using Evidently or WhyLabs open-source library without a
supported enterprise tier, and the audit committee is reading a
KRI feed produced by that library. When the OSS community
support pattern shifts — an upstream maintainer transition, a
release-cadence slowdown, a specific bug in a metric-
computation path — the enterprise has no vendor support to call.
The gap becomes an audit-committee moment: the head is asked
"who supports the platform producing this signal?" and the
answer is "the open-source community, on best effort." The
remedy is the explicit OSS-vs-enterprise-tier decision the head
takes for each KRI-feeding surface — OSS is defensible for
non-audit-committee-facing use, but the audit-committee-facing
KRI feed typically warrants the supported enterprise tier.

**The evaluator-does-CFO-escalation pattern.** The level-35
evaluator has been escalating vendor pain — outages, missed SLA,
support-responsiveness degradation — to the CFO or the CIO
without the head's involvement. The CFO reads the escalation
as function-immaturity ("why is a level-35 engineer bringing
this to me instead of the head?") and the head loses standing.
The vendor, watching the shape, reads the enterprise's
escalation discipline as unstructured and calibrates
accordingly. The remedy is the explicit escalation-authority
split described earlier — the evaluator escalates to the head,
the head escalates to the CxO layer, and the shape is stated
plainly at the beginning of each vendor engagement so nobody is
confused.

## Composition with adjacent modules

- **The budget line** in chapter [01 — Owning the AI-Governance
  Function Budget Line](01-governance-function-budget-line.md)
  is where the observability vendor spend sits as a line item;
  the P&L discipline in this chapter is the substantive content
  underneath that line.
- **The GRC-for-AI vendor P&L** in chapter [03](03-grc-for-ai-vendor-pnl.md)
  is the parent shape this chapter mirrors at smaller scope; the
  evidence-store integration between the GRC-for-AI platform
  and the observability platform is what makes the KRI feed
  work.
- **The AI-runtime security vendor P&L** in chapter [05 — The
  AI-Runtime Security Vendor P&L](05-ai-runtime-security-vendor-pnl.md)
  overlaps with observability on prompt-injection detection and
  on LLM-eval overlay boundary; the head runs the two P&Ls
  distinctly but reads the overlap explicitly at each renewal.
- **The AIMS metric surface** in
  [[mod-102-running-the-program]] and the KRI/KPI portfolio in
  [[mod-107-program-measurement-and-maturity]] chapter 01 are
  what the observability stack feeds; the head's ownership of
  the observability P&L is what keeps that feed defensible.
- **The level-35 evaluator relationship discipline** in
  [[mod-108-leading-the-governance-function]] chapter 03 (the
  coaching-and-career-pathing cadence) and the function-shape
  discipline in that module's chapter 01 are where the
  evaluator's role is authored; this chapter's coordination
  shape composes with that authoring.
- **The incident-leadership discipline** in
  [[mod-110-incident-leadership]] runs against the observability
  stack because observability alerts are frequently the
  incident-first-signal; a fragile observability stack produces
  a fragile incident-detection surface.
- **The audit-committee reporting posture** in
  [[mod-103-board-and-audit-committee-reporting]] is where the
  KRI feed the observability stack produces is read; the head's
  substantive ownership of the observability vendor line is
  what makes that reporting defensible under audit-committee
  scrutiny.

## Summary

- The AI-observability category sits at the operational-
  monitoring boundary between the AI runtime and the governance
  function's evidence store. The head does not own operational
  monitoring; the head owns the P&L and the audit-committee
  frame around the observability stack because the stack feeds
  the KRI portfolio and the AIMS metric surface.
- The named vendors are Fiddler AI, Arthur AI, WhyLabs, and
  Evidently, with three adjacent categories the head reads:
  hyperscaler-native observability (SageMaker Model Monitor,
  Azure ML monitoring, Vertex AI monitoring), MLOps-platform-
  native monitoring (Databricks, Weights & Biases, Neptune,
  Comet, MLflow enterprise), and the LLM-eval overlay (Arize,
  LangSmith, Braintrust, HumanLoop, Confident-AI, Patronus).
- The load-bearing coordination is with the level-35 `ai-
  evaluation-engineer`. The head owns the P&L; the evaluator
  owns the tooling requirements. The head consolidates the
  requirements into a CFO-scope selection or renewal case. The
  two co-run the vendor-satisfaction pulse — the evaluator on
  operational friction, the head on P&L friction — and take one
  consolidated read to the vendor. The head reserves escalation
  authority to CFO scope; the evaluator does not open technical-
  support tickets in the head's name; the scope split is
  explicit.
- The observability P&L covers base licence (per-model, per-
  prediction, per-data-volume, or per-seat depending on
  vendor), data-egress and data-plane cost, storage cost tied
  to retention policy, integration labour, professional-
  services envelope, and — for OSS-heritage vendors — the
  explicit OSS-versus-enterprise-tier decision.
- Renewal and escalation follow the same four-step ladder as
  the GRC-for-AI category at smaller scale. Switching cost is
  real; the head does not open replacement without a data-
  portability plan.
- The consolidation-or-expansion decision has three postures:
  consolidate on a single vendor, best-of-breed across sub-
  categories, or hyperscaler-native plus specialty overlay.
  The head authors the decision at each renewal.
- Five anti-patterns the head refuses: the "observability is an
  ML platform team decision" abdication, the double-monitoring
  pattern, the under-scoped SaaS-egress pattern, the OSS-and-
  enterprise-tier confusion, and the evaluator-does-CFO-
  escalation pattern.
- Chapter [05 — The AI-Runtime Security Vendor P&L](05-ai-runtime-security-vendor-pnl.md)
  runs the parallel discipline for the runtime-security vendor
  category, with a distinct level-35 counterpart (`ai-infra-
  security`) and a distinct overlap with the observability
  category on prompt-injection and LLM-eval boundary; the two
  chapters compose.
