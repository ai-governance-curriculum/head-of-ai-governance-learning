# The AI-Runtime Security Vendor P&L — Coordinated with the Level-35 AI-Infra-Security Engineer and the CISO

## Motivation

AI runtime security is the fastest-moving, most vendor-fragmented
category in the AI-governance vendor portfolio. The category
boundary is unstable. The same vendor may position, across four
quarters, as red-team-as-a-service, as a model-firewall, as a
prompt-injection defence layer, as an ML-BOM producer, and as a
model-supply-chain attestation provider — sometimes because the
product has genuinely evolved, sometimes because the go-to-market
messaging has re-aimed. The threat surface itself is moving
underneath the vendors. Prompt-injection landed as a material
concern only a few years ago; model-supply-chain attestation is
still stabilising; adversarial-ML testing is being productised in
real time. The head who runs this category with the same posture
the head runs the GRC-for-AI category —
chapter [03-grc-for-ai-vendor-pnl](03-grc-for-ai-vendor-pnl.md),
with multi-year contracts and a single-vendor consolidation bias
— is a head who signs long-term commitments to fast-shifting
product bets.

Meanwhile the CISO is running an adjacent portfolio. Network,
endpoint, identity, cloud-posture, SIEM, SOC, DLP, and the
traditional-security vendor mix (Palo Alto, Crowdstrike, Wiz,
Snyk, Splunk, Sentinel, Chronicle, and peers) sit inside a
security-P&L discipline substantially more mature than the AI-
runtime-security P&L the head is standing up. The head's P&L has
to be legible to the CISO as a peer to that discipline, not as a
shadow-security procurement running around the CISO's stack.
Where the head runs the portfolio without CISO alignment, the
CISO reads the head as running shadow security; where the head
defers the portfolio entirely to the CISO, the AI-specific threat
surface is under-covered because the CISO's tools were not
designed for it. The right posture is neither extreme; it is a
co-managed portfolio run at CxO scope by two peers, with the
level-35 AI-infra-security engineer as the operating spine.

This chapter is how the head runs that portfolio. Not the pilot
execution — the level-35 engineer runs pilots. Not the enterprise-
security posture — the CISO owns that. What the head runs is the
P&L: the commercial framing of pilots, the contract terms, the
acquisition-clause discipline, the CISO-shared cost allocation,
the consolidation-or-expansion decision, and the escalation with
the vendor (or with the acquiring parent where the vendor has
been acquired). The head is the account-side CxO owner; the
level-35 engineer is the technical owner; the CISO is the
enterprise-security peer. The three roles compose, and the
composition is the discipline the chapter is naming.

## Core concept — the category map, the coordination pattern, and the P&L shape

Three things have to be true before the head runs the runtime-
security P&L competently. The head has to hold a working map of
the vendor category and its adjacent categories. The head has to
run a specific coordination pattern with the level-35 engineer and
with the CISO — a pattern that is different from the coordination
pattern chapter [04-ai-observability-vendor-pnl](04-ai-observability-vendor-pnl.md)
describes for the observability category. And the head has to
frame the P&L in the specific commercial shape this category
takes — short contract terms, acquisition-clause discipline,
CISO-shared cost allocation, retainer-plus-per-engagement
red-team economics.

### The vendor category map

The named vendors in this category, positioned briefly against
the public-material-consistent description at the time of
authoring. Every named product-scope claim carries a
`needs-research` marker because the category moves quarterly and
the head verifies current scope against current public material
before signing anything.

**Robust Intelligence.** AI security and validation platform
covering pre-deployment testing and runtime protection. Believed
acquired by Cisco in 2024; the acquisition changes the
enterprise-account posture materially — the head is negotiating
with a large-enterprise-security-vendor parent rather than with
the acquired-brand independent team.
<!-- needs-research: verify Cisco / Robust Intelligence acquisition status and current product-line positioning under Cisco. -->

