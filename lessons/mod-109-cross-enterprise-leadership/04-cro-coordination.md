# CRO Coordination Pattern — Composing the AI Risk Portfolio into Enterprise Risk

## Motivation

The AI risk portfolio the head runs is *not* a separate risk
program. It is a *portfolio* within the enterprise risk
management (ERM) framework the Chief Risk Officer owns. The
CRO owns the parent — ISO 31000 or COSO ERM, the enterprise
risk register, the appetite-tolerance-limit framework, the
risk-committee report line to the board, and the second-line
independence discipline across the enterprise (of which the
head's function is one instance). The head extends the parent
into AI: the AI-specific risk taxonomy, the AI-appetite
translation, the AI risk register that contributes rows into
the enterprise register, and the second-line challenge for
AI-specific first-line decisions.

The failure mode is a head who treats AI risk as sui generis
and refuses to compose it with the CRO's parent framework. The
CRO then reads the head as a rival second-line function, the
risk committee reads two overlapping risk portfolios, and the
audit committee reads a governance duplication that no one can
defend to the CFO. The other failure mode is the head who
copies the CRO's framework wholesale and produces AI risk work
that is generic risk work in AI-flavoured language, without the
substantive AI-specific challenge the enterprise needs.

The coordination pattern is what avoids both. It rests on a
composition discipline (the AI risk register composes into the
enterprise risk register), a shared language discipline (the
head uses the CRO's appetite / tolerance / limit vocabulary
faithfully), and a reporting-line discipline (in many
enterprises the head reports solid-line or matrixed into the
CRO, with independent audit-committee access preserved).

The pattern draws on ISO 31000:2018 (risk management —
guidelines), ISO/IEC 27005:2022 (information security risk
management), ISO/IEC 23894:2023 (AI risk management guidance),
COSO ERM 2017 (Enterprise Risk Management — Integrating with
Strategy and Performance), the Basel Committee's operational
risk framework where relevant to banking-sector enterprises,
and the IIA Three Lines Model (2020) that positions the head's
function within the enterprise's line-of-defence architecture.

## Core concept — composition, not annexation

The load-bearing move is *composition*. The AI risk portfolio
composes into the enterprise risk framework the way a subject-
matter risk portfolio composes with any other subject-matter
risk portfolio in a well-run ERM function. Cybersecurity risk
composes; conduct risk composes; operational risk composes;
credit risk composes (in banks); AI risk composes on the same
principle.

Composition means: the AI risk portfolio has its own taxonomy,
its own methodology, its own depth of analysis, and its own
governance forum (the AI Governance Council chaired by the
head, per chapter [[11-chairing-the-governance-council]]). But
its outputs — the top-of-portfolio risks, the appetite-breach
events, the material control failures — flow *up* into the
CRO's enterprise risk register on a common schema, at a common
cadence, in a common language. The CRO's enterprise risk
committee reads the aggregated view; the AI Governance Council
reads the disaggregated view; both views agree on the shared
data because the composition is faithful.

Annexation is what happens when the head builds an AI risk
program that is parallel to the enterprise risk program rather
than composing with it. The two programs use different
appetite frameworks; the AI risk register uses "critical /
material / general" while the enterprise register uses
"tier 1 / tier 2 / tier 3"; the reporting cadences are
misaligned; the risk committee reads two documents that seem
to describe the same enterprise but do not. The CRO ends up
having to reconcile the two before every risk-committee
meeting, which is the failure mode.

## The three coordination surfaces

### Surface 1 — the AI risk taxonomy composed with the enterprise risk taxonomy

The enterprise risk taxonomy is the CRO's artefact. It classes
risks by parent category (strategic, financial, operational,
compliance, reputational, and typically further sub-categories)
and provides the vocabulary the enterprise register uses. The
head's AI risk taxonomy is more granular in the AI dimension
and it references the enterprise taxonomy explicitly.

The interface is a mapping: each AI risk class in the head's
taxonomy maps to one or more enterprise risk classes in the
CRO's taxonomy. Examples:

- **AI-model performance risk** (accuracy degradation,
  distribution shift) maps to *operational risk — model
  performance* under the enterprise taxonomy; in banks
  specifically it also maps to *model risk* under the CRO's
  MRM sub-taxonomy.
- **AI-safety risk** (unsafe outputs, safety-critical failure
  modes) maps to *operational risk — safety* or, where the AI
  is embedded in a physical product, *product safety risk*.
- **AI-fairness risk** (disparate impact, prohibited-basis
  discrimination) maps to *compliance risk — fair-lending / fair-
  employment* and to *reputational risk*.
- **AI-privacy risk** (memorisation, unauthorised disclosure)
  maps to *compliance risk — privacy* and to *operational
  risk — data*.
- **AI-security risk** (prompt injection, model extraction,
  training-data poisoning) maps to *operational risk —
  cybersecurity* under the CISO adjacency (chapter 01).
- **AI-third-party risk** (foundation-model provider,
  RAG source, MLOps vendor) maps to *third-party risk*.
- **AI-legal-obligation risk** (EU AI Act non-compliance,
  sector-specific violations) maps to *compliance risk —
  regulatory*.
- **AI-governance risk** (governance-runtime failure, control-
  bypass) maps to *operational risk — governance*.

The mapping is joint-authored (head's level-50 architect and
the CRO's risk-taxonomy lead) and versioned in the CRO's
enterprise risk-framework document. When the CRO revises the
enterprise taxonomy, the AI mapping is revised in parallel;
when the head's function surfaces a new AI risk class, the
CRO's taxonomy either extends to accommodate it or the mapping
places it under an existing class.

Cadence: annual joint review at the enterprise risk framework
update; ad-hoc when a new AI risk class is surfaced. Joint
owner: CRO's risk-taxonomy lead and head's level-50 architect.

### Surface 2 — appetite, tolerance, and limit language

The CRO's appetite framework (see
[[mod-103-board-and-audit-committee-reporting]] chapter 03)
is the enterprise's articulation of the exposure the board
tolerates. It uses a common vocabulary — typically *appetite*
(the level the enterprise chooses), *tolerance* (the level
beyond which the enterprise is not comfortable), *limit* (the
level beyond which the enterprise will not go, often a
regulatory floor or a board-imposed ceiling).

The head uses the same vocabulary. Every AI-scope appetite,
tolerance, and limit statement uses the CRO's terminology,
maps to a specific clause in the CRO's appetite framework, and
is ratified in the CRO's annual appetite-review cycle. The
head does not invent AI-specific risk-language variants — no
"AI risk envelope", no "safety headroom", no "innovation
tolerance". If the AI-specific concept does not map to the
CRO's vocabulary, the head negotiates with the CRO to extend
the vocabulary; the head does not build a parallel one.

Examples:

- **Control-effectiveness appetite** (from
  [[mod-103-board-and-audit-committee-reporting]] chapter 03):
  the CRO's appetite band for the control-testing pass rate
  is the source; the KRI threshold on control-testing pass
  rate (KRI 1 in [[mod-107-program-measurement-and-maturity]]
  chapter 01) derives from that band.
- **AI-incident appetite.** The CRO's operational-loss
  appetite framework provides the parent; the head negotiates
  the AI-specific translation — how many material AI
  incidents per year is the appetite, at what severity, with
  what estimated impact — and the AI-incident appetite is a
  sub-clause of the CRO's operational-loss appetite.
- **AI-third-party concentration appetite.** The CRO's
  third-party concentration appetite (typical in banks under
  SR 23-4 / OSFI B-10) sits as parent; the AI-third-party
  concentration appetite (specifically for foundation-model
  providers and evaluation-suite vendors) is a sub-clause the
  head co-authors with the CRO's third-party-risk lead.

The rule the head holds: *no AI-scope threshold is set that
departs from the CRO's appetite framework without the CRO in
the room ratifying it*. This is the rule that keeps the CRO on
the head's side during a KRI breach conversation — the CRO
ratified the threshold and defends it with the head.

Cadence: annual at the CRO's appetite review; ad-hoc when a
new AI-specific appetite is proposed. Joint owner: CRO's
appetite-framework lead and head's level-50 architect, with
the head personally accountable for the AI-scope translation.

### Surface 3 — the enterprise risk register composition

The enterprise risk register is the CRO's artefact. It lists
the enterprise's top risks, their assessed exposure, their
current mitigation status, their KRI status, and the
accountable executive per risk. It goes to the risk committee
at the risk committee's cadence (typically quarterly).

The AI risk portfolio composes into the enterprise register as
follows:

- **AI-portfolio-material risks appear in the enterprise
  register.** Not every AI risk appears; the CRO's threshold
  for enterprise-register appearance is applied (typically
  risks that could produce material financial, regulatory, or
  reputational loss). The head's function is accountable for
  proposing which AI risks meet the threshold; the CRO's risk
  team ratifies.
- **The head is the named accountable executive** for each AI
  risk in the enterprise register. The head does not delegate
  this accountability to the level-50 architect; the register
  names the head personally.
- **The AI-portfolio-summary view** (all AI risks aggregated)
  appears as a single row in the enterprise register, with a
  link to the head's detailed AI risk register. This is the
  composition pattern — the enterprise register carries the
  summary; the AI register carries the detail.
- **KRI thresholds ride the enterprise register's convention.**
  Where an AI risk's KRI is threshold-triggered (see
  [[mod-107-program-measurement-and-maturity]] chapter 01),
  the enterprise register's RAG convention is what the risk
  committee reads.
