# The Multi-Year Hiring Plan — Headcount Ladder, Sourcing, Interview Loop, Compensation

## Motivation

Chapter [[01-function-org-shape-and-reporting-lines]] fixed the
shape — five role archetypes on the level ladder, a chosen
reporting-line pattern, a documented succession picture. This
chapter fills the shape with people, across a horizon long enough
that hiring is planned rather than reactive.

A function hired reactively — every headcount opened after the
work has already piled up on the head's or the level-50
architect's desk — spends the year behind. The head who calls in
a hurried recruiter search after a Q2 volume spike is a head who
will not close the requisition until Q4, will not onboard the hire
to productivity until Q1 next year, and will spend the intervening
nine months either burning out the incumbents or defending
missed deliverables to the audit committee. The multi-year hiring
plan is the discipline that runs hiring against a horizon rather
than against a backlog.

The plan is also the head's negotiating instrument. The CFO's
budget cycle ([[mod-113-budget-vendor-p-and-l-and-investment-case]])
authorises headcount by year; the plan is what the head takes into
that cycle. The CRO's second-line coordinator reviews the plan
for coherence with the risk operating model; the CAE reads it for
capacity-to-cooperate on third-line-audit engagement (chapter
[[05-cae-and-third-line-coordination]]). The plan has to survive
each of those reads without redefinition.

This chapter is the discipline underneath the plan. Not one open
requisition — a horizon. Not one candidate — a sourcing strategy.
Not one interview — an interview loop with a repeatable shape.
Not one salary offer — a compensation-band positioning that
survives the offer conversation and the retention conversation
that follows.

## Core concept — the plan has a horizon, a ladder, and a shape

The plan has three dimensions the head defends explicitly.

**Horizon.** Three years is the practical planning horizon for
most enterprises. One year is the annual budget window; three
years is long enough to see the shape of the function converge
against the maturity trajectory
([[mod-107-program-measurement-and-maturity]] chapter 03) and the
regulatory horizon ([[mod-105-regulatory-change-management]]
chapter 01). Five-year plans read as speculative to the CFO;
one-year plans read as absent forward planning to the audit
committee. Three years is what the head presents, with year-one
detail sufficient for budget commitment and year-two and year-
three trajectory sufficient for planning alignment.

**Ladder.** The plan names headcount by level — how many level-15
analysts, how many level-25 engineers, how many level-35
evaluators, how many level-50 architects (usually one at a small
enterprise, two-to-three at a large enterprise, more if the
function is federated by risk domain per chapter
[[01-function-org-shape-and-reporting-lines]] Shape C). The
ladder distribution matters — a function that is 80% level-15
analyst headcount is a function that will run the intake queue
but will not have the technical depth to run adversarial testing
or write methodology; a function that is 50% level-50 architects
is a function that has authorship capacity but no operational
throughput.

**Shape.** The plan aligns with the shape decision from chapter
[[01-function-org-shape-and-reporting-lines]]. A hub-and-spoke
plan (Shape B) explicitly names which analysts are centralised
and which are embedded, per product line. A federated plan
(Shape C) explicitly names headcount per risk domain. The plan
is legible against the org chart; a plan that adds headcount
without saying where the headcount sits in the shape is a plan
the CRO's coordinator will bounce.

## The year-one headcount ladder — the base-case shape

For a first-year AI-governance function at a mid-to-large
enterprise (a few hundred AI systems in the inventory, one to a
few sector overlays, EU AI Act deployer scope with US federal
exposure), the base-case year-one shape is small. The head builds
first for *credibility with the CRO and the audit committee* and
second for *throughput on the intake queue and the control
library*. A function that hires ten analysts before it has an
architect is a function that runs volume without judgment.

The base-case year-one shape:

- **One head** (level 60) — the reader.
- **One senior AI governance architect** (level 50) — hired
  first, or hired as the first hire the head makes on arrival. The
  architect is the design authority the head consumes from; without
  the architect, the head is doing level-50 work at level-60 pay
  and the program has no design authority underneath.
- **One AI evaluation engineer** (level 35) — the release-
  assurance methodology owner. First-year priority is authoring
  the enterprise's release-assurance methodology (in coordination
  with the architect) so the AIA turnaround time metric
  ([[mod-107-program-measurement-and-maturity]] chapter 01 metric
  6) is defensible from the first quarterly report.
