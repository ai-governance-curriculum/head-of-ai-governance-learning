# The RFI and RFP Response Posture

## Motivation

Requests for information (RFIs) and requests for proposals
(RFPs) that touch AI governance arrive from three quarters —
regulators, industry bodies, and academic or civil-society
researchers — and the enterprise's response to each is a public
or semi-public artefact the head is accountable for. An
enterprise that has no discipline for responding treats each
arrival as a scramble; the response drifts to whoever has the
capacity to draft it; the substance and the tone vary across
responses; and, cumulatively, the enterprise builds a corpus of
responses that contradict each other and reveal the absence of
a settled position.

The chapter-06 discipline in [[mod-104-regulator-engagement]]
covers the public-consultation submission flow — the formal,
docketed regulator consultation with an open comment window.
This chapter is the adjacent discipline for the request-shaped
inbound: an RFI or RFP that arrives *addressed to the
enterprise*, or that arrives in a semi-public forum where the
enterprise's response will be visible to the requester and
often to a broader audience.

The failure mode this chapter opens with is the enterprise's
CTO's office receiving an EU AI Office RFI on GPAI evaluation
methodology, forwarding it to a product manager to draft,
receiving a draft focused on the enterprise's product features,
and returning that to the AI Office. The requester reads a
marketing document where a governance response was expected;
the AI Office adjusts its view of the enterprise's governance
maturity; the head hears about the response two weeks later.
The failure is not the product manager's — the failure is that
the enterprise had no routing discipline for the arrival.

This chapter is that routing discipline. It builds on chapter
06 of [[mod-104-regulator-engagement]] (the public-consultation
process) and on chapters 01 through 03 of this module (the
voluntary-code, standards-body, and public-trust portfolios that
the response cites).

## Core concept — the request taxonomy and its five routing rules

The head runs an intake taxonomy for external requests. Every
inbound falls into one of five categories, and each category
has a specific routing rule.

- **Regulator RFI addressed to the enterprise.** The regulator
  is asking the enterprise, specifically, for information under
  a supervisory or market-surveillance authority. This is the
  head's response, with GC packaging discipline
  ([[mod-104-regulator-engagement]] chapter 07) and the head's
  signature. Chapter 05 of [[mod-104-regulator-engagement]] (the
  exam runbook) is the operating envelope. This chapter's
  discipline does not replace those — it feeds them.
- **Regulator RFI open to the industry.** A regulator publishes
  a request-for-information on a specific topic, addressed to
  "AI providers", "deployers of high-risk AI", or "operators of
  general-purpose AI models". The enterprise may or may not
  respond. If it does, the response goes through the same
  discipline as a public-consultation submission
  ([[mod-104-regulator-engagement]] chapter 06). This chapter's
  discipline covers the stance decision and the routing before
  the drafting cycle begins.
- **Industry-body RFI.** A body the enterprise is a member of,
  or a body soliciting responses from the industry, requests
  information — Frontier Model Forum on a specific frontier-
  safety topic, Partnership on AI on a survey of enterprise
  practice, MLCommons on evaluation methodology contribution. The
  enterprise's response is a members' or peers' communication
  first; it becomes semi-public through the body's own reporting.
- **Academic RFI.** A university research group, a civil-society
  research organisation, or a think tank requests information —
  a survey of enterprise AI governance practice, an interview
  request for a research project, a request for evaluation data.
  The response, if any, is often summarised or quoted in the
  research output; the enterprise's disclosure is public through
  the research once published.
- **Customer / procurement RFP with AI-governance content.** An
  enterprise or public-sector customer's procurement process
  includes AI-governance questions the enterprise's sales team
  is expected to answer as part of the RFP response. The response
  is contractually significant; commitments made in an RFP
  response bind the enterprise if the contract is awarded.

The head does not own the customer RFP process end-to-end — sales
does — but the head owns the *AI-governance content* the response
carries. This chapter treats the customer RFP as the fifth
category because the enterprise's cumulative RFP-response corpus
is a durable record of what the enterprise has committed to
downstream, and the head cannot let sales freelance on
governance commitments.

## Regulator RFIs — the standing surface

The regulator RFI inbound the head expects, across the research-
window jurisdictional landscape, comes from a recurring set of
bodies. The head maintains the operating envelope for each.

