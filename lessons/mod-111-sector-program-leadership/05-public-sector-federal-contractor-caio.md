# Public Sector and Federal Contractor — Leading AI Governance Under the Federal Chief AI Officer Designation and OMB M-25-21

## Motivation

The public-sector head of AI governance operates under a statutory
and executive-branch framework that differs from every private-
sector sector in one specific respect: the head's title, seat, and
minimum accountabilities are set by policy, not chosen. OMB
Memorandum M-25-21, Accelerating Federal Use of AI through
Innovation, Governance, and Public Trust (3 April 2025), directs
each Chief Financial Officers Act agency to designate a Chief
Artificial Intelligence Officer (CAIO), establish an AI Governance
Board, and follow a set of minimum practices for AI use, procurement,
and public transparency. OMB Memorandum M-25-22, Driving Efficient
Acquisition of Artificial Intelligence in Government (3 April 2025),
sets the AI-acquisition companion framework the CAIO's program
operates under.

A private-sector head of AI governance at a federal contractor
serving CAIO-designated agencies faces the same framework from the
other side. The contractor's AI systems become inputs to the agency
CAIO's inventory, risk determinations, and impact assessments. The
contractor's AI vendor obligations extend to the agency's AI use-
case framework — high-impact or otherwise. The federal government's
FedRAMP, NIST SP 800-53, and NIST AI RMF stack is the acquisition
security baseline; NIST AI RMF is the risk-management baseline.

This chapter maps the leadership picture for both cases: a Federal
CAIO leading agency AI governance under M-25-21, and a federal
contractor's head of AI governance leading the enterprise's
posture toward agency CAIOs and the federal AI governance
architecture. It also names the two distinctive interfaces —
Inspector General relations and congressional oversight — that
public-sector leadership has to be designed around and that
private-sector leadership does not.

<!-- needs-research: verify that OMB Memoranda M-25-21 and M-25-22
remain the current governing memoranda for federal AI use and
acquisition, and identify any successor or amending memoranda
issued since April 2025. Federal AI policy has been subject to
significant change through 2025-2026 executive-branch actions;
confirm against whitehouse.gov and cio.gov. -->

## The federal AI governance architecture in one page

- **CAIO designation.** Every CFO Act agency has a designated CAIO
  under M-25-21. The CAIO is a senior official — typically
  reporting to the head of the agency or to a designated deputy —
  with responsibility for coordinating the agency's use of AI,
  promoting AI innovation, managing AI risk, and overseeing
  compliance with the memorandum.
- **AI Governance Board.** Each agency establishes an AI Governance
  Board chaired by the Deputy Secretary (or equivalent) or a
  designee. The Board coordinates agency AI activities across
  components and includes representatives from senior offices
  including OCIO, OCFO, OGC, procurement, privacy, civil rights,
  and mission components. The CAIO is a required Board member.
- **Federal CAIO Council.** OMB, together with the CAIOs of CFO Act
  agencies, operates a CAIO Council under M-25-21 for cross-agency
  coordination.
- **AI Use Case Inventory.** Each agency publishes an annual AI use
  case inventory identifying AI in production or development,
  broken down by mission function, and identifies which uses are
  high-impact per the memorandum's definition.
- **High-impact AI minimum practices.** For AI use cases meeting
  the memorandum's high-impact criteria, agencies apply minimum
  practices covering pre-deployment testing, ongoing monitoring,
  human oversight, providing individuals notice, providing
  remedies, and providing an opt-out where applicable.
- **AI acquisition.** M-25-22 sets the acquisition framework:
  performance-based acquisition preference, contract terms for AI-
  specific rights (data rights, IP, model reuse, transparency),
  and vendor accountability provisions.
- **Public trust and transparency.** Each agency publishes an AI
  Strategy consistent with the memorandum, publishes AI use-case
  inventory updates, and reports periodically to OMB on progress.

<!-- needs-research: verify the specific reporting cadences and
publication deadlines under M-25-21 and M-25-22 as they operate
through 2025-2026. Agency compliance timelines were set relative to
memorandum issuance; confirm current milestones against
cio.gov/ai-in-government. -->

## The Federal CAIO's day-to-day leadership shape

A Federal CAIO's job is the same job in shape as a private-sector
head of AI governance — running a program, reporting to a board,
engaging regulators, positioning externally — but the governmental
context reshapes each element.

### AI Governance Board — chair or member

The Board is chaired by the Deputy Secretary or designee, not by
the CAIO. The CAIO is a required member and is typically the
Board's executive secretary or the equivalent — the person who
prepares the Board's agenda, drives the Board's decisions to
resolution, and represents the Board's decisions inside the
agency's operating cadence. The CAIO is the accountable executive
for AI in the agency in the same way a private-sector head of AI
governance is the accountable executive at an enterprise; the
Deputy Secretary is the CAIO's peer at the equivalent of a Board
Chair position.

