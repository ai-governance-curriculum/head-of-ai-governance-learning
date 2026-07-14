# ISACA COBIT 2019 and NIST CSF 2.0 GOVERN as Sibling Frameworks

## Motivation

An enterprise of any size already has an IT governance framework and a
cybersecurity framework. In the majority of large enterprises, those
frameworks are **ISACA COBIT 2019** (IT governance / enterprise
governance of IT) and **NIST Cybersecurity Framework 2.0** (cyber-risk
management, with a first-class GOVERN function added in the 2.0
release, February 2024). Both are enterprise-scoped, both are the
audit committee's *current* vocabulary for governance and cyber, and
both existed before AI became a first-class risk category.

If the Head of AI Governance ignores this landscape and asks the board
to adopt "another" governance framework specifically for AI, the head
is asking the audit committee to learn a new vocabulary in parallel
with the two they already speak. The audit committee will resist —
correctly. The right move is to position the AI governance function's
frameworks (NIST AI RMF, ISO/IEC 42001, ISO/IEC 38507) as *sibling
references* that **compose with** COBIT 2019 and CSF 2.0 at enterprise
scale, not as rivals.

This chapter shows what those sibling references contribute, where
they compose, and how the head speaks board-fluent COBIT/CSF while
holding an AI-native operating model underneath.

## Core concept: three frameworks, three altitudes, one enterprise

Read the framework stack as three altitudes:

| Altitude | Enterprise IT governance | Enterprise cyber-risk | Enterprise AI risk |
|---|---|---|---|
| Board / directional | COBIT 2019 Governance Objectives (EDM domain) | CSF 2.0 GOVERN function | ISO/IEC 38507 |
| Function / operating | COBIT 2019 Management Objectives (APO, BAI, DSS, MEA) | CSF 2.0 IDENTIFY, PROTECT, DETECT, RESPOND, RECOVER | NIST AI RMF (GOVERN, MAP, MEASURE, MANAGE) |
| Management system | ISO/IEC 27001 (ISMS), ISO/IEC 27005 (info-security risk) | ISO/IEC 27001, ISO 22301 | ISO/IEC 42001 (AIMS), ISO/IEC 23894 (AI risk), ISO/IEC 42005 (AI impact), ISO/IEC 42006 (AIMS certification / audit) |

Each row is a horizontal slice at one altitude. Each column is a
vertical slice through one domain. The head lives in the **AI risk**
column at all three altitudes. The head coordinates with the CIO / CTO
(IT governance column) and the CISO (cyber-risk column) at the same
altitude.

The head's mistake to avoid: pretending the AI column exists in
isolation. It does not. The AI column consumes and extends the other
two columns at every altitude.

## COBIT 2019 — what it contributes

ISACA COBIT 2019 (the 2018-2019 update to COBIT 5) is the enterprise
governance-of-IT framework. It defines:

- **Governance and management objectives** organised into five domains:
  EDM (Evaluate, Direct, Monitor) — governing body scope; APO (Align,
  Plan, Organise), BAI (Build, Acquire, Implement), DSS (Deliver,
  Service, Support), MEA (Monitor, Evaluate, Assess) — management
  scope.
- **A process reference model** with 40 governance and management
  objectives, each with practices, activities, and metrics.
- **Focus areas** — thematic extensions that adapt the core to
  specific domains. ISACA has published dedicated COBIT focus areas
  for **information security**, **DevOps**, and, most importantly for
  this role, a dedicated **information security** guide plus emerging
  **AI-related** guidance and audit materials that ISACA publishes on
  a rolling basis.

At leadership scope, the head uses COBIT 2019 in two ways:

1. **Vocabulary alignment.** When the CIO / CTO speak in EDM / APO /
   BAI / DSS / MEA terms, the head does not translate their
   vocabulary into AI RMF terms and back; the head speaks COBIT.
   Specifically, the AI governance function's operating processes
   compose into APO12 (managed risk), APO13 (managed security), APO14
   (managed data), APO03 (managed enterprise architecture), and
   MEA02 (managed system of internal control). The head knows those
   objective codes because they are the CIO's operating vocabulary.
