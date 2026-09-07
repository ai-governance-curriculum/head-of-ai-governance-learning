# exercise-04: Observability + Runtime-Security Vendor P&L Drill

**Estimated effort:** 2 hours

## Objective

Author the **paired vendor P&L** for the AI-observability and
AI-runtime-security stacks — the two categories where the head
runs the commercial case in coordinated authorship with a
level-35 partner rather than on head-of-function authority alone.
The observability P&L is co-authored with the level-35
`ai-evaluation-engineer`; the runtime-security P&L is co-authored
with the level-35 `ai-infra-security` engineer *and* overlaid
with the CISO joint operating agreement. The deliverable is the
pair the head takes into the CFO cycle and the pair the head
takes into the joint quarterly reviews with the two level-35
partners.

The pair has to survive three stress tests. First, the CFO
asks why the observability line and the runtime-security line
sit on separate P&Ls rather than one — the co-authorship shape
and the distinct level-35 counterparts have to answer the
question in one sentence each, not in a rambling defence of the
category split. Second, the level-35 evaluator asks why the
observability requirements pack is authored inside the head's
P&L artefact rather than in the evaluator's own artefact — the
answer is the consolidation shape from chapter [04](../04-ai-observability-vendor-pnl.md):
the evaluator's requirements sit underneath as the load-bearing
detail, the head consolidates on top, and the evaluator co-signs
the consolidated pack. Third, the CISO asks why the runtime-
security portfolio is not simply carried inside the enterprise
security P&L — the joint operating agreement has to name the
scope split, the cost-allocation formula, and the escalation
channel explicitly.

The pair is the head's authoring instrument in the two vendor
account reviews the head runs (observability quarterly with the
evaluator; runtime-security quarterly with the level-35 security
engineer and — at CxO cadence — with the CISO), the pair is the
substantive content underneath two line items in the year-one
budget from exercise 01, and the pair is what the audit committee
reads (through the KRI feed the observability stack produces and
the security-posture reporting the runtime-security stack feeds)
without ever seeing the P&L directly.

## Prerequisites

- Chapter [04-ai-observability-vendor-pnl](../04-ai-observability-vendor-pnl.md)
  — the named vendors (Fiddler AI, Arthur AI, WhyLabs,
  Evidently), the three adjacent categories (hyperscaler-native,
  MLOps-platform-native, LLM-eval overlay), the coordination
  discipline with the level-35 `ai-evaluation-engineer`, the P&L
  cost categories, the renewal-and-escalation ladder, the
  consolidation-or-expansion postures, and the five anti-patterns
  — read and internalised.
- Chapter [05-ai-runtime-security-vendor-pnl](../05-ai-runtime-security-vendor-pnl.md)
  — the named vendors (Robust Intelligence, Lakera Guard,
  Calypso AI, HiddenLayer, Protect AI, HydroX AI, Cranium,
  TrojAI), the four adjacent categories (red-team-as-a-service
  specialists, ML-BOM tooling, prompt-injection benchmark
  projects, CISO-adjacent traditional security stack expanding
  into AI), the coordination discipline with the level-35
  `ai-infra-security` engineer and with the CISO, the P&L
  composite, the acquisition-clause discipline, and the six
  anti-patterns — read and internalised.
- Chapter [01-governance-function-budget-line](../01-governance-function-budget-line.md)
  because the observability line and the runtime-security line
  both sit on the budget authored there; this exercise produces
  the substantive content underneath those lines.
- [[mod-107-program-measurement-and-maturity]] because the
  observability stack is what feeds the KRI portfolio, and the
  runtime-security stack feeds the security-posture KRIs; the
  P&L defence at audit-committee scope leans on the KRI feed.
- [[mod-109-cross-enterprise-leadership]] because the CISO peer
  coordination substrate is where the CISO joint operating
  agreement in this exercise lives; the exercise composes with
  that substrate rather than replacing it.
- [[mod-108-leading-the-governance-function]] because the
  level-35 evaluator and the level-35 security engineer are
  positions in the ladder authored there; this exercise assumes
  the two positions exist and that the head has running
  coordination cadences with each incumbent.
- [[mod-110-incident-leadership]] because the runtime-security
  P&L carries the red-team-as-a-service retainer that the
  incident-preparedness case is defended on; the retainer
  decision cannot be authored without the incident-leadership
  discipline as a reference.