- **Escalation to the enterprise register.** When an AI risk
  moves in severity or appears newly (e.g., a foundation-
  model provider is de-supported, triggering a
  third-party-concentration event; a new incident class
  surfaces), the head's function nominates the risk to the
  enterprise register on the CRO's schedule.

Cadence: quarterly at the risk-committee cycle; ad-hoc on
material AI-side developments. Joint owner: CRO's enterprise
risk-register lead and head's level-50 architect, with the
head personally as accountable executive for each named AI
risk.

## The reporting-line pattern

In many enterprises, the head reports solid-line or matrixed
into the CRO. The reporting line is not the coordination
pattern; the coordination pattern above holds whether the head
reports to the CRO, the CEO, the CAIO, or elsewhere. But the
reporting line has practical implications the head navigates.

**Where the head reports solid-line to the CRO.** The head is
a direct report; the CRO is the head's manager in the
performance-management sense; the head's function budget is
inside the CRO's function budget. The advantages: risk-side
integration is native, appetite calibration is a working
conversation not a negotiation, second-line independence has a
clear organisational anchor. The disadvantages: the head has
less direct access to the CEO and, without preserved audit-
committee access, the head can be filtered by the CRO on
material risk-committee reporting. The pattern the head
insists on: independent audit-committee access preserved by
charter, executive-session rights preserved, direct
communication with the audit-committee chair on material
issues preserved.

