# exercise-02: Audit Committee Deep-Dive Shape Drill

**Estimated effort:** 3 hours

## Objective

Produce a defensible **audit-committee AI deep-dive pack template**,
plus a worked example, for the enterprise you are working against
(same enterprise as exercise-01 so the two packs compose cleanly).
The pack has to present the three lines as separate views, layer the
external audit and certification-body view over them, and let the
committee act on the composite. Third-line independence has to be
preserved by process, not by intention.

The deliverable is not a summary of what an audit committee sees. It
is the template the head would put in front of the audit committee
next cycle, plus a worked instance the head could defend under a
CAE observer's sampling read.

## Prerequisites

- Chapter [02-audit-committee-deep-dive-shape](../02-audit-committee-deep-dive-shape.md)
  read and internalised.
- Chapter [01-board-report-shape](../01-board-report-shape.md) —
  the audit-committee pack composes with the board pack, so shared
  vocabulary matters.
- The enterprise-context one-pager from exercise-01 (or an
  equivalent scenario).
- A working assumption of the enterprise's Chief Audit Executive
  role and audit-plan structure. Where the enterprise has no
  third-line function, hold that as the scenario and note the
  implication in the exercise.

## Steps

1. **Three-lines coverage map.** Author a one-page mapping of the
   enterprise's AI-scope controls to first-line, second-line, and
   third-line ownership. For each control category (impact
   assessment, evaluation, monitoring, incident response,
   exception approval, vendor onboarding, model deployment gate,
   inventory maintenance), name: the first-line operator, the
   second-line reviewer, and whether the third line has
   scheduled coverage in the current audit-plan period. The map
   is the reference against which the deep-dive pack is drawn.
2. **Pack template — five-cluster shape.** Author the template
   with the five clusters from chapter 02 (first-line control
   effectiveness; second-line coverage and effectiveness; third-
   line findings and remediation; external audit and
   certification-body findings; composite view and committee
   decisions). For each cluster, specify: artefacts,
   length budget, layout convention, and the ownership header
   line (which CxO signs off — see chapter 04).
3. **Second-line honesty section.** Draft the specific fields of
   the second-line-coverage-and-effectiveness cluster with the
   *under-coverage* discipline built in. Every second-line
   report on itself is tempted to over-claim; the template must
   make it hard to over-claim. Include specific prompts the
   template forces the head to answer ("Where in the current
   period did second-line coverage fall short of the standard the
   AIMS calendar prescribes, and why?").
4. **Third-line independence protocol.** Author the half-page
   protocol that governs the head's coordination with the CAE
   for this pack — what the head does and does not do, how draft
   findings return to management for response without violating
   independence, how divergence between second- and third-line
   view is surfaced rather than negotiated. See chapter 02 on
   independence-by-process and chapter 04 on the sign-off flow.
5. **Worked audit-committee pack.** Draft a worked example of the
   pack for one hypothetical quarter, consistent with the
   worked pack from exercise-01. Populate each cluster; include
   at least one third-line finding (drafted at the depth the
   template requires and with a plausible management response),
   at least one external audit or certification-body finding,
   and a composite view that shows explicitly where the three
   lines' views converge and where they diverge.
6. **Watch-list annotation.** Read the worked pack back against
   what the audit committee is watching for (chapter 02: three-
   line divergence, aging findings, exception drift, missing
   root-cause analysis, tail redefinition). Annotate each
   cluster with which watchout it addresses. Any cluster that
   addresses none is either cut or rewritten.

## Deliverables

- `three-lines-coverage-map.md` — the first/second/third line
  ownership map for the enterprise's AI-scope controls.
- `audit-committee-pack-template.md` — the five-cluster
  template with artefacts, ownership headers, and cross-
  references.
- `second-line-honesty-fields.md` — the specific under-coverage
  discipline built into the second-line cluster.
- `cae-independence-protocol.md` — the half-page protocol on
  coordination-without-influence.
- `worked-audit-committee-pack.md` (or `.pdf`) — the populated
  worked example.
- `watchout-annotation.md` — the mapping of clusters to the
  audit committee's watchouts.

## Acceptance criteria

- The three-lines coverage map is at the level of specific
  control categories, not "AI risk generally." An observer can
  trace any specific control to a named line and, for the third
  line, to a specific audit-plan slot.
- The pack template has an ownership header per cluster naming
  the CxO who signs off before circulation. Third-line clusters
  name the CAE explicitly and note that the head does not
  edit third-line content.
- The second-line honesty section includes at least two
  specific prompts forcing the head to name under-coverage. A
  template that lets the second line report on itself without
  ever surfacing a gap is a template the audit committee will
  find suspicious.
- The worked pack shows an explicit divergence between second-
  and third-line view somewhere. A pack where the three lines
  always agree is a pack whose independence is not visible.
- The watchout annotation shows every cluster mapping to at
  least one watchout; clusters mapping to none are cut or
  rewritten before submission.

## Stretch goals

- Draft the audit-plan input the head would submit to the CAE
  for the coming period — the topics the head thinks warrant
  third-line consideration, in the form of a written request
  (see chapter 02 on the head's written-request discipline).
  This is *input to* the CAE's plan, not a directive.
- Draft the ISO/IEC 42006 sampling brief — the short document
  that would guide the certification body through the head's
  own function's evidence during a certification-body audit.
  Chapter 02's second-line-coverage cluster is where the
  sampling brief lands.
- Author a "divergence-resolution memo" template — the format the
  head uses to communicate to the audit-committee chair when
  second- and third-line view will remain divergent through
  distribution. See chapter 04 on conflict-escalation.
- Circulate the pack to a peer with third-line audit background
  (CIA-certified internal auditor, retired CAE, or equivalent)
  and incorporate one round of critique.

## Notes and starter guidance

- The most difficult section to author well is the second-line-
  coverage cluster on the head's own function. The template
  should make honest under-coverage reporting easy and dishonest
  over-claim hard. Prompts like "which non-conformities are open
  past target date and why" and "which audit-plan slots slipped
  and why" are load-bearing.
- Do not paper over three-line divergence. If second- and third-
  line view diverge on a specific finding, the pack shows both
  views and lets the committee decide. Reconciling divergence
  before the committee sees it is an integrity failure the
  audit committee will eventually notice.
- The CAE is not the head's peer in the traditional sense —
  the CAE is independent. The protocol you author for
  coordination is what makes the head-CAE working relationship
  robust to that structural distance.
- Every finding on the pack has a target remediation date and an
  owner. Findings without either become the aging tail that
  chapter 02 names as the strongest signal of program trouble.
