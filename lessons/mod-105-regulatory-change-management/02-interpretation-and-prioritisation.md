# Interpretation and Prioritisation of a Landing Obligation

## Motivation

Chapter 01 built the scanning system that pulls regulatory-change
items to the head's attention with the right timing. This chapter
covers what happens after an item crosses from watch into active or
priority — the workflow that turns a raw obligation into an
operating decision the enterprise can act on.

The failure mode this chapter closes is subtler than the failure
mode chapter 01 closed. A head with a good scanning system can still
lose the program in interpretation. The item arrives on the tracker
at the right time; the analyst summarises it accurately; and then
the enterprise does one of three things that all look like activity
but produce no useful output. It treats every landing item as a
priority and burns the interpretation queue on items that did not
need it. It treats every item as watch and misses the compliance
date because "we were still gathering facts". Or — most common —
it interprets each item in isolation, so that by the end of the
year the head has thirty perfectly-scoped interpretation memos and
no picture of how the thirty stack together against the operating
program.

The interpretation-and-prioritisation workflow is the discipline
that produces useful output. It is a program-management workflow,
not a legal-analysis workflow — the head does not deliver legal
opinions ([[mod-104-regulator-engagement]] chapter 07). It is what
the head does *with* legal opinions to keep the enterprise's AI
program running.

The reference frame is the enterprise's operating model as designed
by the level-50 architect ([[mod-102-running-the-program]] chapters
01 through 06 depend on that design), the regulatory crosswalk the
architect maintains (chapter 04 in mod-102), and the ISO/IEC 42001
AIMS clause 4.2 requirement to determine relevant interested
parties' requirements — which, translated into head vocabulary, is
"figure out what a regulator's expectation of the enterprise now
is".

## Core concept — the intake-to-disposition workflow

Every item that reaches interpretation goes through the same
seven-step workflow. The steps are named because a head who cannot
name them cannot troubleshoot when one of them is failing.

1. **Intake** — the item is formally opened, the responsible desk
   owner assigned, the SLA calculated.
2. **Packaging** — the desk produces the packaged obligation
   (attachment analysis, technical-feasibility assessment,
   operational-cost sketch) covered in chapter 02 of this section.
3. **Legal opinion** — GC delivers the interpretive opinion on the
   packaged obligation.
4. **Portfolio prioritisation** — the head decides where the
   interpreted obligation sits in the portfolio queue relative to
   other landing items and to the running program.
5. **Handoff to the architect** — the level-50 architect receives
   the interpreted, prioritised obligation and updates the
   crosswalk and control-library delta.
6. **Change-management plan authoring** — chapter 03 covers the
   plan shape the head authors from the delta.
7. **Disposition** — the register is closed on the interpretation
   step; the change-management plan takes over the operational
   tracking. The register memory holds the trace.

Each step has an owner, an artefact, and an SLA. The rest of this
chapter walks the steps and lands the priority framework — the
piece of the workflow the head personally owns and personally
adjudicates.

## Step 1 — intake

Intake is administrative but it is where the enterprise most often
loses interpretation velocity. An item on the tracker gets promoted
to active or priority (chapter 01 triage rules), and then nothing
happens for eleven days while somebody works out who owns it. Those
eleven days are the difference between a defensible interpretation
posture and a rushed one.

The intake discipline the head enforces:

- The moment an item is promoted (at the weekly digest read, at
  the monthly portfolio review, or ad hoc on urgent escalation), a
  desk owner is named. The owner is a specific person, not a team.
- The SLA clock starts. Active items have a 30-day SLA to reach
  step 5 (architect handoff). Priority items have a 14-day SLA.
  These SLAs are program-management defaults, not legal
  requirements; they may compress when a regulator has already set
  a compliance date.
- The item's register record is annotated with the intake
  timestamp, the owner, and the SLA. A single missed SLA is
  telemetered to the head at the weekly digest read; a pattern of
  missed SLAs is a program problem the head addresses in the
  quarterly deep scan.

Intake is boring and it is where the head's discipline shows.

## Step 2 — packaging the obligation

