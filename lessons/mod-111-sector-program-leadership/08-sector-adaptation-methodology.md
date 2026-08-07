# The Sector-Adaptation Methodology at Leadership Scope

## Motivation

Chapters 01-07 walked seven sectors — banking, insurance, health
system, pharmaceutical, public sector and federal contractor,
frontier lab, and critical infrastructure — one at a time. That
walk-through is where the head of AI governance sees the specific
regulators, instruments, counterparts, and cadences of each sector.
It is not the head's methodology. It is content the methodology
operates on.

The methodology itself lives at leadership scope. The
senior-ai-governance-architect (the paired level-50 role — see
[[mod-101-role-scope-and-leadership-shape]] chapter 04) is
accountable for the enterprise operating design that produces
sector blueprints — the concrete control frameworks, evidence
pipelines, and workflow patterns the enterprise runs. The head
inherits those blueprints and adapts them at three specific
surfaces the architect does not own:

1. The sector-specific regulator-engagement pattern the enterprise
   commits to (which regulator gets what tone, what channel, what
   escalation stance, on what cadence).
2. The board-reporting cadence and content adjustments the sector
   requires (Quality Committee for a health system; Safety and
   Security Committee for a frontier lab; NAIC bulletin state-by-
   state view for an insurer; NERC CIP posture line for a bulk-
   electric operator).
3. The external-positioning posture the enterprise takes into
   voluntary codes, industry bodies, and public commentary that
   the sector's public expectations shape.

This chapter names the adaptation methodology, walks through how it
works, and closes the module by tying the sector work back into the
running program from [[mod-102-running-the-program]] and the board-
reporting shape from [[mod-103-board-and-audit-committee-reporting]].

## Core concept — the architect-designed blueprint versus the head-adapted engagement pattern

The level-50 senior-ai-governance-architect produces sector
blueprints. A banking blueprint specifies the AI-inside-MRM control
framework, the SR 11-7-aligned validation workflow, the SR 23-4
third-party AI attestation pattern. A pharma blueprint specifies
the GxP-aligned AI validation approach, the PCCP submission
workflow, the pharmacovigilance-AI validation pattern. A frontier-
lab blueprint specifies the capability-threshold evaluation
workflow, the mitigation-standard implementation pattern, the
publication pipeline.

The head does not re-author the blueprint. The head:

- Reviews the blueprint against the enterprise's actual regulatory
  footprint, org design, and stakeholder geography.
- Adopts the blueprint where it fits.
- Requests architect-authored refinement where the blueprint needs
  to be sharpened for a specific instrument, jurisdiction, or
  workflow.
- Layers the head-scope adaptations on top: the regulator-
  engagement pattern (who fronts each regulator, at what tone, on
  what cadence, with what escalation posture), the board-reporting
  content and cadence tuned to the sector's board conventions, and
  the external-positioning posture the sector expects.

The separation preserves the operating architect's authority over
control design and the head's authority over external posture.
Where the two functions blur, the enterprise experiences the same
failure mode a bank experiences when MRM and AI governance blur
without a written protocol: split answers at examination, unclear
accountability at incident, inconsistent evidence pipelines.

## The four-step adaptation methodology

### Step 1 — read the sector against the architect's baseline blueprint

The head reads the architect's baseline blueprint against three
lenses.

- **Instrument coverage.** Does every material sector instrument
  the head reads under chapters 01-07 have a corresponding control
  or evidence element in the blueprint? Where a gap appears
  (Colorado Regulation 10-1-1 was signed after the last blueprint
  refresh; NYDFS Circular Letter No. 7 emerged as a new
  instrument), the head opens a change request with the architect.
- **Jurisdictional coverage.** Does the blueprint's evidence
  pipeline serve every jurisdiction the enterprise operates in?
  Where the enterprise has expanded footprint (opened a UK
  subsidiary that brings PRA SS1/23 into scope for a bank; opened
  a Colorado line of business that brings Regulation 10-1-1 into
  scope for an insurer), the head opens a change request with the
  architect.