**Lakera Guard.** LLM prompt-injection defence and guardrails
positioning, developer-first go-to-market. The company also
maintains the Gandalf prompt-injection benchmark as a community-
visible artefact that has drawn attention to the category.
<!-- needs-research: verify current Lakera Guard product scope, deployment shape, and Gandalf benchmark positioning. -->

**Calypso AI.** LLM security and observability positioning for
enterprise, with government-adjacent positioning in the go-to-
market.
<!-- needs-research: verify current Calypso AI product scope and government-adjacent positioning. -->

**HiddenLayer.** Model-security platform positioning covering
adversarial-ML detection and model-supply-chain protection.
<!-- needs-research: verify current HiddenLayer product scope, particularly the split between adversarial-ML detection and model-supply-chain protection. -->

**Protect AI.** AI security spanning ML-model scanning
(ModelScan), SBOM-for-ML tooling, and adjacent open-source and
commercial products. Believed acquired by Palo Alto Networks;
the acquisition, like the Cisco / Robust Intelligence
acquisition, changes the enterprise-account posture.
<!-- needs-research: verify Palo Alto Networks / Protect AI acquisition status and current product-line positioning under Palo Alto Networks. -->

**HydroX AI.** AI security and red-teaming positioning.
<!-- needs-research: verify current HydroX AI product scope and red-teaming go-to-market posture. -->

**Cranium.** AI security and third-party risk posture covering
the model-supply-chain angle for enterprises that consume many
third-party models.
<!-- needs-research: verify current Cranium product scope and third-party-risk positioning. -->

**TrojAI.** Model-security platform anchored in adversarial-ML
and model-firewall positioning.
<!-- needs-research: verify current TrojAI product scope, particularly the model-firewall claim. -->

Beyond the named-vendor list, the head maintains awareness of
four adjacent categories that overlap the runtime-security P&L
without belonging entirely inside it.

- **Red-team-as-a-service specialists.** A set of firms
  specialising in AI red-team engagements — some pure-play, some
  extensions of established offensive-security firms.
  <!-- needs-research: verify current red-team-as-a-service specialist landscape for AI systems; note pure-play entrants and offensive-security-firm extensions. -->
- **ML-BOM / model-supply-chain attestation tooling.**
  CycloneDX ML-BOM and SPDX 3.0 AI profile are the reference
  formats emerging in the community; commercial tooling from
  Cranium, HiddenLayer, Protect AI, and adjacent parties
  produces or consumes these formats.
  <!-- needs-research: verify current CycloneDX ML-BOM and SPDX 3.0 AI profile status; verify which named commercial vendors produce or consume them. -->
- **Prompt-injection benchmark projects.** Lakera Gandalf as a
  visible example; other academic and community benchmarks
  exist and evolve.
  <!-- needs-research: verify current prompt-injection benchmark landscape; note academic vs commercial provenance for each. -->
- **The CISO-adjacent traditional security stack expanding into
  AI.** Wiz, Snyk, Crowdstrike, Palo Alto Networks, and peers
  are extending their existing platforms into AI-specific
  coverage. This matters to the head because the CISO's
  incumbent security stack will make coverage claims into the
  head's runtime-security portfolio; the head has to run a
  substantive coverage-gap analysis rather than defer to the
  claim.
  <!-- needs-research: verify current AI-security product-line status for Wiz, Snyk, Crowdstrike, Palo Alto Networks, and other CISO-adjacent traditional-security vendors. -->

The head does not need a substantive relationship with every
vendor in this map. The head does need to hold it well enough
to recognise a positioning shift at renewal, to recognise
category overlap when three tools claim to solve the same
threat model, and to recognise the difference between a mature
category (which consolidates) and an unstable one (which does
not).

### The coordination pattern with the level-35 AI-infra-security engineer and the CISO