- **California Privacy Protection Agency (CPPA).** RFIs on
  Automated Decisionmaking Technology (ADMT) implementation,
  risk assessments, and CCPA / CPRA-adjacent AI matters. Routed
  through the CPPA rulemaking channels and, for enterprise-
  addressed RFIs, direct correspondence.
- **EU AI Office.** RFIs on GPAI provider practice, on evaluation
  methodology, and on Code of Practice implementation. Routed
  via the AI Office correspondence channel or the Code of
  Practice working-group secretariat.
  <!-- needs-research: verify the current channel(s) through
  which the EU AI Office issues RFIs to GPAI providers, and the
  standing operating cadence of any GPAI monitoring surveys,
  against digital-strategy.ec.europa.eu/en/policies/ai-office. -->
- **NIST.** RFIs on AI RMF revisions, on new profiles, on
  crosswalks. Announced via the AI Resource Center (AIRC) and
  via Federal Register notices. Docketed publicly.
- **US AI Safety Institute (US AISI).** RFIs on evaluation
  methodology, on red-teaming practice, on frontier-model
  disclosure practice. Routed via NIST and, for AISIC members,
  via the consortium working-group structure.
  <!-- needs-research: verify the current organisational status
  of US AISI and the current channels through which it issues
  RFIs, given the evolving institutional context. -->
- **Sector regulator RFIs.** Federal Reserve on AI in model
  risk, OCC on AI-vendor overlays to SR 23-4, NAIC AI Working
  Group on state-level enforcement patterns, FDA on GMLP / PCCP
  practice, EBA / ECB on AI in banking, MHRA on medical-device
  AI, EMA on AI in the medicinal product lifecycle, and the
  equivalents in other geographies. Routed through the sector-
  regulator supervisory channels the head has established
  under [[mod-104-regulator-engagement]] chapter 04.
- **National AISI equivalents.** UK AISI, CAISI (Canada), AI
  Verify Foundation / IMDA (Singapore), and equivalents. RFIs
  on evaluation methodology and on frontier-model practice,
  often coordinated across the AISI network.
  <!-- needs-research: verify the current organisational names,
  sponsoring departments, and issuing channels for the UK AISI,
  CAISI, and other national AISI-network members, against
  their respective landing pages. -->

The head does not need to memorise every issuing channel. The
head maintains a *register of expected issuing bodies*, per
jurisdictional footprint, with a named intake owner (see
below) so that any inbound is routed to the right channel
inside the enterprise on arrival.

## Industry-body and academic RFIs

Industry-body RFIs run on the members' cadences of the bodies
the enterprise is a member of (chapter 01). The intake is the
level-50 architect or the operating owner assigned to the body
at sign-on; the response is the operating owner's draft with
the head's substantive review; the artefact is a members-only
submission first and a body-published summary second. Where
the body publishes the enterprise's contribution attributed
(with the enterprise's consent or subject to the body's
publishing rules), the response is treated as a semi-public
artefact and archived on the same terms as a public
submission ([[mod-104-regulator-engagement]] chapter 06
archive discipline).

Academic RFIs run on the researcher's own cadence and often
without a hard deadline. The intake is the head's office (or
Communications, depending on the enterprise's routing);
the response requires a clearer decision than a regulator RFI
because the head has more latitude to decline. The four-move
stance from chapter 01 applies: respond, decline with recorded
rationale, defer with revisit date, or watch (i.e. observe
the research when it publishes without contributing). Common
declines: research whose framing prejudices the enterprise's
position, research whose data-sharing request exceeds what
the enterprise's privacy or commercial constraints permit,
research whose author is in active adversarial engagement
with the enterprise on a related matter.

The default posture is *engage* — declining academic engagement
is not costless (the enterprise reads as opaque or
adversarial in the resulting publication) and thoughtful
engagement is a credibility asset. But engage does not mean
respond to everything; the head decides per request.

## Customer RFPs with AI-governance content

