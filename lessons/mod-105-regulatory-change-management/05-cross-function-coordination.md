# Cross-Function Coordination on Regulatory-Change Rollout

## Motivation

Chapter 03 named seven lanes in the change-management plan.
Chapter 04 named the compliance-date posture the plan delivers.
Neither chapter addresses the coordination problem that any
practising head recognises within the first month of running a
material regulatory change: the plan and the posture live inside
the head's function, and the enterprise's operating reality lives
in six other functions the head does not manage. If the head
cannot make those six functions move in step, the plan and the
posture stay on paper.

The failure mode this chapter closes is the *coordination miss*.
The level-50 architect updates the crosswalk on time; product
does not adjust its roadmap because product was not consulted
until after the plan was signed; engineering objects to the
sequencing but only surfaces the objection at a governance
council two months later; legal delivers an opinion that
conflicts with a procurement clause the enterprise has already
committed to; HR delivers training that lags the rollout by a
quarter; communications is bypassed and reads about the
enterprise's readiness posture in the trade press. Each miss is
individually small. Together they undo the plan.

The reference frame is the IIA Three Lines Model
([[mod-101-role-scope-and-leadership-shape]] chapter 04) plus
the AI Governance Council operating pack
([[mod-102-running-the-program]] chapter 01). Coordination is
governance work, not project-management work. It is the head's
personal responsibility to run coordination as governance — with
committees, minutes, decision records, and a written engagement
contract with each peer.

## Core concept — six coordination lanes

Regulatory-change rollout runs across six coordination lanes.
Each lane has one CxO peer (or a small named set) who is the
head's primary counterpart. Each lane has a specific artefact the
head expects from the peer and a specific artefact the head
delivers in return. Coordination is the exchange of those
artefacts, on schedule, with disagreements adjudicated at named
committees rather than in the head's inbox.

- **Lane A — the level-50 architect and product / engineering.**
- **Lane B — legal (General Counsel) and, where relevant, outside
  counsel.**
- **Lane C — procurement and the enterprise supplier base.**
- **Lane D — HR, Learning & Development, and (where in scope)
  Chief Compliance / Ethics.**
- **Lane E — communications (Chief Communications Officer) and,
  where relevant, investor relations.**
- **Lane F — CxO peers on adjacent risk vectors (CISO, CIO / CTO
  / CDO, CPO / DPO, CRO, CAE, CFO).**

The rest of this chapter walks each lane, names the artefact
exchange, and lands the governance forum where disagreement is
adjudicated.

## Lane A — level-50 architect and product / engineering

This is the most intimate coordination and the one the head runs
weekly rather than by exception.

### What the head expects from the architect

The level-50 senior AI governance architect
([[mod-101-role-scope-and-leadership-shape]] chapter 07 covers the
downward engagement contract) delivers three artefacts for a
material regulatory change:

- The crosswalk delta — how the new obligation maps into the
  enterprise's control library, its policy taxonomy, its risk
  taxonomy, and the ISO/IEC 42001 AIMS clauses.
- The control-library update — the specific new or modified
  controls, their test procedures, their evidence definitions.
- An engineering-impact sketch — which product surfaces, which
  platform capabilities, and which model registry entries are
  affected, at what depth.

### What the head delivers to the architect

- The prioritised interpretation output (chapter 02).
- The GC opinion reference and any GC-imposed drafting
  constraints on the crosswalk.
- The head's posture proposal (chapter 04) so the architect knows
  which changes need engineering ready by the compliance date
  versus which land in a transition window.

### Where product and engineering come in

Product and engineering are not the architect's subordinates.
They are peer functions who own delivery. The head, working
through the architect, engages product and engineering early —
ideally at the moment chapter 02 promotes an item to *active*.
Product and engineering leadership sit on the AI Governance
Council; the council is where roadmap-versus-obligation
sequencing disagreements land.

The head's rule of thumb: any regulatory change that requires
more than two sprints of engineering work is discussed with the
head of engineering personally before the change-management plan
is authored, not after. Late engagement is the pattern that
produces objections at wave B of chapter 03 lane 2 — which is
already too late to redraft the CEO letter.

### Where disagreement lives

Disagreements between the head and product / engineering on
sequencing, scope, or transition posture live at the AI
Governance Council. Escalations from the council go to the CIO /
CTO / CDO's operating committee or, for enterprise-scale changes,
to the executive committee. GC is consulted on any disagreement
touching legal interpretation of the obligation itself.

