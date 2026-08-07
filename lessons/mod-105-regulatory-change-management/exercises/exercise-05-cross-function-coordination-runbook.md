# exercise-05: Cross Function Coordination Runbook

**Estimated effort:** 2 hours

## Objective

Author the **cross-function coordination runbook** the head runs
for a material regulatory-change rollout — the artefact that keeps
six coordination lanes running in step across peers the head does
not manage. The runbook is the head's own operating discipline
turned into a document a delegate can pick up cold and use.

The runbook has the six lanes chapter 05 names — the level-50
architect and product / engineering (lane A); legal / GC (lane B);
procurement (lane C); HR, L&D, and Chief Compliance (lane D);
communications and IR (lane E); adjacent CxO peers (lane F, which
covers CISO, CIO / CTO / CDO, CPO / DPO, CRO, CAE, CFO). Each lane
has a named peer, a specific artefact exchange (in and out from
the head's side), an SLA on the exchange, a named forum for
adjudicating disagreement, and the coordination-pack view that
holds the whole together.

The deliverable is two-part. Part one is the runbook itself — the
six-lane operating document. Part two is the coordination pack for
one specific in-flight regulatory change, populated against the
runbook. Together they show the head can both design the
coordination discipline and operate it against a specific scenario.

The runbook has to survive two stress tests. First, a functional
peer (CIO / CCO / CHRO) reads their own lane and can see their
inbound artefact ask, their outbound expectation, their SLA, and
the forum where disagreement lands — without the head having to
brief them. Second, a governance-council chair (the head) can run
a monthly coordination review against the pack in 45 minutes and
identify which lanes are at risk and which need escalation.

## Prerequisites

- Chapter [05](../05-cross-function-coordination.md) — the six-
  lane coordination shape, the artefact-exchange discipline, the
  forum discipline, and the three anti-patterns — read and
  internalised.
- Chapter [03](../03-change-management-plan-shape.md) — the
  seven-lane change-management plan the coordination runbook
  operates against. Exercise 03's plan is a strong prerequisite
  scenario.
- Chapter [04](../04-speed-versus-readiness-tension.md) — the
  compliance-date posture the head defends across the four
  rooms; several of the six lanes carry the posture into their
  own domain (procurement into supplier communication, HR into
  training substance, communications into external posture).
- [[mod-101-role-scope-and-leadership-shape]] chapter 04 (IIA
  Three Lines Model), chapter 06 (CxO adjacency map), chapter 07
  (downward engagement contract with the level-50 architect).
- [[mod-102-running-the-program]] chapter 01 (AI Governance
  Council) — the head's own forum where lane-A disagreements
  land.
- [[mod-103-board-and-audit-committee-reporting]] chapters 02
  and 04 — audit-committee deep-dive and CxO sign-off flow that
  several lanes feed into.
- [[mod-108-leading-the-governance-function]] — the level-50
  architect and level-15 analyst hire-and-role architecture.
- [[mod-109-cross-enterprise-leadership]] — the CISO, CIO / CTO
  / CDO, and CPO / DPO coordination patterns that lane F leans
  on.
- A specific in-flight regulatory change to populate the
  coordination pack against. Reuse the exercise-03 or exercise-
  04 scenario for continuity across the module.

## Steps

1. **Enterprise context and scenario setup.** Author the short
   header — enterprise sector, jurisdictional footprint, the
   regulatory change the coordination pack is populated
   against (regulator, obligation citation, effective date,
   `<!-- needs-research: ... -->` where the effective date is
   uncertain), the head's coordination-desk owner (typically
   the desk owner from exercise 02).
2. **Lane A — level-50 architect and product / engineering.**
   Author the lane specification and the coordination-pack
   entry:
   - Named peer(s): the level-50 architect (named role), the
     head of product AI (named role), the head of engineering
     AI (named role).
   - Head-to-peer artefacts: the prioritised interpretation
     output (exercise 02), the GC opinion reference and any
     drafting constraints, the head's compliance-date posture
     (exercise 04) so the architect knows which changes need
     engineering ready by the date versus which land in a
     transition window.
   - Peer-to-head artefacts: the crosswalk delta, the control-
     library update, the engineering-impact sketch.
   - SLA: weekly working cadence with the architect; formal
     handoff at each of the seven interpretation-workflow steps
     that touches the architect.
   - Forum for disagreement: AI Governance Council (chair: the
     head). Escalation to the CIO / CTO / CDO operating
     committee or, for enterprise-scale changes, the executive
     committee.
   - Rule of thumb: any regulatory change requiring more than
     two sprints of engineering work is discussed with the
     head of engineering personally before the change-management
     plan is authored.
   Populate the pack entry with a current-status snapshot for
   the scenario (what artefact is due when, current status,
   any disagreement in flight).