- **One or two AI risk engineers** (level 25) — the technical
  challenge capacity. First-year priority is one systematic red-
  team pass across the highest-tier AI systems in the enterprise
  inventory ([[mod-102-running-the-program]] chapter 06) and the
  authoring of the adversarial-testing methodology the evaluation
  engineer will roll into release assurance.
- **Two to four AI governance analysts** (level 15) — the
  operational load-bearer. First-year priority is running the
  intake queue, running the first cycle of impact assessments
  against the ISO/IEC 42005 shape
  ([[mod-102-running-the-program]] chapter 06 adjacent), and
  building the evidence-collection pipeline that feeds the KRI
  portfolio ([[mod-107-program-measurement-and-maturity]]
  chapter 01).

Total year-one: six to nine standing FTEs plus the head. Enterprises
with heavier sector overlays (banking with SR 11-7 model-risk-
management adjacency, medical device with FDA GMLP scope) add a
sector-specific level-35 evaluator; enterprises with material
frontier-agent surface add a level-40 agentic safety engineer
(per [[mod-101-role-scope-and-leadership-shape]] chapter 01).
Enterprises at Shape D (matrixed-from-source) run smaller
standing headcount and higher matrix loading against the same
delivered scope, with the trade-offs chapter
[[01-function-org-shape-and-reporting-lines]] surfaces.

## The year-two and year-three trajectory

Year two typically deepens the level-25 and level-35 bench and
adds embedded analysts (if the head moved to Shape B in year
one and the embed pattern has proved out). Year three typically
adds a second level-50 architect (if the enterprise is federating
by domain) or an additional level-35 evaluator (if the enterprise
is deepening within domains).

The head does not present the year-two and year-three trajectory
as a straight-line expansion. The trajectory is *contingent* on
signals the plan names explicitly:

- **AI portfolio growth signal.** If the AI system inventory
  grows past N systems (the specific number depends on the
  enterprise's operating model), the analyst headcount must grow
  proportionally, or the AIA turnaround metric will slip. The
  head names the trigger in the plan so the budget conversation
  does not have to be reopened when the trigger fires.
- **Regulatory obligation signal.** If a specific regulation
  moves from horizon-scanned to in-force (EU AI Act Article 55
  GPAI obligations at a specific date; a new state DOI AI-model
  bulletin adoption; an OMB M-25-21 requirement change), the
  headcount plan names which role would be added on the trigger.
- **Third-line audit engagement signal.** If the CAE's audit plan
  puts a material AI-governance engagement on the calendar (chapter
  [[05-cae-and-third-line-coordination]]), the head names the
  analyst or evaluator headcount that would be added to support
  the engagement without pulling load off standing operations.
- **Incident-load signal.** If AI incident volume (chapter
  [[mod-110-incident-leadership]]) rises above the base rate
  the program was staffed against, the head names the risk-
  engineer headcount that would be added to absorb the
  investigation load.

The trigger-contingent plan is more defensible than a straight-
line plan. The CFO reads it as a head who is planning for the
enterprise's actual growth shape rather than for the head's
preferred expansion trajectory.

## Sourcing strategy — the two candidate populations

The head does not source from one population. The AI-governance
function's talent supply is genuinely two populations, and the
head runs distinct sourcing strategies against each.

### Population A — career switchers from adjacent second-line disciplines

The larger of the two populations. These are experienced
practitioners in adjacent disciplines who bring transferable
depth into AI-governance roles.

- **Internal audit.** IIA-credentialed auditors (CIA), COSO/ERM
  practitioners, IT auditors (CISA). Bring: independence
  discipline, evidence discipline, three-lines fluency, audit-
  committee-facing craft. Need to learn: AI system technical
  literacy, model-risk vocabulary, AI-specific control taxonomies.
- **Privacy.** IAPP-credentialed privacy professionals (CIPP,
  CIPM, CIPT), data protection officers, GDPR / CCPA / PIPEDA
  practitioners. Bring: regulatory-obligation fluency, DPIA
  authoring, regulator-engagement muscle memory, evidence and
  disclosure discipline. Need to learn: AI-specific risk
  categories beyond privacy, model-testing methodology, AI supply-
  chain evidence shapes.
- **Model-risk management (banking).** SR 11-7 / OCC 2011-12 /
  OSFI E-23 practitioners, quantitative validators, model risk
  officers. Bring: model-lifecycle discipline, effective-
  challenge muscle, quantitative fluency, regulator-engagement
  experience. Need to learn: AI-specific risk categories beyond
  traditional model risk (fairness, safety, alignment), the
  broader AI regulatory landscape beyond SR 11-7.
- **Legal (regulatory technology, AI/data).** Regulatory counsel,
  privacy counsel, technology transactions counsel with AI
  exposure. Bring: regulatory interpretation craft, regulator-
  engagement fluency, contract craft for AI supply chain. Need
  to learn: hands-on technical evaluation methodology, the
  separation between legal opinion and governance advice
  ([[mod-104-regulator-engagement]] chapter 07). Legal-source
  hires often land as architects or as heads themselves rather
  than at analyst or engineer levels.
- **Product and engineering (with governance interest).** Senior
  ML engineers, MLOps leads, product managers who have
  encountered AI risk in-role. Bring: technical AI literacy,
  first-line credibility, systems fluency. Need to learn: second-
  line-independence discipline (the challenge is *not*
  contributing to the product), audit-committee-facing craft, the
  regulatory-obligation vocabulary. Product- and engineering-
  source hires are the most valuable *when* they successfully
  make the second-line transition and the most costly *when* they
  do not.

For each source discipline, the head names in the sourcing
strategy: which levels the source is a natural match for (a
CIA-credentialed auditor typically enters at level 25 or 35;
an SR 11-7 model validator typically enters at level 35 or 50;
a privacy counsel with a decade of DPO experience typically
enters at level 50 or as head-in-waiting), what the specific
onboarding investment is for the switch, and what the retention
risk is (a career switcher who does not feel their prior
expertise is being used loses interest inside two years).

### Population B — early-career practitioners from AI-governance credential cohorts

The smaller but faster-growing population. These are
practitioners with focused AI-governance credentials from
programs that are new but are gaining traction with employers.

- **IAPP AIGP (Artificial Intelligence Governance Professional).**
  Certification launched by IAPP in 2024; the body of knowledge
  covers foundations of AI, AI impacts and responsible AI
  principles, AI development lifecycle, and AI governance and
  risk management. AIGP-credentialed candidates typically enter
  at level 15 or level 25 with some prior professional
  experience.
- **ISO/IEC 42001 Lead Implementer / Lead Auditor cohorts.**
  Certification programs offered by accredited training
  providers (BSI, PECB, LRQA and others) around the ISO/IEC
  42001 AI management system standard. Lead Implementer cohorts
  are typically strong for architect-track hires; Lead Auditor
  cohorts are strong for evaluation-engineer-track hires and for
  candidates who will interface with certification-body audits.
- **BABL AI training programs.** Practitioner and auditor
  programs from BABL AI focused on AI audit and impact
  assessment craft.
- **ForHumanity certifications.** ForHumanity Fellows program and
  independent auditor accreditations against the ForHumanity
  Independent Audit of AI Systems (IAAIS) criteria. ForHumanity-
  credentialed candidates are strong for third-party-audit and
  assurance-facing roles.
- **NIST AI RMF training** through NIST-recognised providers, and
  **Responsible AI Institute** cohorts and certifications.
- **University AI-governance programs.** A small but growing
  number of universities offer graduate certificates or
  concentrations in AI policy / AI governance / AI ethics; hires
  from these programs typically enter at level 15 with strong
  regulatory-literacy but less operational muscle.

<!-- needs-research: verify current cohort volume, tuition ranges,
and employer-recognition levels for each named credential program
against each program's own published statistics. Numbers move
year over year and should not be quoted from memory. -->

For each credential source, the head names the entry level, the
onboarding rotation the hire runs before productive delivery
(chapter [[03-coaching-and-career-pathing]] runs the rotation),
and the retention consideration (early-career hires expect a
clear progression path; a hire from an AIGP cohort at level 15
without a visible path to level 25 will move to a competitor
inside eighteen months).

### Sourcing channels beyond credentials

Beyond credentialed populations, the head runs the practical
sourcing channels: internal transfers (from audit, privacy, MRM,
legal, product, engineering — often the strongest early hires),
external recruiters specialising in privacy / compliance / risk
placements who have expanded into AI-governance, professional-
society talent boards (IAPP AI governance job board, ACM SIGAI,
IEEE Ethics in Action, Partnership on AI job board where
present), conference-driven sourcing (IAPP AI Governance Global,
NeurIPS ML Safety workshops, AAAI/ACM AIES, USENIX AI Village,
sector conferences), and inbound applications to a well-
positioned function.

The head does not rely on one channel. A function whose talent
pipeline is 90% one external recruiter is a function whose
pipeline collapses if the recruiter leaves the firm or drops
the account.

## The interview loop — a repeatable shape per role

The interview loop is designed *once* per role level and run
repeatedly. Ad hoc interview loops produce ad hoc hiring
decisions, and ad hoc hiring decisions are the source of the
regretted hires the head has to manage out inside eighteen
months (chapter [[07-difficult-people-leadership-conversations]]).

Each loop has a fixed shape.

### Level-15 analyst loop

Approximately five stages, four to six weeks end-to-end.

1. **Recruiter screen.** Basic fit, motivation, compensation
   expectations, work-authorisation, availability. Recruiter-
   sourced; a first pass before the head's or team's time.
2. **Hiring-manager screen** (30–45 minutes with the head or a
   level-35 evaluator). Motivation for AI-governance work
   specifically, prior evidence of second-line discipline (in
   an adjacent role or in academic work), one working-through
   of an intake-queue scenario.
3. **Technical assessment.** A time-boxed take-home or a
   working session — a written scenario in which the candidate
   is given a redacted AI system description and asked to draft
   the first-cut impact-assessment shape. Assessed against a
   rubric with the level-35 evaluator.
4. **Panel loop** (two to three panels, 30–45 minutes each).
   Panelists: one level-25 or level-35 team member on technical
   craft; one adjacent-function partner (from audit, privacy, or
   MRM) on cross-function collaboration; one product or
   engineering partner on first-line-facing craft. Each panelist
   assesses against a written rubric.
5. **Head interview** (30–45 minutes with the head). Culture-
   add, values alignment, career-trajectory conversation. The
   head does not use this interview to re-run the technical
   assessment; the head is looking for whether the candidate is
   someone the head can develop.

Debrief and decision within one week of the last interview.
Written debrief per interviewer against the rubric; head
decides with input from the panel; hiring loop closes with a
written decision minute.

### Level-25 engineer / level-35 evaluator loop

Approximately six stages, six to eight weeks end-to-end. Adds a
deep-technical panel on the specific craft (red-team, fairness,
adversarial-ML, evaluation methodology) and a working-session
component in which the candidate walks through prior work on the
craft (with appropriate confidentiality controls) with two
technical panelists.

### Level-50 architect loop

Approximately seven stages, eight to ten weeks end-to-end. Adds
a design-authorship exercise (the candidate authors a short
proposed extension to the enterprise's control library against a
provided scenario), a CxO panel (the CRO, the General Counsel,
and often the CAIO participate in a joint 45-minute conversation
with the candidate to assess the candidate's ability to hold
their own at CxO scope), and a formal reference-check protocol
(three references, structured questions, minuted).

### Level-60 head loop

Runs at the CRO or CEO scope, not at the head's scope. The
head-in-post participates in the loop for their own successor
only where the succession picture is a genuine planned handover
(chapter [[01-function-org-shape-and-reporting-lines]]
succession discipline); more commonly the head-in-post authors
the succession one-pager the CRO or CEO takes into the loop.

## The sign-off flow — who has to say yes

The interview loop produces a recommendation; the sign-off flow
turns the recommendation into an offer. Sign-off is *not*
automatic on interview panel consensus; sign-off is a specific
authorisation step per level.

- **Level-15 analyst.** Head signs off after loop debrief.
  Recruiter processes the offer.
- **Level-25 engineer / level-35 evaluator.** Head signs off
  after loop debrief; CRO's second-line coordinator is
  notified for information (not authorisation) unless the offer
  is materially outside band (see compensation-band positioning
  below).
- **Level-50 architect.** Head signs off with CRO ratification
  (formal, in writing). The CRO's ratification is on the
  candidate specifically, not on the requisition; a candidate
  the head recommends who the CRO would not ratify is a hire
  the head does not extend.
- **Level-60 head successor.** CRO signs off (or CEO, depending
  on reporting shape) with audit-committee-chair notification
  and, in some regulated sectors, regulator no-objection where
  the head-of-second-line role is a fit-and-proper regulated
  position.

Sign-off failures — an offer extended without the CRO ratification
step, an offer extended before reference checks close, an offer
extended with a compensation package outside the band without
compensation-committee sign-off — are exactly the kinds of
process failures that show up in the third-line audit engagement
as findings. The head runs the sign-off flow *exactly* as
authored; the flow is not a suggestion.

## Compensation-band positioning

The head does not run compensation as a per-offer negotiation.
The head runs compensation as a *positioning* discipline against
market benchmark, refreshed annually, ratified by the compensation
committee (via HR) as the standing framework for the function.

Three positioning postures the head chooses among.

**At-market.** The function pays at the market median for each
level, as measured against a peer-set the compensation function
maintains. Predictable, defensible, and low-risk on retention if
the peer-set is well-chosen. This is the default posture for
most functions. Risk: the head may lose offers to firms
positioned above market.

**Above-market at senior levels, at-market at junior levels.**
The function pays at the 60th–75th market percentile for level-50
and level-60 (where the talent pool is genuinely thin and the
cost of a mis-hire is highest), and at the median for level-15
and level-25 (where the pool is deeper). Common in enterprises
that have made the case to the compensation committee that
level-50 architect talent is a strategic capacity investment.
Risk: the wedge between senior and junior bands creates
progression-conversation friction (a level-25 engineer who is
strong will notice the wedge and either negotiate up or leave
for a firm at the head's peer-set that pays their level above
market).

**Above-market across the ladder.** The function pays at the
75th–90th percentile across all levels. Uncommon; typically
justified only at frontier labs, in enterprises where AI-
governance credibility is a first-order strategic differentiator,
or in enterprises with severe adverse-selection risk on second-
line hires (the enterprise's reputation makes it hard to
recruit unless it pays a premium). Risk: unsustainable if the
enterprise's compensation posture more broadly is at-market —
the AI-governance function becomes a compensation outlier that
attracts internal attention.

The head runs one posture, ratifies it with the compensation
function and the CRO annually, and defends it on data (the
peer-set benchmark refreshed annually, the offer-acceptance and
offer-decline data from the prior year, the regretted-loss data
for departures). The head does not defend the posture on
narrative ("AI-governance talent is scarce") — the compensation
committee has heard every function argue that every function's
talent is scarce.

### The compensation-band definition

For each level, the head with HR authors a band with:

- **Base salary range.** Minimum, midpoint, maximum per level.
- **Variable / bonus target.** As a percent of base, aligned with
  the enterprise's variable-compensation framework for the
  function's family.
- **Equity range** (where applicable). As appropriate to level and
  enterprise practice.
- **Total compensation range.** The composite the recruiter uses
  in the offer conversation.
- **Positioning-posture reference.** Where the band sits against
  the peer-set benchmark (median, 60th-75th, 75th-90th) with the
  peer-set named.
- **Locality adjustments.** Where the enterprise operates in
  multiple geographies with distinct compensation markets.

The band is the recruiter's authority. A recruiter who is
authorised to extend within-band offers without further sign-off
runs the offer conversation fluidly; a recruiter who has to
escalate every offer inside band is a recruiter running against
a compensation framework that does not exist yet, and the head
fixes the framework before running the next requisition.

Outside-band offers require a specific sign-off — the head plus
the compensation function, with the CRO informed and (for level-
50 and above) the compensation committee informed at the
next scheduled cycle. Outside-band offers are exceptions, and the
exception rate is a signal — if the head extends outside-band
offers more than occasionally, the band itself is likely
mis-positioned and the head takes it back to the compensation
committee for re-baselining rather than continuing the exception
pattern.

## Anti-patterns the head does not permit

**The reactive-hiring posture.** The head opens requisitions when
the current headcount is already burning out. The result is
requisitions that close months late, hires who join a team in
crisis, and a compounding retention problem. The remedy is the
multi-year plan with trigger-contingent expansion — headcount
opens on the trigger, not on the crisis.

**The single-population sourcing pattern.** The head sources
exclusively from career switchers, or exclusively from credential
cohorts, or exclusively from internal transfers. The pipeline is
thinner than it needs to be and the function's cognitive
diversity is limited. The remedy is the two-population strategy
above, run in parallel with named channels per population.

**The ad hoc interview loop.** The head runs different interview
shapes per candidate because the head is busy or because different
panelists are available. The variance in interview shape produces
variance in signal quality, and the loop cannot be calibrated
across candidates. The remedy is the fixed loop per level, with
written rubrics per stage.

**The premature architect hire.** The head hires a level-50
architect who has design authority but no operational discipline,
because the architect was available and the requisition was open.
Six months in, the head discovers the architect is running the
control library as their personal design project rather than as
an operating asset the function consumes and defends. The remedy
is the design-authorship exercise in the loop (a genuine design
challenge the candidate works through, assessed on both craft and
operability) and the CRO ratification on the specific candidate.

**The comp-band-negotiation-per-offer pattern.** The head lets
recruiters go to the head for every offer because the head has
not authored the band. Offers stretch out, candidates decline,
and the pattern surfaces as slow-hiring in the annual metric
review. The remedy is the annually-ratified band with
recruiter-authority for within-band offers.

**The "we hired a great analyst but they got no onboarding"
pattern.** The head closes requisitions but does not stand up
the onboarding rotation from chapter
[[03-coaching-and-career-pathing]]. New hires spend their first
three months figuring out the function's shape and its systems
by themselves, and either burn out or leave. The remedy is
that the interview loop and the onboarding rotation are
authored together — a requisition does not open until the
onboarding rotation is documented.

## Composition with adjacent modules

- **The function shape** in
  [[01-function-org-shape-and-reporting-lines]] is the input to
  the plan; the plan builds headcount against the shape.
- **The coaching cadence** in
  [[03-coaching-and-career-pathing]] is what turns hires into
  productive team members; the onboarding rotation is authored
  together with the interview loop.
- **The budget cycle** in
  [[mod-113-budget-vendor-p-and-l-and-investment-case]] is
  where year-one headcount authorisation happens; the multi-
  year plan is the head's negotiating instrument in that cycle.
- **The regulatory-change register** in
  [[mod-105-regulatory-change-management]] chapter 01 provides
  the trigger inputs for the year-two and year-three trigger-
  contingent trajectory.
- **The AIA turnaround, evidence-completeness, and MTTR metrics**
  in [[mod-107-program-measurement-and-maturity]] chapter 01
  are the load metrics the plan is calibrated to.
- **The IIA Three Lines Model** at leadership scope in
  [[mod-101-role-scope-and-leadership-shape]] chapter 04 sets
  the second-line-independence discipline the sourcing strategy
  respects, particularly for product- and engineering-source
  hires who have to make the second-line transition.
- **The cross-functional coordination discipline** in
  [[mod-109-cross-enterprise-leadership]] is where the head's
  own relationships with the CRO, CAE, and CAIO — the sign-
  off, ratification, and CxO-panel partners in this chapter —
  live at cadence.

## Summary

- The multi-year hiring plan has three dimensions: horizon
  (three years — one year detailed, two-and-three trajectory),
  ladder (headcount by level, distributed to match the shape's
  work), and shape (aligned with the function shape from
  chapter [[01-function-org-shape-and-reporting-lines]]).
- The base-case year-one function is small — one head, one
  level-50 architect, one level-35 evaluator, one to two
  level-25 engineers, two to four level-15 analysts, plus
  sector-specific additions. The plan builds credibility and
  judgment before it builds volume.
- Year two and year three are trigger-contingent — expansion
  fires on named signals (AI portfolio growth, regulatory
  obligation change, third-line audit engagement, incident
  load) rather than on straight-line assumption.
- Sourcing runs against two candidate populations — career
  switchers from adjacent second-line disciplines (audit,
  privacy, MRM, legal, product/engineering) and early-career
  practitioners from AI-governance credential cohorts (IAPP
  AIGP, ISO/IEC 42001 LI/LA, BABL AI, ForHumanity, NIST AI RMF
  training, university programs) — with distinct sourcing
  channels and distinct onboarding needs per population.
- The interview loop is designed once per role level and run
  repeatedly, with a fixed stage sequence, written rubrics per
  stage, and a debrief-with-decision cadence.
- The sign-off flow is per-level, in writing: analyst-through-
  evaluator by the head, architect by the head with CRO
  ratification, head-successor by the CRO or CEO with audit-
  committee notification and (in some sectors) regulator no-
  objection.
- Compensation is a positioning discipline — one posture (at-
  market, above at senior, above across), ratified annually,
  with bands per level (base, variable, equity, total, locality)
  and recruiter-authority for within-band offers.
- Five anti-patterns the head refuses: reactive hiring, single-
  population sourcing, ad hoc interview loop, premature
  architect hire, comp-band-negotiation-per-offer; plus the
  "no onboarding" pattern the coaching-cadence chapter
  addresses.
- Chapter [[03-coaching-and-career-pathing]] runs the onboarding
  and career-pathing cadence against the hires this plan
  produces; chapter [[04-second-line-independence-balance]]
  runs the independence discipline that shapes what "productive"
  looks like for hires from first-line adjacent sources; chapter
  [[05-cae-and-third-line-coordination]] carries the
  ratification-and-audit-readiness discipline that the sign-off
  flow reads against.