Chapter [04-ai-observability-vendor-pnl](04-ai-observability-vendor-pnl.md)
described the coordination pattern with the level-35 AI-
evaluation engineer on the observability portfolio. The runtime-
security portfolio uses the same structural pattern — head-owns-
P&L, engineer-owns-technical-integration — with a critical
additional axis: the CISO. The observability portfolio does not
have a CISO overlay; the runtime-security portfolio does.

The head owns the P&L: contract, commercial terms, vendor CxO
relationship, defence to the CFO.

The level-35 AI-infra-security engineer authors the technical
requirements the head cannot author personally: prompt-injection
defence coverage against the enterprise's model deployment
shape; prompt-injection benchmark performance against public and
internal benchmarks the engineer chooses (Gandalf-adjacent,
Garak, PyRIT, and whatever else survives the engineer's
review<!-- needs-research: verify current OSS AI-security tooling landscape including Garak, PyRIT, and adjacent tools; note maintenance status and adoption. -->);
throughput at production QPS for inline-inference deployments;
egress data-plane discipline (does the vendor's tool exfiltrate
inference content to a vendor-hosted plane, and is that
acceptable under the enterprise's data-handling posture);
integration with the enterprise ISMS, SIEM, and SOC (Splunk,
Sentinel, Chronicle, Crowdstrike-endpoint, or whatever the
enterprise runs); model-supply-chain attestation format support
(CycloneDX ML-BOM, SPDX 3.0 AI profile); and the offensive-
security engagement scope a red-team retainer would need to
deliver.

The head and the level-35 engineer jointly coordinate with the
CISO. The CISO owns the enterprise security posture; the AI-
runtime security overlay sits inside that posture. Coordination
has two distinct tiers.

- **CxO-scope coordination — head to CISO.** The head briefs
  the CISO on the AI-runtime-security portfolio at a defined
  cadence (quarterly is common), covering the vendor portfolio,
  the coverage-gap analysis against the CISO's existing stack,
  material contract decisions in the next two quarters, the
  shared-cost allocation position, and the incident posture the
  AI systems carry. The CISO briefs the head on the enterprise
  security posture and where AI-specific threats intersect it.
  This is peer coordination, not reporting.
- **Operating-scope coordination — level-35 engineer to CISO's
  security architects.** The level-35 engineer works with the
  CISO's security architects on the integration surface: how
  runtime-security tooling wires into the SIEM, how alerts
  route through the SOC, how detection rules compose with the
  enterprise's existing detection, how the ML-BOM integrates
  with the enterprise's SBOM discipline, how offensive-security
  engagements coordinate with the CISO's red-team calendar.
  Neither tier substitutes for the other.

The head does not run the operating-scope coordination
personally, but confirms it is happening. A level-35 engineer
not in regular contact with the CISO's security architects is a
portfolio the head has to correct.

### Vendor pilots and red-team engagements

Two commercial patterns are specific to this category.

**Vendor pilots.** Almost every runtime-security vendor sells
through a pilot. The level-35 engineer runs the pilot on the
technical side — deployment, test-plan execution, data-plane
discipline verification, integration for the pilot scope, and
the technical recommendation. The head runs the commercial
framing: pilot-cost cap (paid, unpaid, or hybrid); pilot-outcome
criteria (what has to be true for the pilot to convert); path-
to-production commercial shape (the contract shape the
enterprise would sign if the pilot succeeds); and exit
disposition (what the enterprise commits to at the end of an
unsuccessful pilot). A pilot without a commercial frame is a
pilot the vendor converts to a support-ticket queue after ninety
days, with no path to a decision. Every pilot has a documented
commercial frame before it begins.

**Red-team engagements.** Red-team-as-a-service is commonly sold
on retainer plus per-engagement. The retainer buys readiness (a
pre-scoped engagement team, familiarity with the enterprise's AI
systems, a scheduling window the enterprise can draw against);
each engagement is priced per scope and duration. The head owns
the retainer P&L — whether the retainer is worth carrying, at
what tier, and against which vendor. The level-35 engineer owns
the engagement scope — what each engagement targets, what the
success criteria are, and what the report has to deliver. A
retainer with no engagements is readiness spend that never
converts; engagements without a retainer are higher-priced one-
off buys that lose the readiness benefit. The retainer decision
is made against the incident-preparedness case from chapter
[02-multi-year-investment-case](02-multi-year-investment-case.md);
the head defends the retainer to the CFO on that basis.

## What the runtime-security P&L covers

The P&L for this category is not a single contract line. It is a
composite of licence spend, retainer spend, engagement spend,
integration labour, and shared-cost allocation. The head runs it
as a portfolio, and the head's budget line (from chapter
[01-governance-function-budget-line](01-governance-function-budget-line.md))
carries the composite total.

