# Calibration from Public Incident Data

## Motivation

The head of AI governance closes this module with an
incident-readiness stack that looks, on paper, complete. The
eight AI-specific incident classes from
[[01-incident-command-shape-at-leadership-scope]] cover the
substantive failure surface at leadership scope. The
cross-function coordination discipline from
[[02-cross-function-incident-coordination]] gives the head one
bridge, seven pens, and seven pre-negotiated coordination
surfaces to invoke under time pressure. The Article 73
execution runbook from
[[03-article-73-filing-at-incident-time]] and the US
serious-incident disclosure map from
[[04-us-serious-incident-disclosure-map]] give the head a
filing posture against every material regime. The
post-incident learning cycle from
[[05-post-incident-learning-cycle-sponsorship]] gives the head
a sponsorship discipline that turns each incident into risk
register, control library, and policy delta. The difficult
incident conversations from
[[06-difficult-incident-conversations]] give the head the
scripts for the briefings that step out of the bridge.

The stack is only as calibrated as the head's view of what
actually happens in the field. Every element of it — the eight
classes, the disclosure map, the tabletop scenarios rehearsed
with the delegate, the rehearsal briefings — encodes an
implicit answer to the question "what does an AI incident look
like at an enterprise like ours". If the head's answer to that
question is drawn only from the enterprise's own risk register,
its own incident log, and its own near-miss experience, the
answer is a small sample from a distribution the head has not
actually observed. The stack that sits on top of the small
sample will look complete right up to the moment an incident
lands that the sample did not carry — at which point the head
is at the audit committee explaining why a class of failure
that has been happening publicly for years was not on the
enterprise's tabletop.

The failure mode is specific and worth naming concretely. An
enterprise operating a hiring-AI product line has a head whose
own risk register carries systemic bias event (class 2 from
chapter 01) as a residual-scored, adequately-controlled risk.
The head has not read the years of publicly documented
disparate-impact incidents in hiring AI that the AI Incident
Database and adjacent public sources carry. The enterprise's
own tabletop scenarios for class 2 are drawn from the head's
internal understanding of the enterprise's own system, not
from the peer-benchmark pattern of what has actually gone
wrong at other hiring-AI enterprises — the class of feature
that surfaced the bias, the length of time between the bias
starting and being detected, the regulator that opened the
inquiry, the specific redress instrument the peer offered, the
specific documentation the peer wished the peer had authored
before the regulator asked for it. When the enterprise's own
systemic-bias incident materialises — as it does — the head
walks into the regulator conversation carrying an internal
account that ignores every peer-response signal that had been
publicly available. The regulator has read the same public
sources the head has not, notices the omission, and reads the
head as under-prepared. The head's credibility with that
regulator does not recover on the strength of the current
incident's response alone. The head lost credibility before
the incident opened, by not having done the peer-benchmarking
that the regulator assumes the head has done.

Public incident data is where the head defends against this
failure. It is not a compliance exercise; it is a discipline
of calibration that keeps every other element of the stack
honest. This chapter is the discipline. Section by section it
walks the three primary public sources (the AI Incident
Database, the OECD.AI incidents monitor, the MIT AI Risk
Repository), two additional lower-cadence sources (MITRE
ATLAS case studies, regulator enforcement actions), the
annual calibration exercise the head runs against all of
them, the near-miss discipline that supplies the
enterprise's own ground-truth alongside the peer benchmark,
and the peer-benchmarking discipline that composes both into
the head's external-positioning posture.

## Core concept — public incidents are peer-benchmark, not probability distribution

The load-bearing conceptual move in this chapter is a
distinction the head has to hold cleanly and that is easy to
lose under the pressure of quantitative expectation. Public
incident data is a **peer benchmark**. It is not a **probability
distribution** for the head's own enterprise.

The distinction matters because the two readings produce
different products. A head who reads public incident data as a
probability distribution ends up trying to compute the annual
likelihood that the enterprise itself will suffer a class-3
prompt-injection incident, or a class-5 jailbreak-driven harm
event, or a class-8 evaluator-corruption event, on the basis
of the frequency with which those classes appear in the public
catalogue. The computation is illegitimate for reasons the
head names for the room whenever the question arises:

- The public catalogue has systematic reporting bias. Incidents
  that produce public harm and public disclosure are
  over-represented; incidents that were contained privately and
  never disclosed are under-represented. The base rate the
  catalogue reveals is a lower bound on the true incidence, not
  an estimate of it.
- The catalogue is a mixed population. Frontier-developer
  incidents, deployer incidents, consumer-application incidents,
  and public-sector deployment incidents all appear in the same
  register with different underlying rates and different
  applicability to any specific enterprise.
- The enterprise's own posture is not the catalogue's average
  posture. The catalogue's implicit denominator — how many
  enterprises are operating an equivalently exposed system —
  is not observed. The head's enterprise carries its own
  control stack, its own maturity level, its own vendor mix,
  and its own risk register, none of which the catalogue's
  peer-average captures.
- The near-miss population — events that could have been
  incidents and were not, either because a control caught them
  or because the vulnerable population did not materialise — is
  systematically absent from the public catalogue. A rate
  computed against public incidents alone treats the enterprise
  as though it had no controls, which is not the fact pattern
  the head is trying to model.