3. **Lane B — legal (GC) and outside counsel.** Author the
   lane specification:
   - Named peer: General Counsel; where relevant, the outside
     counsel workstream lead (with the note that outside
     counsel is engaged through GC, not directly by the head).
   - Head-to-GC artefacts: the packaged obligation (chapter 02
     step 2), the change-management plan draft (chapter 03),
     the compliance-date posture proposal (chapter 04),
     regulator-facing draft artefacts before they go out.
   - GC-to-head artefacts: the interpretive opinion on the
     packaged obligation, ongoing review of drafting, the
     defensive-posture memo supporting the compliance-date
     posture, coordination on the supervisory-dialogue posture.
   - SLA: GC opinion turnaround (typically 14 days from
     packaging for active items, faster for priority items);
     regulator-facing draft review turnaround (typically 5
     working days).
   - Forum for disagreement: joint session with GC, written
     statement of disagreement following
     [[mod-104-regulator-engagement]] chapter 07 discipline;
     GC's view prevails on legal interpretation, head's view
     prevails on technical fact.
   - The head-and-GC boundary is called out explicitly: no
     back-channel to outside counsel; head does not paraphrase
     GC's opinion in downstream artefacts.
   Populate the pack entry for the scenario.
4. **Lane C — procurement and the supplier base.** Author the
   lane specification:
   - Named peer: head of procurement (named role); the
     specific procurement analyst assigned to AI-supplier
     contracts.
   - Head-to-procurement artefacts: the packaged obligation with
     attachment analysis focused on supplier surfaces; the GC
     opinion and GC-imposed drafting constraints on contract
     clauses; the compliance-date posture; the head's priority
     ranking on which supplier relationships to amend first.
   - Procurement-to-head artefacts: the material-contract
     inventory, contract-audit output per material contract,
     new-contract template update, supplier-communication
     draft, post-change verification plan.
   - SLA: contract audit within 30 days of the change-
     management plan approval; amendment negotiation timeline
     aligned to the compliance date; supplier communication
     issued after wave B of chapter 03 lane 2.
   - Forum for disagreement: CFO's procurement committee or the
     AI Governance Council when the trade-off is between
     contract discipline and continuity of supply.
   Populate the pack entry.
5. **Lane D — HR, L&D, and Chief Compliance / Ethics.** Author
   the lane specification:
   - Named peer: CHRO or head of L&D; where present, the
     Chief Ethics / Compliance officer.
   - Head-to-HR artefacts: content substance for each of the
     three training tiers (chapter 03 lane 3), the policy
     update for AI-governance-specific policy language, the
     named subject-matter expert from the AI-governance
     function.
   - HR-to-head artefacts: the training-refresh plan with LMS-
     enforceable completion SLA per tier, updated acceptable-
     use policy content, escalation on training-completion
     gaps.
   - SLA: content sign-off from the head 30 days ahead of
     wave C rollout; LMS completion window (typically 30–60
     days from wave C); escalation on gaps within 5 working
     days of the completion window closing.
   - Forum for disagreement: CHRO operating committee or AI
     Governance Council. Do not shortcut HR by publishing
     training through the AI-governance function's own channel.
   Populate the pack entry.
6. **Lane E — communications and investor relations.** Author
   the lane specification:
   - Named peer: Chief Communications Officer; where the
     obligation could produce a materiality event, the head of
     Investor Relations (via CFO).
   - Head-to-Communications artefacts: the plain-English
     substance the enterprise will and will not claim, GC
     review status on any draft, the compliance-date posture
     (chapter 04) so Communications understands the readiness
     posture.
   - Communications-to-head artefacts: the external-posture
     draft aligned to the compliance-date posture, the
     proactive-communication decision (blog post / trust-centre
     update / customer briefing yes-or-no), the media-response
     protocol for the compliance-date window.
   - IR (separate coordination): where the obligation could
     produce a materiality event, the head briefs IR through
     the CFO on the substance IR needs; IR decides on
     disclosure, not the head.
   - SLA: external-posture draft finalised before wave D of
     chapter 03 lane 2; media-response protocol activated 30
     days ahead of the compliance date.
   - Forum for disagreement: joint CCO / GC / head session,
     escalated to the executive committee if unresolved.
   Populate the pack entry.