The CAIO's operating relationship with the AI Governance Board
resembles the private-sector head's relationship with the audit
committee — see [[mod-103-board-and-audit-committee-reporting]] for
the operating cadence — but with the agency-specific frequency,
membership, and reporting requirements set by M-25-21 rather than
by charter negotiation.

### AI Use Case Inventory

The inventory is public. That is a structural difference from every
private-sector sector: an insurer's regulator inventory is not
public; a bank's model inventory is not public; a federal agency's
AI use-case inventory is published on the agency website and
aggregated to cio.gov. The public visibility changes the CAIO's
governance calculus. Every entry is subject to public reading,
FOIA request, journalist inquiry, congressional question, and
advocacy scrutiny. The CAIO's inventory discipline is designed for
that public read from the first version.

### High-impact AI determinations

The memorandum's high-impact criteria attach when an AI use case's
output serves as a principal basis for decisions or actions that
have a legal, material, binding, or significant effect on the
rights, privileges, or access of individuals or communities. The
CAIO — with the Board — makes the determination for each AI use
case. Underdetermination invites scrutiny; overdetermination
consumes resources needed elsewhere. The determination is written
down, the reasoning is documented, and the record is defensible if
challenged.

### Minimum-practice compliance

For each AI use case determined high-impact, the CAIO ensures the
minimum practices under the memorandum are met: pre-deployment
testing appropriate to the use case, ongoing monitoring, human
oversight, notice, remedy, and (where applicable) opt-out. The
practices themselves are described in the memorandum; the CAIO's
leadership work is running the compliance program that produces
evidence of each practice for each in-scope use case, on a cadence
that satisfies the memorandum's reporting requirements to OMB.

### The FedRAMP + NIST SP 800-53 + NIST AI RMF interface

Federal AI acquisition and operation sits inside three technical
frameworks the CAIO does not own but must operate through.

- **FedRAMP** (Federal Risk and Authorization Management Program)
  governs the security authorisation of cloud services used by
  federal agencies. AI systems delivered as cloud services, or
  cloud-hosted, obtain a FedRAMP authorisation at the appropriate
  impact level (Low, Moderate, High). The CAIO coordinates with
  the CIO and the CISO on the security-authorisation posture; the
  Authorising Official (AO) — typically a senior CIO / CISO office
  official — signs the Authorization to Operate.
- **NIST SP 800-53** (Security and Privacy Controls for Federal
  Information Systems) is the underlying control catalog FedRAMP
  and agency-native security programs implement. AI systems in
  federal use inherit the applicable 800-53 controls. Rev 5 and
  its ongoing revisions include controls that touch AI (personally
  identifiable information handling, machine-learning attack
  surface, adversarial AI).
- **NIST AI Risk Management Framework** (AI 100-1) is the risk-
  management baseline for AI in federal use. Agencies apply the AI
  RMF to their AI use cases either directly or through a NIST AI
  RMF profile (a tailored application of the framework for a
  specific context). NIST's Generative AI Profile (AI 600-1) is
  the leading profile for GenAI systems.

The three frameworks intersect at the AI system's authorisation:
security-authorised under FedRAMP or an agency ATO built on 800-53,
risk-assessed under NIST AI RMF, and use-case-authorised under
M-25-21 minimum practices. The CAIO coordinates the three.

### Inspector General relations

Every CFO Act agency has an Inspector General. IGs conduct
independent audits, inspections, evaluations, and investigations of
agency programs and operations, and report to Congress. AI systems
are an increasing focus of IG work, with topics including AI
governance implementation, high-impact AI compliance, AI acquisition
oversight, and AI-related privacy and civil rights impact.

The CAIO's IG posture is straightforward: cooperative, evidence-
based, and non-defensive. The IG is not the CAIO's adversary. IGs
routinely find governance gaps that the CAIO's own program needs to
close, and the CAIO's job is to make the closing efficient. The
CAIO's operating relationship with the IG includes early
consultation on planned IG work in the AI space, timely response to
IG document requests, participation in IG exit interviews on AI-
related audits, and prompt agency response to IG recommendations.

Where an IG finding materially challenges the CAIO's own
governance decision — a high-impact determination the IG reads as
incorrect, a compliance record the IG reads as insufficient — the
CAIO's response is the technical author's response: what the CAIO
did, what evidence supported the decision, what the CAIO will
change if anything, and what the CAIO will defend as sound
notwithstanding the IG's view. General Counsel is inside the
response drafting; the agency head signs the response to the IG.

### Congressional oversight

Committees with AI jurisdiction — House Oversight and Accountability,
Senate Homeland Security and Governmental Affairs, House Energy and
Commerce, Senate Commerce, and the appropriations subcommittees for
each agency — hold hearings, issue letters, and request briefings.
The CAIO is regularly named as a briefing witness or a hearing
witness at hearings on agency AI use.

Congressional oversight preparation is a distinct discipline. The
CAIO's briefing is prepared with the agency's legislative affairs
office fronting the committee-relationship channel. The CAIO's
written responses to congressional questions are cleared through
legislative affairs, the general counsel, and OMB where the
question touches administration policy. The CAIO's oral testimony
is rehearsed against the committee's likely lines of inquiry.

