# Engaging the AI Safety Institute Network

## Motivation

The AI Safety Institute network is not a regulator, and a head of
AI governance who treats it as one will get the engagement pattern
wrong in both directions — over-lawyering technical conversations
that should be candid, and under-preparing for the reputational
weight the network's outputs increasingly carry. AISIs are
technical safety bodies. They evaluate frontier models, publish
methods, convene the emerging community around AI safety science,
and coordinate cross-jurisdictionally on what "responsible" looks
like. They do not (in general) issue fines, open investigations,
or bring enforcement actions. Engagement with them is voluntary.

That voluntariness is precisely why the head of AI governance
needs a deliberate posture. Enterprises that are not frontier labs
still have four reasons to be present in the AISI conversation.

First, signalling. When a national competent authority, a sector
regulator, or an audit committee asks how the enterprise tracks
frontier safety science, "we are a member of the AI Safety
Institute Consortium and we contribute to its working groups" is
a materially different answer to "we read the papers." The former
is a running relationship; the latter is a reading list. See
chapter 01 of this module for how NCA-facing narratives take up
these relationships.

Second, access to evaluation science. AISIs publish evaluation
methodologies, benchmark designs, and — in the UK case — open
tooling (Inspect) that enterprises can pull into their own
pre-deployment testing. This is not academic reading. It is
technique the enterprise's evaluation function can consume and
which then flows into the running program.

Third, input on emerging standards. Voluntary AISI methodologies
have a strong tendency to become the reference shape that
regulators, auditors, and later standards bodies converge on.
Enterprises that shape the drafting have a smaller adaptation cost
than enterprises that read the finalised version.

Fourth, community. The AISI network is the room where the
technical safety conversation happens across enterprises, frontier
labs, academia, civil society, and regulators. Heads of AI
governance who are not in that room learn the emerging norms one
regulatory cycle late.

The purpose of this chapter is to give the head a designed pattern
for that engagement, not a reactive one.

## Core concept: a distributed network of technical safety bodies

The AI Safety Institute network is not a single organisation. It
is a set of national or regional technical bodies, each with its
own funding line, its own mandate, and its own relationship to its
home government, coordinating through a series of joint
declarations and technical exchanges. The head needs to track each
of the bodies below and understand where the enterprise sits in
relation to each.

### The bodies to track