The head who tries to compute a Bayesian prior against the
public catalogue ends up either dramatically over-scoring the
residual risk (because the catalogue over-samples visible
harm) or dramatically under-scoring it (because the catalogue
misses the enterprise's own novel exposure). The audit
committee that receives such a computation reads it as
false-precision quantification, which is worse than no
quantification. The regulator that receives it reads it the
same way. The class of computation is the wrong output from
the discipline.

The right output is different. The head reads public incident
data with the same craft the head reads regulator enforcement
actions from [[mod-104-regulator-engagement]] — as case
material for a rehearsed response, not as an input to a rate
calculation. For every public incident the head walks, the
head produces four outputs:

- **What happened.** The head reconstructs the incident to a
  fidelity sufficient to reason about it — the AI system
  involved, the class of failure per the taxonomy from
  [[01-incident-command-shape-at-leadership-scope]], the
  contributing conditions, the harm produced.
- **What class of failure it was.** The head names the class
  or the combination of classes from the eight-class taxonomy.
  If the incident does not fit the taxonomy, the head names
  the gap; the gap is itself a calibration output.
- **What the peer's response was.** The head reads the public
  record for the peer enterprise's containment, disclosure,
  regulator interaction, remediation, and (where public)
  post-incident learning. The head names whether the peer got
  the response right or wrong.
- **What the enterprise would have done differently.** The
  head walks the incident against the enterprise's own
  runbooks — the eight-class taxonomy, the disclosure map,
  the coordination surfaces, the RCA sponsorship discipline —
  and names the specific move the enterprise would have made
  differently, or the specific gap in the enterprise's own
  posture the incident reveals.

The output of the four is not a probability; it is a rehearsed
response the head now has that the head did not have before
reading the incident. Public data feeds calibration; it does
not feed enterprise risk scoring. The head defends the
distinction whenever a peer function or a board member asks
for the illegitimate computation, and names the legitimate
output instead.

## The three primary sources

Three public sources sit at the centre of the head's
calibration discipline. Each has a distinct structure, a
distinct calibration signal, and a distinct reading cadence.
The head consumes each on its own cadence, and the outputs
compose into the annual calibration exercise the section below
frames.

### AI Incident Database (incidentdatabase.ai)

The AI Incident Database — usually referred to as the AIID —
is the crowdsourced catalogue of AI incidents originally
sponsored by the Partnership on AI and maintained as a public
open-source register.
<!-- needs-research: verify current custodianship of the AIID
(originally under Partnership on AI, may have changed hands
or moved to an independent stewardship model), verify the
current URL structure and record schema -->
The catalogue's structure carries an incident record for each
reported event, with a narrative description, source
citations (news articles, academic papers, regulator filings,
public disclosures), taxonomy annotations contributed by the
catalogue's editorial community, and cross-references to
related incidents. The catalogue is search-able by AI system,
by developer, by deployer, by harm type, and by contributor
taxonomy.

What the head reads the AIID for is three signals.

The **pattern-of-failure surface** signal is the primary one.
For each of the eight incident classes from
[[01-incident-command-shape-at-leadership-scope]], the AIID
carries a corpus of publicly reported cases that describe how
the class has materialised at peer enterprises. The head reads
the corpus not for individual case detail but for the
distribution — how many cases fit each class, which
sub-patterns within each class recur, which sub-patterns
appear once and have not repeated, which classes carry a long
tail of ongoing cases and which classes have plateaued. The
distribution signal is what the head uses to prioritise
tabletop-scenario coverage. If the AIID's class-2 (systemic
bias) corpus for hiring-AI systems shows a sub-pattern
(specific feature category, specific detection lag, specific
regulator response) recurring across multiple public cases,
that sub-pattern belongs on the enterprise's tabletop
whether or not the enterprise's own risk register has surfaced
it yet.

The **regulator-response signal** is the second. Where a
public incident triggered a regulator engagement — an
enforcement action, a consent decree, a public settlement, a
sector-supervisor inquiry, an anti-discrimination-regulator
investigation — the AIID's source citations typically link to
the regulator's own published output. The head reads the
regulator's output against the head's own disclosure map from
[[04-us-serious-incident-disclosure-map]]. Where a regulator
has treated a class of incident as within a specific
disclosure obligation the head's own map already carries, the
public case is confirming calibration; the head's map is
correctly reading the regulator. Where a regulator has
treated a class of incident as within a disclosure obligation
the head's map did not carry — a novel interpretation, a
sector-specific extension, an emerging enforcement priority
— the public case is signalling that the head's map needs an
update.

The **peer-response signal** is the third. For each public
incident the head reads what the peer enterprise did — how it
communicated, whether it contained the incident quickly or
let it run, whether it filed promptly or was seen to file
late, whether the redress instrument it offered was accepted
by affected parties or rejected, whether the sector-share
decision was to contribute the lesson or to hold it. The
peer-response signal is direct calibration for the difficult
conversation rehearsals from
[[06-difficult-incident-conversations]] — the head runs the
rehearsal against the peer's actual case as though the peer
were the enterprise, and the head's response is scored against
what the peer did.

Reading cadence. The head walks the AIID's new incidents
quarterly. The walk does not require reading every record;
the head reads the executive summary of each new record and
reads the full record for any incident that plausibly touches
one of the eight classes the head is calibrating. The head
also does targeted lookups on demand — when a new tabletop
scenario is being designed, when a peer function raises a
question about a specific class of failure, when a regulator
inquiry references a public case the head does not yet
recognise. The quarterly walk is the calibration cadence; the
targeted lookup is the response cadence.

