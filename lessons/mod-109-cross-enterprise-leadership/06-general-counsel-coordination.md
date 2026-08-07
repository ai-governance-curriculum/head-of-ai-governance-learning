# General Counsel Coordination Pattern — Packaging Interpretation, Not Delivering Legal Opinion

## Motivation

The head of AI governance interprets AI-specific regulatory
obligations every working week — reading Article 6, 9, 16, 26,
27, 55, 72, and 73 of the EU AI Act; interpreting sector-
supervisory letters (SR 11-7 with AI extensions, NAIC AI Model
Bulletin, FDA GMLP, NYC Local Law 144, CPPA ADMT regulations);
tracking state-and-provincial statutes as they come into
force. That interpretation is the head's craft.

Interpretation is not a *legal opinion*. In every developed
legal regime, a formal legal opinion is a specific instrument
delivered by a lawyer, carrying attorney-client privilege,
subject to professional responsibility standards (ABA Model
Rules 2.1 and 2.3 in US context; Bar Council rules in UK;
equivalent professional bodies elsewhere), and forming the
basis on which the enterprise can rely for regulatory-
posture defence. The General Counsel — or their delegate — is
the accountable executive for delivering legal opinion. The
head is not.

The failure mode is a head who blurs the two. The head
delivers what looks like a legal opinion — "here is our
position on Article 22 for this system" — to a business
audience or an external counterparty, without GC
concurrence. When the interpretation is later challenged (in
regulator engagement, in litigation discovery, in an
enforcement action), the enterprise cannot claim to have
relied on it as an opinion because it was not one; it can
also not disavow it because it was delivered on the
enterprise's letterhead. The interpretation becomes an
exposure the enterprise cannot manage.

The coordination pattern in this chapter is what prevents the
blur. It rests on a clear distinction (the head *packages*
interpretation for GC; GC *delivers* legal opinion), an
explicit interface on regulator engagement (head engages
operationally; GC advises on legal exposure), and joint
disciplines on litigation posture, whistleblower and
regulator-complaint intake, and SAR / MOU / MRA management.

The pattern draws on the ABA Model Rules of Professional
Conduct (specifically Rules 2.1 — Advisor and 2.3 —
Evaluation for Use by Third Persons), the IIA Three Lines
Model (which positions GC as an assurance-and-advisory
function separate from second-line risk management), the
regulator-engagement pattern in
[[mod-104-regulator-engagement]] chapter 07 (engagement-
versus-legal-opinion boundary), and the head's own
professional-conduct posture (AIGP-certified, ISO/IEC 42001
Lead-Implementer / Lead-Auditor–certified, or equivalent
professional practice standards).

## Core concept — the head packages; GC delivers

The load-bearing move is a two-word discipline: the head
*packages*; GC *delivers*.

**Packaging** is the head's craft. Given a regulatory text (an
EU AI Act article, a state statute, a sector supervisory
letter) and a specific enterprise fact pattern (a specific AI
system, a specific processing activity, a specific
operational choice), the head assembles the interpretation:
what the text says, how the text applies to the fact pattern,
what the head's function's position is on the application,
what the supporting evidence is (from the AIMS, the
evaluation suite, the third-party evidence pack), what
alternative interpretations exist and why they are less
preferred. The packaging is a *briefing* to GC.

**Delivery** is GC's craft. Given the packaged interpretation
from the head, GC either endorses the interpretation as legal
opinion (the enterprise can rely on it under attorney-client
privilege), modifies it with GC's own legal reasoning, or
substitutes a different opinion. GC's opinion is what the
enterprise carries into regulator engagement, litigation, or
any other formal legal posture.

Two consequences.

- **External-facing communications on regulatory
  interpretation carry GC's opinion, not the head's
  interpretation.** When a customer, a counterparty, a
  regulator, or a court asks for the enterprise's position
  on a regulatory obligation, the position is GC's opinion
  as informed by the head's packaging. The head does not
  deliver the position to the external counterparty
  directly under regulatory-opinion framing.
- **Internal-facing communications carry the head's
  interpretation, clearly labelled as second-line
  interpretation.** When the AI Governance Council, the
  product-owner community, or the enterprise workforce
  needs to know how to operate under a regulatory
  obligation, the head provides interpretation — clearly
  framed as *governance interpretation for operational
  purposes*, not as legal opinion — and the head cites GC's
  standing opinion where GC has issued one.

## The four coordination surfaces

### Surface 1 — regulator-obligation interpretation packaging

The head's function produces regulatory-interpretation
packages on a running basis. Each package has a shape GC can
consume efficiently.

The package template (typically 3–8 pages):