**Where the head reports matrixed to the CRO and solid-line to
the CAIO or CEO.** More common in enterprises with a strong
CAIO. The head coordinates deeply with the CRO on risk
substance but sits outside the CRO's function organisationally.
The pattern: an explicit matrixed-report protocol — what the
CRO expects from the head (appetite ratification, register
composition, second-line challenge on AI-specific first-line
decisions), what the CAIO / CEO expects, and how disagreements
between them are resolved.

**Where the head reports solid-line to the CEO.** Less common
at level 60 but present in some enterprises. The head has
direct executive access; the risk-side integration is
authored by the coordination pattern in this chapter, not by
the reporting line.

In all cases: the *head is a second-line function*. This is
the invariant that the reporting line does not change. The
head produces second-line challenge on first-line AI decisions;
the head has an audit-committee-visible reporting line for
second-line-material events; the head coordinates with the CAE
on third-line audit engagement (see chapter
[[05-cae-coordination]]).

## The interface document

Consolidated in a single interface document co-signed by the
head and the CRO, ratified in the CxO adjacency map. The
document has, at minimum:

1. **Composition principle.** The AI risk portfolio composes
   into the enterprise risk framework; it does not run as a
   parallel program.
2. **Taxonomy mapping.** The joint mapping between the AI risk
   taxonomy and the CRO's enterprise risk taxonomy.
3. **Appetite / tolerance / limit vocabulary.** The shared
   vocabulary; the requirement that AI-scope thresholds derive
   from the CRO's appetite framework and are ratified by the
   CRO.
4. **Enterprise risk register composition.** How AI-portfolio-
   material risks appear in the enterprise register, who the
   accountable executive is, how KRI thresholds route, how
   escalation works.
5. **Reporting-line specifics.** Whether the head reports
   solid-line, matrixed, or otherwise; the invariants
   preserved regardless (second-line status, independent
   audit-committee access, executive-session rights).
6. **The escalation ladder.** When the composition breaks —
   an AI risk that the head believes belongs in the
   enterprise register but the CRO's team excludes; a
   threshold the CRO does not ratify but the head believes is
   appetite-relevant; a matrixed-reporting disagreement —
   how the head and the CRO escalate. Typically: head-and-CRO
   peer conversation, then the CEO or the audit-committee
   chair.
7. **The joint audit-committee / risk-committee appearance.**
   Once a year, the head appears jointly with the CRO on the
   risk-committee's AI-and-risk review, and jointly with the
   CAE on the audit-committee's programme-effectiveness
   review. Joint appearances are the discipline that keeps
   the composition honest.
