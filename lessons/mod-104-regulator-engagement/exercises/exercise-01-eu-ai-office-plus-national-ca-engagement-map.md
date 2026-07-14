# exercise-01: EU AI Office + National-CA Engagement Map

**Estimated effort:** 3 hours

## Objective

Produce a working **EU AI Act engagement map** for a specific
hypothetical (or actual) enterprise you would run — or already run —
the AI governance program at. The map covers all three layers of the
Chapter VII architecture (Union bodies, Member-State national
competent authorities, notified bodies) plus the escalation ladder
that determines who at the enterprise carries each regulator
interaction and where GC picks it up.

The deliverable is not a study note about Chapter VII. It is the
document the head walks into the first relationship meeting with a
national competent authority carrying, and the document the head
refers back to for the next twelve months when an inbound request or
consultation arrives.

The map has to be usable under pressure. The test is whether a
delegate covering for the head could pick it up cold, identify the
right body to route an inbound to, name the enterprise counterpart
and the GC hand-off, and act — without asking the head first.

## Prerequisites

- Chapter [01](../01-eu-ai-act-chapter-vii-engagement-map.md) —
  Reading EU AI Act Chapter VII as the Engagement Map — read and
  internalised. The three-layer / three-posture framing is the
  spine of this exercise.
- [[mod-101-role-scope-and-leadership-shape]] — specifically the CxO
  adjacency chapter — for the head-side counterpart architecture
  (CISO peer, CPO peer, CRO peer, GC hand-off shape).
- [[mod-102-running-the-program]] — the running-program artefacts
  (system inventory, risk register, supply-chain evidence
  discipline) that the map draws from.
- [[mod-103-board-and-audit-committee-reporting]] — the
  regulator-engagement cluster of the quarterly board pack
  (cluster 4) that this map feeds.
- A concrete enterprise in mind, with an assumed sector (banking,
  insurance, health, pharma, public sector, frontier lab, tech
  platform, industrial) and an assumed EU footprint across at
  least three Member States.

## Steps

1. **Enterprise context one-pager.** Author the half-page context
   the map will operate against: sector; primary EU establishment
   (Member State and legal entity); jurisdictional footprint across
   at least three Member States with the local legal entity in
   each; Annex III high-risk categories the enterprise's systems
   fall into (name the categories, not "several"); whether the
   enterprise provides or deploys a general-purpose AI model in
   scope of Chapter V; any sectoral regulator regime the enterprise
   also sits under (banking supervision, medicines, product
   safety, telecoms, professional services). Every subsequent
   artefact refers back to this one-pager.
2. **Union-layer map.** For each of the four Union-layer bodies —
   EU AI Office, European Artificial Intelligence Board, Advisory
   Forum, Scientific Panel — author a row with: the engagement
   stance as a specific verb phrase ("attend the quarterly industry
   convening via DIGITALEUROPE", "submit a written position
   through the sector body", "observe published outputs only", not
   "engage with"); the head-side counterpart at the enterprise (the
   head personally, Government Affairs, chief scientist, sector-
   body delegate); the cadence (quarterly, on-consultation-only,
   monthly monitoring); the trigger that moves the engagement to a
   higher tier of intensity.
3. **Member-State map.** For each Member State in the enterprise's
   footprint (minimum three), author a row with: the current
   designated NCA (both notifying authority and market
   surveillance authority) — mark
   `<!-- needs-research: verify [Member State] NCA designation
   against the Commission's published list at
   digital-strategy.ec.europa.eu -->` where the designation is
   unclear at your knowledge cutoff, and name the specific fact to
   verify; the enterprise's local counterpart (subsidiary GC, local
   head of compliance, country manager, sector-regulatory lead);
   the head's assessment of the NCA's supervisory culture (GDPR-
   lineage, product-safety-lineage, new-authority, sector
   regulator); the first-relationship-meeting agenda (four to six
   items, specific — introductions, system inventory walk-through,
   Article 26 obligations posture, Article 72/73 mechanics
   discussion, mutual expectations on cadence).
4. **Lead-NCA designation.** Explicitly name which of the Member-
   State NCAs is the enterprise's *lead* NCA and why — primary EU
   establishment, sector fit, or majority of high-risk systems.
   Author the additional relationship investment for the lead NCA
   above the baseline for other NCAs: named liaison at the
   enterprise, standing meeting cadence, proactive briefings on
   material system changes.
5. **Notified-body map.** For each Annex III category the
   enterprise falls into that requires third-party conformity
   assessment, author a row with: the notified-body engagement
   path (direct supplier-management relationship with a named
   notified body if one is contracted; open scoping if not);
   the enterprise-side owner (the head, with the level-50
   architect and the operating owner); the accreditation and
   harmonised-standards frame (CEN-CENELEC JTC 21 output the
   assessment leans on); the contractual conformity-assessment
   cycle cadence.
6. **Escalation ladder.** Author the five-rung ladder from routine
   engagement through formal action: routine engagement (standing
   cadence, factual updates); information request (market
   surveillance powers, structured response); examination
   (targeted supervisory review, evidence packages under Article
   17 QMS and Annex IV technical documentation); formal action
   (enforcement, corrective measures, market withdrawal
   proceedings); litigation (judicial review, appeals). For each
   rung name the internal owner, the GC involvement level (advised,
   consulted, co-owner, lead), and the trigger for moving to the
   next rung.
7. **GC hand-off overlay.** Draw the GC hand-off point explicitly
   on every rung of the escalation ladder and on every row of the
   Union-layer and Member-State maps. The overlay is a single
   column: "GC role at this engagement" with one of {not involved,
   advised of correspondence, reviews before send, co-authors, GC
   leads}. The map is not usable without this column — if a
   delegate cannot tell whether to loop in GC before responding,
   the delegate will guess wrong under pressure.