- **Workflow fit.** Does the blueprint's workflow structure align
  with the enterprise's actual org design and existing operating
  cadences? Where friction exists (the blueprint assumes an MRM
  function co-located with AI governance but the enterprise runs
  them separately; the blueprint assumes a Quality function that
  the enterprise does not have), the head negotiates the workflow
  shape with the architect and adapts the affected workflow
  chapters (see [[mod-102-running-the-program]] chapter 04).

### Step 2 — design the sector-specific regulator-engagement pattern

The regulator-engagement pattern from chapter 04 of [[mod-104-regulator-engagement]]
is generic across all sectors. In the head's sector-adaptation
work, the pattern is instantiated for each regulator the sector's
chapter identifies. Per regulator:

- Named enterprise counterpart (individual and function).
- Formal channel (letter, examination, submission, MOU).
- Informal channel (industry-body, trade association, advisory
  committee, speech circuit).
- Peer-fronting decision (who fronts routine; who fronts on
  escalation).
- Cadence.
- Escalation stance pre-decided at each tier of the sector-specific
  escalation ladder.

The instantiation is the head's work, not the architect's. The
architect's blueprint may name the regulator as in-scope; the head
names how the enterprise engages the regulator.

### Step 3 — adapt the board-reporting cadence and content to sector conventions

The generic board-reporting shape from [[mod-103-board-and-audit-committee-reporting]]
applies across all sectors. Sector-specific adaptations include:

- **Health system.** The Quality Committee (or Quality and Compliance
  Committee) receives clinical-governance content directly; the
  Audit Committee receives the Regulatory and Compliance cluster.
  AI-in-clinical-decisioning content splits accordingly.
- **Banking.** The Risk Committee — often distinct from the Audit
  Committee at large banks — receives the MRM and third-party-risk
  content; the Audit Committee receives internal-control content;
  AI-specific reporting maps to both.
- **Insurance.** State-DOI examination status is reported per
  state or per aggregation-rule cluster; the board pack's
  regulator-engagement cluster carries the state-by-state view
  where the state-DOI footprint is large.
- **Pharmaceutical.** The R&D or Science and Technology Committee
  receives AI-in-drug-development content; the Audit Committee
  receives GxP and regulatory-affairs content.
- **Federal agency.** The AI Governance Board (under M-25-21) is
  the primary reporting body, chaired by the Deputy Secretary
  or designee; the Federal CAIO's reporting cadence is set by
  the memorandum, not by charter negotiation.
- **Federal contractor.** The Audit Committee receives the
  federal-customer regulatory posture; the Business Development
  Committee (if the enterprise has one) receives the CAIO
  relationship map.
- **Frontier lab.** A dedicated Safety and Security Committee
  (or its equivalent) is the primary body for RSP / Preparedness /
  FSF content; the Audit Committee receives compliance content.
- **Critical-infrastructure operator.** The Safety Committee or
  Risk Committee receives OT AI, reliability, and sectoral-
  regulator content; the Audit Committee receives the compliance
  and incident-notification content.

The board-reporting adaptation is a design artefact the head
authors and the audit committee (or the equivalent primary
committee) ratifies. The adaptation is stable across quarters —
regenerating the reporting structure quarterly is a governance
failure — but is refreshed when material sector or footprint change
requires it.

### Step 4 — adapt the external-positioning posture

The generic external-positioning discipline from [[mod-106-external-positioning-and-voluntary-codes]]
applies across all sectors. Sector-specific adaptations include:

- **Banking.** Bank Policy Institute, ABA, RMA, IIF, and equivalents
  are the primary industry-association surfaces. FSB and FSOC AI
  workstreams are policy-adjacent. AICPA / IFAC on AI risk
  management is external-auditor-adjacent.
- **Insurance.** ACLI, NAMIC, PCI (now APCIA), Reinsurance
  Association of America, and equivalents are primary industry
  associations. IAIS at the international level.
- **Health system.** AHA, FAH, AMGA, and specialty-society AI
  positions are primary industry surfaces. Health Sector
  Coordinating Council (HSCC) on cyber.
- **Pharmaceutical.** PhRMA, BIO, EFPIA, IFPMA, and equivalents.
  ICH as the international harmonisation body.
- **Federal agency.** The Federal CAIO Council under M-25-21 is
  the primary cross-agency coordination surface. Interagency AI
  policy processes through OMB, OSTP, and NSC.
