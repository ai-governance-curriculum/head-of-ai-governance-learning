# IIA Three Lines Model at Leadership Scope

## Motivation

The IIA Three Lines Model (2020, replacing the earlier 2013 Three Lines
of Defense model) is the enterprise assurance operating model most
audit committees speak fluently. It defines three roles — *management*
(first line), *risk management and compliance* (second line), and
*internal audit* (third line) — and describes how they coordinate with
the *governing body* to achieve enterprise objectives.

At level 60, the Head of AI Governance is *the* second-line accountable
executive for the AI Governance family. That is the load-bearing claim
of the role. Everything else in the operating model — coordination
with first-line product and engineering, interface to the third-line
CAE, direct access to the audit committee, escalation of unresolved
risk — flows from that single positional fact.

This chapter reads the Three Lines Model at leadership scope, defines
the specific failure mode (operational-distance failure) that ruins
second-line credibility, and explains how the head coordinates without
crossing lines.

## Core concept: the three lines and the governing body

The IIA Three Lines Model has four positions:

- **Governing body** — accountable to stakeholders for oversight, sets
  the enterprise's direction, delegates responsibility, oversees
  management. For AI, the board with the audit committee and (where
  it exists) the risk committee and the technology committee.
- **First line — management** — owns products, services, and the
  operational risks that come with them; owns delivery. For AI, this
  is the product / engineering / data-science / MLOps / model-owner /
  business-owner community. First line runs the AI.
- **Second line — risk and compliance functions** — provides
  expertise, support, monitoring, and challenge on risk and
  compliance-related matters. For AI, this is the AI governance
  function led by the head at level 60.
- **Third line — internal audit** — provides independent, objective
  assurance and advice, primarily to the governing body. Owned by the
  Chief Audit Executive (CAE) under the IIA International Professional
  Practices Framework (IPPF).

The 2020 update to the model dropped the "of defense" phrasing and
emphasised *alignment* rather than *defence*. That change matters: it
is why the head coordinates with the first line rather than policing
it, and why the head advises the third line rather than reporting to
it.

## Where the head owns

The head at level 60 owns the *second-line function for AI*. Concretely
that means the head is accountable for:

- **The AI risk framework** — inherited by design from the level-50
  architect, but operated by the head. The risk taxonomy, appetite
  statement, tolerance limits.
- **The AIMS under ISO/IEC 42001** — running the management system to
  ISO/IEC 42006 audit-body inspection quality; internal audit rounds,
  management-review cadence, corrective-action follow-through.
- **The enterprise AI risk register at portfolio cadence** — the top-N
  risks that go to the risk committee.
- **The AI control library operation** — monitoring first-line
  operation of the controls the level-50 architect defined; challenge
  where operation is deficient.
- **The compliance-obligation crosswalk** — status against EU AI Act,
  sector rules, state acts, international regulation.
- **The independent challenge** — the ability and willingness to
  challenge first-line design and release decisions, including
  stop-shipping challenges, without being subordinate to the challenged
  party.
- **The regulator interface** — engagement with EU AI Office, national
  CAs, US AISI + AISIC, UK AISI, sector regulators (Fed / OCC / FDIC /
  OSFI / NAIC / FDA / MHRA / EMA / EEOC / FTC / CFPB / HHS OCR / CPPA /
  Colorado AG / UK ICO / CISA + NCSC).
- **The independent access to the audit committee** — direct
  reporting line preserved regardless of solid-line management.

Those seven items are the second-line envelope. Losing any one
compromises the head's credibility as the second line.

## Where the head coordinates first line (does not replace)

The Three Lines Model is explicit that the second line does not do the
first line's job. That is the single most common mistake in AI
governance function design: the second-line function absorbs first-
line accountability under the name of "helping."

The head coordinates first line by:

- **Advising, not deciding, on first-line risk decisions.** First line
  decides. Second line advises and challenges. A first-line product
  owner is the accountable decision-maker for whether to ship;
  second-line challenge is *escalated* if unresolved, not *overridden*
  by fiat. Stop-shipping authority lives in the governance council
  (chaired by the head) with an appeal path to the CAIO / CEO, not in
  the head unilaterally.
- **Embedding second-line partners with first-line teams**, where the
  organisation-shape supports it, without those partners *becoming*
  first-line. The IIA's 2020 update explicitly notes that first- and
  second-line roles can blend when management explicitly assigns risk
  responsibilities — but the head has to be careful the second-line
  independence is preserved when they blend.
- **Owning the governance council with cross-line membership**,
  including first line, second line, GC, and non-voting third-line
  observers when the CAE agrees.
- **Owning the AI system inventory quality bar** at second-line scope,
  while the first line maintains the entries.

The clearest single test: does the first line know it owns the risk
outcome, or does it silently believe the second line is the one
accountable? If the second line is silently accountable, the model has
collapsed and any regulator or third-line auditor will find it.

## Where the head interfaces with third line

The third line — internal audit under the CAE — provides independent
assurance to the governing body. The head does not report to the CAE;
the CAE does not report to the head. The head and the CAE are peers
whose functions coordinate.

The head interfaces with the third line by:

- **Sharing the AI audit universe** — the CAE authors the audit plan;
  the head briefs the CAE on risk hotspots so the third-line plan can
  focus there.
- **Coordinating on the AI-audit programme**, but without co-authoring
  it. The CAE's independence is inviolable. The IIA Standards (IPPF)
  specify the CAE's independence requirement; the head respects it.
- **Providing evidence access** — the AIMS evidence store, the risk
  register, the incident logbook, the crosswalk status — for third-
  line audit fieldwork.
- **Receiving third-line audit findings** and running the corrective
  action follow-through, reported to the audit committee.
- **Joint audit-committee appearances** at least annually — the CAE
  reports on third-line findings; the head reports on second-line
  operating status and corrective-action closure; the audit committee
  hears both together.

An enterprise where the CAE and the head are not visibly aligned on
the AI audit programme is one where the audit committee will ask why.
An enterprise where the CAE and the head appear to be a single voice
is one where the third line's independence has quietly failed.

## The failure mode: operational-distance failure

*Operational-distance failure* is the single most common way a
second-line AI function loses credibility. It has two symmetric forms.

**Form A — too close.** The head, or the head's team, is embedded so
deeply with the first line that it is not credibly independent. The
head signs off on release packets that they helped author; the head is
the person the CAIO / CIO trusts to keep AI shipping; the second line
looks like a rubber stamp. Auditors, regulators, and the audit
committee eventually notice. Trust collapses when the first stop-
shipping decision is escalated and the head cannot demonstrably say no.

**Form B — too far.** The head, or the head's team, is so isolated
from the first line that they have no operational context, and their
challenge becomes stale. Model-card templates never get updated for
the reality of the codebase; risk classifications miss the real
failure modes; the second line becomes irrelevant. First line stops
inviting them to design reviews. When something goes wrong,
regulators find that the second line "existed" but never had ground
truth.

Both forms are lethal. The correct operating distance is: second-line
partners deeply embedded in first-line design conversations, briefing
back to the second-line chain of accountability daily; the head
personally reserving stop-shipping challenge and never authoring the
material being challenged; the AIMS operating with visible
non-conformities that get closed rather than hidden.

The IIA's 2020 update specifically calls out that first- and second-
line roles can blend, and that when they do, *management must be
explicit about who owns what*. If the head cannot answer "who owns
which risk decision here, in writing" for any first-line-plus-second-
line pairing, the distance is wrong.

## Cross-line failure modes to watch for

Two other cross-line pathologies show up in AI governance functions
and matter at level 60:

- **Second line drafting for first line.** The head's team writes the
  first-line's model card, then reviews it. This is not independent
  review; it is auto-conformance. When it happens once for time
  pressure and the head does not correct it, it happens twice, then
  becomes policy.
- **Third line evaluating second line's own controls without
  independence.** If the CAE's team was staffed from the head's team
  without a two-year cooling-off period, third-line independence is
  compromised on paper before any audit runs. The CAE (not the head)
  owns this staffing invariant, but the head must be alert to it and
  raise it with the audit committee if it slips.

## Reporting-line variations and the invariant

The head's solid-line reporting can vary — to the CAIO, to the CRO, to
the CIO / CTO / CDO, to the GC, or, in a small number of
enterprises, directly to the CEO. The dotted-line usually completes the
matrix (typically to CRO if solid-line is CAIO, or to CAIO if solid-
line is CRO).

The Three-Lines invariant is: **independent access to the audit
committee is preserved regardless of solid-line management.** The head
must be able to escalate to the audit committee without going through
the CAIO or CRO if the escalation *is about* CAIO or CRO behaviour —
for example, a stop-shipping decision that CAIO is overruling on
strategy grounds. That access is what preserves second-line
independence. It should be documented in the head's charter and in
the audit committee charter, and it should be tested annually
(a "walkaround" — the audit-committee chair calls the head directly,
without CAIO in the room, once a year).

## Composition with COSO ERM

Where the enterprise runs COSO ERM (2017) as the parent risk framework,
the Three Lines model is the operating model that COSO ERM assumes. COSO
defines the risk governance vocabulary — appetite, tolerance, capacity,
categories — and the Three Lines model defines who does what with it.
For AI, that means the head is the second-line executive who
operationalises the COSO risk-appetite statement for the AI domain,
using the level-50 architect's AI risk taxonomy.

## Example — a Three-Lines-shaped release-decision escalation

A high-risk AI system (say a resume screener in-scope for EU AI Act
Annex III and NYC Local Law 144) is nearing release. Second-line
review identifies a fairness metric outside the enterprise's tolerance
limits. What each line does:

- **First line (product owner + engineering lead)** — decides whether
  to ship. Wants to ship; disputes the metric.
- **Second line (head's team)** — provides the challenge; the metric
  is defensible; the tolerance limit is board-approved. The head's
  senior partner brings the challenge to the AI governance council.
- **Governance council (chaired by head)** — cannot resolve locally;
  the council escalates to the executive committee. The head briefs
  the CAIO and the CRO in parallel with a written recommendation to
  hold release until the fairness metric is remediated.
- **Executive committee (with CAIO / CIO / CTO / GC / CRO)** — decides
  to hold, with a two-week remediation window.
- **Third line (CAE)** — observes the process without intervening;
  post-decision, the CAE's team audits the escalation and the
  governance council minutes to confirm the operating model was
  followed.
- **Audit committee** — receives a written summary in the next
  quarterly board pack as a material governance event.

That is one release decision, correctly handled under the Three Lines
Model. Each line stayed in its lane. The head owned the challenge and
the escalation, not the release decision itself.

## Summary

- The IIA Three Lines Model (2020) places the head at level 60 as the
  second-line accountable executive for AI, coordinating with the
  first line and interfacing with the third line via the CAE.
- The head's seven-item second-line envelope — framework, AIMS, risk
  register, control operation, crosswalk, challenge, regulator
  interface, plus independent audit-committee access — defines the
  role's positional boundaries.
- The single largest failure mode is operational-distance failure —
  too close to first line (rubber stamp) or too far (irrelevant).
  Both are fatal; the correct distance is embedded but independent.
- The head must never draft first-line artefacts and then review them;
  must never merge with third-line staffing without cooling-off; and
  must never surrender independent audit-committee access to a
  solid-line manager.
- Under any reporting-line variation (CAIO, CRO, CIO, GC, CEO),
  independent audit-committee access is the invariant; it should be
  in writing in the head's charter and tested annually.