- **The regulatory text.** The specific article, clause, or
  provision, cited by primary source (EUR-Lex for EU law,
  Federal Register or the agency's own publisher for US
  federal, the state legislature for state statutes, the
  regulator's own publication for supervisory letters). Not
  a summary; the actual text.
- **The fact pattern.** The specific enterprise circumstance
  the interpretation applies to — a specific AI system, a
  specific processing activity, a specific operational
  choice. Named against the AIMS inventory ID where relevant.
- **The head's interpretation.** How the head reads the text
  as applying to the fact pattern, with reasoning. Reasoning
  is grounded in the text, in any supervisory guidance the
  regulator has published, in the enterprise's own
  compliance history, and in professional standards
  (ISO/IEC 42001, NIST AI RMF, IAPP AIGP body of knowledge).
- **Alternative interpretations considered.** What other
  readings of the text exist, why they were considered, why
  they were not preferred. The head does not present the
  interpretation as if it were the only possibility; the
  head names the alternatives so GC can evaluate the
  reasoning fully.
- **Supporting evidence.** References to the specific AIMS
  artefacts, evaluation results, third-party evidence packs,
  or other operational evidence that supports the
  interpretation. GC will read the evidence; the head
  provides it in structured form.
- **The head's ask of GC.** Typically one of three:
  endorsement of the interpretation as GC's legal opinion,
  modification with a specific proposed direction,
  substitution with GC's own preferred reading. The head
  states which is being asked for, with the underlying
  reason (a regulator engagement pending; a product-owner
  decision awaiting; a board reporting cycle approaching).

GC's response fits the template inversely — a legal opinion
memo referencing the head's package, endorsing / modifying /
substituting, with GC's own reasoning appended and the
opinion's scope of application named (which systems, which
fact patterns, what date range).

Cadence: packages produced on a running basis per the
regulatory-change discipline in
[[mod-105-regulatory-change-management]]; standing package
inventory maintained; annual joint review of the standing
opinions to catch any that have gone stale (regulator has
updated guidance, enterprise fact pattern has changed).
Joint owner: the head's level-50 architect on the packaging
craft, with the head personally accountable for the ask; GC's
AI-legal lead on the delivery craft.

### Surface 2 — regulator engagement (operational versus legal)

The regulator-engagement pattern from
[[mod-104-regulator-engagement]] chapter 07 is the working
distinction: the head *engages* regulators on operational
matters (Article 72 post-market monitoring reports, Article 73
serious-incident reports, sector-exam coordination, public-
consultation submissions, supervisory-authority correspondence
on operational scope); GC *delivers legal opinion* on any
regulator interaction where legal privilege attaches or where
the interaction carries formal legal-position implications.

The interface specifies:

- **Standing engagement scope for the head.** Article 72 and
  73 filings, sector-supervisory-letter operational responses,
  regulator-examination day-to-day operational coordination,
  public-consultation submissions (operational scope), NIST
  AI RMF and equivalent public-consultation submissions. The
  head is the accountable executive; the level-50 architect
  drafts; GC is briefed as advisory.
- **Standing GC lead for legal-exposure interactions.**
  Enforcement actions (received or anticipated), litigation-
  adjacent regulator interactions, MOUs / MRAs / regulatory
  agreements with legal binding, subject-access-request
  legal analysis, SAR / regulatory-inquiry replies with
  legal-privilege character.
- **The mixed-engagement protocol.** For interactions that
  straddle — a regulator examination that is technically
  operational but signals enforcement interest; a
  supervisory-authority correspondence that touches on
  enforcement history; a public-consultation submission that
  carries litigation-adjacent language — the head and GC
  jointly assess the engagement and decide the lead
  designation. The default posture: when the engagement is
  ambiguous, GC is briefed; when GC assesses legal-privilege
  character, GC becomes the lead.
- **The evidence-privilege protocol.** For evidence produced
  by the head's function that may be discoverable in
  litigation or subject to regulator inspection, the head
  coordinates with GC on the privilege posture — what
  evidence is prepared with attorney work-product protection,
  what evidence is prepared in ordinary course, what evidence
  the head's function does not prepare because the head is
  not the attorney and cannot claim work-product protection.

Cadence: standing engagement per the regulatory calendar; ad-
hoc on new-engagement classification. Joint owner: the head on
the operational-lead side; GC on the legal-lead side; with an
explicit protocol for the mixed engagements.

### Surface 3 — litigation posture, whistleblower and complaint intake

Where the enterprise is party to litigation involving AI
systems — a product-liability claim, a discrimination claim, a
data-subject class action, a shareholder claim on AI-related
disclosure — GC is the accountable executive for litigation
posture. The head's function supports:

- **Fact-witness readiness.** The head's team members may be
  called as fact witnesses; the head coordinates with GC's
  litigation lead on deposition preparation, evidence
  production, and testimony preparation.
- **Documentary-evidence production.** The AIMS artefacts,
  risk register, incident log, evaluation results, and other
  head's-function evidence are subject to discovery. The
  head coordinates with GC on discovery-response protocol —
  what evidence is produced, in what format, with what
  privilege claims, with what redaction discipline.
