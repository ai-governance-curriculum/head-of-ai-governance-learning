# CxO Content Ownership and Sign-Off Before Circulation

## Motivation

A board pack that surprises the CRO, the CAE, the General Counsel,
or the CISO on the day of the meeting is a board pack that has
already failed. Board packs are not journalism. They are jointly
authored artefacts of the enterprise's assurance function, and each
cluster has an *owner* — an executive whose accountability is on the
line for the content. Circulation without those owners' sign-off is
one of the fastest ways for a head of AI governance to lose the trust
of the CxO peer group, and losing that trust is losing the ability
to run the program.

This chapter is the head's operating discipline for who owns what
content in the pack, who signs off before circulation, and how the
sign-off flow is run so it is fast enough to hit the audit-committee
distribution date without cutting corners on ownership.

## Core concept: the head owns the *pack*, not every *word*

The head is the pack's *editor*. Content ownership is distributed
across the CxO peer group:

- The head owns the AIMS operating discipline content, the portfolio
  risk-register content, the AI-specific KRIs, the exception
  posture, the AI-system inventory content, and the aggregate
  narrative that ties the pack together. The head signs off on the
  pack as a whole.
- The **Chief Risk Officer** owns the parent risk framework, the
  appetite framework, and the composition of AI risk with the
  enterprise risk taxonomy. The CRO signs off on cluster content
  that touches appetite calibration, deviation reporting, and
  parent-risk composition.
- The **Chief Audit Executive** owns the third-line audit findings,
  the audit plan, and management-response validation. The CAE
  presents third-line content directly (chapter 02 develops the
  independence discipline). The head does not author or sign off
  on CAE content; the head signs off on management response.
- The **General Counsel** (or Chief Compliance Officer, depending
  on reporting-line configuration — see
  [[mod-101-role-scope-and-leadership-shape]] chapter 06) owns the
  regulator-engagement summary, the legal-privilege posture on any
  content that touches active enforcement, and material-disclosure
  implications. GC signs off on the regulator-engagement cluster
  and on any content flagged as privileged or as potentially
  price-sensitive under listing rules.
- The **CISO** owns AI-specific security signal, security-incident
  content, and third-party security-attestation content. CISO signs
  off on incident-summary content that touches security, on
  supply-chain content that touches vendor security posture, and
  on any KRI that traces to security telemetry.
- The **Chief Privacy Officer / DPO** owns privacy-impact content
  and privacy-incident content. Where privacy risk is a first-order
  category in the appetite framework, CPO/DPO signs off on the
  privacy cluster within the risk register.
- The **Chief Technology Officer** (and the head's own line manager
  where the head reports through the CTO or CIO) owns platform,
  build/buy, and engineering-standards content that lands in the
  technology-committee cut of the pack (chapter 03).

Sign-off is not editorial rubber-stamp. Sign-off is *this content is
mine, I have read it, and I stand behind it in front of the
committee*. A CxO who has not signed off on their cluster does not
have that cluster in the pack.

## The sign-off flow

A defensible sign-off flow works backward from the committee
distribution date. The typical distribution window is five to seven
business days before the meeting (varying by enterprise convention
and by whether the committee reads on tablet or paper). The flow
compresses to fit that window and expands where the window is more
generous.

A workable seven-business-day flow before distribution:

- **T-7 — evidence lock**. All input evidence is locked in the
  AIMS document control. Every KRI value, every risk-register
  update, every incident-log entry, every regulator correspondence
  reference, every audit-finding number that will land in the pack
  is captured with a version stamp and a source citation. After
  T-7 the pack draws only from locked evidence.
- **T-6 — first draft to content owners**. The head circulates the
  first full draft to each cluster's content owner, with the
  specific cluster highlighted. Each owner has an assigned
  reviewer window closing at T-4.
- **T-4 — content-owner sign-off due**. Each owner returns
  sign-off, comments, or requested edits. Sign-off is captured in
  writing (email or the GRC platform's workflow — verbal sign-off
  is not sign-off).
- **T-3 — reconciliation and second draft**. The head incorporates
  edits, resolves conflicts (where two owners want different
  things, the head negotiates or escalates — see below), and
  circulates a second draft with change log.
- **T-2 — final sign-off**. Content owners re-approve their
  clusters against the reconciled draft. Any late change requires a
  re-run of the specific cluster's sign-off.