- **Federal contractor.** ITI, BSA, Chamber of Commerce, plus
  sector-specific vendor coalitions.
- **Frontier lab.** Frontier Model Forum, Partnership on AI,
  MLCommons, IEEE AI standards work, ISO/IEC JTC 1/SC 42, White
  House Voluntary Commitments, Seoul Commitments.
- **Critical-infrastructure operator.** Sector-specific ISACs
  (Information Sharing and Analysis Centers), sectoral coordinating
  councils (SCCs), and cross-sector coordination through the
  Critical Infrastructure Partnership Advisory Council (CIPAC).

The head's external-positioning portfolio inventory (from
[[mod-106-external-positioning-and-voluntary-codes]] chapter 02)
includes sector-specific bodies alongside cross-sector bodies. Each
body has a signed / considered-and-declined / under-consideration /
watched status recorded, and each active engagement has an owner.

## The multi-sector enterprise — reconciling the adaptations

Some enterprises operate in more than one sector. A bank with an
insurance subsidiary operates under banking and insurance sector
frameworks. A hospital that also markets an in-house-developed
diagnostic AI operates under hospital-accreditation and FDA-device
frameworks. A telecom that owns a media property operates under
telecom-critical-infrastructure and (in some cases) consumer-AI
frameworks. A defense contractor selling to civilian agencies
operates under federal-contractor and sector-specific regulator
frameworks.

The head's methodology for a multi-sector enterprise is:

1. Every applicable sector chapter's adaptation is executed. No
   sector is skipped because "the primary sector is banking" or
   "the primary market is health."
2. Where adaptations overlap on the same instrument or the same
   counterpart, the more stringent adaptation prevails and is
   applied enterprise-wide, unless the enterprise's group structure
   isolates the entity.
3. The board-reporting adaptation reflects the multi-sector reality
   — a group Audit Committee reads the aggregate posture; entity-
   level boards (a bank subsidiary board, an insurance subsidiary
   board) read the entity-specific slice.
4. The external-positioning portfolio inventory includes each
   sector's industry-association surface, and cross-portfolio
   consistency is a live consideration (a public position in the
   banking sector may need to be reconciled with a public position
   in the insurance sector).

The multi-sector head does not run multiple parallel programs. The
head runs one program that is instantiated correctly per sector.
That is the value of adaptation as methodology: it is the same
head, running the same underlying discipline, adapting to each
sector's specifics without losing coherence.

## The methodology's fit with the level-40 sector-adaptation work

The senior-ai-governance-architect at level 50 designs the
enterprise operating architecture. The head at level 60 adapts the
regulator-engagement pattern, board-reporting cadence, and
external-positioning posture on top of that architecture. The
level-40 architect-under-architect role (the individual contributor
in the paired track — see [[mod-101-role-scope-and-leadership-shape]])
executes sector-specific technical work inside the architect's
blueprint.

The three levels compose in a specific stack:

- Level 40 authors the technical implementation of a sector
  control (the SR 11-7-aligned validation package for a specific
  banking AI model; the GMLP-aligned lifecycle documentation for
  a specific FDA submission).
- Level 50 authors the sector blueprint (how SR 11-7 alignment is
  achieved enterprise-wide; how GMLP-aligned documentation is
  produced enterprise-wide).
- Level 60 (the head, this chapter) authors the regulator-
  engagement pattern, the board-reporting adaptation, and the
  external-positioning posture for the sector, and holds the
  accountable-executive tier for the sector's overall regulatory
  posture.

The head does not do level-40 or level-50 work. The head does not
delegate level-60 work to level-40 or level-50 roles. The
enterprise's governance quality depends on the three levels
staying in their respective scopes and communicating cleanly
across the boundaries.

## Refreshing the adaptation — the cadence question

The sector-adaptation methodology is not a one-time exercise. It
is refreshed on a cadence that reflects the pace of change in each
adapted surface.

- Regulator-engagement pattern per regulator: reviewed quarterly
  as part of the regulator-inventory refresh in [[mod-104-regulator-engagement]]
  chapter 04, refreshed materially when a new instrument, a new
  regulator counterpart, or a status change requires it.
- Board-reporting cadence and content: reviewed annually with the
  audit committee (or the equivalent primary committee), refreshed
  materially when the enterprise's board structure changes, the
  sector's board conventions shift, or the reporting design
  produces a boardroom question the head could not answer.