**Model-firewall / prompt-injection-defence licence.** Often
per-inference or per-endpoint priced. Pricing interacts with the
enterprise's inference-volume trajectory — a per-inference
contract defensible at year one can be indefensible at year
three if AI adoption has scaled by an order of magnitude. The
head negotiates volume tiers and volume-scaling caps at signing.

**Red-team-as-a-service retainer plus per-engagement.** The
retainer is defended on the incident-preparedness case; each
engagement is charged and modelled against the specific scope.

**Model-scanning and ML-BOM tooling.** Often SaaS-plus-agent
priced. The head confirms that the model-supply-chain
attestation format the tool produces is one the enterprise's
downstream consumers can consume — CycloneDX ML-BOM, SPDX 3.0 AI
profile, or a well-documented vendor-native format that maps to
one of those.

**Adversarial-ML testing platform.** Either standalone or
bundled with model-scanning and model-firewall lines. The head
asks whether the platform is genuinely separately priceable, or
bundled such that the enterprise is paying for capability the
level-35 engineer will not use.

**Model-supply-chain attestation subscription.** Cranium,
HiddenLayer, Protect AI, and adjacent parties sell this at a
subscription tier that overlaps model-scanning and adversarial-
ML testing; the head disambiguates capability across vendors to
avoid double-counting.

**Integration labour with the enterprise SIEM and SOC.** This
line is usually under-budgeted at signing and materially real
at deployment. The level-35 engineer estimates the labour; the
head carries it in the P&L; the CISO's team does the integration
work (or the head's function funds the CISO's team's time — the
allocation is negotiated).

**CISO-shared cost allocation.** Where the tooling covers both
AI-specific and enterprise-general security scope, the head and
CISO agree an allocation split. A model-firewall that inspects
LLM inference is AI-specific; the head carries most of that
cost. A model-scanning tool that also scans traditional binaries
in an ML pipeline touching the CI/CD toolchain is partially
enterprise-general; some portion of that cost belongs in the
CISO's budget. A ML-BOM tool that feeds the enterprise's
existing SBOM discipline is partly enterprise-general on the
same logic. The head does not accept the entire cost inside the
governance-function budget when the tool covers general
enterprise scope too; the head negotiates the allocation with
the CISO, documents the split, and re-negotiates at contract
renewal or when the tool's scope changes.

## Renewal-and-escalation discipline

The renewal discipline in this category echoes chapter
[03-grc-for-ai-vendor-pnl](03-grc-for-ai-vendor-pnl.md) in
structure — the head runs a defined renewal cycle, negotiates
against a defensible position, and holds an escalation path when
the vendor is materially underperforming. Three distinctives
matter here specifically.

**Short contract terms preferred.** The vendor landscape moves
quarterly. Twelve-month terms are often more defensible than
thirty-six-month terms in this category, even at a higher per-
year price, because the option value of exiting a mistaken
commitment at twelve months is substantial. The head does not
sign the three-year term the sales team pushes on the argument
that "the category will settle by then"; the sales team does
not know that, and the head does not carry the downside risk.

**Acquisition-clause discipline.** The vendor may be acquired
mid-term — Robust Intelligence and Protect AI are recent visible
examples, and there will be more. The head negotiates change-of-
control clauses at signing. Specific positions to secure:

- A termination-for-convenience right if the vendor is acquired
  by a party the enterprise identifies as commercially or
  strategically unacceptable (a competitor to the enterprise, a
  vendor the enterprise has an existing exclusionary
  relationship with, a party the enterprise's regulator would
  find problematic).
- A price-hold clause preventing the acquiring parent from
  materially re-pricing the product mid-term.
- A product-continuity clause preventing the acquiring parent
  from discontinuing the specific product-line the enterprise
  is licensed for without notice and a migration path.
- A data-portability clause that survives the acquisition —
  the enterprise's inference logs, ML-BOM records, and
  detection rules remain portable.

None of these clauses is bullet-proof against an acquiring
parent that is determined to re-negotiate, but each one raises
the friction against the outcomes the head wants to avoid.

**Escalation with the acquiring parent.** Where the vendor has
been acquired, the head opens escalation with the parent CxO
account team, not with the acquired-brand team. The parent
controls the roadmap now; the acquired-brand team may still
carry the account relationship but does not carry the product
decision. The head's peer inside the parent is the parent's
enterprise-account CxO — for Cisco, the Cisco enterprise
security leadership; for Palo Alto Networks, the Palo Alto
Networks enterprise security leadership. The head cultivates
that peer relationship before it is needed.

The four-stage escalation path from chapter
[03-grc-for-ai-vendor-pnl](03-grc-for-ai-vendor-pnl.md) applies
here — first to the account executive, second to the vendor (or
parent) CxO sponsor, third internally to the CFO and CIO with
the material-underperformance case, fourth as contract
termination and replacement. The category's fast movement means
the fourth stage is exercised more frequently than in the GRC-
for-AI category; termination is a real option that fits the
category's volatility, not the nuclear option it is elsewhere.

## The consolidation-or-expansion decision

The consolidation-or-expansion decision from chapters
[03-grc-for-ai-vendor-pnl](03-grc-for-ai-vendor-pnl.md) and
[04-ai-observability-vendor-pnl](04-ai-observability-vendor-pnl.md)
recurs here with the acquired-parent overlay. The head considers
three postures.

**Single-vendor consolidation.** Attractive for operational
simplicity — one contract, one integration surface, one CxO
relationship. Risky in a fast-shifting category because the
single vendor's roadmap becomes the enterprise's threat-coverage
profile; if the vendor's roadmap diverges, or the vendor is
acquired and the parent re-prioritises, the enterprise carries
the divergence. The head does not default to consolidation in
this category the way the head might in a mature category.

**Best-of-breed.** Often necessary given category fragmentation.
Different vendors are strong on different threat models —
prompt-injection defence, adversarial-ML testing, model-supply-
chain attestation, red-team engagement, model-scanning — and
coverage is stronger when the per-threat-model vendor is the
strongest available. The cost is more contracts, more
integration surface, and more vendor relationships to run at
CxO scope. The head accepts that cost when category
fragmentation warrants it.

**Open-source-anchored.** Some enterprises anchor on OSS —
Gandalf-adjacent benchmarks, Garak, PyRIT, and adjacent tooling<!-- needs-research: verify current OSS AI-security tooling landscape and maintenance status; note projects that have moved between hobbyist and vendor-backed models. -->
— and use commercial tooling narrowly. This posture minimises
lock-in and maximises transparency; it requires more level-35
engineer time and puts the enterprise closer to the underlying
technical craft. The head considers this posture when the
level-35 engineer is genuinely capable of running it.

None of the three is universally correct. The head picks against
the enterprise's specific level-35 engineering capacity, threat
surface, and CISO-adjacent stack, and re-visits at each material
contract renewal.

## Anti-patterns the head does not permit