Packaging is a translation exercise. The desk owner reads the raw
obligation — the regulation, the guidance, the standard, whatever
form the item takes — and produces a *packaged obligation memo*
with five components. This is the same five-component packaging
discipline that [[mod-104-regulator-engagement]] chapter 07
introduces for GC-facing regulator interactions. It is imported
into interpretation here because the head cannot ask GC a useful
question without it.

- **Plain-English summary.** Two to three sentences: what does
  this obligation *require* the enterprise to do, in operational
  terms. Not "the AI Act says X" — "the AI Act requires the
  enterprise to do X, on Y systems, by Z date."
- **Attachment analysis.** Which systems, decisions, actors,
  business lines, and data flows within the enterprise does the
  obligation attach to? The attachment analysis leans directly on
  the level-50 architect's AI system inventory
  ([[mod-102-running-the-program]] chapter 06) and the crosswalk
  (chapter 04 of that module). If the obligation is scoped to
  "high-risk" or to a specific use-case category, the attachment
  analysis names the specific systems inside and outside.
- **Technical-feasibility sketch.** For each attachment point,
  what can the enterprise technically do to comply, what can it
  not yet do, what would the delta take to close.
- **Operational-cost sketch.** A defensible estimate of what
  compliance would cost — engineering effort, run-cost, vendor
  spend, opportunity cost from feature-scope reduction. The
  estimate does not need to be a full P&L exercise (chapter 03
  authors the plan and chapter 06 in mod-113 covers cost
  authoring) but it needs to be defensible enough that GC's
  opinion has a cost signal to weigh.
- **The specific question for GC.** The desk formulates the
  precise interpretive question: does the obligation attach in
  this way, on these facts, and what defences would the
  enterprise have if a regulator disagreed with the attachment
  analysis. If the desk cannot formulate the question, the desk
  does not yet understand the obligation and it goes back to
  packaging.

Packaging is where the AI-governance analyst desk demonstrates its
value. A well-packaged obligation makes GC's job efficient and
makes the head's prioritisation defensible. A poorly-packaged
obligation is either an oversized interpretation project or a
misdirected legal-opinion ask.

## Step 3 — legal opinion

GC receives the packaged obligation and delivers an opinion in
their own vocabulary. The head does not rewrite GC's opinion, does
not soften it in downstream artefacts, and does not extract a
paraphrase for the running program without GC's sign-off. The
disagreement discipline in [[mod-104-regulator-engagement]] chapter
07 applies here identically.

The opinion typically has three components:

- **Interpretation.** How GC reads the obligation on the facts
  packaged. This may include reasoning under recitals, prior
  precedent, or Member-State transposition where relevant.
- **Attachment position.** Whether the obligation attaches as the
  desk packaged it, attaches differently, or does not attach on
  the packaged facts.
- **Defensive posture.** What the enterprise's defensive
  arguments would look like if a regulator took a different
  attachment position. This lets the head weigh whether an
  argument for narrower attachment is worth the enforcement risk.

The opinion is an internal artefact, privileged where the
enterprise's counsel treats it as such, and stored under the
document-retention discipline the enterprise runs for legal work.
The register memory (chapter 01) records that the opinion exists
and where; it does not restate the opinion's substance.

## Step 4 — portfolio prioritisation

Step 4 is where the head personally makes a decision that only the
head can make. The prior steps produce inputs. Step 4 produces the
enterprise's next operating move.

The failure mode this step exists to close: the enterprise
interprets each obligation in isolation, produces a plan for each,
and by the end of a quarter has committed the level-50 architect
and the operating teams to more concurrent change than they can
absorb. That is program failure, and it looks nothing like the
regulator's fault.

The head prioritises against four axes.

### Axis 1 — compliance-date proximity

The regulator's own timeline is the first axis. A final rule with
a compliance date twelve weeks away outranks a final rule with a
compliance date twelve months away, all else equal. "All else
equal" is doing a lot of work in that sentence — see the other
axes below.

Within compliance-date proximity, the head distinguishes:

- **Hard compliance dates** — statutory effective dates, adopted
  regulation dates, mandatory-standard-citation dates in the OJEU.
  Missing these dates creates enforcement exposure the enterprise
  cannot mitigate.
- **Soft compliance dates** — supervisory-expectation dates,
  code-of-practice publication dates, standards revisions. The
  enterprise has more room to sequence, but a soft date that the
  head misses becomes a hard problem in the next examination.