- External-positioning posture: reviewed annually against the
  portfolio inventory in [[mod-106-external-positioning-and-voluntary-codes]]
  chapter 02, refreshed materially when a new industry body
  emerges, an existing body's positioning shifts, or the enterprise's
  public commitments require it.
- The architect's underlying blueprint: refreshed on the
  architect's own cadence; the head reads the refresh, executes
  the adaptation implications, and re-ratifies with the audit
  committee where the material.

## The failure modes the methodology is designed to prevent

The adaptation methodology exists to prevent five specific failure
modes.

1. **Framework transplantation.** Taking a banking framework and
   applying it to an insurer; taking a pharma framework and
   applying it to a health system. The failure appears as
   examiners reading the framework as unfamiliar and unresponsive
   to their sector's actual expectations. The methodology
   prevents this by grounding each sector's adaptation in the
   sector's own chapter and instrument set.
2. **Framework proliferation.** Running seven parallel governance
   frameworks because the enterprise operates in seven sectors.
   The failure appears as inconsistent evidence, uncoordinated
   external posture, and confused stakeholders. The methodology
   prevents this by grounding the enterprise in one program that
   is adapted per sector.
3. **Board-reporting misfit.** Producing an audit-committee pack
   in the generic shape from [[mod-103-board-and-audit-committee-reporting]]
   without adapting to the sector's actual board structure. The
   failure appears as directors reading a pack that does not match
   what their committee is actually accountable for. The
   methodology prevents this by naming the sector-specific board
   adaptations in step 3.
4. **External-positioning drift.** Signing onto a voluntary code
   or joining an industry body without checking against sector
   expectations, or standing outside a sector's expected
   engagement without a documented rationale. The failure appears
   as sector stakeholders reading the enterprise as either
   opportunistic (signing without commitment) or absent (missing
   from where the sector expects to see the enterprise). The
   methodology prevents this by grounding the external-positioning
   portfolio in each sector's expected surfaces.
5. **Head-architect blur.** The head running programme-design
   decisions the architect should run, or the architect fronting
   regulator relationships the head should front. The failure
   appears as the enterprise experiencing inconsistent
   accountability and the board unable to answer "who is
   accountable for X." The methodology prevents this by keeping
   the three-level scope stack (level 40, level 50, level 60)
   explicit.

## Summary

- The enterprise operating design (control frameworks, evidence
  pipelines, workflow patterns) comes from senior-ai-governance-
  architect (level 50) sector blueprints. The head (level 60)
  adapts the regulator-engagement pattern, board-reporting
  cadence, and external-positioning posture on top.
- The four-step adaptation methodology: read the sector against
  the architect's baseline blueprint; design the sector-specific
  regulator-engagement pattern per regulator; adapt board-
  reporting cadence and content to the sector's board conventions
  (Quality Committee for health; Risk Committee for banking;
  R&D Committee for pharma; Safety and Security Committee for
  frontier lab; sector-specific bodies elsewhere); adapt the
  external-positioning posture to the sector's expected surfaces.
- A multi-sector enterprise runs one program instantiated
  correctly per sector, not multiple parallel programs. Where
  adaptations overlap, the more stringent prevails and is applied
  enterprise-wide unless group structure isolates the entity.
- The level-40 / level-50 / level-60 scope stack must remain
  explicit — level 40 implements technically, level 50 designs
  blueprints, level 60 adapts external posture and holds
  accountability. Blur between levels produces board-visible
  accountability failures.
- The methodology is refreshed on cadences appropriate to each
  surface: regulator-engagement quarterly, board-reporting
  annually, external-positioning annually, architect-blueprint
  refresh on the architect's own cadence.
- The methodology prevents five failure modes: framework
  transplantation, framework proliferation, board-reporting
  misfit, external-positioning drift, and head-architect blur.
  Each failure has a governance-visible signature; the methodology
  addresses each at its root.
- With the methodology in place, the sector chapters 01-07 stop
  being seven separate walk-throughs and become seven instances
  of the same underlying leadership discipline. That is what
  makes sector-program leadership a leadership skill rather than
  a sector-specific specialisation.