- The exercise-01 artefacts (year-one budget and the two vendor
  lines specifically) and the enterprise context one-pager the
  head runs against.

## Steps

1. **Inherit the enterprise context.** Confirm the context one-
   pager is current and reference it. The enterprise's sector,
   AI portfolio scope, hyperscaler footprint, existing CISO
   stack, and jurisdictional overlay all drive the specific
   vendor decisions this exercise produces. In particular note
   the incumbent observability vendor (if any), the incumbent
   runtime-security tooling (if any), and the CISO's current
   position on AI-specific coverage inside the enterprise
   security stack.

2. **Author the observability requirements pack — co-authored
   with the level-35 evaluator.** Open the requirements
   authorship jointly with the level-35 `ai-evaluation-engineer`.
   The pack is the evaluator's artefact in substance; the head
   consolidates it into CFO-legible language on top. Contents
   per chapter [04](../04-ai-observability-vendor-pnl.md):
   - Functional envelope — the metric coverage the platform has
     to produce (data drift, prediction drift, concept drift,
     fairness-metric surface, calibration monitoring, LLM
     output-quality metrics, hallucination-and-groundedness
     signal, prompt-injection detection where relevant), the
     evaluation-harness integration surface, the alerting shape,
     and the on-call-integration surface.
   - Non-functional envelope — retention targets, latency
     targets, throughput targets, deployment-shape constraints
     (SaaS, private-deployment, in-VPC), and data-residency
     constraints.
   - Audit-committee frame — the KRI feed the platform has to
     produce reliably, the SLA position the platform has to
     hold, the certifications the platform has to carry.
   The level-35 evaluator signs the pack; the head signs the
   consolidation. A requirements pack the evaluator has not
   signed fails the co-authorship discipline and is not a
   requirements pack the head can defend at CFO scope.

3. **Author the observability P&L per incumbent or shortlist
   vendor.** For each vendor on the incumbent-and-shortlist list
   (at minimum the named-category vendors Fiddler AI, Arthur AI,
   WhyLabs, Evidently, plus any relevant hyperscaler-native and
   LLM-eval-overlay adjacencies), author a P&L that carries:
   - Base licence with the specific pricing metric (per-model,
     per-prediction, per-data-volume, per-seat) and the modelled
     multi-year cost curve against the enterprise's production-AI
     trajectory.
   - Data-egress and data-plane cost.
   - Storage cost against the retention policy the audit
     committee's evidence-lookback requirement drives.
   - Integration-labour envelope (ML platform team time,
     evaluator time, vendor professional services where
     applicable).
   - Professional-services envelope with a scoping-discipline
     note.
   - Where the vendor has OSS heritage (Evidently, WhyLabs, and
     LLM-eval-overlay vendors where applicable), the explicit
     OSS-vs-enterprise-tier decision for the specific KRI-feeding
     use case.
   - SLA position (platform availability, support-response
     tiers) as claimed against the vendor's own public materials.
     Do not invent numbers; where the SLA figure is not verified,
     mark it `<!-- needs-research: verify SLA position against
     the vendor's current contract templates -->`.
   - Renewal disposition — retain, renegotiate, replace, or
     hold-open-until-consolidation-decision.
   - Coverage-versus-requirements gap — what the vendor covers
     against the requirements pack from step 2 and what the
     vendor does not.

4. **Author the observability escalation ladder.** Instantiate
   the four-stage ladder from chapter [04](../04-ai-observability-vendor-pnl.md)
   for the incumbent vendor: account executive → vendor CxO
   sponsor → CFO/CIO internal escalation → replacement. For
   each stage:
   - The trigger that opens the stage (a specific
     underperformance pattern, not a single incident).
   - The evidence pack the head brings (invoice-vs-model
     variance, SLA-miss pattern, roadmap-slip pattern, evaluator's
     technical read).
   - The counterparty role and the head's own role in the
     conversation.
   - The response window before the next stage opens.
   - The evaluator's role in each stage (present at stage one to
     substantiate the technical read; present at stage two if the
     head requires it; not present at internal-escalation stage,
     because that is CxO peer-to-peer).