**The three-vendors-doing-the-same-thing pattern.** The head has
signed with three vendors whose prompt-injection defence
products overlap materially. Nobody has taken the consolidation
decision because the category is confusing and each vendor
claims to be strong on a different flavour of the problem. The
enterprise pays three licences and runs three integration
surfaces for one coverage need. The remedy is the level-35-
engineer-led coverage-gap analysis and the head-led
consolidation decision against it.

**The three-year-contract-in-a-one-year-category pattern.** The
head signed a thirty-six-month contract because the discount
was material and the sales pitch on category stability was
persuasive. Fifteen months in, the roadmap has shifted — the
vendor has re-positioned, the contracted capability has been
de-prioritised, or the acquisition has landed and the parent
has re-prioritised. The head is locked in for another
twenty-one months. The remedy is the short-contract-term
discipline and the acquisition-clause discipline; the head does
not sign the thirty-six-month term in an unstable category on a
discount argument.

**The "CISO doesn't need to know" pattern.** The head has stood
up AI-runtime-security tooling without CISO alignment. The
tooling duplicates capability the CISO's existing stack carries,
conflicts with the CISO's detection rules, or routes alerts
through a channel the SOC does not read. The CISO reads the
head as running shadow security; the audit committee reads the
two-portfolio pattern as governance failure. The remedy is the
CxO-scope and operating-scope coordination pattern the chapter
names.

**The red-team-once-and-shelve pattern.** The head bought a
one-time red-team engagement two years ago, filed the report,
and never funded the retainer. Findings are stale; the AI
systems have evolved; the enterprise has no ongoing offensive-
security capability; the incident-preparedness case is authored
on the assumption of a retainer the head is not carrying. The
remedy is a real retainer decision — either the head funds a
retainer at a defensible tier, or articulates why the
enterprise's risk profile does not warrant one and defends the
omission on the incident-preparedness case.

**The acquisition-orphan pattern.** The vendor has been
acquired, the acquiring parent has re-prioritised or
discontinued the product-line, and the head has not moved
because switching cost is real and the tool still technically
works. The enterprise runs on an orphaned platform whose roadmap
has stopped. The remedy is the acquisition-clause discipline
(termination and product-continuity protection in the contract)
and the head's willingness to invoke it when the parent's
disposition warrants; the head does not carry an orphaned
platform on inertia.

**The "we already have Wiz / Crowdstrike / Palo Alto" pattern.**
The head has deferred to the enterprise-security stack's
coverage claim without a substantive coverage-gap analysis. The
CISO's tools were designed for cloud-posture, endpoint, network,
and identity; they are being extended into AI-specific coverage,
but unevenly. The AI-specific threat surface — prompt injection,
adversarial-ML manipulation, model-supply-chain compromise,
jailbreak attempts against production LLM endpoints — is under-
covered. The remedy is the level-35-engineer-led coverage-gap
analysis and the head's disposition to fund AI-specific tooling
where the analysis reveals a real gap after the CISO's stack is
credited for what it does cover.

## Composition with adjacent modules

- **The budget line item** in chapter
  [01-governance-function-budget-line](01-governance-function-budget-line.md)
  carries the runtime-security P&L's composite total; this
  chapter's detail sits underneath it.
- **The multi-year investment case** in chapter
  [02-multi-year-investment-case](02-multi-year-investment-case.md)
  — specifically the incident-preparedness case — is what the
  red-team retainer, the incident-response reserve, and the
  ML-BOM subscription are defended on.
- **The GRC-for-AI vendor P&L** in chapter
  [03-grc-for-ai-vendor-pnl](03-grc-for-ai-vendor-pnl.md) shares
  the structural discipline but not the category volatility;
  the head runs the two portfolios distinctly.
- **The AI-observability vendor P&L** in chapter
  [04-ai-observability-vendor-pnl](04-ai-observability-vendor-pnl.md)
  overlaps this chapter on prompt-injection detection;
  observability tools sometimes carry basic prompt-injection
  detection, runtime-security tools sometimes carry basic
  inference-quality signals; the head disambiguates and does
  not double-pay.