Two anti-patterns the head avoids on the AIID. The first is
reading it as a compliance checklist — walking each record and
asking "did we have this control" as though the AIID were the
enterprise's own audit register. The AIID is not that; it is
calibration material, and reading it as a checklist collapses
the calibration signal into false reassurance ("we have
controls against every public incident, therefore we are safe")
or false alarm ("we do not have controls against every public
incident, therefore we are unsafe"). Neither reading is
correct; both waste the calibration signal. The second is
treating individual AIID records as evidence for a
quantitative rate calculation, which is the illegitimate
computation the core-concept section refused.

### OECD.AI AI Incidents Monitor (oecd.ai/en/incidents)

The OECD.AI AI Incidents Monitor sits inside the OECD.AI
observatory as the OECD's structured surface for AI-related
incidents. The monitor's methodology, taxonomy, and update
cadence sit under the OECD Working Party on AI Governance's
oversight.
<!-- needs-research: verify OECD.AI monitor scope, current
methodology (whether purely news-aggregation-driven or with
editorial curation), taxonomy structure, and update cadence
-->
The monitor's structure differs from the AIID. Where the AIID
is a curated catalogue of individual incident records, the
OECD monitor operates as an aggregation surface across news
reporting worldwide, with the OECD's own taxonomy overlaid to
sort incidents by AI system type, by affected sector, by
geography, by harm type, and by trend.

What the head reads the OECD monitor for is two signals the
AIID does not carry as cleanly.

The **cross-jurisdictional pattern signal** is the primary
one. Because the monitor aggregates across news reporting
worldwide with a common taxonomy overlay, the head sees when
a class of incident is now surfacing in more than one Member
State — the same class of hiring-AI disparate-impact event
reported in three different jurisdictions inside the same
quarter, the same class of generative-AI harm event surfacing
in six sectors across a year. The pattern signal tells the
head that the class is no longer a single-jurisdiction concern
that a peer function might dismiss as jurisdictionally
distant; it is a cross-border pattern that the head's own
multi-jurisdictional disclosure map from
[[04-us-serious-incident-disclosure-map]] and the head's
Article 73 execution discipline from
[[03-article-73-filing-at-incident-time]] both have to be
calibrated against.

The **international regulator-response signal** is the
second. An incident that triggers a regulator response in a
single Member State is calibration for the head's engagement
with that Member State's competent authority. An incident that
triggers responses in multiple Member States, or triggers
attention from an international body — the OECD itself, the
Council of Europe, the G7 Hiroshima AI Process working
groups, UN adjacencies — is calibration for the head's
multi-jurisdictional incident plan. The head reads the
international response for the coordination pattern the peer
had to run (or failed to run), and calibrates the head's own
plan accordingly. Where a peer had to file the same
substantive incident to five national CAs in the EU plus the
AI Office plus two US federal regulators plus one US state
regulator, the head reads that multi-recipient coordination
pattern and asks whether the head's own filing-recipients
register from [[03-article-73-filing-at-incident-time]] could
have handled the same load.

Reading cadence. The head walks the OECD monitor quarterly,
timed to compose with the regulatory-change-management cadence
from [[mod-105-regulatory-change-management]]. The
regulatory-change-management review is where the head sees
what regulators have newly said; the OECD monitor is where
the head sees what regulators have newly done. The two
readings together produce a calibrated view of the current
international regulatory posture that the head carries into
the audit committee and into peer-CxO briefings. Where the
OECD monitor surfaces an incident with a
regulatory-change-management dimension that the head's own
horizon scan had not yet caught, the incident is the trigger
to update the scan.

The monitor's aggregation methodology carries a caveat the
head keeps in view. Because the monitor is news-aggregation-
driven with a taxonomy overlay, it reflects what the news is
reporting, not necessarily what has happened. Slow-burn
incidents that never surface in the news are absent from the
monitor's view even if they appear in the AIID's curated
record. The head reads the OECD monitor alongside the AIID
rather than as a replacement for it.

### MIT AI Risk Repository (airisk.mit.edu)

The MIT AI Risk Repository is the meta-taxonomy of AI risks
compiled by the MIT CSAIL / FutureTech research programme
from the academic literature. Where the AIID and the OECD
monitor are incident registers — records of things that have
happened — the MIT repository is a taxonomy — a structured
enumeration of risk categories, cross-referenced against the
academic papers that describe each.
<!-- needs-research: verify current custodianship of the MIT
AI Risk Repository (MIT CSAIL / FutureTech is the originating
programme; verify current stewardship and any collaboration
partners), verify the current version, the current taxonomy
structure (number of top-level categories, number of leaf
categories), and the current update cadence -->
The repository's structure carries the taxonomy itself, the
academic-source database that populates each taxonomy leaf,
and (typically) a cross-reference to public incidents where
the risk category has materialised in observable form.

What the head reads the MIT repository for is two signals
neither the AIID nor the OECD monitor carries.

The **risk-taxonomy completeness signal** is the primary one.
The head walks the MIT repository's taxonomy against the
enterprise's own AI risk register from
[[mod-102-running-the-program]]. For each leaf category in
the repository the head asks whether the enterprise's own
register carries an equivalent line, whether at a materially
similar residual score or with a materially different one, or
whether the register does not carry an equivalent line at
all. The categories the register does not carry are
completeness gaps — classes of risk the academic literature
is describing that the enterprise's own risk framing has not
absorbed. Not every gap requires a register update; some
categories are genuinely inapplicable to the enterprise's own
AI portfolio (a category framed for frontier-model
capabilities the enterprise does not train, a category framed
for autonomous-weapons deployments the enterprise does not
build). But every gap the head identifies is a decision the
head makes explicitly — "this category does not apply because"
— and the decision is documented, so that when a future review
asks whether the register was calibrated against the current
taxonomy, the head has an answer.

The **emerging-class signal** is the second. The MIT repository
is populated from the academic literature, which typically
runs eighteen to thirty-six months ahead of public incidents
and further ahead of regulator response. A category that has
appeared in the repository but has not yet materialised in
public incidents is a leading indicator — a class of risk the
academic literature is now describing that the enterprise
should consider before the incidents start appearing publicly.
The head reads emerging categories for the ones with plausible
applicability to the enterprise's own portfolio, and
commissions the level-50 senior AI governance architect to
draft a preliminary risk-register entry — even if the entry's
initial residual score is low — so that the register carries
the category before an incident forces it.

Reading cadence. The head walks the MIT repository annually,
as an input to the enterprise's own risk-register annual
review. The annual cadence reflects the repository's own
update rhythm (taxonomy revisions happen on a slower cadence
than incident aggregation) and the enterprise's own
risk-register review cycle (annual major review with
incident-driven interim updates). The annual walk is a
dedicated block on the head's calendar, typically two to
three working days, in which the head and the senior
architect walk the taxonomy leaf by leaf and produce a
completeness delta the register review then absorbs.

Two anti-patterns the head avoids on the MIT repository. The
first is treating the repository as the enterprise's own risk
taxonomy — importing the repository's leaf structure directly
into the register. The repository is a meta-taxonomy for the
whole field; the enterprise's register is a taxonomy for the
enterprise's own portfolio. The two do not have the same shape
and should not. The head uses the repository to check the
register for completeness, not to replace it. The second is
treating an emerging category the repository names as
automatically requiring a register entry. The head reads each
emerging category against the enterprise's own applicability
threshold and adds only the categories that are plausibly in
scope. Adding every emerging category collapses the register's
signal-to-noise.

## Two additional sources at lower cadence

Beyond the three primary sources, two additional public
surfaces sit on the head's calibration reading list at lower
cadence. Neither is a substitute for the three above; each
supplies a specific calibration signal the three do not.

### MITRE ATLAS Case Studies

MITRE ATLAS is the adversarial threat landscape for AI
systems — the security-side taxonomy of attack techniques
against AI, structured analogously to MITRE ATT&CK for
enterprise IT. Alongside the technique taxonomy, ATLAS
publishes case studies of real AI attacks, each mapped to the
ATLAS technique(s) it exercised.
<!-- needs-research: verify current ATLAS case-study
publication cadence, current case-study count, and current
technique-taxonomy version -->

What the head reads ATLAS case studies for is
**security-flavoured incident calibration**. Where the AIID
and the OECD monitor carry the general AI-incident surface,
ATLAS case studies concentrate on the security dimension —
prompt-injection attacks, model-extraction attacks,
adversarial-example attacks, training-data poisoning
attacks, membership-inference attacks. The head reads ATLAS
case studies not primarily for the head's own preparation but
for the head's coordination with the CISO from
[[mod-109-cross-enterprise-leadership]] chapter 01. The CISO's
detection engineering, red-team programme, and threat-intel
function all consume ATLAS material as first-order input; the
head reads it to be calibrated for the joint conversations
that follow. Where an ATLAS case study surfaces a technique
the CISO's stack does not yet detect, or a technique for
which the CISO's detection is calibrated against a different
threat model than the AI-substantive one the head carries,
the case study is the material for the next joint
conversation between the head and the CISO.

Reading cadence. The head reads ATLAS case studies on
release — the case-study publication cadence is the reading
cadence. Where a case study has an incident class that
touches the enterprise's own portfolio, the case study is a
targeted input to the head's next coordination cadence with
the CISO's team. The head does not batch ATLAS case studies
into the quarterly walk of the AIID and the OECD monitor;
security-dimension calibration benefits from tighter cadence
than the other calibration reads.

### Regulator enforcement actions and public settlements

For the disclosure-map calibration specifically, the head
reads published regulator enforcement actions and public
settlements as a distinct source separate from the AIID's
regulator-response signal. Where the AIID cites regulator
actions as an incident's downstream consequence, published
enforcement actions are the primary record — the regulator's
own account of what the enterprise did wrong, what the
regulator required, what the settlement carried, and what
the ongoing obligation is.

The specific sources the head reads:

- **US state attorney general settlements** with an AI
  dimension. Where a state AG has settled a matter with an
  enterprise for conduct involving an AI system, the
  settlement documents (typically published on the state AG's
  website and often summarised in enforcement bulletins)
  carry the regulator's specific characterisation of the
  conduct and the specific remedy required. The head reads
  these for the state-AG-specific enforcement lens on AI
  incidents.
- **EU data protection authority decisions** with an AI
  dimension. Where a Member State DPA has issued a fine, a
  binding decision, or a corrective measure against an
  enterprise's AI system under GDPR (Articles 22, 24, 25,
  32, 33, 34 among others), the decision text on the DPA's
  own site is the primary record. The head reads the DPAs
  with the most active AI enforcement postures (typically
  France's CNIL, Italy's Garante, Ireland's DPC, and the
  European Data Protection Board's guidance) as standing
  reading.
  <!-- needs-research: verify current EDPB and Member State
  DPA guidance on AI systems under GDPR, current fine
  levels, and the specific articles most frequently cited in
  AI-related decisions -->
- **US federal enforcement actions.** The FTC has been the
  most visible US federal enforcer on AI matters — deceptive
  claims about AI capability, deceptive AI-generated
  content, AI-in-marketing conduct — with published consent
  orders and press-release-level summaries.
  <!-- needs-research: verify current FTC enforcement docket
  on AI matters, and confirm the FTC's primary enforcement
  authorities under Section 5 -->
  The EEOC has published enforcement guidance and
  enforcement matters on AI-in-hiring and AI-in-employment
  conduct.
  <!-- needs-research: verify current EEOC enforcement
  posture on AI-in-hiring and the specific guidance
  documents in force -->
  The FDA has published enforcement action on AI-enabled
  medical devices where post-market surveillance surfaced
  issues; the CFPB has published matters on AI-in-lending.
  <!-- needs-research: verify current FDA enforcement docket
  on AI/ML SaMD post-market matters, and current CFPB
  enforcement docket on AI-in-lending -->
- **Sector-supervisor actions.** For regulated sectors, the
  sector supervisor's public actions (SEC enforcement on
  AI-related disclosure matters, state insurance regulators
  on NAIC-adjacent AI matters, federal banking supervisors
  on model-risk-management enforcement) round out the
  disclosure-map calibration.

What the head reads regulator enforcement actions for is the
**difficult-conversation calibration** the head carries into
the rehearsal discipline from
[[06-difficult-incident-conversations]]. Every published
enforcement action is a rehearsal script for the
regulator-facing difficult conversation. The head reads the
action's factual account, notes where the enterprise's
response was seen by the regulator as adequate and where it
was seen as inadequate, notes the specific language the
regulator used to characterise inadequacy (evasion, delay,
inconsistency, unresponsiveness, over-explanation), and
calibrates the head's own rehearsal accordingly. Where the
regulator's public language on a peer's inadequacy is
specific enough to be quotable, the head keeps a private
library of regulator-language patterns that composes with the
difficult-conversation rehearsal.

Reading cadence. The head reads regulator enforcement
actions monthly, aligned to the regulator-engagement cadence
from [[mod-104-regulator-engagement]]. The monthly cadence
reflects the tempo at which regulator actions typically
publish and the tempo at which the head's own regulator
engagement runs. The reading composes with the horizon-scan
work from [[mod-105-regulatory-change-management]] but is a
distinct reading — the horizon scan is for what regulators
have said or proposed, the enforcement-actions reading is
for what regulators have actually done.

## The annual calibration exercise

The three primary sources and the two additional sources
compose into an annual calibration exercise the head runs and
signs. The exercise is the head's disciplined way of turning
the year's public incident data into concrete updates on the
enterprise's own readiness stack — not as an intellectual
exercise, but as a specific set of decisions the head takes
and records.

The exercise runs annually. The head schedules it as a
dedicated block on the calendar — typically two to three
working days, timed to compose with the enterprise's own
risk-register annual review from
[[mod-102-running-the-program]] and with the audit
committee's annual incident-cluster briefing under
[[mod-103-board-and-audit-committee-reporting]] cluster 3.
The senior AI governance architect at level 50 is the head's
principal partner for the exercise; the level-25 AI risk
engineer supplies the enterprise's own near-miss log (see the
section below) as one of the inputs.