2. **Composition points.** COBIT's EDM domain is the CIO / IT-side
   analogue of ISO/IEC 38507. The head does not duplicate EDM for AI;
   the head extends EDM03 (managed risk) with the AI risk taxonomy,
   and extends EDM04 (managed resources) with the AI-specific vendor
   and third-party ecosystem.

An enterprise where the head of AI governance cannot map their
operating objectives to COBIT 2019 objective codes will find the
CIO / CTO and the audit function talking past them.

## NIST CSF 2.0 — what the GOVERN function adds

NIST published CSF 2.0 in February 2024 as an update to CSF 1.1. The
single most consequential change was the addition of **GOVERN** as a
first-class function alongside IDENTIFY, PROTECT, DETECT, RESPOND, and
RECOVER. That change is directly relevant to the head, for two reasons.

**One:** CSF 2.0 GOVERN is the CISO's parent operating shape for
cybersecurity governance. It includes categories for organisational
context (GV.OC), risk management strategy (GV.RM), roles /
responsibilities / authorities (GV.RR), policy (GV.PO), oversight
(GV.OV), and cybersecurity supply-chain risk management (GV.SC). The
shape is analogous to NIST AI RMF GOVERN — deliberately, because NIST
authored both — and it is the single most useful bridge between the
CISO's world and the head's world. When the CISO speaks GV.OC, the
head hears GOVERN 1 (organisational context) in AI RMF vocabulary.
The isomorphism is not coincidence.

**Two:** CSF 2.0 explicitly extends coverage of cybersecurity to AI
systems. The head does not run the CSF GOVERN function; the CISO
does. But the head's AI-specific extensions to cybersecurity risk
(prompt injection, model extraction, adversarial ML, training-data
poisoning) map into GV.SC (supply-chain risk) and into IDENTIFY, and
the head coordinates with the CISO on that mapping.

The head reads CSF 2.0 GOVERN as *the CISO's sibling to my GOVERN* —
same shape, adjacent domain, and the coordination point is:

- GV.OC ↔ GOVERN 1 (context and mission)
- GV.RM ↔ GOVERN 1 + GOVERN 2 (risk management strategy)
- GV.RR ↔ GOVERN 2 (accountability structures)
- GV.PO ↔ GOVERN 1 (policy)
- GV.OV ↔ GOVERN 2 + GOVERN 4 (oversight and culture)
- GV.SC ↔ GOVERN 6 (third-party / supply-chain risk)

Explicitly writing that map at composition time is what stops the
head and the CISO from duplicating each other's board reporting.

## The composition pattern the head runs

Composition means: for every AI governance activity, name the
enterprise-parent objective it slots into, and the enterprise-parent
executive who owns that objective. Some examples:

- **AI risk register** at portfolio cadence → composes into COBIT
  APO12 (managed risk) → sponsored by CRO or CIO depending on
  enterprise; head is the AI-column contributor to the enterprise risk
  register, not a separate register.
- **AI security controls** (prompt-injection defence, model-
  extraction detection, adversarial-ML monitoring) → composes into
  CSF 2.0 PROTECT / DETECT under CISO ownership, with the head as
  AI-column contributor. See CISA / NCSC *Guidelines for Secure AI
  System Development* (2023) for the joint reference the head and
  the CISO can point to.
- **AI vendor tiering** → composes into COBIT APO10 (managed vendors)
  and CSF 2.0 GV.SC (cyber supply chain) with the head as the
  AI-column contributor, using the level-50 architect's third-party
  program design.
- **AI incident response** → composes into CSF 2.0 RESPOND / RECOVER
  under CISO / SOC ownership at the runbook layer, with the head as
  the AI-specific-incident coordinator and the executive who owns
  Article 73 and equivalent regulator notification. See
  [[mod-110-incident-leadership]].
- **AI system inventory** → composes into COBIT BAI09 (managed
  assets) and BAI03 (managed solutions identification and build) at
  the IT-asset layer, with the AI-specific inventory extended by
  model-and-system cards, ML-BOM, and evidence architecture from the
  level-50 architect.