- **The AIMS operating calendar and the control library** in
  [[mod-102-running-the-program]] are what runtime-security
  tooling produces evidence into.
- **The KRI/KPI portfolio and the maturity assessment** in
  [[mod-107-program-measurement-and-maturity]] carry the
  security KRIs (prompt-injection block rate, red-team-finding
  severity distribution, ML-BOM coverage, adversarial-ML
  detection rate) that feed the audit committee's read on
  runtime-security posture.
- **The CxO vendor-relationship discipline** in
  [[mod-108-leading-the-governance-function]] chapter 06 is the
  substantive relationship discipline the head applies with the
  vendor's account executive and, where acquired, with the
  acquiring parent's CxO team.
- **The cross-enterprise CISO coordination** in
  [[mod-109-cross-enterprise-leadership]] is the CxO-scope
  substrate the CISO conversation lives inside.
- **The incident-leadership discipline** in
  [[mod-110-incident-leadership]] is what the red-team retainer
  actually unlocks — a real incident response capability with
  offensive-security familiarity with the enterprise's AI
  systems. The retainer is what makes the discipline executable.
- **The sector-program leadership** in
  [[mod-111-sector-program-leadership]] carries sector-specific
  threat models (financial-services adversarial-ML patterns,
  healthcare model-integrity threats, defence supply-chain
  assurance) that the head factors into portfolio design.

## Summary

- AI runtime security is the fastest-moving, most fragmented
  vendor category in the AI-governance portfolio; the head does
  not run it with the GRC-for-AI category's posture, and does
  not defer it entirely to the CISO's existing stack.
- The head runs a working map of the named vendors — Robust
  Intelligence (believed acquired by Cisco), Lakera Guard,
  Calypso AI, HiddenLayer, Protect AI (believed acquired by
  Palo Alto Networks), HydroX AI, Cranium, TrojAI — plus the
  adjacent categories of red-team-as-a-service, ML-BOM tooling,
  prompt-injection benchmarks, and the traditional-security
  stack expanding into AI. Every vendor scope claim carries a
  `needs-research` marker because the category moves quarterly.
- Coordination is three-role — head owns the P&L, level-35
  AI-infra-security engineer owns the technical requirements
  and operational integration, CISO owns the enterprise-security
  posture. Head and engineer jointly coordinate with the CISO —
  head at CxO scope, engineer with the CISO's security
  architects at operating scope.
- The P&L is a composite: model-firewall licence, red-team
  retainer plus per-engagement, model-scanning and ML-BOM,
  adversarial-ML testing, model-supply-chain attestation, SIEM
  and SOC integration labour, and a negotiated CISO-shared cost
  allocation where the tool covers both AI-specific and
  enterprise-general scope.
- Renewal favours short contract terms in an unstable category;
  the head negotiates acquisition-clause protection (termination
  for unacceptable acquirer, price hold, product continuity,
  data portability) at signing; where the vendor is acquired,
  escalation goes to the acquiring parent's CxO account team.
- The consolidation-or-expansion decision has three postures —
  single-vendor, best-of-breed, open-source-anchored — picked
  against the enterprise's level-35 engineering capacity,
  threat surface, and CISO-adjacent stack, and revisited at
  each material renewal.
- Six anti-patterns the head refuses: three-vendors-doing-the-
  same-thing, three-year-contract-in-a-one-year-category, "CISO
  doesn't need to know", red-team-once-and-shelve, acquisition-
  orphan, and "we already have Wiz / Crowdstrike / Palo Alto"
  without a coverage-gap analysis.
- Chapter [06-assurance-body-relationship-pnl](06-assurance-body-relationship-pnl.md)
  runs the assurance-body P&L that carries the independence
  signal the audit committee reads; the runtime-security P&L
  here and the assurance-body P&L next compose into the total
  vendor-portfolio picture the head defends at the annual budget
  cycle.