Congressional oversight is not adversarial by default. Members ask
questions the CAIO can answer, and the CAIO answers with the same
technical author's discipline the IG relationship rests on. Where a
member's question touches administration policy, the CAIO answers
to the agency's role and defers policy-scope questions to OMB or
the White House through legislative affairs.

## The federal contractor's parallel program

A private-sector head of AI governance at a federal contractor
faces the CAIO framework from the vendor side. The contractor's AI
systems become subjects of the agency CAIO's inventory, risk
determinations, and impact assessments. The contractor's AI
governance program adjusts to the framework in five ways.

1. **AI product characterisation for CAIO consumption.** The
   contractor's AI systems are characterised in language and
   structure that maps to the agency CAIO's use-case inventory
   requirements — mission function, use case description, model
   type, data inputs, human-oversight design, monitoring, notice
   and remedy design if the system is high-impact.
2. **Contract terms alignment.** M-25-22's acquisition-side
   framework directs agencies toward specific contract terms on
   data rights, IP, model reuse, transparency, and vendor
   accountability. The contractor's contracts function operates
   against those terms in the agency's solicitation; the head
   contributes the AI-specific technical positions the terms rest
   on.
3. **FedRAMP posture.** Cloud-delivered AI products are FedRAMP-
   authorised at the impact level the target agencies require. The
   head coordinates with the CISO on the AI-specific dimensions of
   the FedRAMP authorisation package.
4. **NIST AI RMF alignment.** The contractor's AI products are
   documented against the NIST AI RMF and the applicable NIST AI
   RMF profiles (Generative AI, sector-specific profiles as they
   are issued). Documentation is designed to feed the agency
   CAIO's risk-assessment process directly.
5. **CAIO relationship management.** The head engages agency CAIOs
   at the level of a peer executive, on a cadence appropriate to
   the contractor's business with the agency. The peer-fronting
   discipline from [[mod-104-regulator-engagement]] chapter 04
   applies: business-development or account management fronts the
   commercial channel; the head fronts the AI governance
   substantive dimension.

## The head's board-level story — federal agency version

The CAIO's board — the AI Governance Board and the agency head — 
reads the CAIO's program against three beats.

1. Every AI use case in the agency's inventory has a defensible
   high-impact determination and a documented minimum-practice
   compliance status. The public inventory reflects reality; the
   next OMB report to Congress is defensible.
2. The AI acquisition portfolio is inside M-25-22's framework, with
   contract terms aligned to the memorandum, vendor accountability
   provisions active, and FedRAMP + NIST 800-53 + NIST AI RMF
   authorisation coherent per system.
3. IG and congressional postures are cooperative and current. Open
   IG recommendations are closing on plan; congressional inquiries
   have been answered on time.

## The head's board-level story — federal contractor version

The contractor's board reads a different but parallel three beats.

1. Every product sold into federal customers is characterised for
   CAIO consumption, FedRAMP-authorised or on the authorisation
   path, NIST AI RMF-aligned, and defensible if it becomes a high-
   impact system in an agency's inventory.
2. Contract terms across the federal book of business are aligned
   to M-25-22 expectations, and vendor accountability provisions
   the enterprise has committed to are met.
3. The CAIO relationship map (which agencies the enterprise sells
   into, who fronts each CAIO relationship, what's open in each
   relationship) is current, in the enterprise's regulator
   inventory analog for public-sector customers.

## Summary

- OMB M-25-21 (3 April 2025) and M-25-22 (3 April 2025) frame the
  Federal CAIO regime: designated CAIO per CFO Act agency, AI
  Governance Board chaired by Deputy Secretary or designee, Federal
  CAIO Council, public AI Use Case Inventory, high-impact minimum
  practices, and AI acquisition framework.
- The Federal CAIO's operating model differs from a private-sector
  head in three important respects: the AI Use Case Inventory is
  public, high-impact determinations attach to individual and
  community rights, and Inspector General plus congressional
  oversight are standing supervisory surfaces.
- Federal AI operates through three intersecting technical
  frameworks the CAIO coordinates: FedRAMP for cloud-service
  security authorisation, NIST SP 800-53 for the underlying
  control catalog, and NIST AI RMF (with the Generative AI Profile
  AI 600-1) for AI risk management.
- IG relations are cooperative and evidence-based. Congressional
  oversight is prepared through legislative affairs, general
  counsel, and OMB where administration policy is touched.
- A federal contractor's head of AI governance adapts the
  enterprise's program to the CAIO regime from the vendor side:
  AI product characterisation for CAIO consumption, M-25-22
  contract-terms alignment, FedRAMP posture, NIST AI RMF
  alignment, and CAIO relationship management.
- Board-level stories differ between the agency and contractor
  cases but share a three-beat structure: portfolio in the
  applicable framework, acquisition or contract terms coherent,
  external supervisory posture (IG and congressional for agency;
  CAIO relationship for contractor) current.