The exercise walks the eight incident classes from
[[01-incident-command-shape-at-leadership-scope]] against the
year's public data. For each of the eight classes the head
and the architect produce four outputs:

- **The peer-benchmark corpus for the class.** The
  enumerated set of public incidents the year has surfaced
  that fit the class, drawn from the AIID, the OECD monitor,
  ATLAS case studies where security-flavoured, and the
  enforcement-action record where a regulator engaged.
- **The pattern deltas for the class.** What has changed in
  the class's pattern between last year and this year — new
  sub-patterns that have appeared, existing sub-patterns
  that have accelerated or plateaued, regulator responses
  that have shifted, sector responses that have shifted.
- **The enterprise-readiness delta for the class.** What
  needs to change in the enterprise's own readiness to
  reflect the pattern deltas — new tabletop scenarios, new
  disclosure-map entries, new coordination-surface pre-work,
  new KRIs, new controls.
- **The prioritisation delta for the class.** Whether the
  class as a whole is now higher-priority, lower-priority,
  or unchanged in the enterprise's own readiness stack,
  based on the year's evidence.

The exercise then walks the outputs against the enterprise's
own readiness artefacts and produces the specific updates:

- **The disclosure map from [[04-us-serious-incident-disclosure-map]]** is refreshed for
  the year — new regulator interpretations, new
  jurisdiction-specific enforcement patterns, new
  sector-supervisor postures.