7. **Lane F — adjacent CxO risk vectors.** Author the lane
   specification with sub-entries for each CxO peer whose risk
   vector overlaps the obligation:
   - **CISO** — where the obligation touches AI security
     (model-weight protection, prompt-injection defence, supply-
     chain security under CISA / NCSC guidance). Coordination
     artefact: joint memo where the two functions' controls
     interlock; joint incident-response runbook; joint board
     briefing on the security-adjacent portion.
   - **CIO / CTO / CDO** — where the change touches platform
     capabilities (model registry, telemetry, data-governance
     tooling). Concurrence on delivery dates recorded at the
     AI Governance Council; sequencing disagreements land at
     the CIO / CTO / CDO operating committee.
   - **CPO / DPO** — where the obligation is privacy-adjacent
     (CPPA ADMT, GDPR-lineage ADM rules, Colorado AI Act
     overlaps with the CPA). Coordination artefact: joint
     interpretation memo, joint DPIA / AIA where the impact
     assessments overlap.
   - **CRO** — where the change shifts a risk taxonomy,
     tolerance limit, or appetite statement. Coordination in
     advance of the CRO's risk-committee briefing.
   - **CAE** — the third-line audit programme calibrates
     against the posture. Coordination early so the audit
     programme is not calibrated against a stale operating
     design.
   - **CFO** — where the change carries material cost
     (engineering effort, vendor spend, external audit /
     certification cost). No budget committed without CFO
     approval.
   For the scenario, mark which of the sub-lanes are active and
   which are peripheral. Populate the pack entry per active
   sub-lane.
8. **Forum discipline map.** Author the map that ties every
   coordination decision to a named forum:
   - AI Governance Council — cross-function decisions where the
     head is chair.
   - Executive committee — enterprise-wide decisions with
     material cost, headcount, or reputational exposure.
   - CIO / CTO / CDO operating committee — engineering-
     sequencing decisions.
   - CFO's operating or procurement committee — budget-and-
     supplier decisions.
   - Risk committee — risk-appetite decisions.
   - Audit committee — third-line-coordinated decisions and
     material-change briefings.
   For the scenario, name the upcoming touchpoints at each
   forum in the next four weeks (the "next four weeks" section
   of the coordination pack).
9. **Anti-pattern audit.** For the scenario, name specifically
   which of chapter 05's three anti-patterns the head is at
   risk of falling into and the mitigation:
   - Bilateral back-channel (two peers agree outside a forum).
   - Consensus tax (every decision requires every peer's
     active concurrence).
   - Head-does-it-all (head steps into peers' execution when
     peers do not move).
   For each anti-pattern that applies, name the specific
   mitigation. Write the anti-patterns that do not apply as
   such.
10. **Coordination pack.** Assemble the populated pack as a
    single artefact — the change identifier and obligation, one
    section per active lane with the current-status snapshot,
    the AI Governance Council agenda items in flight, the next
    four weeks of coordination touchpoints. The pack is a
    living document updated weekly by the desk owner and
    reviewed by the head at the weekly digest read.

## Deliverables

- `runbook-header.md` — the enterprise context, scenario, and
  desk-owner header.
- `lane-A-architect-and-engineering.md` — lane spec + pack entry.
- `lane-B-legal.md` — lane spec + pack entry.
- `lane-C-procurement.md` — lane spec + pack entry.
- `lane-D-hr-and-training.md` — lane spec + pack entry.
- `lane-E-communications.md` — lane spec + pack entry.
- `lane-F-adjacent-cxo.md` — sub-entries per active CxO peer.
- `forum-discipline-map.md` — the forum map + next-four-weeks
  touchpoints.
- `anti-pattern-audit.md` — the three-anti-pattern audit with
  mitigations.
- `coordination-pack.md` — the single-artefact assembled pack
  the head reviews weekly.

## Acceptance criteria

