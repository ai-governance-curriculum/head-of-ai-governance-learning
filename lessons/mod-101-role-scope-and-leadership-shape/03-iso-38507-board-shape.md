# ISO/IEC 38507 as the Board-Facing Shape

## Motivation

ISO/IEC 38507:2022 — *Information technology — Governance of IT —
Governance implications of the use of artificial intelligence by
organizations* — is unusual in the AI standards landscape in one
important way: it is a **board-facing** standard, published under the
ISO/IEC 38500-series family (which is the ISO/IEC standard series for
IT governance directed at the *governing body*). Where the AI RMF talks
to the second line, and where ISO/IEC 42001 talks to the AIMS operator,
ISO/IEC 38507 talks to the board and the executive that reports to the
board on AI.

For a Head of AI Governance at level 60, this is the standard that
defines *what the board holds the head accountable for*, phrased in
governance-body vocabulary that a director or an audit-committee chair
already speaks. It is the single most useful standard for translating
"what my function does" into "why the board should trust it," because
the standard was written to be understood by directors.

This chapter reads ISO/IEC 38507 as the definitional shape of the
board-facing responsibilities the head owns, and shows how it composes
with — but does not overlap — NIST AI RMF GOVERN
([[02-nist-ai-rmf-govern-leadership-shape]]) and ISO/IEC 42001.

## Core concept: the ISO/IEC 38500-family model

The ISO/IEC 38500 family models IT governance as a three-verb loop that
the governing body performs: **evaluate → direct → monitor**. The
governing body evaluates the current and future use of a technology
family, directs the preparation and implementation of plans and
policies to ensure use meets business objectives, and monitors
conformance to policies and performance against plans.

ISO/IEC 38507 takes that three-verb loop and specialises it for AI.
The standard is deliberately structured around what a *governing body*
does (not what a management team does), and specialises for AI at the
level of governance considerations, not implementation controls. Read
that way, the head of AI governance is the executive whose job is to
give the board *what it needs to* **evaluate → direct → monitor** AI
credibly.

## What ISO/IEC 38507 says the board must consider

The standard organises what the governing body must consider around
five clusters of decisions. Read the clusters as the five columns of the
head's board-facing responsibility map. (The precise language and
numbering in the standard is what you cite in a control catalog; here
we paraphrase for shape.)

- **Governance and stewardship of AI use.** Whether AI use aligns with
  the enterprise's values, purpose, and stewardship obligations —
  including obligations to customers, employees, communities, and
  wider society. The head's board-facing artefact: the AI use policy,
  the AI ethics posture, and the mapping from enterprise values to
  operating controls.
- **Policies for AI use, including risk appetite.** Whether the
  enterprise has articulated its position on AI risk and reward, and
  the appetite for particular AI risk classes. The head's board-facing
  artefact: the AI risk appetite statement, the risk-tolerance limits,
  and the portfolio heat map.
- **Culture and values.** Whether AI use is consistent with the
  enterprise's stated culture and values, and whether the workforce
  has the competence to use AI safely. The head's board-facing
  artefact: the workforce competence attestation, the culture-of-
  risk-management evidence set, the near-miss and psychological-safety
  metrics.
- **Compliance obligations for AI use.** Whether the enterprise meets
  its legal, regulatory, and contractual obligations for AI. The
  head's board-facing artefact: the cross-jurisdiction crosswalk
  status, regulator-engagement summary, and material-change register.
- **Risk of AI use, including reliance risk and third-party risk.**
  Whether the enterprise's AI risk exposures are known, measured,
  managed, and reported — including the risk that comes from *relying
  on* AI (automation bias, deskilling) and from third-party AI
  suppliers. The head's board-facing artefact: the risk register at
  portfolio cadence, the third-party AI vendor tiering and status,
  the incident logbook.

Each cluster is a column in the board's dashboard, and the head is the
executive who owns each column's evidence. Nothing in that list is
optional; nothing in that list is somebody else's.