## Lane B — legal and outside counsel

Legal coordination for regulatory-change work is dense and it is
where the head is most likely to drift.

### What the head expects from GC

- The interpretive opinion on the packaged obligation (chapter 02
  step 3).
- Ongoing review of drafting for public statements, regulator-
  facing filings, and material internal communications that
  touch the obligation.
- A defensive posture memo (part of the opinion) that supports
  the head's compliance-date posture (chapter 04).
- Where the regulator is an active supervisor, coordination on
  the supervisory-dialogue posture the enterprise takes on the
  change.

### What the head delivers to GC

- The packaged obligation (chapter 02 step 2).
- The change-management plan draft, so GC can flag any lane
  where the plan creates or increases legal exposure.
- The compliance-date posture proposal, so GC can either endorse
  the residual-risk acceptance or object.
- Regulator-facing draft artefacts (filings, statements,
  responses to information requests) before they go out.

### Outside counsel

For material changes — a new statutory regime, a first-of-kind
enforcement action against a peer, an area where enterprise
counsel does not have deep specialist expertise — GC brings in
outside counsel. The head does not choose outside counsel and
does not manage the engagement — that is GC's role — but the
head is a substantive counterpart in outside-counsel workstreams
because the head has the operating context outside counsel needs
to advise well.

The head does not go around GC to outside counsel and does not
receive advice from outside counsel through non-GC channels. This
is the head-and-GC boundary discipline
([[mod-104-regulator-engagement]] chapter 07) reinforced.

### Where disagreement lives

Substantive disagreement with GC is rare on regulatory-change
work and is resolved through the disagreement discipline in
[[mod-104-regulator-engagement]] chapter 07 — joint session,
written statement of disagreement, documented resolution, GC's
view prevails on legal interpretation and the head's view
prevails on technical fact.

## Lane C — procurement and the supplier base

Procurement coordination is where regulatory change most often
fails silently. Contracts are signed, suppliers are engaged, and
nobody noticed the obligation attached at the supplier boundary
until a customer asks about supplier compliance.

### What the head expects from procurement

- An inventory of material AI-supplier contracts (drawn from the
  supplier inventory the level-50 architect maintains under
  [[mod-102-running-the-program]] chapter 04).
- A contract-audit output for each material contract: does the
  contract cover the new obligation, and if not, what
  amendments are needed and on what timeline.
- A template update — the enterprise's standard AI-supplier
  contract template gets a new-obligation clause the enterprise
  will use on future procurements.
- A supplier-communication draft (chapter 03 lane 7) for the head
  to review substantively.
- A post-change verification plan — how procurement will confirm
  each material supplier has moved.

### What the head delivers to procurement

- The packaged obligation and its attachment analysis, focused
  on supplier surfaces.
- The GC opinion and any GC-imposed drafting constraints on
  contract clauses.
- The compliance-date posture, so procurement can sequence
  contract amendments against the date.
- The head's priority ranking on which supplier relationships to
  amend first.

### Where disagreement lives

Procurement typically does not disagree with the head on
regulatory-change substance — the head is the substance authority
— but disagreement can surface on sequencing and on supplier-
relationship diplomacy (a supplier the enterprise depends on,
where a heavy-handed contract amendment ask would jeopardise the
relationship). Disagreement lands at the CFO's procurement
committee or at the AI Governance Council when the trade-off is
between contract discipline and continuity of supply.

## Lane D — HR, L&D, and Chief Compliance / Ethics

Training and policy propagation live in this lane. HR coordination
is where a plan lives or dies at the "does anyone actually behave
differently" test.

### What the head expects from HR / L&D

- A training-refresh plan for each of chapter 03 lane 3's three
  tiers, with a completion SLA the enterprise's LMS can enforce.
- Updated content for the enterprise's mandatory AI acceptable
  use policy where the obligation touches acceptable use.
- Escalation on training-completion gaps at the level and
  cadence agreed in the plan.

Where the enterprise has a distinct Chief Ethics / Compliance
function, HR coordinates with that function on curriculum
substance; the head remains the substance authority for AI-
governance-specific training content.

### What the head delivers to HR / L&D

- Content substance — what the training needs to convey, at what
  depth, for each role-based population.
- The policy update — the head owns the drafting of AI-
  governance-specific policy language; HR owns the acceptable
  use policy shell.
- A named subject-matter expert from the AI-governance function
  who is available for HR / L&D questions during content
  authoring.

### Where disagreement lives