- **The tabletop scenarios rehearsed with the delegate** per
  [[01-incident-command-shape-at-leadership-scope]] are
  updated — scenarios retired that the peer evidence shows
  are no longer representative, scenarios added that the
  peer evidence shows are now representative, scenarios
  revised for sub-pattern shifts within a class.
- **The rehearsal conversations from
  [[06-difficult-incident-conversations]]** are updated —
  new regulator-language patterns from the enforcement
  actions the year surfaced, new peer-response patterns
  from the AIID that the head's rehearsal has to now
  account for.
- **The KRI / KPI portfolio from
  [[mod-107-program-measurement-and-maturity]]** is
  reviewed — indicators that are no longer surfacing the
  right signal because the class's pattern has shifted,
  indicators that need to be added because the year's
  evidence shows a signal the portfolio does not carry.
- **The risk register from
  [[mod-102-running-the-program]]** is fed the
  completeness deltas from the MIT repository walk, the
  emerging-class flags from the repository, and any
  register lines the AIID's pattern has re-scored for
  residual likelihood.

The output of the exercise is a written **calibration note**
the head signs. The note is not the full working set — the
underlying walk of the AIID, the OECD monitor, and the MIT
repository stays in the head's and the architect's working
files. The calibration note is the leadership-visible summary
that lands on the audit committee under
[[mod-103-board-and-audit-committee-reporting]] cluster 3.