## How ISO/IEC 38507 composes with NIST AI RMF and ISO/IEC 42001

The three standards address the same subject at different altitudes.
Understanding the composition is what stops the head from arguing about
"which standard to adopt" — the answer is all three, at different
audiences.

| Standard | Altitude | Primary audience | What the head delivers under it |
|---|---|---|---|
| ISO/IEC 38507 | Governing body | Board / audit committee / director | Board-facing evidence for the five clusters above; direction–monitoring cadence |
| NIST AI RMF | Second-line function | Head of AI Governance and function | GOVERN function operating shape; MAP / MEASURE / MANAGE per-system methodology sponsorship |
| ISO/IEC 42001 | Management system | AIMS operator and certification body | AIMS Statement of Applicability, operating calendar, non-conformity closure, management-review record; ISO/IEC 42006 audit-body quality |

The head's job is to run *all three* without confusing the audiences.
ISO/IEC 38507 answers "board, are we governing AI?" ISO/IEC 42001
answers "auditor, is our management system operating?" NIST AI RMF
answers "second line, is our risk process credible?"

At level 60, none of these three is optional. All three land on the
head. And the head's public identity — the standard used in the
board pack — is ISO/IEC 38507, because that is the standard the board
was written for.

## The five clusters, translated into the head's board pack

For each ISO/IEC 38507 cluster, the following are the specific
board-pack artefacts that discharge the head's board-facing
accountability. (Details on how to author each land in
[[mod-103-board-and-audit-committee-reporting]]; here we list the
mapping so the shape is clear.)

- **Governance and stewardship of AI use** →
  - AI use policy summary (one page)
  - Enterprise AI purpose statement, mapped from enterprise values to
    operating principles (one page)
  - Stakeholder-engagement summary (customer / employee / community
    engagement on AI use)
- **Policies for AI use, including risk appetite** →
  - AI risk appetite statement approved by the risk committee
  - Portfolio heat map by risk class (fairness, privacy, safety,
    security, reliability, transparency, human oversight, robustness)
  - Tolerance-and-limit breach register with remediation status
- **Culture and values** →
  - Workforce competence attestation (training completion, sub-
    populations, certifications held by first-line and second-line)
  - Near-miss and raise-a-concern report
  - Culture-of-risk-management pulse metric (if the enterprise runs
    one)