- **Expert-witness support.** Where the enterprise's
  litigation posture calls for expert testimony on AI-
  specific matters, the head may be called (rare, because
  the head is enterprise-embedded and may not qualify as
  independent) or, more commonly, an external expert is
  engaged by GC and the head briefs the external expert.
- **Litigation-hold discipline.** When GC issues a litigation
  hold on evidence categories the head's function produces
  (AIMS artefacts, risk register entries, incident-log
  records, evaluation results, correspondence with regulators
  on the litigation-adjacent scope), the head's team
  implements the hold and does not delete or overwrite
  covered evidence.

The whistleblower and regulator-complaint intake is a specific
GC-owned surface. The enterprise's whistleblower channel
(mandatory under Sarbanes-Oxley for US-listed, the EU
Whistleblower Directive for EU-scoped employers, and
equivalent regimes elsewhere) is typically administered by GC
or a joint GC / audit-committee-secretariat structure.
Complaints touching on AI-specific matters — AI-safety
allegations from employees, algorithmic-discrimination
allegations from data subjects, foundation-model use
allegations from contract counterparties — route to GC's
intake and, where the substance is AI-specific, GC engages the
head as substantive advisor.

The head does *not* handle whistleblower complaints directly;
the head does not know the identity of the whistleblower
(protected by design in properly-run programs); the head
receives the substantive matter for advisory input at GC's
direction. The head does not investigate whistleblower
allegations independently; the CAE (or GC-directed external
counsel) leads investigations.

### Surface 4 — SAR / MOU / MRA management

Specific instruments the head coordinates with GC on.

- **Subject Access Requests (SARs).** Under GDPR Article 15
  and equivalent statutes (CCPA / CPRA, DPDPA, etc.), the
  DPO's SAR process is the parent (chapter [[03-cpo-dpo-coordination]])
  but GC has a formal legal role where the response
  implicates legal risk. The head's function provides the
  AI-specific technical inputs; GC provides the legal
  posture on the response's legal implications.
- **Memoranda of Understanding (MOUs).** Where the enterprise
  enters MOUs with regulators, with peer institutions on
  AI-safety collaboration, with AI safety institutes
  (see [[mod-104-regulator-engagement]] chapter 03), GC is
  the accountable executive for the legal instrument; the
  head's function is the accountable executive for the
  substantive AI-specific commitments the MOU carries.
- **Mutual Recognition Arrangements (MRAs).** Where the
  enterprise's assurance evidence (ISO/IEC 42001
  certification, notified-body attestations under EU AI Act
  conformity assessment, sector-specific assurance) is
  accepted across jurisdictions under MRAs, GC is the
  accountable executive for the MRA's legal instrument. The
  head's function coordinates on the substantive assurance
  content.
- **Enforcement-adjacent settlements or consent decrees.**
  Where the enterprise enters a settlement, consent decree,
  or non-prosecution agreement carrying AI-specific
  operational obligations, GC is the accountable executive
  for the legal instrument; the head's function is the
  accountable executive for the operational obligations'
  implementation and for reporting on adherence to GC.

Cadence: instrument-by-instrument, with a standing MOU / MRA /
settlement register the head and GC jointly maintain. Joint
owner: GC's transactional lead on the legal-instrument side;
the head's level-50 architect on the substantive-content side.

## The interface document

Consolidated in a single interface document co-signed by the
head and GC, ratified in the CxO adjacency map. The document
has, at minimum:

1. **The packaging-versus-delivery principle.** Head
   packages; GC delivers. The principle is the load-bearing
   discipline of the interface.
2. **The four surfaces.** Regulator-obligation interpretation
   packaging, regulator engagement (operational versus
   legal), litigation posture and whistleblower / complaint
   intake, SAR / MOU / MRA management — each with the
   template, the cadence, and the joint owners.
3. **The mixed-engagement protocol.** For engagements that
   straddle operational and legal, the joint-assessment
   protocol and the default posture.
4. **The evidence-privilege protocol.** The specific
   privilege posture for head's-function evidence,
   coordinated with GC's guidance.
5. **The whistleblower / complaint boundary.** The head does
   not handle whistleblower complaints directly; the head
   provides substantive advisory input at GC's direction;
   the head does not investigate independently.
6. **The escalation ladder.** When the interface breaks — GC
   delivers an opinion the head disputes on substantive
   grounds; the head's packaging is not accepted by GC and
   the underlying regulator engagement is time-sensitive;
   the mixed-engagement designation is contested — how the
   head and GC escalate. Typically: peer conversation, then
   the CEO or the audit-committee chair.