8. **Feed-to-board-pack annotation.** For each row where an active
   engagement, information request, examination, or notified-body
   finding would land in the quarterly board pack's regulator-
   engagement cluster (see
   [[mod-103-board-and-audit-committee-reporting]] chapter 01
   cluster 4), annotate the row with the board-pack line it feeds.
   Rows that never surface to the board are annotated as such.

## Deliverables

- `enterprise-context.md` — the scenario one-pager (sector,
  footprint, Annex III exposure, GPAI exposure, sectoral overlay).
- `union-layer-map.md` — the four-row table for AI Office, AI
  Board, Advisory Forum, Scientific Panel with stance, counterpart,
  cadence, escalation trigger, GC hand-off.
- `member-state-map.md` — one row per Member State in the
  footprint, with NCA identification (or needs-research marker),
  local counterpart, supervisory-culture assessment, first-meeting
  agenda, GC hand-off.
- `lead-nca-designation.md` — the named lead NCA with rationale
  and the additional relationship investment.
- `notified-body-map.md` — one row per Annex III category
  requiring third-party assessment, with notified-body path,
  enterprise-side owner, standards frame, cycle cadence.
- `escalation-ladder.md` — the five-rung ladder with owner, GC
  role, and progression trigger per rung.
- `board-pack-feed.md` — the annotation showing which map rows
  surface into board-pack cluster 4 and how.

## Acceptance criteria

- The engagement stance for every named Union-layer body is a
  specific verb phrase ("attend the quarterly convening", "submit
  a written position", "co-sign the industry-body submission",
  "observe published outputs only"), not "engage with" or
  "monitor."
- Every Member State the enterprise operates in has an NCA named
  or an explicit `<!-- needs-research: ... -->` marker with the
  specific fact to verify and the source to verify against. No
  Member State is left blank.
- The lead NCA is explicitly designated with a stated rationale;
  the additional relationship investment above the baseline is
  named, not implied.
- Every Annex III category on the enterprise-context one-pager
  appears on the notified-body map, or is explicitly annotated as
  not requiring third-party conformity assessment.
- The escalation ladder has an internal owner at every rung, and
  the GC hand-off column has a defined role at every rung. No rung
  is silent on GC. A delegate reading only the ladder can tell
  when to phone GC.
- Every row across the Union-layer map, Member-State map, and
  notified-body map carries the GC hand-off overlay column
  populated with one of the defined values.
- The board-pack feed annotation covers every row that would
  surface to cluster 4; rows that would not surface are annotated
  as such rather than left silent.

## Stretch goals

- Draft a mock first-relationship-meeting agenda for one specific
  named NCA, at meeting-invite depth — attendees on both sides,
  90-minute time-boxed agenda, pre-reads to send, notes owner,
  follow-up commitments template.
- Map the engagement map back to the regulator-engagement cluster
  of the quarterly board pack from
  [[mod-103-board-and-audit-committee-reporting]] — produce the
  one-page cluster-4 view for the current quarter, populated from
  the engagement map rows.
- Author the map-maintenance discipline (who updates the map on
  which trigger, versioning convention, review cadence, onboarding
  hand-off protocol for a new head or delegate). The map is a
  living artefact; if the maintenance discipline is not named the
  map decays inside six months.
- Produce a redlined version of the map assuming one specific
  Member State re-designates its NCA mid-year — what changes, what
  does not, and how the change flows to the board pack.
- Extend the map with the sectoral-regulator overlay (for banking:
  the ECB/EBA/national prudential supervisor; for medicines: EMA
  and national medicines agencies; for telecoms: BEREC and NRAs),
  showing which sectoral regulator engagements interact with which
  AI Act NCA engagements and where the head coordinates versus
  where the sector CxO peer leads.

## Notes and starter guidance

The most common first-cut failure is a map that reads as a Chapter
VII study guide with an engagement column bolted on. The map is not
a study guide. Cut every sentence that does not tell a delegate
what to *do* under pressure. If a row cannot be reduced to
{trigger, body, counterpart, GC role, next action}, the row is
under-authored.

The second common failure is over-claiming direct engagement with
Union-layer bodies. For most enterprises the head does not have a
direct bilateral with the EU AI Office. Writing "quarterly bilateral
with AI Office" for a mid-size deployer signals to a peer reviewer
that the head does not understand the architecture. The stance for
most Union bodies is mediated — via industry bodies, via
consultations, via Member-State NCA channels. Chapter 01 is
explicit on this; the map has to reflect it.

The third common failure is silence on the GC hand-off. A map that
does not tell the delegate whether to loop in GC before responding
will produce inconsistent behaviour under pressure, and inconsistent
behaviour is the pattern that turns a cooperative-counterparty file
into a problem file. Force yourself to fill the GC column on every
row and every rung, even where the answer is "not involved."

On the Member-State NCA rows, resist the pull to guess an NCA
designation you are not sure of. Regulators notice organisations
that get their name wrong in first correspondence. The
`<!-- needs-research: ... -->` marker is the right move — it flags
the specific fact and the source to verify it against, and it
survives the twelve-month working-document lifecycle.

On the notified-body map, remember that not every Annex III system
requires third-party conformity assessment. The regulation carves
which systems do. Where the enterprise has an Annex III system that
does not require third-party assessment, the row still exists on
the map — annotated as internal conformity assessment under
Article 43 with the enterprise-side owner named — so that the map
covers the full high-risk portfolio, not only the notified-body
subset.

The map is a working document, not a polished deliverable. Version
it, date it, keep it in the same repository as the running-program
artefacts, and refer to it in the first ten minutes of every
regulator conversation. A map that is not open on the head's screen
during the call is a map the head has not actually adopted.