- **T-1 — head sign-off and distribution package prepared**. The
  head signs off on the pack as a whole and the secretariat
  prepares the distribution package (pack, pre-read, executive
  summary, formal decision items).
- **T-0 — distribution**. The pack goes to committee members.

Where the meeting cadence is compressed (monthly board delta,
between-quarter update), the flow compresses to three business days
with the same steps in a tighter window. Where the meeting is a
substantive audit-committee deep-dive, the flow may extend to
ten business days.

## Conflict escalation between content owners

Two content owners will occasionally want mutually inconsistent
things. The classic examples:

- The CAE's third-line finding phrases a control weakness in a way
  the second line (the head's own function) considers factually
  inaccurate. Third-line independence means the head does not edit
  the finding; the head *does* file management response naming the
  factual disagreement, and the audit committee sees both.
- The General Counsel wants an incident described in language
  narrower than the CISO believes is technically complete, on
  privilege or ongoing-investigation grounds. The head convenes GC
  and CISO to agree the wording; where they cannot agree, the
  matter is escalated to the audit-committee chair *before*
  distribution, with the head's recommendation and the reasons for
  the disagreement.
- The CRO wants an appetite-deviation entry framed against a
  refreshed appetite statement the risk committee has not yet
  ratified. The head declines to backdate — the pack reports
  against the appetite in force at period-end and notes the
  proposed refresh as a decision item in the appropriate cluster.

The head's job in each case is to *hold the discipline that
disagreement is visible*. A pack in which every CxO agrees on every
word is a pack that has been over-negotiated and has lost signal.

## Owner-visibility discipline

Committee-visible material must be *visibly owned*. That means:

- Each cluster of the pack names its owner in a header line
  ("Cluster owner: General Counsel; content sign-off: 2026-Q3
  reporting cycle, dated T-2").
- Decisions requested cite the specific accountable owner for
  execution if approved.
- Where a content owner has dissented from the pack's
  characterisation of their cluster, the dissent is captured
  either in the cluster itself or in a named annex — visibly,
  not silently.
- Where the pack draws on evidence produced by an owner other than
  a CxO signatory (a first-line control operator, a vendor, a
  third-party assessor), the source is cited so a committee member
  can trace back.

## Sign-off is a control

Sign-off is *itself* an AIMS control. The GRC-for-AI platform (or
the equivalent workflow tool) captures the sign-off event, the
signer, the timestamp, the version of the document signed on, and
the comments if any. The signing artefact is part of the AIMS
document control and is inspectable by a certification body under
ISO/IEC 42006 sampling.

Where sign-off is captured by email, the email is filed against the
document under a controlled retention path. Where sign-off is
captured by a workflow tool, the tool's audit log is exported and
retained on the same schedule.

The sign-off record answers a specific question a regulator or a
CAE will eventually ask: *who at this enterprise stood behind this
statement on this date?*

## What the sign-off flow does not do

It does not resolve substantive disagreements about facts, appetite,
or strategy. Those get resolved in council, in committee, or by
executive escalation. Sign-off is a discipline that surfaces
disagreement early enough for those escalations to happen
*before* the committee meets, not on the day.

It does not turn the head into a pass-through. The head still owns
the aggregate narrative — the "here is what has moved and here is
what the committee should notice" summary that ties the clusters
together. Aggregation is a synthesis, and synthesis is a judgement,
and the head signs off on that judgement.

It does not replace working relationships. The flow described here
is the *contingency* — the discipline the head can fall back on
when things get tense. In steady state, most sign-off happens
through informal peer discussion and the flow is a lightweight
formalisation. When things get tense, the flow is what keeps the
program's credibility intact.

## Summary

- The head owns the pack; content is distributed across the CxO
  peer group (CRO, CAE, GC, CISO, CPO/DPO, CTO, and where relevant
  the CAIO) and each cluster has a named owner who signs off
  before circulation.
- The sign-off flow works backward from the committee distribution
  date; a seven-business-day flow with evidence-lock, first draft,
  owner sign-off, reconciliation, final sign-off, head sign-off,
  and distribution is a defensible baseline.
- Owner conflicts are resolved by the head, escalated to the
  committee chair when they cannot be, and always made *visible*
  rather than negotiated into silence.
- Sign-off is itself an AIMS control and is captured in the GRC
  platform or the document-control system, retained on the same
  schedule as other AIMS records, and inspectable by a
  certification body.
- The flow does not replace substantive disagreement or working
  relationships; it is the discipline that makes the pack
  defensible when either is under stress.