7. **The joint audit-committee appearance.** Once a year, the
   head and GC appear jointly at the audit committee on the
   AI-regulatory-and-legal posture — the standing legal
   opinions, the material regulator engagements, the
   material litigation exposure, the SAR volume and AI-
   specific SAR patterns. Joint appearance is the discipline
   that keeps the interface honest.
8. **The review cadence.** Annual review of the interface
   document; ad-hoc on material regulatory or legal
   developments.

## Anti-patterns the head does not permit

**The freelance legal opinion.** The head delivers a
regulatory-interpretation position to an external
counterparty (a regulator, a customer, a court, a partner
enterprise) as if it were a legal opinion, without GC's
prior endorsement. The remedy is: external-facing regulatory
positions carry GC's opinion; the head packages, GC
delivers, and the delivery is GC's action.

**The GC-bypass on ambiguous engagement.** The head decides a
regulator engagement is operational when it has legal
exposure implications, and proceeds without briefing GC. The
enterprise later finds itself in an enforcement-adjacent
position without GC's legal posture prepared. The remedy is:
when the engagement is ambiguous, GC is briefed; the default
is to over-brief GC, not to under-brief.

**The privilege-blind evidence production.** The head's team
produces documents in a form that would be privileged if
prepared under GC direction, but the documents are not
prepared under GC direction and so carry no privilege
protection. In subsequent litigation, the documents are
discoverable and expose the enterprise more than necessary.
The remedy is: the evidence-privilege protocol governs which
evidence categories are prepared under GC's direction with
work-product protection, and which are prepared in ordinary
course without.

**The whistleblower substantive-role overreach.** The head
receives a whistleblower complaint routed through GC and
begins investigating independently, contacting employees or
witnesses without GC coordination. The whistleblower
protection is compromised; the investigation is compromised;
the enterprise's regulatory position is compromised. The
remedy is: whistleblower complaints are GC-and-CAE-led; the
head advises at their direction; the head does not
investigate independently.

**The regulator-side over-explaining.** Under regulator
questioning, the head volunteers legal reasoning that goes
beyond the operational scope of the engagement. The
reasoning may be earnest and technically correct, and it may
create a legal exposure the enterprise cannot walk back. The
remedy is: the head answers within the engagement's
operational scope; when the regulator's question crosses
into legal-interpretation territory, the head engages GC
before answering and, where necessary, defers the answer
until GC has been consulted.

## Composition with adjacent modules

- The **CxO adjacency map** in
  [[mod-101-role-scope-and-leadership-shape]] chapter 06 is
  the parent boundary document.
- The **engagement-versus-legal-opinion boundary** in
  [[mod-104-regulator-engagement]] chapter 07 is the source
  discipline this chapter operationalises across the four
  surfaces.
- The **regulatory-change discipline** in
  [[mod-105-regulatory-change-management]] surfaces the new
  regulatory instruments the head packages and GC delivers
  on.
- The **CPO / DPO coordination** in chapter 03 of this
  module covers the SAR handling that involves GC.
- The **CISO coordination** in chapter 01 covers the
  incident-adjacent privileged-evidence posture.
- The **incident-leadership discipline** in
  [[mod-110-incident-leadership]] is where the litigation-
  hold and privilege protocols become operational under
  incident time pressure.

## Summary

- The head *packages* regulatory interpretation. GC *delivers*
  legal opinion. The head does not deliver legal opinion to
  external counterparties; the head does not blur the two on
  the enterprise's letterhead.
- Four coordination surfaces carry the work: regulator-
  obligation interpretation packaging (3–8-page template,
  regular cadence), regulator engagement (operational versus
  legal, with a mixed-engagement protocol), litigation
  posture and whistleblower / complaint intake (GC-led with
  head as substantive advisor), SAR / MOU / MRA management
  (joint instrument-by-instrument).
- The mixed-engagement protocol defaults to over-briefing
  GC; when engagements are ambiguous between operational and
  legal, the head briefs GC before the engagement proceeds.
- The evidence-privilege protocol governs which head's-
  function evidence is prepared under GC direction with
  work-product protection and which is prepared in ordinary
  course; the head does not accidentally produce privilege-
  blind evidence that later exposes the enterprise.
- Whistleblower and regulator-complaint intake is GC-and-CAE-
  led; the head advises at their direction; the head does
  not investigate independently or contact witnesses
  independently.
- Five anti-patterns to refuse: freelance legal opinion, GC-
  bypass on ambiguous engagement, privilege-blind evidence
  production, whistleblower substantive-role overreach,
  regulator-side over-explaining.
- The interface document — co-signed by head and GC — is
  ratified in the CxO adjacency map, reviewed annually, and
  the head and GC appear jointly at the audit committee on
  the AI-regulatory-and-legal posture once a year.
- Chapter [[07-cfo-coordination]] turns to the CFO
  adjacency — budget, ROI reporting, capital planning,
  contingency reserve for regulator fines and remediation
  programs.