- **Compliance obligations for AI use** →
  - Cross-jurisdiction crosswalk status (green/amber/red for each
    obligation family under the level-50 architect's crosswalk)
  - Regulator-engagement summary (open matters, exams, filings under
    EU AI Act Article 72 and Article 73, sector filings)
  - Material-change register (regulations that have changed since
    the last board pack, with impact assessment)
- **Risk of AI use, including reliance and third-party** →
  - AI risk register at portfolio cadence (top-N risks)
  - Third-party AI vendor tiering, status, and incident summary
  - Incident logbook with severity, closure status, and lessons
    incorporated
  - Reliance-risk indicators (automation-bias monitors, deskilling
    signal where relevant)

Every artefact in that list has a named author, a cadence, and a
control-ID in the level-50 architect's evidence architecture. The head
does not author any of these from scratch each quarter; the head owns
the *cadence* and the *board-facing narrative*. The artefacts flow up
from the operating discipline of the AIMS.

## The "evaluate → direct → monitor" loop in practice

The three-verb loop from ISO/IEC 38500 is not decorative. In practice,
the head's job across the annual cycle is to give the board a *fresh*
opportunity to perform each verb:

- **Evaluate** — the annual AI strategy and risk-appetite review, at
  which the board (usually the full board plus the risk committee)
  evaluates the enterprise's AI trajectory against the five clusters.
- **Direct** — the direction-setting outputs of that review — approved
  policy updates, appetite-limit changes, budget authorisations —
  which the head then implements through the AIMS and reports on
  quarterly.
- **Monitor** — the quarterly board pack and the audit-committee
  deep-dive that let the board monitor conformance and performance,
  with the head as the executive reporting.

Failure to close any loop is a governance failure. Direction without
monitoring means the board approves policy that is not enforced.
Monitoring without direction means the board watches the numbers move
without ever changing appetite. Evaluation without direction or
monitoring means the annual review is theatre. The head's job is to
keep all three verbs alive.

## What ISO/IEC 38507 says the board *does not* do

An underrated feature of ISO/IEC 38507 is what it explicitly leaves to
management. The standard is a governance-body standard; it is not a
management-system standard. That means the board does not:

- Choose specific AI systems to buy, build, or discontinue (management
  decision under the CAIO / CIO / CTO scope).
- Run day-to-day AI risk-management processes (management under the
  head at level 60 and the architect at level 50).
- Author specific control content (level 50 delivers; level 60
  operates).
- Author regulator submissions or legal opinions (level 60 authors
  regulator submissions with GC; GC delivers legal opinion).

Knowing what is not board scope is what stops the head from over-
briefing. A board pack that contains implementation minutiae is
noise; a board pack that answers the five clusters is signal. The head
who reads ISO/IEC 38507 as the shape of the pack writes better board
material for having done so.

## Composition with COSO ERM and ISO 31000

The board's parent framework for enterprise risk oversight is COSO ERM
(2017) in many US enterprises and ISO 31000:2018 in many international
ones. ISO/IEC 38507 does not replace those; it is the AI-specific lens
on top of them. The head's job is to *map* the AI risk into the parent
framework's vocabulary so the audit committee and risk committee do
not have to learn a second set of nouns.

Concretely: if the enterprise runs COSO ERM, then the AI risk register
lines are mapped to COSO's risk-appetite / risk-tolerance / risk-
capacity vocabulary. If the enterprise runs ISO 31000, then the AI
risks are mapped to ISO 31000's likelihood-and-consequence taxonomy.
The head does not force the enterprise to speak ISO/IEC 42001 or NIST
AI RMF vocabulary in the board pack; the head speaks the parent-
framework vocabulary and uses ISO/IEC 38507 to say what is AI-specific
inside that vocabulary.

## Example — an ISO/IEC 38507-shaped audit-committee agenda

An audit-committee AI-risk deep-dive (say quarterly, 90 minutes), read
against ISO/IEC 38507's five clusters, might look like:

- Governance and stewardship of AI use (10 min): stewardship statement,
  any material changes to AI use aligned with enterprise values.
- Policies for AI use and risk appetite (20 min): risk appetite status,
  portfolio heat map, tolerance-and-limit breaches.
- Culture and values (10 min): workforce competence, near-miss report,
  raise-a-concern channel.
- Compliance obligations (20 min): crosswalk status, regulator
  engagement, material regulatory changes.
- Risk of AI use, including reliance and third-party (25 min): risk
  register, third-party status, incident logbook.
- Executive session (5 min): head with audit-committee chair alone.

Ninety minutes, five clusters, one head accountable. That is what
ISO/IEC 38507 looks like when a level-60 role runs it.

## Summary

- ISO/IEC 38507:2022 is the board-facing shape of AI governance,
  written for the governing body, structured around the ISO/IEC 38500-
  family evaluate → direct → monitor loop.
- The standard organises what the board must consider into five
  clusters — stewardship, policies and appetite, culture and values,
  compliance, and risk (including reliance and third-party) — each of
  which becomes a column in the head's board pack.
- ISO/IEC 38507 composes with NIST AI RMF and ISO/IEC 42001 without
  overlapping: 38507 speaks to the board, RMF to the second line,
  42001 to the AIMS operator and auditor.
- The head's job in ISO/IEC 38507 terms is to keep the board's
  evaluate → direct → monitor loop alive every year, and to speak the
  enterprise's parent-framework (COSO ERM or ISO 31000) vocabulary
  when doing so.
- The standard is deliberately silent on management execution — that
  boundary is what keeps the board pack signal-heavy and free of
  implementation noise.