8. **The review cadence.** Annual review of the interface
   document itself; ad-hoc on material changes to the
   enterprise risk framework.

## Anti-patterns the head does not permit

**The parallel appetite framework.** The head authors an AI-
scope appetite framework that uses its own vocabulary and
its own bands, independent of the CRO's. The risk committee
reads it as duplication and the CRO reads it as encroachment.
The remedy is: shared vocabulary, and every AI-scope
threshold ratified by the CRO.

**The enterprise-register bypass.** The head runs a top-ten
AI risk list that never composes into the CRO's enterprise
register. The enterprise register goes to the risk committee
without the AI portfolio's material risks, and the risk
committee is under-informed on AI exposure. The remedy is:
material AI risks appear in the enterprise register on the
CRO's schedule.

**The unratified threshold.** The head sets a KRI threshold
without the CRO's ratification and publishes it in board
reporting. The CRO challenges the threshold at the risk
committee and the head loses the argument in the room. The
remedy is: no threshold is published unratified; the
threshold-calibration workbook is a working session with the
CRO, not a fait accompli.

**The reporting-line abuse.** The head, reporting solid-line
to the CRO, escalates to the audit-committee chair on issues
the CRO would have engaged constructively on. The CRO reads
this as bypass and the trust the reporting line requires is
damaged. The remedy is: the audit-committee-access invariant
exists for genuinely second-line-material events (independence
threats, retaliation concerns, material dissent on risk
matters the CRO refuses to escalate), not as a routine
escalation lever.

**The composition-as-copy failure.** The head produces an AI
risk register that is a copy of the enterprise risk register
with AI-flavoured names, and the AI-specific substance is
absent. The AI Governance Council reads it as generic risk
work; the audit committee reads it as duplication. The remedy
is: the AI risk register is granular in the AI dimension
(training-data poisoning as a specific class, prompt
injection as a specific class, foundation-model
concentration as a specific class), and the composition is
in the summary rows that flow up.

## Composition with adjacent modules

- The **CxO adjacency map** in
  [[mod-101-role-scope-and-leadership-shape]] chapter 06 is
  the parent boundary document.
- The **risk-appetite framework** in
  [[mod-103-board-and-audit-committee-reporting]] chapter 03
  is the enterprise appetite that AI-scope thresholds derive
  from.
- The **AI risk register** in [[mod-102-running-the-program]]
  chapter 03 is the head's register that composes into the
  enterprise register.
- The **KRI/KPI portfolio** in
  [[mod-107-program-measurement-and-maturity]] chapter 01 is
  where the CRO-ratified thresholds appear as measurable
  signals.
- The **CAE coordination** in chapter 05 of this module is
  where third-line assurance engages both the CRO's function
  and the head's function.
- The **incident-leadership discipline** in
  [[mod-110-incident-leadership]] carries incident-driven
  risk-register updates that flow through the composition
  pattern.

## Summary

- The AI risk portfolio *composes* with the CRO's enterprise
  risk framework; it does not run as a parallel program.
  Composition means shared taxonomy, shared appetite
  vocabulary, and register-level composition, with the AI
  portfolio's detail retained in the head's register and its
  summary in the enterprise register.
- Three coordination surfaces carry the work: taxonomy mapping
  (AI-risk classes mapped to enterprise-risk classes),
  appetite / tolerance / limit language (the head uses the
  CRO's vocabulary and derives every AI-scope threshold from
  the CRO's appetite framework), enterprise register
  composition (material AI risks appear in the enterprise
  register with the head as named accountable executive).
- The reporting-line pattern is a practical implementation
  detail — solid-line to CRO, matrixed, or solid-line to CEO
  — with the invariants preserved regardless (second-line
  status, independent audit-committee access, executive-
  session rights).
- Five anti-patterns to refuse: parallel appetite framework,
  enterprise-register bypass, unratified threshold, reporting-
  line abuse, composition-as-copy failure.
- The interface document — co-signed by head and CRO — is
  ratified in the CxO adjacency map, reviewed annually, and
  the head and CRO appear jointly at the risk committee's
  AI-and-risk review once a year.
- The rule that saves the head at the risk committee: *no
  AI-scope threshold is set without the CRO in the room
  ratifying it*. Follow the rule and the CRO defends the
  threshold with the head; break it and the CRO defends the
  threshold against the head.
- Chapter [[05-cae-coordination]] turns to the audit
  adjacency — the third-line CAE's programme, the joint
  audit-committee appearance rhythm, the IIA discipline
  under which the CAE operates independently of both the
  head and the CRO.