- Every lane spec names a specific peer role (not "the
  function"), a specific artefact exchange in both directions
  (not "collaborate"), a specific SLA, and a specific forum
  for disagreement. A peer reading their own lane can operate
  their side without the head briefing them.
- Every lane spec's SLA is dated relative to a concrete
  milestone (compliance date, plan approval, wave B, wave C).
  "As agreed" is not an SLA.
- Lane B (GC) explicitly cites the head-and-GC boundary from
  [[mod-104-regulator-engagement]] chapter 07 and names the
  disagreement-discipline artefacts (joint session, written
  statement, resolution).
- Lane C (procurement) addresses all five sub-lanes chapter 05
  names (contract audit, amendment, template update, supplier
  communication, post-change verification). Silence on any is
  a defect.
- Lane D (HR) explicitly refuses the shortcut of publishing
  training through the AI-governance function's own channel.
  The prohibition is written.
- Lane E (Communications) names the specific claim discipline
  — the enterprise does not make compliance claims; external
  claims belong to Communications and GC jointly with the head
  as substance owner. The head does not release without both
  reviews.
- Lane F is populated per CxO sub-lane, with peripheral sub-
  lanes explicitly marked peripheral rather than omitted.
- The forum discipline map produces a specific forum for every
  category of coordination decision. A category with no forum
  is a defect.
- The anti-pattern audit addresses all three anti-patterns
  explicitly — three paragraphs even where one anti-pattern
  does not apply.
- The coordination pack shows current-status snapshots per
  lane, in-flight disagreements, upcoming forum touchpoints,
  and can be reviewed by the head in 45 minutes.
- Where regulatory-change details (effective dates, obligation
  citations) are uncertain at the knowledge cutoff, a
  `<!-- needs-research: ... -->` marker names the fact and
  the source to verify.

## Stretch goals

- Draft the **peer engagement contracts** — one per lane —
  as the artefact chapter 05 references from
  [[mod-101-role-scope-and-leadership-shape]] chapter 07. Each
  contract states the artefact exchange, the SLA, the forum,
  and the escalation path, and is countersigned by both the
  head and the peer. The contracts are the anti-consensus-tax
  discipline in written form.
- Author a **coordination-pack anti-example** — a pack that
  looks complete but is filled with generic content ("engage
  peers as needed", "communicate the change to stakeholders",
  "align with procurement on suppliers"). Compare it to the
  populated pack from step 10. The anti-example is the
  common first-cut failure; comparing them makes the
  discipline concrete.
- Author the **90-day retrospective** for the coordination
  pack — 90 days after the rollout closes, what worked, which
  lanes hit their SLA, which peer relationships need investment
  before the next rollout, which anti-patterns showed up.
  Feed the retrospective into
  [[mod-107-program-measurement-and-maturity]] chapter 04.
- Extend the runbook with the **sector overlay** for one
  specific sector (banking / insurance / health / medical
  device). The sector CxO peer sitting on top of lane F is
  named ([[mod-109-cross-enterprise-leadership]]), and the
  sector-regulator coordination is added as a sub-lane in
  lane F or lane B depending on the sector's supervisory
  posture.

## Notes and starter guidance

The most common first-cut failure is a runbook that describes
coordination in the abstract — "the head coordinates with GC",
"the head aligns with procurement" — without naming an artefact
exchange, an SLA, or a forum. Coordination in the abstract is
what makes the peer-mediated anti-patterns from chapter 05
appear: the bilateral back-channel is what fills the space when
the runbook does not name the forum; the head-does-it-all
pattern is what fills the space when the runbook does not name
the peer's outbound artefact. Force each lane to be operational.

The second common failure is under-populating lane F. Adjacent
CxO peers do not fit the same one-lane-one-peer shape that
lanes A–E fit. It is tempting to write lane F as "the head
coordinates with adjacent CxOs as needed" and move on. Chapter
05 is explicit that CISO, CIO / CTO / CDO, CPO / DPO, CRO,
CAE, and CFO each have specific coordination shapes depending
on the obligation. Force the sub-lane-per-peer structure, and
explicitly mark the sub-lanes that do not apply for the
scenario rather than omitting them.

On the forum discipline — a coordination question the head
cannot map to a forum is a question the head does not have the
standing to answer alone. This is not a failure mode; it is
the discipline working. When drafting the forum map, if a
category does not map to a forum, either the forum needs to be
added or the category is not a coordination question — it may
be a delegate-owned operational question the head does not
touch.

On the anti-pattern audit — the three anti-patterns are named
because they are common, not because they are exotic. The head
who has run a material regulatory change through to the
compliance date has almost always encountered at least two of
them. Force yourself to name which apply, with the specific
mitigation in place. An audit that says "none apply" is almost
always wrong.

On the coordination pack — the pack is not a status report the
head produces for others; it is the head's own working
document. Its purpose is that the head can look at it and see
the state of coordination in five minutes and can run the
weekly review in 45. If the pack is longer than five pages,
the head is not going to read it and the discipline decays.

On the head-and-GC boundary in lane B — this is where the
runbook most often drifts. The head circulates a draft
regulator-facing filing without GC review "because we're on a
tight deadline". Six months later the filing turns out to have
committed the enterprise to a position GC would have flagged.
The head-does-it-all anti-pattern shows up as GC-shortcut in
this specific way. Force the runbook to make GC's review
non-negotiable on regulator-facing artefacts, even under
timeline pressure.

The coordination runbook is the final artefact in the
mod-105 progression. Scanning (exercise 01) produces awareness;
interpretation (exercise 02) produces decision inputs; the
plan (exercise 03) turns decisions into landing shape; the
posture (exercise 04) adjudicates speed and readiness; the
runbook (this exercise) is what keeps six peer functions
moving in step so that the plan and the posture actually
land. If the runbook is weak, everything upstream is
theoretical.
