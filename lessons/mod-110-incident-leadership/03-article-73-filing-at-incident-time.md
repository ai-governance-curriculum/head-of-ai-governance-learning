# Owning the Article 73 Filing at Incident Time

## Motivation

The general Article 73 filing regime is a set of rules the head of
AI governance knows before any incident happens. Chapter 02 of
[[mod-104-regulator-engagement]] lays that regime out — the three
timelines, the seven-question filing-defence discipline, the
signature ownership, the boundary with the General Counsel. A head
who cannot recite that chapter from memory should not be signing
filings. But knowing the regime is not the same as executing it
under a running clock.

This chapter is about the execution. It is about what the head
actually does in the room from the moment an incident lands to the
moment the filing is signed and transmitted to the national
competent authority. The failure mode this chapter defends against
is the enterprise that knew the general regime cold and still
missed the Article 73(3) two-day timeline because the classification
meeting did not resolve fast enough on whether the event fell into
the widespread-infringement paragraph. The enterprise that
correctly identified the event as reportable and still filed under
the wrong paragraph because the head let the room debate the
technical facts without letting GC own the legal characterisation.
The enterprise that filed on time to the correct national CA and
still received a follow-up letter opening a formal investigation
because the corrective-action commitment in the filing was vague
enough to read as evasion.

Under time pressure, the head does not have the luxury of
re-deriving the general regime. The head has to run a compressed,
decision-forcing meeting that assumes the regime is known and
converges on: is this event within Article 3(49); if yes, which
paragraph of Article 73 governs; when did awareness begin; what
does the filing say; who signs; what happens after the filing goes
in. This chapter walks through each of those moves.

## Core concept — the filing decision is the head's, made under a running clock

The general chapter established that the head signs the filing.
The load-bearing move for incident time is stronger: the head
*decides* the filing under a running clock, in a room the head
convened, with a decision boundary the head enforces.

The SOC does not decide. The architect does not decide. Neither
does the CISO, whose incident lead is on the bridge with a full
technical account. GC does not decide either — GC advises on the
legal characterisation. The head decides.

That distinction is not ceremonial. It is what allows the head to
hold the room to a single decision meeting instead of a rolling
debate that runs past the Article 73(3) two-day clock. The four
peers in the decision have well-defined inputs:

- **GC** owns the legal characterisation — does the event meet
  Article 3(49); which paragraph of Article 73 applies; what
  parallel breach-notification regimes are triggered.
  <!-- needs-research: verify Article 3(49) as the definition
  provision and the paragraph structure of Article 73 in
  Regulation (EU) 2024/1689 -->
- **The architect** owns the technical account — what the AI
  system did, what the evidence shows, what the reconstructed
  timeline says, what the current view of causal link is.
- **The CISO's incident lead** (see [[01-incident-command-shape-at-leadership-scope]])
  owns the containment and remediation posture — what has stopped
  the harm continuing and what is in flight.
- **Regulator Relations** owns the NCA-relationship context — how
  this specific national CA has responded to prior filings from
  the enterprise or from peers, what the current political weather
  is, what the head should expect in the follow-up sequence.

The head reads across all four, applies the seven-question
filing-defence discipline from [[mod-104-regulator-engagement]]
chapter 02, and signs. Anything else — the SOC deciding, the
architect drafting and shipping without a head signature, GC
issuing the filing directly — is a positioning error the head does
not recover from with the NCA. The NCA reads the signature. If the
signature is not the head's, the NCA reads the enterprise as one
that did not take the event seriously enough to put the accountable
executive's name on the filing.

## The incident-time classification decision

The moment an incident bridge escalates to the head's attention,
the first decision to close is the classification decision. Every
other decision in this chapter depends on it. Getting it wrong on
the fast side loses the enterprise nothing but time. Getting it
wrong on the slow side — treating an event as non-reportable when
it meets Article 3(49) — puts the head in front of the NCA
explaining a late filing. That is a conversation the head does not
want to have.

### The classification meeting participants

The classification meeting is small and named. The head convenes:

- The head, chairing.
- The General Counsel (or the GC's designated senior AI-litigation
  counsel where GC is unavailable — the delegate is pre-named, not
  chosen in the moment).