### Axis 2 — attachment breadth

An obligation that attaches to the enterprise's core AI system
inventory outranks one that attaches to a bounded corner. The
attachment analysis from step 2 supplies the input. The head
distinguishes:

- **Enterprise-scale attachment** — the obligation touches
  multiple business lines, most of the AI system inventory, or a
  cross-cutting operational capability (model registry, incident
  reporting, evaluation harness, data-governance).
- **Business-line attachment** — the obligation touches a specific
  BU's AI systems but not the rest of the enterprise.
- **Bounded attachment** — the obligation attaches to a single
  system or a narrow use-case class.

Enterprise-scale attachment justifies priority even when
compliance-date proximity is more distant, because the change-
management plan is bigger and the enterprise needs more runway.

### Axis 3 — enforcement risk

The head's judgement about how likely, how severe, and how visible
enforcement would be if the enterprise did not act. Enforcement
risk is not a legal opinion (GC's opinion covers defensive
posture) — it is a program-management estimate, informed by the
enforcement history of the regulator, the enforcement history of
the enterprise, the political and market salience of the topic, and
the presence of peer enforcement.

The head calibrates enforcement risk with input from GC, from the
enterprise's Government Affairs function, and from industry-body
intelligence. The estimate is documented in the interpretation
record and is revisable as facts change.

### Axis 4 — program-carrying capacity

The final axis is the enterprise's own capacity to absorb change.
The head knows what is already in flight — the running program
([[mod-102-running-the-program]]), other interpretations in the
pipeline, the level-50 architect's engineering queue, the operating
teams' quarterly plans. Adding a priority when the program is
already at capacity produces stalled changes, not compliance.

The head's rebalancing moves when capacity is tight:

- Compress a lower-priority item to a lighter change-management
  plan (chapter 03 covers what "lighter" looks like) to free
  capacity for a higher-priority item.
- Escalate a capacity-constrained conflict to the CxO layer
  (chapter 05) with a clear ask — additional engineering, phasing
  agreement from product, exception-window agreement.
- In extremis, take a documented, dated, board-informed decision
  to accept enforcement risk on a specific item because carrying
  it would break the program on a more critical item. This is a
  head decision, not a delegated one, and the audit-committee is
  informed ([[mod-103-board-and-audit-committee-reporting]]
  chapter 02).

### The priority score in practice

The head does not present the axes as a formula. The head
adjudicates by weighing the four axes in the quarterly portfolio
review, produces a written priority ranking with reasoning, and
publishes it to the level-50 architect, to the operating teams,
and to the CxO layer. Reasoned adjudication defended in writing
beats a numeric score every time; the writing is what a
certification body or an auditor reads.

## Step 5 — handoff to the level-50 architect

Once prioritised, the interpreted obligation is handed to the
level-50 architect. The architect owns the crosswalk update and
the control-library delta — those are architectural artefacts
outside this module's scope. The head owns the *handoff quality*:
that the packaged obligation, the GC opinion, and the priority
ranking are delivered together with a clear ask for the crosswalk
update deliverable.

The architect's output is the delta the change-management plan
(chapter 03) operationalises. The head does not skip step 5 and go
directly from GC opinion to change-management plan authoring; that
skip is how enterprises produce plans that conflict with the
running program's control library.

## Step 6 — change-management plan authoring

Covered in chapter 03. Called out here so the workflow is a full
seven-step loop.

## Step 7 — disposition

The interpretation record is closed. The register memory (chapter
01) is annotated with the interpretation output, the priority
ranking, the crosswalk update reference, and the change-management
plan reference. The item leaves the interpretation queue and enters
the operating program.

The interpretation SLA metrics from
[[mod-107-program-measurement-and-maturity]] chapter 01 read the
disposition timestamps to produce median-time-to-interpretation and
in-SLA percentages the head reports at the quarterly deep scan.

## The batching discipline

Working through the seven-step workflow one item at a time is often
wrong. The head *batches* interpretation when items share
attachment, share crosswalk impact, or share the same GC opinion
input. Batching reduces cost and produces more coherent operating
change.

Two batching patterns worth naming:

- **Same-obligation-family batching.** When a single regulation is
  transposed across multiple Member States (the EU AI Act at NCA
  level, the NAIC AI Model Bulletin across state DOIs, the OECD
  Principles across national implementations), the head batches
  the interpretation with a single GC opinion at Union / model
  level and per-jurisdiction attachment overlays. This is not a
  shortcut; it is the disciplined shape.
- **Overlapping-attachment batching.** When two unrelated
  obligations attach to the same AI system inventory
  cross-section, the head batches the change-management plans
  (chapter 03) so the operating teams absorb one integrated change
  instead of two smaller conflicting ones.

The batching decision belongs to the head at step 4. A desk owner
does not batch on their own initiative because batching commits
capacity across the head's portfolio, which is the head's decision.

## Coordination with legal counsel — engaging without becoming legal

The interpretation workflow is the head's most legal-adjacent
activity. It is also where the head is most likely to drift into
legal-opinion territory. Two disciplines keep the head where the
head belongs.

- **Package, don't opine.** Step 2 packages the obligation. It
  does not state what the obligation *means* in legal terms. It
  states what it *requires* the enterprise to do on the facts.
  This distinction is the same one [[mod-104-regulator-engagement]]
  chapter 07 draws for regulator-facing work; it applies inside
  the enterprise too. A packaging memo that reads like a
  legal-opinion draft has drifted.
- **Route legal-conflict determinations through GC, not through
  the interpretation memo.** When a new obligation appears to
  conflict with an existing obligation (a common pattern between
  the AI Act and sectoral supervision, between US federal and
  state law, between GDPR and AI Act), the interpretation memo
  notes the potential conflict as a question for GC — it does not
  resolve the conflict. GC's opinion covers the resolution.

## Adjacent workflows this does not replace

The interpretation workflow is not a replacement for three adjacent
disciplines that live in other modules and that the head coordinates
with, not against.

- **Risk assessment against risk appetite** — the enterprise AI
  risk register ([[mod-102-running-the-program]] chapter 03) may
  require an interpreted obligation to be reflected as a KRI or
  as an appetite-tolerance-limit adjustment. The interpretation
  workflow feeds the risk register; it does not perform risk
  assessment.
- **Third-party contract renegotiation** — an interpreted
  obligation that changes supplier expectations feeds
  procurement's contract-review pipeline
  ([[mod-102-running-the-program]] chapter 04 covers the third-
  party audit interface). The interpretation workflow triggers
  the pipeline; procurement runs it.
- **Board reporting** — a materially high-priority interpretation
  is reflected in the next quarterly board pack
  ([[mod-103-board-and-audit-committee-reporting]] chapter 01
  cluster 5). The interpretation workflow does not author the
  board section; it feeds it.

## The one-sentence summary

Interpretation-and-prioritisation is the seven-step workflow that
turns a scanned obligation into an operating decision — intake,
package, opine, prioritise, hand off, plan, dispose — with the
head personally adjudicating at the prioritisation step and
staying rigorously on the program-management side of the
head-and-GC boundary throughout.

## Summary

- Scanning (chapter 01) pulls items to attention; interpretation
  turns them into operating decisions. The workflow has seven
  named steps, each with an owner, artefact, and SLA.
- Intake starts the SLA clock and names a specific desk owner —
  active items 30-day SLA, priority items 14-day SLA.
- Packaging produces the five-component memo (plain-English
  summary, attachment analysis, technical-feasibility sketch,
  operational-cost sketch, specific question for GC). This is
  the same discipline as chapter 07 of mod-104 and it is where the
  desk demonstrates value.
- GC delivers the interpretive opinion; the head does not
  paraphrase or soften it, and never restates it as an enterprise
  compliance conclusion.
- Prioritisation is adjudicated by the head against four axes:
  compliance-date proximity, attachment breadth, enforcement risk,
  and program-carrying capacity. The output is a written priority
  ranking, not a numeric score.
- Handoff to the level-50 architect closes the interpretation loop
  and opens the crosswalk / control-library delta that the change-
  management plan (chapter 03) operationalises.
- Batching by obligation family or by overlapping attachment is
  the head's decision at step 4 — not the desk's initiative.
- Interpretation feeds risk register, procurement, and board
  reporting but does not replace them; interpretation stays on
  the program-management side of the GC boundary from step 2
  through step 7.