5. **Author the runtime-security requirements pack — co-authored
   with the level-35 security engineer.** Open the requirements
   authorship jointly with the level-35 `ai-infra-security`
   engineer. Contents per chapter [05](../05-ai-runtime-security-vendor-pnl.md):
   - Prompt-injection defence coverage against the enterprise's
     specific model-deployment shape.
   - Benchmark performance surface — the specific benchmarks the
     engineer chooses (Gandalf-adjacent, Garak, PyRIT, internal
     benchmarks the engineer authors) against which the vendor
     is measured.
   - Throughput at production QPS for inline-inference
     deployments and the acceptable latency budget.
   - Egress data-plane discipline — does the vendor's tool
     exfiltrate inference content to a vendor-hosted plane, and
     is that acceptable under the enterprise's data-handling
     posture.
   - Integration with the enterprise ISMS, SIEM, and SOC (name
     the specific tooling — Splunk, Sentinel, Chronicle,
     Crowdstrike-endpoint, or whatever the enterprise runs).
   - Model-supply-chain attestation format support (CycloneDX
     ML-BOM, SPDX 3.0 AI profile, or documented vendor-native
     format that maps to one of those).
   - Offensive-security engagement scope the engineer would want
     a red-team retainer to deliver.
   The level-35 security engineer signs the pack. Same shape as
   the evaluator's co-authorship — an unsigned requirements pack
   fails the discipline.

6. **Author the runtime-security P&L per incumbent or shortlist
   vendor.** For each vendor on the incumbent-and-shortlist
   list (the named-category vendors are Robust Intelligence,
   Lakera Guard, Calypso AI, HiddenLayer, Protect AI, HydroX AI,
   Cranium, TrojAI; the shortlist may include red-team-as-a-
   service specialists and the CISO-adjacent stack's AI-specific
   coverage claim), author a P&L that carries:
   - Base licence with the specific pricing metric (per-inference,
     per-endpoint, per-model-scan, SaaS-plus-agent, subscription
     tier) and the modelled multi-year cost curve.
   - Red-team retainer plus per-engagement economics where the
     vendor sells that shape.
   - Integration labour with the enterprise SIEM and SOC,
     including the CISO's team's time.
   - CISO-shared cost allocation position for the specific
     vendor (see step 7).
   - SLA position as claimed against the vendor's own public
     materials, with `<!-- needs-research: verify SLA position -->`
     where not verified.
   - Renewal disposition and — critically — the acquisition-
     status flag. Robust Intelligence
     <!-- needs-research: verify current acquisition status -->
     and Protect AI
     <!-- needs-research: verify current acquisition status -->
     are believed to have been acquired; the flag drives the
     escalation-ladder variant in step 8.
   - Coverage-versus-requirements gap against the requirements
     pack from step 5.
   - Contract-term posture (twelve-month preferred, thirty-six-
     month refused unless the acquisition-clause discipline is
     water-tight).
   - Acquisition-clause package — termination-for-unacceptable-
     acquirer right, price-hold clause, product-continuity
     clause, data-portability clause — authored per vendor.

7. **Author the CISO joint operating agreement.** This is the
   distinctive artefact for the runtime-security half of the
   drill. The agreement is a short document (typically two to
   three pages) that the head and the CISO sign jointly and
   revisit annually. Contents:
   - **Scope split.** What the head's portfolio covers (AI-
     specific tooling — model firewall, prompt-injection defence,
     adversarial-ML testing, red-team-as-a-service for AI
     systems, ML-BOM, model-supply-chain attestation) versus
     what the CISO's portfolio covers (enterprise-general
     tooling — network, endpoint, identity, cloud-posture,
     SIEM/SOC, DLP, traditional-security-vendor mix). Name the
     boundary vendors explicitly — a model-firewall that
     inspects LLM inference is head-owned; a Wiz or Snyk
     extension into AI-specific coverage is CISO-owned with an
     AI-specific-coverage-gap review the head runs.
   - **Cost-allocation formula.** For tooling that covers both
     AI-specific and enterprise-general scope, the specific
     formula (percentage split, per-endpoint split, per-scan
     split, or usage-derived split) that determines what portion
     of the cost sits on the head's budget and what portion
     sits on the CISO's budget. The formula is named
     specifically enough that the finance business partner can
     apply it without a new negotiation each cycle.
   - **Escalation channel.** The specific channel through which
     the head opens escalations that touch the CISO's portfolio
     and the CISO opens escalations that touch the head's
     portfolio. Name the peer relationship (head-to-CISO at CxO
     scope; level-35 security engineer to CISO's security
     architects at operating scope) and the standing meeting
     the escalation lands in.
   - **Joint-review cadence.** The quarterly (or other agreed
     cadence) joint review the head and the CISO run against
     the runtime-security portfolio — the standing agenda
     (coverage-gap analysis update, contract decisions coming
     up, incident-posture read, budget-cycle preparation) and
     the artefacts each party brings.
   - **Signature block.** Head and CISO signatures with the
     date; annual re-ratification is a specific action, not an
     assumption.