Customer RFPs — enterprise or public-sector procurements —
increasingly include AI-governance questions the sales team is
expected to answer. The questions typically cover: the
enterprise's AI management system (usually asked as ISO/IEC
42001 conformance or equivalent), the enterprise's NIST AI RMF
implementation, the enterprise's incident-reporting practice,
the enterprise's data-provenance and model-provenance
documentation, the enterprise's evaluation and red-teaming
practice, the enterprise's alignment with any voluntary codes
the customer treats as material, and the enterprise's answer
to sector-specific questions (FDA 21 CFR Part 803 exposure,
CFPB adverse-action-notice practice, FTC-adjacent claims, EU
AI Act deployer / provider posture, and the equivalents).

The head does not draft RFP responses. Sales does, with sales-
engineering support and with the level-50 architect providing
the technical answers. The head owns two things:

- **The answer library.** The enterprise's standing responses
  to the standard AI-governance RFP questions live in a shared
  answer library the sales team draws from. The library is
  head-owned for substance and sales-owned for delivery
  (formatting, tailoring to the customer, integration into
  the RFP response document). The library is versioned and
  dated; a customer that later cites the enterprise's answer
  is citing a specific version.
- **The escalation trigger.** Any question the answer library
  does not cover, or any question that requires a bespoke
  commitment beyond the standing answer (e.g. a customer
  requests a specific SLA on incident notification more
  aggressive than the enterprise's standard, or a customer
  requests a specific evaluation the enterprise does not
  currently run), routes to the head for a decision before
  the response goes out. The trigger is written into the
  sales team's process; sales does not commit the enterprise
  to bespoke AI-governance obligations without the head's
  sign-off.

The joint operating agreement between the head and the Chief
Revenue Officer (or Chief Commercial Officer) codifies these
two. The agreement parallels the head-and-CCO agreement from
chapter 03 and the head-and-GC agreement from
[[mod-104-regulator-engagement]] chapter 07. The audit-
committee chair sees the agreement.

## The internal drafting cycle for RFI responses

For RFI responses (regulator, industry-body, or academic), the
internal drafting cycle mirrors the public-consultation cycle
from [[mod-104-regulator-engagement]] chapter 06, with two
simplifications for the request-shaped case.

- **Intake and stance.** The intake owner (a named delegate on
  the head's office, coordinated with GC and Government
  Affairs) receives the request within one business day of
  arrival, opens a response file in the register, and convenes
  a short stance conversation (head, level-50 architect, GC,
  Government Affairs, and the operating owner of the substantive
  area) within one week. The stance decision — respond, decline
  with rationale, defer, watch — is recorded on the stance memo.
- **Draft ownership.** Every response has a single named draft
  owner, usually the level-50 architect or a domain lead. Not
  the intake owner (who runs process, not substance). Not
  Communications (who reviews delivery, not substance).
- **Contributor pass.** The draft owner pulls contributions
  from named contributors — product, engineering, data
  science, sector experts, risk — on the same schedule
  discipline as the public-consultation cycle (late
  contributions do not enter the draft).
- **CxO peer review.** GC (legal exposure and consistency with
  prior filings), CTO (technical accuracy), CRO (risk-appetite
  consistency), Communications (external tone), Government
  Affairs (political-relationship consistency), and any
  sector-specific CxO peer (CISO for security-adjacent, CPO /
  DPO for privacy-adjacent) review the near-final draft. Time-
  boxed; reviewers who do not respond are recorded as no
  comment.
- **Head sign-off.** The head is the accountable signatory.
  For high-visibility responses (regulator-addressed RFIs
  under supervisory authority, RFIs from the AI Office on
  Code of Practice implementation, sector-regulator RFIs the
  regulator is likely to publish in aggregate), the sign-off
  escalates to CEO or GC or both, per the standing
  escalation matrix from
  [[mod-104-regulator-engagement]] chapter 06.
- **Submission and archive.** The response goes out through
  the appropriate channel and is archived on the same terms
  as a public-consultation submission — versioned, dated,
  cross-referenced to the request, with the stance memo and
  contributor / reviewer records attached.

The two simplifications from the public-consultation cycle:
first, the intake step is where the routing decision is made
(the public-consultation flow assumes the response has already
been triggered; here, the response is optional until the intake
step decides). Second, the stance memo is a *lighter* artefact
for a members-only industry-body RFI or an academic RFI than
for a docketed public consultation — a paragraph rather than a
page, though still recorded.

## The intake register

The RFI / RFP intake register is the operating artefact the
intake owner runs against. Every arrival is logged with:

- Request identifier and source body.
- Arrival date and stated response window.
- Intake owner and initial routing (which of the five
  categories).
- Stance decision (respond, decline, defer, watch) and date.
- Draft owner, if responding.
- Sign-off routing and current status.
- Submission date and channel, if responding.
- Archive link to the response and to the stance memo.
- Public-visibility posture — is the response public, semi-
  public through the requester's summary, or private.

The register is auditable by GC, the CxO peer layer, the
audit-committee chair, and (for external auditors under NDA)
the CAE and third-line audit function. It is not the head's
private notes. A regulator or a certification body that asks
"how does the enterprise handle inbound RFIs" receives the
register as the evidence.

## The lens discipline, applied to RFIs

The three-lens discipline from
[[mod-104-regulator-engagement]] chapter 06 — proprietary
interest, industry-common, principled position — applies to
RFI responses the same way as to public-consultation
submissions. The lens is chosen on the stance memo and re-
confirmed at head sign-off. A regulator RFI response written
in a proprietary-interest lens without signposting is the
credibility failure mode that a subsequent enforcement action
cites as evidence of bad-faith engagement; a regulator RFI
response written in a principled-position lens on facts that
turn out to be commercially advantageous to the enterprise
reads as principled when the enterprise's motive is called
out later.

For customer RFPs, the lens is *typically* proprietary interest
— the enterprise is competing for the contract, and both
enterprise and customer understand that. The head's discipline
here is not the lens choice; it is that the enterprise's answers
in the proprietary-interest lens do not contradict the
principled positions the enterprise has taken in regulator
consultations or in position papers. Contradiction is what the
head watches for.

## What the head does not confuse

Three category errors the head does not make:

- An RFI is not an enforcement instrument. GC will decide
  whether a specific RFI carries formal enforcement or
  investigatory posture; the head does not treat every
  regulator inbound as an enforcement escalation, nor treat
  none of them as one. GC per interaction, per the standard
  boundary.
- An academic RFI is not a marketing opportunity. The head
  does not respond to an academic survey with the enterprise's
  brand-safe messaging; the head responds with the head's
  substantive read, which is usable in academic work. The
  enterprise that treats academic engagement as marketing
  drives away the academic surface that would otherwise be
  useful.
- A customer RFP is not a place to invent new AI-governance
  commitments. Sales' pull toward a distinctive commitment
  that wins the RFP is opposed to the head's discipline of
  standing answers the enterprise can defend consistently.
  The escalation trigger is what mediates.

## Summary

- RFIs and RFPs are request-shaped external interactions. The
  head owns the routing discipline that keeps them coherent.
- The five categories are regulator-addressed RFIs, regulator
  industry-wide RFIs, industry-body RFIs, academic RFIs, and
  customer / procurement RFPs; each has a specific routing
  rule and a specific set of internal owners.
- The standing regulator surface as of the research window
  includes CPPA (ADMT), EU AI Office (GPAI implementation),
  NIST (AI RMF and adjacent), US AISI (evaluation
  methodology), sector regulators (Fed, OCC, NAIC, FDA, EBA /
  ECB, MHRA, EMA, and equivalents), and the AISI-network
  national bodies (UK AISI, CAISI, Singapore, and equivalents).
- The internal drafting cycle mirrors the public-consultation
  cycle from [[mod-104-regulator-engagement]] chapter 06, with
  an added intake-and-stance step at the front and a lighter
  stance memo for lower-visibility responses.
- Customer RFP AI-governance content is head-substance,
  sales-delivery — the head owns the answer library and the
  escalation trigger for bespoke commitments; sales owns the
  RFP-response process end-to-end. The head-and-CRO joint
  operating agreement codifies the split.
- The intake register is the head's operating artefact — one
  row per arrival, with stance, draft owner, sign-off routing,
  and archive link — auditable by CxO peers and the audit-
  committee chair.
- The three-lens discipline (proprietary interest, industry-
  common, principled) applies to RFI responses; contradictions
  across responses are the credibility failure mode the head
  watches for.
- Chapter 05 turns to the harder external decisions — the
  responses that decline, the sign-ons that withdraw, and the
  postures that publicly disagree with a regulator's
  methodology.