Disagreements with HR / L&D typically surface on timeline (HR
wants more runway to prepare content than the head has budgeted)
or on content depth (HR wants shorter, higher-completion
content; the head wants depth that survives a certification-body
sampling). Disagreements land at the CHRO's operating committee
or at the AI Governance Council. The head does not shortcut HR
by publishing training through the AI-governance function's own
channel — that produces a training record HR does not stand
behind, which does not survive audit.

## Lane E — communications and investor relations

External-facing communication coordination is where the head is
most obviously the substance owner and least obviously the
authority owner.

### What the head expects from communications

- An external-posture draft aligned to the compliance-date
  posture (chapter 04) that Communications will hold if a
  journalist, customer, or prospect asks about the enterprise's
  position on the obligation.
- A proactive-communication decision — whether the enterprise
  will issue a blog post, update the trust centre, or brief
  customers on the change.
- A media-response protocol for the window around the
  compliance date.
- Coordination with IR if the obligation creates a materiality
  question for shareholders.

### What the head delivers to communications

- The substance — plain-English descriptions of the obligation,
  the enterprise's posture, the specific artefacts the
  enterprise stands behind.
- GC review status on any draft.
- The compliance-date posture (chapter 04) so Communications
  understands what the enterprise will and will not claim about
  its readiness.

### Investor relations

Where the obligation could produce a materiality event —
enforcement action risk, product-stop-shipping risk, large
compliance-cost commitment — the head briefs IR, coordinated with
CFO and GC, on the substance IR needs for its own disclosure
discipline. IR decides on disclosure. The head does not decide.

### Where disagreement lives

Communications disagreement typically surfaces on how proactive
the enterprise should be — Communications sometimes wants more
proactive disclosure than the head or GC does; sometimes the
inverse. Disagreements land at a joint CCO / GC / head session,
escalated to the executive committee if unresolved. The head does
not release external communication that Communications has not
signed and does not release communication that GC has not
reviewed. External communication is a governance discipline, not
a head-of-function press release.

## Lane F — adjacent CxO risk vectors

The final coordination lane is with CxO peers whose risk vector
overlaps the obligation.

### CISO

Where the obligation touches AI security — model-weight
protection, prompt-injection defence, supply-chain security under
the CISA / NCSC guidance — the CISO is a substantive coordination
partner. The head owns the AI-governance overlay; the CISO owns
the security posture. Coordination artefact: joint memo where
the two functions' controls interlock; joint incident-response
runbook where the obligation touches incidents; joint board
briefing on the security-adjacent portion of the change.
Cross-reference: [[mod-109-cross-enterprise-leadership]] chapter
01 (CISO coordination).

### CIO / CTO / CDO

The enterprise's engineering leadership owns the platforms the AI
program runs on. Coordination with them on regulatory change is
non-negotiable when the change touches platform capabilities
(model registry, telemetry, data-governance tooling). The head
does not commit engineering leadership to a delivery date without
their concurrence. The AI Governance Council is the forum where
concurrence is recorded; the CIO / CTO / CDO's operating
committee is where sequencing disagreements land.
Cross-reference: [[mod-109-cross-enterprise-leadership]] chapter
01.

### CPO / DPO