8. **Author the runtime-security escalation ladder with the
   acquisition-parent variant.** Instantiate the four-stage
   ladder from chapter [05](../05-ai-runtime-security-vendor-pnl.md)
   for the incumbent runtime-security vendor(s). For each
   stage, the same contents as step 4 (trigger, evidence pack,
   counterparty role, response window). Additionally, for
   Robust Intelligence and Protect AI specifically — and any
   other vendor the exercise's own research surfaces as
   acquired — author the acquisition-parent variant:
   - The parent CxO peer inside the acquiring enterprise (Cisco
     enterprise security leadership for Robust Intelligence;
     Palo Alto Networks enterprise security leadership for
     Protect AI). Do not invent named individuals; the ladder
     names the role, not the person.
     <!-- needs-research: verify current acquisition status and confirm the acquiring parent's enterprise-security-account-team role -->
   - The CxO relationship the head cultivates *before* the
     escalation is needed. Escalation-cold with an acquiring
     parent is escalation-into-a-vacuum.
   - The specific escalation ordering — the head opens with the
     acquiring parent's account team, not with the acquired-
     brand team, because the parent controls the roadmap and
     the pricing at renewal.
   - The invocation of the acquisition-clause package from
     step 6 — the head names the specific clause the head is
     invoking (termination-for-unacceptable-acquirer, price-hold,
     product-continuity, or data-portability) when the parent
     is materially re-pricing or re-scoping mid-term.

9. **Author the consolidation-or-expansion decisions on both
   sides.** On the observability side, the head takes one of
   the three postures from chapter [04](../04-ai-observability-vendor-pnl.md)
   — consolidate on a single vendor, best-of-breed across sub-
   categories, or hyperscaler-native plus specialty overlay —
   and names the defence for the chosen posture against the
   enterprise's specific portfolio shape. On the runtime-
   security side, the head takes one of the three postures from
   chapter [05](../05-ai-runtime-security-vendor-pnl.md) —
   single-vendor consolidation, best-of-breed, or open-source-
   anchored — and names the defence against the enterprise's
   level-35 engineering capacity, threat surface, and CISO-
   adjacent stack. Both decisions are dated, both are
   authored with a re-visit trigger, and neither is authored as
   permanent.

10. **Failure-mode audit against the anti-patterns from both
    chapters.** Author a short section per anti-pattern —
    detection signal and recovery action for each. From
    chapter [04](../04-ai-observability-vendor-pnl.md): the
    "observability is an ML platform team decision" abdication;
    the double-monitoring pattern; the under-scoped SaaS-egress
    pattern; the OSS-and-enterprise-tier confusion; the
    evaluator-does-CFO-escalation pattern. From chapter [05](../05-ai-runtime-security-vendor-pnl.md):
    the three-vendors-doing-the-same-thing pattern; the three-
    year-contract-in-a-one-year-category pattern; the "CISO
    doesn't need to know" pattern; the red-team-once-and-shelve
    pattern; the acquisition-orphan pattern; the "we already
    have Wiz / Crowdstrike / Palo Alto" pattern. Eleven
    anti-patterns; eleven paragraphs; the audit is the artefact
    the head reads back to the level-35 partners and to the
    CISO at the annual re-ratification.

## Deliverables

- `observability/requirements.md` — the co-authored requirements
  pack from step 2 with the functional envelope, the non-
  functional envelope, the audit-committee frame, and the level-
  35 evaluator's signature and date.
- `observability/vendor-p-and-l/<vendor>.md` — one file per
  incumbent-and-shortlist observability vendor with the full
  P&L, SLA position, renewal disposition, and coverage-versus-
  requirements gap.
