# NIST AI RMF GOVERN at Leadership Scope, Not as a Compliance Checklist

## Motivation

The NIST AI Risk Management Framework 1.0 (AI 100-1, released January
2023) is the most-referenced non-mandatory AI risk framework in North
American practice. Its four functions — GOVERN, MAP, MEASURE, MANAGE —
are frequently reduced by first-line teams to a checklist: "we did
GOVERN 1.1, we did GOVERN 1.2, therefore we govern." That is not what
the framework is for at leadership scope, and reading it that way makes
the level-60 role look like a paperwork audit.

At leadership scope, GOVERN answers a specific question: *what does a
credible second line for AI look like inside this enterprise, and what
do we produce that proves it exists?* Read that way, the GOVERN function
is a shape — the shape of the accountability, culture, workforce,
policy, and risk-management operating discipline that the head of AI
governance is the accountable executive for. This chapter is how to read
it.

## Core concept: the four functions and where GOVERN sits

The AI RMF 1.0 defines four functions:

- **GOVERN** — cultivate a culture of risk management, including roles,
  responsibilities, accountability, policy, workforce, and the AI risk
  management process itself; enterprise-wide and cross-cutting.
- **MAP** — establish the context and identify risks associated with the
  AI system.
- **MEASURE** — analyse, assess, benchmark, and monitor AI risks and
  their impacts.
- **MANAGE** — allocate resources to map, measure, and manage AI risks,
  and to respond, recover, and communicate about incidents.

GOVERN is the only function that operates at *enterprise* scale rather
than per-system. MAP, MEASURE, and MANAGE run once per AI system (or
per system-family) and iterate through the lifecycle. GOVERN provides
the *containment* — the roles, policies, workforce, and accountability
context inside which MAP / MEASURE / MANAGE actually happen.

That is why GOVERN is the leadership shape. The other three functions
are engineering-and-methodology shapes owned mostly at levels 15 through
40. GOVERN is where the level-60 role's accountability lives.

## GOVERN's six categories, read as a leadership map

The GOVERN function contains six categories (GOVERN 1 through GOVERN 6),
each with several subcategories. At leadership scope, read them as six
questions the head must be able to answer, in writing, with named owners
and evidence, on any Tuesday morning:

- **GOVERN 1 — policies, processes, procedures, and practices are in
  place.** The head's answer: the parent AI policy (owned by head with
  CAIO / CRO sponsorship), the AIMS statement of applicability under
  ISO/IEC 42001, and the policy taxonomy inherited from the level-50
  architect are in force. Any exception or waiver has an owner, an
  expiry, and a report line into the risk committee.
- **GOVERN 2 — accountability structures are in place.** The head's
  answer: the head is the second-line accountable executive; the
  operating-model RACI is published; the AI governance council charter
  is approved by the audit committee; the interface to the third-line
  CAE is documented.
- **GOVERN 3 — workforce diversity, equity, inclusion, and
  accessibility.** The head's answer: hiring plan across levels 15 → 60
  is a board-visible plan, coordinated with CHRO; DEI targets in
  first-line AI teams are visible in the risk register.
- **GOVERN 4 — a culture of critical thinking and psychological safety
  around AI risk.** The head's answer: the incident-and-near-miss
  cadence, the raise-a-concern channel independent of the first line,
  and the escalation-without-fear pattern are all operating and
  reported.
- **GOVERN 5 — engagement with relevant AI actors, including the public
  and affected communities.** The head's answer: the external
  positioning and voluntary-code sign-on discipline (covered later in
  the track) is running; consultation submissions are logged;
  regulator-engagement summary lands in the board pack.
- **GOVERN 6 — third-party risk is addressed.** The head's answer: the
  AI third-party program (tiering, questionnaires, continuous
  monitoring, contract-language, right-to-audit) is running under the
  architect's design and aligned to SR 23-4 third-party guidance and
  ISO/IEC 27036.

Six categories, six answers, one head accountable. That is the shape.

## The Playbook — how to read it at leadership scope

NIST publishes the **AI RMF Playbook** as a companion to the framework
itself. The Playbook is a table of suggested actions, transparency-and-
documentation practices, and reference materials, organised by
subcategory. First-line teams treat it as an implementation cookbook,
and that is fine — but at leadership scope, it does something
different.

At leadership scope the Playbook is a **conformance evidence checklist
that the head can defend to the audit committee, the CAE, a regulator,
or an ISO/IEC 42001 certification body**. Two Playbook uses matter at
level 60:

1. **Coverage discipline.** For each GOVERN subcategory, at least one
   Playbook suggested action must be implemented and evidenced, or the
   head must have a written, dated waiver justifying the gap. That is
   how you avoid "we said we do GOVERN but cannot say what we do."
2. **Maturity signal.** The Playbook's tiered suggested actions
   (transparency-and-documentation practices) let the head plot the AI
   governance function on a maturity trajectory (initial → repeatable
   → defined → managed → optimising) without inventing a new maturity
   model. See [[mod-107-program-measurement-and-maturity]] for how the
   Playbook composes with ISO/IEC 42001, the IAPP AIGP body of
   knowledge, and MLCommons AI Safety in the maturity assessment.

The Playbook is not a bureaucracy. It is the evidence base the head
uses to hold their own function to a written standard.

## GOVERN vs the compliance-checklist trap