For every AI governance activity, the head can name the composition
point on demand. That is what makes the AI governance function feel
like a *coherent extension* of enterprise governance rather than a
new empire.

## What the head does *not* run

Composition also clarifies what belongs elsewhere:

- The head does not run the ISMS under ISO/IEC 27001; the CISO does.
  The AIMS under ISO/IEC 42001 interfaces to but does not replace
  the ISMS.
- The head does not run the enterprise IT governance under COBIT
  2019 EDM; the CIO / CTO do. The AI extension composes into but
  does not replace it.
- The head does not run the cybersecurity function under CSF 2.0; the
  CISO does. The head coordinates on AI-specific extensions and
  interfaces at the joint boundary.

That clarity means the head can be an AI governance executive without
also being a shadow CISO or a shadow CIO. It is protective for
everyone.

## Composition and the board pack

At the board altitude, ISO/IEC 38507 shape (chapter 03) supplies the
head's five-cluster board report. But the audit committee is also
seeing:

- The CIO's IT-governance report shaped by COBIT 2019 EDM domain.
- The CISO's cyber report shaped by CSF 2.0.
- The CRO's enterprise risk report shaped by COSO ERM or ISO 31000.
- The CAE's third-line audit report shaped by IIA IPPF.

The head's ISO/IEC 38507 pack composes into that stack. Where the
head extends the CIO's or CISO's territory for AI-specific reasons,
the extension is *called out and joint-signed*. That prevents the
board from reading "the CIO says X and the head of AI governance
says X-plus-caveat" as internal contradiction. The joint sign-off is
what makes it read as a coherent enterprise position.

## Example — a joint COBIT / CSF / AI RMF crosswalk row

A concrete crosswalk row, at the level the head presents to the audit
committee, might look like:

- **Requirement**: EU AI Act Article 15 (accuracy, robustness,
  cybersecurity for high-risk systems).
- **COBIT 2019 objective**: APO13 (managed security), APO12 (managed
  risk).
- **NIST CSF 2.0**: PR.DS-01, PR.PS-01 (data / platform security);
  DE.CM-06 (external service-provider monitoring).
- **NIST AI RMF category**: MEASURE 2.4, MEASURE 2.5 (robustness,
  reliability); MANAGE 4.1 (post-deployment monitoring).
- **ISO/IEC 42001 Annex A control**: A.8 (operations), A.9
  (performance monitoring).
- **Enterprise control ID**: AI-CTRL-034.
- **Owner**: first line = model owner; second line = head of AI
  governance; third line = CAE.
- **Evidence artefact**: OSCAL assessment plan + CycloneDX ML-BOM +
  quarterly attestation.

That row is what the head brings to the audit committee. It reads as
one requirement across five reference frames because the head speaks
all five.

## Summary

- COBIT 2019 (enterprise IT governance) and NIST CSF 2.0 (enterprise
  cybersecurity with a first-class GOVERN function since Feb 2024)
  are the frameworks the audit committee and the CIO / CISO already
  speak. The head positions the AI governance function's stack —
  NIST AI RMF, ISO/IEC 42001, ISO/IEC 38507 — as *sibling references*
  that compose with them.
- CSF 2.0 GOVERN is deliberately isomorphic to NIST AI RMF GOVERN;
  the six-way category map (GV.OC ↔ GOVERN 1, GV.RM ↔ GOVERN 1+2,
  GV.RR ↔ GOVERN 2, GV.PO ↔ GOVERN 1, GV.OV ↔ GOVERN 2+4, GV.SC ↔
  GOVERN 6) is the CISO-to-head bridge.
- COBIT 2019 EDM is the CIO's board-facing analogue of ISO/IEC 38507
  and the head extends EDM03 (managed risk) and EDM04 (managed
  resources) for AI rather than duplicating.
- Every AI governance activity should map, on demand, to a COBIT /
  CSF composition point and an enterprise-parent executive. That is
  what makes the AI governance function a coherent extension of the
  enterprise rather than a new empire.
- The head does not run the ISMS, the CIO's IT governance, or the
  CISO's cyber function — the head coordinates on the AI-specific
  extension.