- `observability/escalation-ladder.md` — the four-stage
  escalation ladder for the observability incumbent with the
  evaluator's role per stage.
- `runtime-security/requirements.md` — the co-authored
  requirements pack from step 5 with the level-35 security
  engineer's signature and date.
- `runtime-security/vendor-p-and-l/<vendor>.md` — one file per
  incumbent-and-shortlist runtime-security vendor with the full
  P&L, acquisition-status flag, contract-term posture,
  acquisition-clause package, and coverage-versus-requirements
  gap.
- `runtime-security/ciso-joint-operating-agreement.md` — the
  joint operating agreement from step 7 with scope split, cost-
  allocation formula, escalation channel, joint-review cadence,
  and the head-and-CISO signature block.
- `runtime-security/escalation-ladder.md` — the four-stage
  escalation ladder with the acquisition-parent variant for
  Robust Intelligence, Protect AI, and any other acquired
  vendor the exercise's research surfaces.
- `consolidation-decisions.md` — the consolidation-or-expansion
  decisions on both sides with defence, date, and re-visit
  trigger.
- `failure-mode-audit.md` — the eleven-paragraph anti-pattern
  audit.

## Acceptance criteria

- The observability requirements pack is a co-authored artefact.
  A pack the level-35 evaluator has not signed fails the
  criterion; the co-authorship shape is the load-bearing
  distinctive of the observability P&L and the pack cannot be
  authored on head-of-function authority alone.
- The runtime-security requirements pack is a co-authored
  artefact. A pack the level-35 security engineer has not
  signed fails the criterion; same discipline as observability.
- The CISO joint operating agreement names the cost-allocation
  formula and the escalation channel explicitly. An agreement
  that speaks in principle about "shared cost" without naming
  the specific formula fails the criterion. An agreement that
  speaks in principle about "escalation coordination" without
  naming the specific channel fails the criterion.
- Every vendor P&L file — on both sides — carries a TCO
  breakdown, an SLA position, a renewal disposition, and a
  coverage-versus-requirements gap. A vendor P&L that carries
  base-licence spend without integration labour, data-plane
  cost, and — on the runtime-security side — CISO-shared
  allocation is not a P&L, it is a licence-line quote.
- The runtime-security escalation ladder includes the
  acquisition-parent variant for Robust Intelligence and
  Protect AI specifically. A ladder that treats acquired vendors
  the same way it treats independent vendors fails the criterion;
  the parent controls the roadmap and the parent's CxO account
  team is the head's escalation peer.
- Every SLA figure, pricing figure, and benchmark result quoted
  in the P&L files carries a `<!-- needs-research: verify
  [specific fact] against [source] -->` marker where the fact is
  not independently verifiable against the vendor's current
  public materials. Invented specificity is worse than an
  explicit gap.
- The consolidation-or-expansion decisions on both sides carry
  a defence, a date, and a re-visit trigger. A decision authored
  as permanent fails the criterion; both categories move, and
  the decision is authored to move with them.
- The failure-mode audit names, for each of the eleven
  anti-patterns, at least one specific detection signal and one
  specific recovery action.

## Stretch goals

- Author the **audit-committee-facing one-pager** that
  summarises the paired P&L for the audit committee's review
  cycle. The one-pager compresses both sides into: the
  observability line and the KRI-feed defensibility position;
  the runtime-security line and the CISO-joint-management
  position; the two consolidation-or-expansion postures; and
  the head's specific asks (year-one authorisation, contract-
  term postures, acquisition-clause standing authority to
  invoke).
- Author the **vendor-account-review agenda template** the head
  runs quarterly on each side. On the observability side, the
  agenda is co-run with the level-35 evaluator; on the
  runtime-security side, the agenda is co-run with the level-35
  security engineer (and, at annual cadence, with the CISO). The
  template names the standing sections, the artefacts each
  party brings, and the decision cadence.
- Author the **coverage-gap analysis template** the level-35
  security engineer uses against the CISO-adjacent traditional
  security stack (Wiz, Snyk, Crowdstrike, Palo Alto Networks,
  and peers) when a vendor claims AI-specific coverage that
  overlaps the head's portfolio. The template is what defends
  the head against the "we already have Wiz" anti-pattern
  without producing a defensive posture toward the CISO.