**US AI Safety Institute (US AISI)** — established at the National
Institute of Standards and Technology (NIST) under Executive Order
14110 of October 2023 ("Safe, Secure, and Trustworthy Development
and Use of Artificial Intelligence"). Its founding mandate covered
frontier-model evaluation, safety science, and the development of
guidelines for pre-deployment testing.

<!-- needs-research: verify current organisational status, name, and mandate of the US AI Safety Institute against nist.gov/aisi, given that EO 14110 was rescinded by EO 14179 in January 2025 and the institute's rebranding/restructuring under the current administration is evolving -->

**AI Safety Institute Consortium (AISIC)** — the multi-stakeholder
consortium convened by NIST alongside US AISI, with a founding
membership of several hundred organisations spanning enterprises,
model developers, academic researchers, standards bodies, and
civil society groups. Working groups cover topics including
capability evaluations, red-teaming, safe deployment, and
synthetic content authentication.

<!-- needs-research: verify current AISIC membership figure, working group topics, and current organisational sponsorship against the NIST AISIC landing page -->

**UK AI Safety Institute (UK AISI)** — announced by the UK
government in November 2023 in the run-up to the Bletchley Park AI
Safety Summit. Its most widely-adopted public output is Inspect,
an open-source framework for large language model evaluation
released under an MIT licence at
github.com/UKGovernmentBEIS/inspect_ai. The BEIS in the repository
path reflects the department that stood the institute up; the
sponsoring department and the institute's public name have both
changed since founding.

<!-- needs-research: verify the current organisational name of the UK AI Safety Institute (which has been renamed at least once) and its current sponsoring department against the UK government's gov.uk pages -->

**Canadian AI Safety Institute (CAISI)** — announced in 2024 by
Innovation, Science and Economic Development Canada (ISED) as
Canada's national contribution to the AISI network, funded through
Canada's federal AI safety allocation.

<!-- needs-research: verify CAISI's current mandate, funding, and organisational home against ISED Canada announcements -->

**Singapore — AI Verify Foundation and the Singapore AISI-equivalent** —
Singapore's Infocomm Media Development Authority (IMDA) established
the AI Verify Foundation as an open-source testing framework
governance body. Singapore has separately signalled a national AI
safety technical body role within its AISI-network participation.

<!-- needs-research: verify the current name, mandate, and relationship of Singapore's AI safety institute-equivalent (distinct from or aligned with AI Verify Foundation) against IMDA publications -->

**EU Member State bodies** — several EU Member States are
standing up national AI-safety technical competences to complement
the EU AI Office and their designated national competent
authorities under the AI Act. Specific national instances
(Germany, France, the Netherlands, and others) are in flux.

<!-- needs-research: enumerate current EU Member State AI safety institute equivalents and their relationship to the EU AI Office and to the wider AISI network -->

### The coordinating pattern — Bletchley, Seoul, San Francisco

The AISIs are stitched together not by a treaty but by a sequence
of joint declarations and follow-on convenings.

- The **Bletchley Declaration** (November 2023) was signed at the
  UK-hosted Bletchley Park AI Safety Summit by twenty-eight
  countries plus the EU and named the shared concern with frontier
  AI safety.
- The **Seoul Declaration** on AI safety, agreed at the Seoul AI
  Summit in May 2024, extended the Bletchley agenda and — in the
  Seoul Statement of Intent toward International Cooperation on
  AI Safety Science — set out the pattern of cross-recognition
  between national AI Safety Institutes.
- The **San Francisco convening** in November 2024 brought the
  AISI network together as a working technical body and published
  joint outputs on evaluation practice.

<!-- needs-research: verify the exact publication list from the San Francisco AISI convening and any subsequent joint convenings against primary AISI publications -->

The head does not need to follow every convening in detail. The
head does need to know that the AISI network operates as a
coordinated technical body, that cross-recognition of methods and
findings is an explicit part of the pattern, and that a technique
adopted by one AISI is materially likely to be adopted by others.

## The engagement pattern — four modes

Engagement with the AISI network is not a single activity. The
head designs a portfolio across four modes and staffs each mode
deliberately.

### Mode 1 — membership and participation

The most direct mode is membership in the multi-stakeholder bodies
where the AISI conversation is convened.

- **AISIC** — enterprise membership brings access to working
  groups on evaluation, red-teaming, safe deployment, and
  synthetic-content provenance. The enterprise nominates
  technical staff to working groups; the head owns the enterprise
  posture across those nominations.
- **AI Verify Foundation** — Singapore-convened, with a global
  membership. Focused on open-source testing tooling.
- **EU AI Office working groups** — including the drafting groups
  for the General-Purpose AI Code of Practice under the AI Act.
  These are strictly speaking not AISI convenings but they overlap
  substantially with the AISI-network conversation. See
  [[mod-106-external-positioning-and-voluntary-codes]] for the
  voluntary-code engagement pattern.

Membership is not a badge; it is a commitment of technical staff
time. The head decides which bodies the enterprise joins based on
where the enterprise's AI portfolio has substantive input to give
and where the reputational and regulatory return justifies the
staff commitment.

### Mode 2 — voluntary evaluation collaboration

Some AISIs run voluntary pre-deployment evaluation programmes,
where model developers offer models for AISI testing before
public release. The primary consumers of this mode have been
frontier labs. Enterprises that do substantial fine-tuning of
frontier models, that build agent systems with novel capability
profiles, or that deploy at a scale where their deployment
surface is itself of public-interest concern, are increasingly
part of this conversation.

The head's decision here is whether the enterprise ever offers
models for AISI evaluation. For most non-frontier enterprises the
answer is no. For enterprises whose fine-tuning changes capability
in ways that plausibly matter — biosecurity-adjacent, cyber-
offence-adjacent, autonomous-agent-adjacent — the answer is more
nuanced, and the decision to offer is a Council decision (see
[[mod-102-running-the-program]] chapter 01) rather than a head
decision.

### Mode 3 — consultation input

AISIs and adjacent bodies routinely put drafts out for consultation
— evaluation methodologies, benchmark designs, safety standards,
red-teaming protocols. Enterprise perspective on those drafts is
actively sought. The head owns the enterprise's consultation
posture: which drafts the enterprise responds to, who drafts the
response, how legal and product sign-off happens, and how the
submitted response is captured in the enterprise's
governance-artefact record. Chapter 06 of this module covers the
written-submission side of this discipline in detail.

### Mode 4 — information exchange

The lowest-touch mode is receiving AISI publications, attending
open convenings, and tracking research. This is table stakes — no
enterprise with a serious AI governance function should be doing
less than this — but it is not itself an engagement posture. It
is what the enterprise does before it decides which of the
higher-touch modes to invest in.

## The Inspect discipline

Of the AISI outputs currently available to enterprises, UK AISI's
Inspect framework (github.com/UKGovernmentBEIS/inspect_ai) is the
clearest example of an output an enterprise can actively consume
rather than merely track. Inspect is an MIT-licensed Python
framework for building and running evaluations against language
models. It ships with a task abstraction, a solver abstraction, a
scorer abstraction, and integrations with common model providers.

The enterprise's evaluation function can adopt Inspect for its own
pre-deployment testing. The value is not just the code — the
value is that the enterprise's evaluation posture becomes legible
in a shape a regulator, an auditor, or an AISI counterpart
already recognises. When the audit committee (see
[[mod-103-board-and-audit-committee-reporting]] chapter 02) asks
what evaluation discipline the enterprise runs against its
customer-facing GenAI systems, "we run an Inspect-based evaluation
suite tuned to our deployment context, with the suite versioned
in the AI system inventory" is a materially stronger answer than
a bespoke internal harness with no external referent.

Inspect is one example. The wider principle is that AISI outputs
are inputs to the enterprise's running program. See
[[mod-102-running-the-program]] for the operating discipline into
which those inputs feed.

## The head's engagement calendar

The head runs an annual engagement rhythm across the four modes,
with each item on the calendar assigned an attendance level —
head attends personally, head sends a nominated peer (the
level-50 architect, a senior technical staffer, or a named subject
matter expert), enterprise makes a written submission, or
enterprise tracks only.

A working shape for that calendar:

- **AISIC plenaries and working-group cadences** — head or
  designated peer attends; working-group technical contributions
  staffed to nominated engineers with head sign-off on any
  position that commits the enterprise.
- **UK AISI publications and Inspect release cycle** — evaluation
  function tracks releases; head reviews once per quarter for
  material shifts.
- **Seoul-line joint convenings and San Francisco-line technical
  convenings** — head attends the annual set-piece; sends a peer
  to intermediate technical convenings; captures readout in the
  governance-artefact record.
- **Bletchley-line summit convenings** — head or an executive
  peer attends the biennial summit-level convening; the
  enterprise's position for the summit is a Council-approved
  position (see [[mod-102-running-the-program]] chapter 01).
- **CAISI, AI Verify Foundation, and EU Member State bodies** —
  attendance decisions made per body based on the enterprise's
  operating footprint in that jurisdiction.
- **Consultation submissions** — the head maintains a rolling
  view of open consultations across the network and decides
  submission-by-submission (see chapter 06 of this module).

The calendar is a working artefact. It is reviewed at least
annually, tied to the AI governance function's operating budget
(see [[mod-113-budget-vendor-p-and-l-and-investment-case]]), and
its outputs — attended convenings, submitted responses, adopted
methodologies — feed the CxO and board reporting shape (see
[[mod-103-board-and-audit-committee-reporting]] chapter 04).

## AISI engagement is not enforcement engagement

The final discipline is to keep AISI engagement clearly separated
in the head's mind from enforcement-body engagement.

Chapters 01, 02, and 04 of this module cover engagement with
national competent authorities, EU AI Office and EU AI Board
interactions on Article 72 and Article 73 obligations, and the
regulator-exam runbook. Those engagements are legally consequential.
Legal privilege matters, position statements are drafted with
General Counsel, and every communication is potentially discoverable
in enforcement or litigation.

AISI engagement is technical peer engagement. Candour is expected.
Legal privilege is generally not at stake in a working-group
technical exchange. Position statements are enterprise positions,
not legal opinions. The head's job is to make sure the enterprise's
technical staff engaging with AISIs know which conversation they
are in — and to make sure that the enterprise never inadvertently
treats an AISI counterpart as a regulator or, worse, treats a
regulator counterpart with the informality appropriate to an AISI
working group.

The clean separation is a discipline. When it slips — when a
technical exchange with an AISI drifts into what looks like a
regulatory disclosure, or when a regulator conversation acquires
the informal shape of a technical working group — the head is the
person who catches it and re-frames.

## Summary

- The AISI network is a distributed set of national technical
  safety bodies coordinated through Bletchley (Nov 2023), Seoul
  (May 2024) and follow-on joint convenings — not a regulator, and
  engagement is voluntary and reputational.
- Track the bodies deliberately: US AISI at NIST (current status
  under review post-EO 14179), AISIC, UK AISI (Inspect), CAISI,
  Singapore's AI Verify Foundation and AISI-equivalent, and
  emerging EU Member State bodies.
- Design engagement across four modes — membership /
  participation, voluntary evaluation collaboration, consultation
  input, information exchange — and staff each mode with a named
  attendee and a named position-owner.
- Consume AISI outputs into the running program: Inspect
  (github.com/UKGovernmentBEIS/inspect_ai) is the clearest
  current example of AISI tooling an enterprise evaluation
  function can adopt directly.
- Run an annual engagement calendar with attendance levels — head
  personal, peer-delegated, written submission, or track-only —
  tied to the function's operating budget and reflected in board
  reporting.
- Hold the discipline of separation: AISI conversations are
  technical peer conversations; NCA and enforcement conversations
  are legally consequential. Never let the two blur.