- The senior AI governance architect (level 50) — the head's
  technical brief-holder on what the AI system did and what the
  evidence shows.
- The CISO's incident lead — the person running the incident
  bridge, holding the containment picture in real time.

The DPO joins if there is any signal that personal data is
implicated. Comms, Government Affairs, Regulator Relations, the
CRO, and the board interface come in at the sign-off meeting later
(see below), not at the classification meeting. Widening the
classification meeting past this four-plus-one dilutes it into a
briefing and lets the classification decision drift.

### The GC's role in classification

The classification decision is a legal characterisation before it
is anything else. Article 3(49) defines a serious incident by
reference to specific harm categories — death of a person or
serious harm to health, serious and irreversible disruption of
critical infrastructure, an infringement of Union law protecting
fundamental rights, or serious harm to property or the environment.
<!-- needs-research: verify the four Article 3(49) harm categories
and their exact wording in Regulation (EU) 2024/1689 -->
Whether the event as reconstructed falls inside any of those
categories is a question the head does not answer alone. GC owns
that call.

The head's job in the meeting is to hold the boundary. Under
pressure, technical peers will drift into legal characterisation
("that is not really a fundamental-rights infringement, is it") and
legal peers will drift into technical assertion ("but the model
must have done X"). The head names the boundary and holds it: the
architect and the CISO's lead describe what the system did and
what the evidence shows; GC characterises whether that meets
Article 3(49); the head reads across and confirms the position.

If GC's characterisation is uncertain — the event sits close to a
category boundary and GC needs an hour to consult sector-specific
material — the head does not push GC to a snap answer. The head
holds the room, restates the timeline pressure, and confirms the
next checkpoint. If the timeline pressure is severe (Article 73(3)
territory) the head files under the more-onerous interpretation
and lets GC narrow it later. Filing early on a marginal case is
recoverable; missing a two-day clock is not.

### The awareness-date evidence discipline

Every Article 73 timeline runs from the moment of awareness. The
enterprise's account of when awareness was established is what the
NCA will test first in any follow-up. The evidence for that
account has to exist in real time; it cannot be reconstructed
after the filing.

The head's team maintains the awareness-date evidence as the
incident is unfolding, not after. The evidence stack is:

- **The originating alert or ticket** — the first signal in the
  monitoring system, the customer complaint, the peer-enterprise
  notification, the media report. Timestamped in the source
  system. The head's team does not paraphrase; the raw record is
  captured.
- **The incident-bridge minutes** — running notes from the bridge
  the CISO's incident lead is chairing. Every escalation, every
  hand-off, every decision timestamped and attributed.
- **The escalation record** — the sequence of who was notified
  when, up to and including the moment the head was pulled in.
- **The classification-meeting notes** — the meeting the head has
  just convened, with attendees, timing, and the classification
  decision recorded verbatim.

The architect operates this evidence discipline in real time. The
head confirms in the classification meeting that the awareness
date the enterprise is asserting is defensible against the evidence
stack. If it is not — if there is a plausible earlier awareness
date the enterprise cannot rebut — the head uses the earlier date
and adjusts the clock accordingly. Filing against a defensible
awareness date that the NCA cannot puncture is worth more than
filing against a favourable date that unravels under the first
information request.

### The escalation path when classification is contested

Sometimes the classification decision does not close. The
architect and GC read the event differently; the CISO's incident
lead reads the containment posture as one thing and GC reads the
legal-characterisation implications differently. The head chairs
to a decision, but where the enterprise is genuinely split — where
reasonable senior people disagree on whether the event meets
Article 3(49) — the head escalates rather than force a call the
head is not certain of.

The escalation path is: head to CEO, in the moment, on the phone
if necessary. The head brings the two positions, the timeline
pressure, and a recommendation. The CEO either endorses the
head's recommendation, endorses the alternative, or asks the head
to file under the more-onerous interpretation and let the position
be revised after further analysis. The CEO does not adjudicate the
substantive legal question; the CEO decides the risk posture the
enterprise takes under uncertainty. That is a CEO-level call, not
a head-level one, and the head's discipline is to know when to
raise it.

The CEO escalation is rare. Most classification decisions close
inside the meeting. But the head does not treat the escalation
path as a last resort or a failure signal. It is the pressure
relief that keeps the classification decision honest. A head who
never escalates a genuinely contested classification is a head who
is either not seeing contested cases or is forcing calls that do
not have consensus underneath them.

## The multi-Member-State routing decision

Article 73 requires reporting to the market-surveillance
authorities of the Member States where the incident occurred.
<!-- needs-research: verify that Article 73(1) frames the recipient
as the market-surveillance authorities of the Member States where
the incident occurred, in Regulation (EU) 2024/1689 -->
For an AI system deployed across the Union, that framing frequently
produces more than one recipient. The head decides at incident
time which national CAs are in scope and how the enterprise
coordinates across them.

The routing decision has three moves.

**First, geographic scope of the incident.** The architect walks
the head through the deployment surface: which Member States'
users, customers, or protected populations were exposed to the
event; where the harm materialised; where the affected AI system
was operating. The head confirms the list. Geographic ambiguity
resolves toward inclusion; if the enterprise is uncertain whether a
particular Member State was affected, the enterprise treats it as
in scope and files. Under-filing on a marginal Member State is a
larger exposure than over-filing.

**Second, the lead-NCA selection where multiple Member States are
in scope.** Where more than one national CA is a recipient, the
head names an internal lead-NCA relationship — usually the CA of
the Member State where the enterprise's EU seat is established, or
where the harm was most concentrated. That lead-NCA relationship
does not change the obligation to file to every affected CA; it
sets the enterprise's internal single-point-of-contact discipline
so that the follow-up sequence does not fragment into parallel
uncoordinated engagements. Regulator Relations operates the
coordination; the head owns the choice of lead-NCA and confirms
it with GC. The Chapter VII coordination discipline covered in
[[mod-104-regulator-engagement]] chapter 01 gives the head the map
of who at each national CA the enterprise has an existing
relationship with; the head uses that map to name the lead-NCA
that is best positioned to hold the primary conversation without
short-changing the others.
<!-- needs-research: verify whether Chapter VII of Regulation
(EU) 2024/1689 defines a lead-authority mechanism analogous to
GDPR one-stop-shop, or whether coordination across national CAs
is purely mutual-assistance under Article 74 or equivalent -->

**Third, the EU AI Office interaction where a GPAI system is
implicated.** Where the AI system in scope is a general-purpose AI
model — or is a high-risk AI system that integrates a GPAI model
in a way that puts GPAI-specific obligations in play — the EU AI
Office is on the engagement map alongside the national CA. The
head confirms with GC whether the specific event triggers a
GPAI-specific serious-incident obligation and, if so, whether the
notification runs through the national CA or directly to the AI
Office.
<!-- needs-research: verify the specific mechanism by which GPAI
serious-incident obligations under Chapter V of Regulation (EU)
2024/1689 route to the EU AI Office — whether via the national
CA under Article 73 with AI Office notification, or via a distinct
direct-notification path, and the exact article reference -->
Regulator Relations coordinates the mechanics; the head owns the
decision to treat the AI Office as an active participant in the
filing engagement, not as a passive downstream recipient.

For a routing decision that spans, say, four Member States plus
the AI Office, the head compresses the internal coordination into
a single tracking artefact — a filing-recipients register the
architect maintains — showing every recipient, the applicable
timeline, the responsible internal lead for that recipient, the
filing text variant (if any national CA requires a specific form
or additional detail), and the sign-off status. The head reads
across the register before signing anything. If a recipient is
missing or a variant is not aligned with the master text, the
head catches it.

## The filing content composition under time pressure

The seven-question filing-defence discipline from
[[mod-104-regulator-engagement]] chapter 02 is the test the head
applies before signing. Under the running clock, the head does
not apply the discipline from scratch — the enterprise composes
the filing against a pre-built template so that composition and
review happen in parallel.

The composition pattern is:

- **The architect drafts against the template.** The template is
  pre-built and rehearsed against Exercise 03 of this module and
  Exercise 02 of [[mod-104-regulator-engagement]]. It has a
  section per one of the seven questions plus the header
  metadata: enterprise identity and role (provider or deployer),
  affected AI system identity, awareness date, causal-link
  assertion, applicable Article 73 paragraph, recipient national
  CA. The architect fills the template against the current
  evidence, marking sections that are not yet settled.
- **GC reviews for interpretive gotchas.** GC reads the draft for
  wording that inadvertently commits the enterprise to a legal
  position it does not intend, that admits facts contested in
  parallel proceedings, that narrows or broadens statutory
  definitions unhelpfully, or that undermines privilege. GC
  turns the review inside a named window that the head has
  committed to in the classification meeting.
- **The head reads for defensibility.** The head walks the seven
  questions in order and asks: is the answer here one I can
  defend without qualification to the NCA next week when they
  call. Where the answer is not defensible — vague, evasive, or
  narrower than the evidence supports — the head sends it back
  for re-work with a specific instruction, not a general request
  for improvement.
- **Sign-off routes per the pre-agreed flow.** The Exercise 02
  runbook in [[mod-104-regulator-engagement]] names the sign-off
  flow: architect drafts, GC clears legal, CISO's incident lead
  clears containment/remediation, head signs, Regulator Relations
  transmits. The head does not invent the routing under
  pressure; the head follows the pre-agreed flow. Where the pre-
  agreed flow does not fit the specific event — an unusual
  routing to an unfamiliar national CA, a GPAI-specific
  notification the enterprise has not filed before — the head
  names the deviation in real time and records the rationale.

The composition-under-time-pressure discipline is not a mechanical
production line. The head reads every draft. But the reading is
against a known template, a known set of questions, and a known
sign-off routing. The compression comes from having done the
preparation work outside incident time so that incident-time
effort is decision effort, not authoring effort.

## The filing-decision meeting shape

Once the classification decision is closed and the composition
work is in flight, the head convenes the filing-decision meeting.
This is the meeting the head runs to sign — the room where the
final content is reviewed, the sign-off is executed, and the
downstream coordination is aligned. It runs like the audit-
committee decision meetings in [[mod-103-board-and-audit-committee-reporting]]
chapter 04: named participants, named agenda, named duration, no
drift into open discussion.

**Participants.** The head, chairing. GC. The senior AI
governance architect. The CISO's incident lead. Regulator
Relations. The Comms lead (for external-comms alignment, not for
input on the filing content). The DPO if personal data is in
scope. The board interface — usually the head sends a written
briefing to the audit-committee chair and the risk-committee chair
in parallel, rather than pulling either into the meeting.

**Agenda.** Four items, in order:

1. Classification confirmation. GC restates the Article 3(49)
   position, the Article 73 paragraph, the awareness date, and
   the applicable timeline. The head confirms. If anything has
   shifted since the classification meeting, this is where it
   surfaces.
2. Filing content review. The architect walks the filing text
   against the seven questions. The head reads for defensibility.
   Sign-offs from GC (legal) and the CISO's incident lead
   (containment/remediation) are captured on the artefact. The
   head signs.
3. Sign-off routing and transmission. Regulator Relations
   confirms the recipient list, the transmission mechanism for
   each recipient, the confirmation-of-receipt tracking, and the
   filing-recipients register status.
4. External-comms coordination. Comms restates the customer,
   press, employee, and partner posture that has to be aligned
   with the filing text. Comms does not draft what goes to the
   NCA; Comms aligns everything else with what does. The head
   confirms the alignment.

**Duration.** Under 60 minutes. If the meeting runs longer, the
head has let the room drift. The meeting is not the place to re-
open classification, re-draft filing text, or debate technical
attribution. Those have all happened upstream. If they have not,
the meeting adjourns and the head reschedules once the upstream
work is closed.

**Cadence for evolving incidents.** Some serious incidents evolve
over hours or days between the initial filing and the follow-up.
The head reconvenes the filing-decision meeting each time material
new information alters the seven-question position — a
containment posture that has failed, a corrective-action
commitment the enterprise cannot meet, a new affected population.
Each reconvening produces either a supplemental filing to the NCA
or a decision that the update is captured in the follow-up
sequence rather than a supplemental filing. GC advises; the head
decides.

## The follow-up interaction posture

The filing is not the end. Chapter 02 of
[[mod-104-regulator-engagement]] lays out the general shape of
follow-up interaction — the written information request within a
small number of weeks, the follow-up meeting, the on-site
inspection in more serious cases, the closing or investigation-
opening letter. The incident-time chapter emphasises the head's
personal ownership of every one of those touchpoints.

The head does not hand off the follow-up sequence to the architect
because the acute phase is over. The NCA reads continuity of
representation. If the head signed the filing and then disappears
from the follow-up sequence — replaced by the architect or by GC —
the NCA reads the enterprise as one where accountable-executive
attention was performative for the filing and does not extend into
the sustained engagement. That reading is durable.

The head personally owns four follow-up commitments:

- **The written information request response.** The architect
  drafts against the request; the head reviews and signs the
  cover letter. If the response is voluminous, the head reads at
  minimum the executive summary and the answer to every question
  that the head expects to be asked about in a follow-up meeting.
- **The follow-up meeting.** The head attends. The architect
  accompanies as technical brief-holder; GC accompanies for legal
  interpretation. The head chairs the enterprise's side of the
  meeting and holds the technical position (what the system did,
  what the enterprise did about it). GC holds the legal position.
  Regulator Relations owns the meeting logistics and the record.
- **The on-site inspection.** Where an inspection is called, the
  head is the host of record. The head is present for the opening
  meeting, the closing meeting, and any inspector interaction
  that touches enterprise-level positioning. Between-times the
  architect and the CISO's incident lead handle the technical
  facilitation. The head does not treat inspection presence as a
  ceremonial appearance; the head is available for the duration.
- **The corrective-action plan.** The plan the enterprise commits
  to in the filing is a personal commitment of the head. The head
  tracks it against the named dates, reviews progress at the
  regular operating cadence, and notifies the NCA proactively if
  a milestone will slip before the milestone is missed. The head
  who lets a corrective-action milestone slip silently is the
  head who receives the follow-up letter opening a formal
  investigation.

The head builds a filing engagement register that tracks every
open Article 73 filing across every national CA the enterprise
has ever filed to. The register shows the filing date, the
recipient, the current status, the next expected interaction, the
open information requests, the open corrective-action commitments,
and the responsible internal lead for each. Regulator Relations
operates the register; the head reads it at the monthly operating
review. Filings do not close in the head's attention until the
NCA has issued a closing letter or an equivalent signal.

## The GPAI serious-incident specifics

Where the enterprise is a provider of a general-purpose AI model,
or a deployer whose deployment triggers GPAI-provider obligations
by virtue of the deployment shape, the incident-time filing map
extends. The EU AI Office sits alongside the national CA on the
engagement map. Chapter V of the Regulation establishes the GPAI-
specific regime, including serious-incident notification
obligations that the head has to know at incident time.
<!-- needs-research: verify that Chapter V of Regulation (EU)
2024/1689 governs GPAI provider obligations and that GPAI-
specific serious-incident notification obligations exist and are
distinguishable from the Article 73 regime for high-risk AI
systems -->

The head decides at incident time whether the event triggers a
GPAI-specific notification in addition to the Article 73 notification
to the national CA. GC advises on the characterisation. Regulator
Relations coordinates the mechanics — whether the AI Office is
notified directly, notified through the national CA, or notified
in parallel via a distinct channel.
<!-- needs-research: verify the specific notification mechanism for
GPAI serious incidents to the EU AI Office — direct, via national
CA, or parallel — including exact article reference -->
The classification meeting and the filing-decision meeting extend
to cover the GPAI position: a GPAI provider does not treat the AI
Office as an afterthought to the national-CA filing. The AI Office
interaction has its own follow-up sequence, its own information
requests, and its own relationship posture. The head runs it as a
peer relationship to the national-CA relationship, not as a
subordinate one.

For enterprises that are not GPAI providers but whose incident
implicates an upstream GPAI model they deploy, the head's move is
different: the head coordinates with the upstream provider on
their filing position and confirms that the enterprise's own
filing accurately reflects the upstream provider's characterisation
of the model behaviour. That coordination is a contractual matter
that should be pre-negotiated in the provider contract (see the
supply-chain evidence discipline in [[mod-102-running-the-program]]
chapter 06 material), but under incident-time pressure the head
opens the coordination directly with the counterpart at the
upstream provider and does not wait for procurement channels.

## Composition with adjacent modules

The chapter composes tightly with the rest of the track.

- [[mod-104-regulator-engagement]] chapter 02 is the general
  Article 73 regime this chapter executes against; chapter 01 is
  the Chapter VII engagement map the routing decision reads from;
  chapter 06 covers the durable AI Office relationship the GPAI-
  incident sequence rides on.
- [[mod-103-board-and-audit-committee-reporting]] chapter 04 is
  the decision-meeting shape the filing-decision meeting mirrors;
  the incident-and-near-miss cluster in the board reporting
  cadence is where the Article 73 filing is briefed to the board.
- [[01-incident-command-shape-at-leadership-scope]] is the
  incident-command structure the filing decision sits inside;
  [[02-cross-function-incident-coordination]] is the coordination
  discipline the classification meeting and filing-decision
  meeting operationalise.
- [[04-us-serious-incident-disclosure-map]] is the next-chapter
  counterpart — the US-side equivalent map of federal, state, and
  sector serious-incident disclosure obligations, which the head
  runs in parallel to the Article 73 filing when an incident has
  both EU and US exposure.
- [[05-post-incident-learning-cycle-sponsorship]] is what happens
  after the filing engagement closes — the sponsored learning
  cycle that turns the incident into control-library and policy
  updates.
- [[mod-109-cross-enterprise-leadership]] gives the CxO
  coordination patterns the head applies to the CISO, GC, Comms,
  and CEO interactions the incident-time filing decision runs
  through.

## Summary

- The general Article 73 regime is known before the incident; the
  head's incident-time job is to execute it under a running clock
  without re-deriving it. Chapter 02 of
  [[mod-104-regulator-engagement]] is the regime; this chapter is
  the execution.
- The filing decision is the head's, made in a room the head
  convened. GC characterises the event legally; the architect
  holds the technical account; the CISO's incident lead holds
  containment; Regulator Relations holds the NCA-relationship
  context. The head reads across and signs.
- Classification is the first decision to close, and it is a legal
  characterisation before it is anything else. The head chairs;
  GC characterises against Article 3(49); the head holds the
  boundary against technical peers drifting into legal argument
  and legal peers drifting into technical assertion. Where the
  enterprise is genuinely split, the head escalates to the CEO
  rather than force a call.
- The awareness-date evidence stack — originating alert, incident-
  bridge minutes, escalation record, classification-meeting notes
  — is maintained in real time, not reconstructed after. A
  defensible awareness date beats a favourable one.
- The routing decision names every affected Member State's
  national CA, picks a lead-NCA for coordination discipline, and
  extends to the EU AI Office where GPAI obligations are in
  play. A filing-recipients register captures every recipient,
  timeline, and sign-off status; the head reads across it before
  signing.
- The filing text is composed against a pre-built template; the
  architect drafts, GC clears legal, the head reads for
  defensibility using the seven-question discipline, and the head
  signs. Sign-off routing follows the pre-agreed flow rather than
  being invented under pressure.
- The filing-decision meeting is under 60 minutes, with four
  agenda items: classification confirmation, filing content
  review, sign-off routing, external-comms coordination. Evolving
  incidents reconvene the meeting rather than let filing content
  drift out of alignment.
- The filing is the opening move of a durable engagement. The
  head personally owns the written-information-request response,
  the follow-up meeting, the on-site inspection, and the
  corrective-action plan against its named dates. Continuity of
  the head's representation across the sequence is what the NCA
  reads.
- Where a GPAI model is implicated, the EU AI Office is on the
  engagement map alongside the national CA. The head runs the AI
  Office as a peer relationship, not a subordinate one, and
  coordinates upstream with GPAI providers whose model behaviour
  is referenced in the enterprise's own filing.