The calibration note answers four questions in
audit-committee-appropriate language:

- **What new class of incident is the head now preparing
  for?** The year's public evidence has surfaced a class of
  failure the enterprise's readiness stack did not
  previously cover. The head names the class, names the
  peer evidence, names the specific readiness updates the
  head has commissioned.
- **What existing class is now higher-priority based on
  public evidence?** A class the enterprise carried at a
  given priority is now higher-priority because the year's
  evidence shows the class's frequency, its harm severity,
  its regulator-response intensity, or its cross-jurisdictional
  spread has increased. The head names the class, names the
  evidence, names the priority change.
- **What class had been treated as high-priority is now
  lower-priority?** A class the enterprise carried at a
  given priority is now lower-priority because the year's
  evidence shows the class's frequency has plateaued, the
  peer response has converged on effective controls, the
  regulator has moved on, or the sector has developed
  standing infrastructure that reduces the residual
  exposure. The head names the class, names the evidence,
  names the priority reduction.
- **What the delta means for the year-ahead investment
  plan.** The priority changes have investment implications
  — new controls to build, new tabletop capacity to fund,
  new team capabilities to hire for, new external
  engagements to sponsor. The head names the investment
  deltas the calibration note implies, and composes them
  with the annual budget cycle the enterprise runs.

The calibration note is signed by the head and briefed to the
audit committee. The audit committee is not asked to approve
each substantive change; the audit committee is asked to note
that the calibration discipline has been run, that its output
is the note in front of them, and that the specific changes
land in the risk register, the control library, the
disclosure map, and the year-ahead plan on the running
cadences those artefacts each carry.

## The near-miss discipline

Public incident data is peer calibration; the enterprise's
own near-misses are ground truth. The head's calibration
stack is incomplete without both, because the two carry
different signals that neither reproduces.

A **near-miss** is an event that could have been an incident
and was not, either because a control caught it before harm
crystallised, because the containment window was inside the
harm-threshold that would have made the event reportable, or
because the vulnerable population that would have been
affected did not materialise (the affected model was not
routed production traffic in the window the event was live,
the RAG corpus poisoned was not consumed by any production
query during the poisoning window, the jailbreak that
succeeded produced output no downstream user actually saw).
The near-miss is not an incident under the enterprise's
severity taxonomy; the head does not file it, does not
publicly disclose it, does not treat it as a board-notifiable
event under normal cadence. But the near-miss is the highest-
signal single artefact the head has for calibrating the
enterprise's own controls, because it is a case where the
control stack was actually tested by an event with real
adversarial or environmental origin, and the head can see
which controls held, which controls partially held, and which
controls would have failed had the near-miss propagated one
step further.

The head builds a **private near-miss log** — separate from
the incident register the audit committee sees, separate
from the DFIR incident record the CISO's team maintains, and
inside the head's own function's artefact store. The
separation is deliberate. The near-miss log carries events
that were not incidents, and the head does not want the log
to be misread by an external audience (a regulator receiving
a subpoena, a plaintiff's counsel in a discovery request, a
journalist making a public-records request) as though the
log were a hidden incident register. The near-miss log is
what its name says — near-misses, evaluated as near-misses,
and used as calibration.

The log's schema carries, per near-miss:

- The near-miss narrative — what happened, in language
  parallel to but distinct from an incident narrative.
- The class per the eight-class taxonomy from
  [[01-incident-command-shape-at-leadership-scope]] the
  near-miss maps to.
- The controls that caught it — which specific entries in
  the control library operated, at which specific step in
  the near-miss's trajectory.
- The controls that would have caught it next — which
  entries would have operated at the next step if the
  first control had not.
- The controls that would have failed to catch it — where
  the head sees a gap in the enterprise's stack that the
  near-miss reveals.
- The disposition — whether the near-miss triggers a
  control update, a policy update, a training update, or is
  recorded as calibration only.

The log feeds the same annual calibration exercise the public
data feeds. Where the annual exercise walks the public data
for peer-benchmark signal, the exercise also walks the
near-miss log for enterprise ground-truth signal. The two
walks compose into a single output — the risk register earns
its keep or fails to on the strength of both. A register line
that carries a specific class at a specific residual score is
validated when both the peer benchmark and the near-miss log
show the class materialising at frequencies and severities
consistent with the score; it is invalidated when either
source shows the class materialising differently than the
score implies.

Ownership of the near-miss log is deliberate and layered.
The **level-25 AI risk engineer** maintains the log — logs
each near-miss as it surfaces (typically from the routine
operating cadence of the AIMS's monitoring, red-team
programme, evaluation function, or ad-hoc reports from
product teams), populates the schema for each entry, and
maintains the log's referential integrity. The **level-50
senior AI governance architect** reviews the log at a
monthly cadence — spot-checks the engineer's dispositions,
identifies patterns across near-misses that a single-entry
review would miss, and commissions the artefact updates any
patterns imply (control revisions, policy clauses, training
material). The **head** reviews the log at a monthly cadence
as part of the head's own operating review — reads the
month's new near-misses, notes the architect's dispositions,
challenges any disposition that reads as too generous or too
severe, and identifies any near-miss that warrants elevation
to a formal incident classification.