Where the obligation is a privacy-adjacent obligation (CPPA
ADMT rulemaking, GDPR-lineage automated decision-making rules,
Colorado AI Act's overlaps with the CPA), the CPO or DPO is a
peer substance authority on the privacy portion. Coordination
artefact: joint interpretation memo where the two obligations
attach; joint DPIA / AIA where the impact assessments overlap.
Cross-reference: [[mod-109-cross-enterprise-leadership]] chapter
02.

### CRO

The CRO owns the enterprise risk framework the AI-governance
function's risk register nests inside. Regulatory-change work
that shifts a risk taxonomy, tolerance limit, or appetite
statement is coordinated with the CRO in advance. The CRO's
risk-committee briefing (mod-103 chapter 03) receives the update
after coordination.

### CAE

The Chief Audit Executive owns third-line audit. Regulatory-
change rollout that will be audited (whether by the third line
or by an external auditor) is coordinated with the CAE early so
that the audit programme calibrates against the enterprise's
posture, not against a stale operating design. Cross-reference:
[[mod-108-leading-the-governance-function]] chapter 05.

### CFO

Where the change carries material cost — engineering effort,
vendor spend, external audit / certification cost — the CFO is
coordinated on the budget impact. The head does not commit
budget the CFO has not approved. Cross-reference:
[[mod-113-budget-vendor-p-and-l-and-investment-case]] chapter
01.

## The coordination pack — the artefact that holds coordination together

Six coordination lanes running in parallel is unmanageable without
a single document that shows the head, and every peer, the state
of coordination at any moment. The head maintains a coordination
pack for each material regulatory change with a fixed shape:

- The change identifier and the obligation.
- For each of the six lanes: the peer, the current expected
  artefacts (in and out), the SLA, the status, and any
  disagreement in flight.
- The upcoming AI Governance Council agenda item(s) referencing
  the change.
- The next four weeks of coordination touchpoints on the head's
  calendar.

The pack is a living artefact updated weekly by the change's
desk owner (from chapter 02) and reviewed by the head at the
weekly digest read (chapter 01). It is not distributed broadly —
peers receive lane-specific summaries — but it is the head's
single source of truth for the change's coordination state.

## The forum discipline

Coordination happens at forums, not in the head's inbox. The
head's discipline: name the forum where each coordination
decision belongs, refuse to make coordination decisions outside
that forum, and hold peers to the same discipline.

- The AI Governance Council owns cross-function decisions where
  the head is the chair (see [[mod-102-running-the-program]]
  chapter 01).
- The executive committee owns enterprise-wide decisions with
  material cost, headcount, or reputational exposure.
- The CIO / CTO / CDO operating committee owns
  engineering-sequencing decisions.
- The CFO's operating or procurement committee owns
  budget-and-supplier decisions.
- The risk committee (mod-103 chapter 03) owns risk-appetite
  decisions.
- The audit committee (mod-103 chapter 02) owns third-line-
  coordinated decisions and material-change briefings.

A coordination question the head cannot map to a forum is a
question the head does not have the standing to answer alone.
Escalating it to a forum is not weakness; it is governance
working.

## The coordination anti-patterns

Three anti-patterns to name and refuse.

- **The bilateral back-channel.** Two peers agree to a
  coordination move outside a forum, without the third peer who
  is affected. The move works until it does not, at which point
  the third peer surfaces the disagreement in a way that
  embarrasses everyone. The head does not participate in
  bilateral back-channels on material decisions.
- **The consensus tax.** Every coordination decision requires
  every peer's active concurrence, so no decision moves. The
  head calibrates: concurrence is required from peers with
  substantive exposure; awareness is required from peers whose
  exposure is peripheral. The distinction is written into the
  engagement contracts (mod-101 chapter 07) and defended at the
  AI Governance Council.
- **The head-does-it-all pattern.** The head steps into peers'
  execution when peers do not move. This produces short-term
  delivery and long-term coordination breakdown — peers stop
  moving because the head will do it. The head's discipline:
  escalate slippage to the peer's own CxO chain, not do the
  peer's work.

## The one-sentence summary

Cross-function coordination on regulatory-change rollout is six
lanes — architect / product / engineering, legal, procurement,
HR / L&D, communications / IR, and adjacent CxO peers — each
with a named counterpart, a written artefact exchange, and a
named forum for adjudicating disagreement; the head runs
coordination as governance, not project management, and holds
peers to the same discipline.

## Summary

- Regulatory-change rollout runs across six coordination lanes
  the head does not manage but must coordinate: architect /
  product / engineering, legal, procurement, HR and L&D,
  communications and IR, and adjacent CxO peers (CISO, CIO /
  CTO / CDO, CPO / DPO, CRO, CAE, CFO).
- Each lane has a named counterpart, a specific artefact
  exchange (in and out), an SLA, and a named forum where
  disagreement is adjudicated.
- The AI Governance Council is the head's own forum; escalations
  route to the executive committee, the CIO / CTO / CDO
  operating committee, the CFO's procurement committee, the
  risk committee, or the audit committee depending on the
  decision.
- The coordination pack is a living document the head maintains
  for each material change — six lanes, current artefact
  status, disagreements in flight, upcoming touchpoints — and
  is the head's single source of truth.
- Three anti-patterns to refuse: bilateral back-channels,
  consensus tax, head-does-it-all pattern. The head runs
  coordination as governance and holds peers to the same
  discipline.
- Where the head is the substance authority (all lanes), the
  head is not necessarily the delivery owner. Communications
  releases, procurement contracts, HR training, engineering
  code, and legal opinions belong to peers; the head supplies
  substance and reviews for accuracy, and does not go around
  peers when peers are slow.