- Draft the **red-team retainer-tier decision case** — the
  specific commercial case for whether the enterprise carries
  a red-team retainer at a specific tier, defended on the
  incident-preparedness case from
  [[mod-110-incident-leadership]] and priced against the
  engagement-per-year expectation the level-35 security
  engineer authors.
- Author the **acquisition-parent relationship-cultivation
  plan** — the specific plan the head runs to establish the
  CxO peer relationship with Cisco enterprise security
  leadership (for Robust Intelligence) and Palo Alto Networks
  enterprise security leadership (for Protect AI) before the
  escalation is needed. The plan sits alongside the executive-
  relationship discipline in [[mod-108-leading-the-governance-function]]
  chapter 06.

## Notes and starter guidance

The most common first-cut failure is the head who authors the
observability requirements pack alone. The observability
category is the level-35 evaluator's technical craft — the head
does not personally know what the enterprise's specific model-
deployment shape needs from drift detection, and a requirements
pack the evaluator has not signed reads at the vendor account
review as a head who has not done the coordination work. Open
the pack authorship jointly, let the evaluator carry the
technical detail, consolidate on top in CFO-legible language,
and get the evaluator's signature before the pack enters the
vendor conversation. Same discipline on the runtime-security
side with the level-35 security engineer.

The second common failure is the runtime-security P&L authored
in isolation from the CISO. The temptation is real — the head
owns the AI-governance function, the CISO is a peer not a
manager, and the head's P&L discipline is authored on the head's
timeline. Authoring in isolation produces the "CISO doesn't need
to know" anti-pattern from chapter 05, the shadow-security read
the CISO carries into the audit committee, and the coverage-gap
that the CISO's existing stack would have closed if anyone had
asked. Open the CISO joint operating agreement authorship as a
peer conversation, not as a head-briefs-CISO exercise. The
agreement is signed by both parties; the cost-allocation formula
is negotiated, not imposed; the escalation channel is agreed,
not announced. The agreement is annual; the co-authorship shape
is what makes the annual re-ratification a substantive
conversation rather than a signature refresh.

The acquisition-parent overlay for Robust Intelligence and
Protect AI is the head's tell for whether the head is reading
the runtime-security category currently. A P&L that treats
Robust Intelligence as an independent vendor two years after
the Cisco acquisition
<!-- needs-research: verify current acquisition status -->
is a P&L authored from stale category knowledge; the head
loses the acquiring-parent escalation channel and misses the
acquisition-clause discipline that would have protected the
enterprise from mid-term re-pricing. Same for Protect AI under
Palo Alto Networks
<!-- needs-research: verify current acquisition status -->.
Author the acquisition-parent variant explicitly, name the
parent CxO peer role (not a named individual — the ladder names
the role and the head cultivates the specific person separately),
and treat the acquiring parent as the counterparty the head
now negotiates with. The acquired-brand team may carry the
account relationship warmly, but they do not carry the roadmap
decision and they do not carry the pricing lever at renewal.

On the SLA and pricing figures — the temptation is to invent
plausible-sounding numbers because the P&L reads sharper with
specifics. Invented specificity is worse than an explicit gap.
The audit committee reads a fabricated 99.9% SLA in the P&L
and, on discovering the fabrication, discounts the entire P&L.
Mark every unverified figure with the `<!-- needs-research -->`
marker, run the verification cycle before the P&L enters the
CFO conversation, and the P&L survives contact with the vendor
and the audit committee both. The chapter itself carries such
markers around vendor scope and acquisition status; the
exercise inherits the discipline.

The paired P&L is a living artefact. Version it, date it,
refresh both requirements packs at the annual joint review with
the level-35 partners, refresh the CISO joint operating
agreement annually with a co-signature, refresh the vendor P&L
files at each renewal cycle, and refresh the consolidation-or-
expansion decisions at each material shift in either category
(a named acquisition, a category entrant with substantive
positioning, an incumbent's roadmap re-aim). A paired P&L that
has not been touched since it was authored is a P&L the two
categories have already outrun — observability moves quarterly
on the LLM-eval overlay, runtime security moves quarterly on
almost every dimension, and the head who does not refresh is
the head who defends stale artefacts at CFO scope.
