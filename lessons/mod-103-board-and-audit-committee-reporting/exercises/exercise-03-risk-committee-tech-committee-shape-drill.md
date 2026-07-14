# exercise-03: Risk-Committee (or Technology-Committee) AI Shape Drill

**Estimated effort:** 3 hours

## Objective

Produce a defensible **risk-committee (or technology-committee) AI
pack template**, plus a worked example, for the enterprise you are
working against (same enterprise as exercises 01 and 02). The pack
has to layer AI content onto the parent risk framework the CRO has
already established — COSO ERM, ISO 31000, or the local equivalent
— rather than inventing a parallel framework. If the enterprise
routes AI to a technology committee instead of a risk committee (or
to both), the pack has to reflect the routing.

The deliverable is not a summary of what a risk committee sees. It
is the template the head would put in front of the risk (or
technology) committee at the next appetite-calibration cycle, with
a worked instance that shows the head's design under a CRO's
challenge.

## Prerequisites

- Chapter [03-risk-committee-and-tech-committee-shape](../03-risk-committee-and-tech-committee-shape.md)
  read and internalised.
- Chapter [07-frontier-lab-tiered-frameworks](../07-frontier-lab-tiered-frameworks.md)
  read — the capability-tier discipline lands in this pack.
- The enterprise-context one-pager from exercise-01.
- A working assumption of the enterprise's parent risk framework
  (COSO ERM in most US enterprises; ISO 31000 elsewhere) and the
  current AI risk taxonomy from mod-102 chapter 03.

## Steps

1. **Routing decision one-pager.** Write a half-page identifying
   the committee(s) AI risk routes to at this enterprise, the
   scope each committee holds, and the rationale for the
   routing. Where the enterprise routes to both a risk committee
   and a technology committee, name what each sees and how the
   two views are kept consistent. Where a routing change is
   anticipated, note the transition discipline (chapter 03).
2. **Parent-framework composition map.** Draft the one-page map
   showing how AI risk composes with the parent risk framework
   in force. For each parent risk category the enterprise runs
   (operational, technology, cyber, model, credit, market,
   insurance, patient-safety, legal, compliance, reputational
   — the set will vary by enterprise), note: whether AI
   contributes to the category, the current AI-specific
   contribution, and any cross-category interaction. For
   financial-services enterprises, name the model-risk-
   management framework (Federal Reserve SR 11-7, OCC Bulletin
   2011-12, OSFI Guideline E-23, EBA / ECB model-risk guidance)
   and how AI systems are treated under it.
3. **Pack template — five-cluster shape.** Author the template
   with the five clusters from chapter 03 (portfolio appetite
   calibration; capability-tier posture and escalations; parent-
   risk composition; treatment and monitoring at portfolio
   scope; technology-committee-specific build/buy and
   resilience content where applicable). For each cluster,
   specify artefacts, length budget, layout, and CxO ownership
   header.
4. **Capability-tier framework.** Draft the capability-tier
   framework the pack presents in cluster 2. For each tier:
   entry criteria (evidence-defined, per chapter 07 move 1);
   pre-committed responses (chapter 07 move 2); named
   stop-shipping triggers with authorising body (chapter 07
   move 3); the review cadence for the tier definition itself
   (chapter 07 move 4). Aim for three to five tiers, no more.
   Tie the tier definitions to the enterprise's own risk
   taxonomy and deployment scope; do not import frontier-lab
   risk categories verbatim.
5. **Worked risk-committee pack.** Draft a worked example of the
   pack for one hypothetical appetite-calibration cycle,
   consistent with the worked packs from exercises 01 and 02.
   Populate each cluster; include at least one appetite
   deviation with treatment; at least one tier-migration event;
   at least one stop-shipping trigger that has fired in a prior
   cycle (or the head's honest note that none has fired and the
   implication of that); and a specific appetite-calibration
   decision requested.
6. **CRO-challenge dry run.** Read the worked pack back
   against the risk committee's watchouts (chapter 03: vague
   appetite, quietly buried deviations, AI treated as bolt-on
   rather than overlay, post-hoc capability-tier response,
   never-fired stop-shipping triggers). For each watchout,
   annotate the pack where it is answered (or where it fails
   and needs revision).

## Deliverables

- `routing-decision.md` — the half-page routing rationale.
- `parent-framework-composition-map.md` — the composition of AI
  risk with the parent risk taxonomy.
- `risk-committee-pack-template.md` — the five-cluster template.
- `capability-tier-framework.md` — the tier definitions,
  pre-committed responses, and stop-shipping triggers.
- `worked-risk-committee-pack.md` (or `.pdf`) — the populated
  worked example.
- `cro-challenge-annotation.md` — the watchout mapping.

## Acceptance criteria

- The routing decision is specific to the enterprise's board
  committee structure, not generic. If the routing is unusual
  (a newly constituted AI committee, split scope), the rationale
  is clear.
- The parent-framework composition map shows AI as an *overlay*
  on the existing risk taxonomy, not as an added category. For
  financial-services enterprises, the composition with
  model-risk-management is explicit.
- The capability-tier framework has three to five tiers with
  evidence-defined entry criteria, pre-committed responses,
  named stop-shipping triggers, and a named review cadence.
  Tiers defined by narrative ("Tier 1 is the highest-impact
  systems") without evidence criteria are disqualifying.
- The worked pack includes at least one appetite deviation with
  treatment applied and the appetite-recalibration implication
  named — not swept under a subcategory.
- The pack includes an honest position on stop-shipping
  triggers: either at least one that has fired with root cause,
  or the head's explicit note that no trigger has fired and the
  implication (thresholds may be too permissive; monitoring may
  be under-detecting).
- The CRO-challenge annotation shows every watchout answered
  explicitly in the pack.

## Stretch goals

- Author the appetite-calibration decision paper the pack
  supports — the specific request-for-decision the committee
  will vote on, with the recommended appetite adjustment and
  the rationale.
- For a financial-services enterprise, draft the section of the
  pack that would land at a supervisory examiner reading the
  model-risk-management overlay — the specific evidence the
  examiner would sample under SR 11-7 (or the relevant local
  equivalent).
- Read one current published version of a frontier-lab tiered
  framework (Anthropic RSP, OpenAI Preparedness Framework,
  Google DeepMind FSF) and write a half-page note on which
  design moves you adapted for your enterprise capability-tier
  framework and which you did not, with rationale. See chapter
  07 for the shape.
- Circulate the pack to a peer with CRO-level experience (or an
  operating risk-committee member) and incorporate one round of
  critique.

## Notes and starter guidance

- The parent-framework composition is the load-bearing move. A
  risk committee that reads AI as an isolated new category will
  drift into treating it separately, which is how AI risk stops
  being real risk-managed and starts being a compliance
  exercise. The pack fights that drift.
- Resist the urge to make the capability-tier framework look
  like a frontier-lab framework in miniature. The enterprise's
  risk taxonomy, deployment scope, and operating reality are
  different; the framework has to fit those. Chapter 07 is
  explicit on what does *not* transfer.
- Never-fired stop-shipping triggers are the honest tell that
  the head has to surface. A pack that quietly avoids the
  question is a pack a committee member with risk fluency will
  notice.
- Appetite statements are worth stress-testing before the pack
  is submitted. A statement that cannot be measured against
  cannot be governed against; if you cannot write a specific
  KRI query that would tell you whether the appetite is
  breached, the appetite is not real.