A common misread is: "we generated a spreadsheet with every AI RMF
subcategory as a row, marked most of them green, therefore we govern."
That is a checklist artifact, not a governance function. Three tests
detect the trap:

1. **Does the checklist include named accountable executives, not just
   categories?** GOVERN 2 is about accountability structures; a row
   labelled "GOVERN 2.1" with no owner named fails the row's own
   requirement.
2. **Is the evidence machine-consumable by the third line and by a
   regulator?** A screenshot of a slide deck is not evidence. Control
   IDs, dated attestations, model-and-system-card artifacts, OSCAL
   assessment plans, CycloneDX ML-BOMs, SLSA attestations — those are
   evidence.
3. **Would the framework's absence be visible?** GOVERN's presence
   should be detectable by outsiders — for example, an external
   auditor should be able to observe the council cadence, the risk
   register updates, the incident logbook. If nothing external would
   change if GOVERN "went missing," the framework is decorative.

The head's read of GOVERN is passing all three tests continuously.

## Composition with the Generative AI Profile (NIST AI 600-1)

NIST published the **Generative AI Profile (AI 600-1)** in July 2024 as
an overlay on the RMF specifically for generative AI risks — synthetic
content, information integrity, information security, human-AI
configuration, and so on. The head does not re-derive it. The head
treats it as a *published overlay on the GOVERN, MAP, MEASURE, MANAGE
categories* that the enterprise adopts wherever GenAI is in scope
(which, by 2026, is nearly everywhere) and that the architect at level
50 folds into the enterprise crosswalk.

At leadership scope this matters because most of the enterprise's
board-relevant AI risk is GenAI risk. If the board pack does not have
a Generative AI Profile overlay on GOVERN 1 (policy for GenAI),
GOVERN 3 (workforce implications of GenAI), GOVERN 5 (public trust
posture in the GenAI era), and GOVERN 6 (GenAI supply-chain — third-
party foundation model providers), the board pack is not current.

## What GOVERN does *not* say

Reading GOVERN as leadership shape also requires knowing what the
framework does not do:

- **GOVERN does not authorise a reporting line.** Whether the head
  reports to CRO, CAIO, CIO, or directly to the audit committee is a
  governance-arrangement question decided by the board; NIST is
  intentionally silent.
- **GOVERN does not specify an AIMS.** ISO/IEC 42001 does that, and
  the head runs the AIMS operating calendar under the architect's
  design; NIST AI RMF composes with ISO/IEC 42001 but does not replace
  it.
- **GOVERN does not deliver a regulatory-obligation crosswalk.** The
  architect's cross-jurisdiction crosswalk composes the RMF onto the
  EU AI Act, sector rules, state acts, and international regulations.
- **GOVERN does not obligate any specific control.** It sets shape;
  the control library at level 50 sets the specific controls.

That silence is a feature. It is why the RMF is durable across
jurisdictions and sectors, and why the head can defensibly use it as
the second-line shape even under legal regimes that never mention
NIST.

## Example — a GOVERN-shaped one-page board answer

If the audit-committee chair asks the head "how do you govern AI
here?" — the following one-page answer is defensible under GOVERN
because it names accountability, evidence, and cadence for each of the
six categories:

- **GOVERN 1 — policy and process.** Parent AI policy and thirteen
  sub-policies in force; ISO/IEC 42001 AIMS certified by [certification
  body] on [date]; management-review cadence quarterly; exceptions
  logged with expiry.
- **GOVERN 2 — accountability.** Head of AI Governance accountable at
  second line; AI governance council chaired by the head, meeting
  monthly; audit committee AI-risk deep-dive quarterly; third-line
  audit programme owned by CAE, joint appearance annually.
- **GOVERN 3 — workforce.** Multi-year hiring plan approved; DEI
  metrics reported to CHRO monthly; training completion for first-
  line AI teams at 96% (target 100%).
- **GOVERN 4 — culture.** Independent raise-a-concern channel
  reported quarterly to the audit committee; incident-and-near-miss
  learning cycle running; three material near-misses reviewed this
  quarter.
- **GOVERN 5 — external engagement.** Voluntary-code portfolio (EU
  AI Office GPAI Code of Practice, G7 Hiroshima Code, White House
  Voluntary AI Commitments where applicable) reviewed at last
  quarterly board pack; two public-consultation submissions filed;
  regulator-engagement summary attached.
- **GOVERN 6 — third-party.** AI third-party inventory 100% covered
  by tiering; tier-1 vendors monitored continuously; two vendor
  incidents managed this quarter without customer impact.

That is one page. That is what GOVERN means, at level 60, in
production.

## Summary

- Read the AI RMF's GOVERN function as the shape of a credible
  second-line function, not as a checklist. GOVERN's six categories
  translate directly into six answerable questions about
  accountability, policy, workforce, culture, external engagement,
  and third-party risk.
- The Playbook is the coverage-and-maturity evidence base — the head
  uses it to hold their own function to a written standard.
- The Generative AI Profile (AI 600-1) is the published overlay for
  generative AI risk; adopt it, do not re-derive it.
- GOVERN does not set the reporting line, the AIMS, the crosswalk, or
  the controls; those come from ISO/IEC 38507
  ([[03-iso-38507-board-shape]]), ISO/IEC 42001, the level-50
  architect, and the sector regulator. GOVERN sets the *shape*.
- One-page board answers to GOVERN 1 through GOVERN 6 are the
  minimum defensible artefact of the level-60 role.