The head's monthly review is the discipline that keeps the
log honest. A near-miss log that never elevates any near-miss
to formal incident status is signalling either that the log
is under-populated (the enterprise is missing near-misses
because the surfacing mechanisms are inadequate) or that the
elevation threshold is set too high (near-misses that should
be filed as incidents are being dispositioned as near-misses
because filing carries perceived cost). Either failure is a
calibration failure the head names, either failure destroys
the log's value as ground truth, and the head's monthly
review is where each failure gets caught early. The head
does not delegate the review to the architect on a permanent
basis; the head reads the log personally, because the log is
where the enterprise's own control stack is being tested
against reality, and the head's calibration of the whole
readiness stack depends on the head having read what the log
shows.

## The peer-benchmarking discipline

Beyond public incident data itself, the head runs a specific
peer-benchmarking discipline that reads what peer enterprises
publish about their own AI-incident readiness — for both what
they say and what they omit. The discipline is one of the
head's inputs into the annual calibration exercise and
composes with the head's external-positioning discipline from
[[mod-106-external-positioning-and-voluntary-codes]].

Three peer-publication categories carry the material the head
reads.

**Annual transparency reports.** Some AI developers,
particularly frontier developers, publish periodic
transparency reports — typically annually, sometimes
quarterly for the most publication-active — describing their
safety-and-security programme, their evaluation results, the
incidents they have publicly disclosed, the controls they
operate, and their engagement with sector infrastructure.
The transparency reports vary widely in candour and in
substantive depth; the head reads the reports across the
active peer set and calibrates the enterprise's own posture
accordingly. Where a peer's transparency report is more
substantive than the enterprise's own on a specific
dimension, the head considers whether the enterprise should
match the substantive depth on that dimension. Where a peer's
transparency report is thinner, the head reads the thinness
as either a signal that the peer has less to say (a
calibration signal for the peer's maturity) or a signal that
the peer has more to say but chose not to (a calibration
signal for the peer's disclosure posture).
<!-- needs-research: verify current transparency-report
publication cadence and current publishing peer set (Anthropic,
OpenAI, Google DeepMind, Meta, Microsoft AI, and any others
publishing on regular cadence) -->

**Published post-mortems.** Occasionally a peer enterprise
will publish a post-mortem of an incident — either
voluntarily as part of the peer's transparency programme, or
under a regulator-imposed obligation. Published
post-mortems are rare and high-signal artefacts. The head
reads every published post-mortem the year surfaces, in
depth, because the post-mortem carries the peer's own
narrative account of what went wrong, what the peer did
about it, and what the peer changed. The head walks the
post-mortem against the head's own RCA sponsorship
discipline from [[05-post-incident-learning-cycle-sponsorship]]
and asks — would the enterprise's RCA discipline have
produced a post-mortem of this depth; would the head have
signed a post-mortem framed this way; where does the
post-mortem stop short of the head's own standard, and
where does the post-mortem go beyond it.

**Regulator-imposed disclosures.** Public consent decrees
between regulators and peer enterprises, published
enforcement actions with settlement-imposed disclosure
requirements, and other regulator-required disclosures carry
material the peer would not have published voluntarily. The
head reads these with particular attention because the
regulator has typically required the disclosure to make a
specific point about the peer's inadequacy that the head
does not want to repeat at the enterprise. The
regulator-imposed disclosure is calibration for the
difficult regulator conversation from
[[06-difficult-incident-conversations]] at higher intensity
than the routine enforcement action, because the disclosure
is the peer's own account of failing under the regulator's
supervision.

The head reads peer transparency reports the same way the
head reads peer sustainability reports or peer
governance-committee charters — for both what they say and
what they omit. The omission signal is often the more
informative. A transparency report that discloses evaluation
results but omits red-team findings; a transparency report
that discloses controls but omits the incidents those
controls were tested by; a transparency report that
discloses aggregate figures but omits the disaggregation the
head knows the peer has — each omission signals a specific
posture the peer has chosen and a specific dimension on
which the peer has chosen to be less transparent. The head
reads the pattern of omissions as calibration for the
enterprise's own transparency posture, which composes into
the public-trust posture from
[[mod-106-external-positioning-and-voluntary-codes]].

The head produces a lightweight **peer-comparison note**
twice a year — timed to compose with the transparency-report
publication cadence and with the enterprise's own
external-positioning review. The note is short (typically
two to four pages), read by the head and the senior
architect, and used as an input to the enterprise's own
external-positioning discipline. The note is not published
externally; it is an internal calibration artefact. The
audit committee sees the note's existence as evidence of the
discipline but is not routinely briefed on its contents,
because the note contains the head's own reading of peers'
postures and the enterprise's own comparative posture, and
that reading is more useful as internal working material
than as board-visible product.

## Composition with adjacent modules

- [[mod-102-running-the-program]] is where the risk register
  the annual calibration exercise updates lives. The
  MIT-repository completeness walk feeds the register's
  taxonomy review; the near-miss log feeds the register's
  residual-scoring review; the AIID and OECD monitor
  pattern signals feed the register's emerging-risk section.
- [[mod-103-board-and-audit-committee-reporting]] cluster 3
  is where the annual calibration note lands. The
  calibration note is not itself an incident report; it is a
  meta-level report on the head's own calibration
  discipline, and it sits under the incident-and-near-miss
  cluster as evidence that the discipline is running.
- [[mod-104-regulator-engagement]] is the parent framing
  for the enforcement-action reading discipline. The
  enforcement-action reading composes with the general
  regulator-engagement cadence and with the specific
  regulator-relationship-management work in that module's
  chapter on relationship management.
- [[mod-105-regulatory-change-management]] is the parent
  horizon scan the OECD monitor reading composes with.
  Where the OECD monitor surfaces a regulator response the
  horizon scan had not yet caught, the monitor is the
  trigger to update the scan.
- [[mod-106-external-positioning-and-voluntary-codes]] is
  where the peer-comparison note lands as an input to the
  enterprise's own transparency posture and voluntary-code
  engagement portfolio.
- [[mod-107-program-measurement-and-maturity]] is where the
  KRI / KPI portfolio the calibration exercise reviews
  lives. The calibration note names indicator revisions the
  portfolio needs; the portfolio's own review cadence
  absorbs them.
- [[mod-109-cross-enterprise-leadership]] chapter 01 is
  where the CISO coordination the ATLAS case-study reading
  feeds into runs. The head does not read ATLAS in
  isolation; the head reads it to be calibrated for the
  joint conversation with the CISO's team.
- [[01-incident-command-shape-at-leadership-scope]] is the
  eight-class taxonomy this chapter's calibration exercise
  walks against. The public-data calibration is the
  discipline that keeps the taxonomy live and honest;
  without it the taxonomy is a static frame that ages out.
- [[03-article-73-filing-at-incident-time]] and
  [[04-us-serious-incident-disclosure-map]] are where the
  disclosure-map refresh the annual calibration exercise
  produces lands. The disclosure map is not authored once
  and left; the annual calibration is the discipline that
  keeps it current against the actual enforcement pattern.
- [[05-post-incident-learning-cycle-sponsorship]] is the
  RCA sponsorship discipline the head reads peer
  post-mortems against. Peer post-mortems are calibration
  for the head's own RCA standard, and the head reads
  every one the year surfaces.
- [[06-difficult-incident-conversations]] is where the
  regulator-language patterns from the enforcement-action
  reading and the peer-response patterns from the AIID
  feed into the rehearsal library. The calibration
  exercise refreshes the rehearsal library annually with
  the year's new material.

## Summary

- Public incident data is peer benchmark, not probability
  distribution. The head reads it as case material for a
  rehearsed response, not as input to a rate calculation.
  For every public incident the head walks, the output is
  four items: what happened, what class of failure per the
  eight-class taxonomy, what the peer's response was, what
  the enterprise would have done differently.
- Three primary sources sit at the centre of the head's
  calibration discipline: the AI Incident Database (AIID)
  for pattern-of-failure, regulator-response, and
  peer-response signals at quarterly cadence; the OECD.AI
  AI Incidents Monitor for cross-jurisdictional pattern and
  international regulator-response signals at quarterly
  cadence aligned to regulatory change management; and the
  MIT AI Risk Repository for risk-taxonomy completeness and
  emerging-class signals at annual cadence aligned to the
  risk-register review.
- Two additional sources sit at lower cadence: MITRE ATLAS
  case studies for security-flavoured incident calibration
  read on ATLAS release and consumed via the CISO
  coordination surface, and regulator enforcement actions
  and public settlements for disclosure-map and
  difficult-conversation calibration read monthly aligned
  to the regulator-engagement cadence.
- The annual calibration exercise walks the eight incident
  classes from
  [[01-incident-command-shape-at-leadership-scope]] against
  the year's public data and produces four outputs per
  class: the peer-benchmark corpus, the pattern deltas, the
  enterprise-readiness delta, and the prioritisation delta.
  The exercise refreshes the disclosure map, the tabletop
  scenarios, the rehearsal library, the KRI / KPI
  portfolio, and the risk register.
- The output of the exercise is a written calibration note
  the head signs and briefs to the audit committee under
  [[mod-103-board-and-audit-committee-reporting]] cluster
  3. The note answers what new class the head is now
  preparing for, what existing class is now higher-priority
  based on public evidence, what class is now
  lower-priority, and what the delta means for the
  year-ahead investment plan.
- Public incidents are peer calibration; the enterprise's
  own near-misses are ground truth. The head builds a
  private near-miss log — separate from the audit
  committee's incident register — that carries the events
  that could have been incidents and were not. The log
  schema names controls that caught the near-miss,
  controls that would have caught it next, and controls
  that would have failed. The level-25 AI risk engineer
  maintains the log; the level-50 senior AI governance
  architect reviews monthly; the head reads personally at
  monthly cadence.
- The peer-benchmarking discipline reads what peer
  enterprises publish about their own AI-incident
  readiness — annual transparency reports, published
  post-mortems, regulator-imposed disclosures — for both
  what they say and what they omit. The head produces a
  lightweight peer-comparison note twice a year that lands
  as an input to the enterprise's own external-positioning
  discipline from
  [[mod-106-external-positioning-and-voluntary-codes]].
- The calibration discipline is the discipline that keeps
  every other element of the head's incident-readiness
  stack — the eight-class taxonomy, the disclosure map,
  the coordination surfaces, the RCA sponsorship, the
  rehearsal library — from ageing out. Without it, the
  stack looks complete right up to the moment an incident
  lands that the sample did not carry.
