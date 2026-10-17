---
name: content-qa-test-designer-skill
description: Design reproducible content-quality test cases, positive and negative fixtures, and evidence-based rubrics for marketing drafts. Use for a QA plan or test suite, not automated publication or detector evasion.
---

# Content QA Test Designer
Adapted on 2026-10-16 from the Promptfoo simple-test case/assertion structure; see THIRD_PARTY_NOTICES.md.

## Inputs
Reuse permitted brief/context first. Capture the draft or workflow under test, intended audience/channel, source-of-truth facts, mandatory constraints, allowed stylistic freedom, and cost/tool limits. Track source ID, location/date, permitted use and unresolved conflicts. Ask only for critical missing inputs.

## Build the test plan
1. Turn requirements into observable checks. Keep factual/content gates separate from subjective style scores. Unsupported material claims block acceptance regardless of style.
2. Define a rubric before looking at candidate outputs: factual support, required information, task usefulness, channel fit and style. Give anchors and a decision rule. Use pass/fail for objective rules; for subjective checks use 0=violates, 1=partial, 2=meets, with evidence and uncertainty.
3. Create at least one positive fixture, one negative fixture, one acceptable paraphrase, and one polished-but-factually-wrong fixture. Include missing-source or contradictory-source behavior when relevant.
4. For each case record ID, purpose, input/source IDs, candidate content, expected accept/reject/review decision, checks, reason, and execution status. Fixtures are fictional unless actual inputs are explicitly authorized. Expected labels are design intent, never measured results.
5. Prefer exact checks for fixed terms and human review for meaning. A keyword match cannot prove a claim true; absence of a preferred phrase cannot prove a valid paraphrase wrong.
6. Calibrate with labeled fixtures. A false accept accepts a known invalid output; a false reject rejects a known valid output. Keep uncertain labels out of these denominators and report them separately. False-accept rate = false accepts / known-invalid evaluated cases; false-reject rate = false rejects / known-valid evaluated cases. If denominator is zero, report N/A.
7. If execution is requested, use available authorized tools or a transparent manual review. Record candidate version, method/reviewer, timestamp, observed decision, evidence and disagreements. Never substitute expected labels for observations. No paid model calls by default.
8. Return assets/qa-plan-template.md plus the fixture set. Report unexecuted cases, coverage limits, blockers and the next useful test. Do not promise universal reliability from a small set.

See examples/fictional-qa-plan.md for a compact design-only example. Optional external harness integration is out of scope for this first version; no runtime dependencies or API keys are needed.

## Uncertainty in expected decisions
Treat time words such as "weekend", "soon", "now" and "still available" as factual/date or availability claims when they describe the offer, not as harmless style. Check their source and applicable date. Do not supply omitted actors, dates, quantities or terms to make a fixture complete.

Do not grade against one side of an unresolved conflict. Keep both source versions and label affected fixtures Needs review until an authorized resolution identifies the standard; recency alone is not a supersession rule. Do not mark one side Reject merely for contradicting the other. Missing-source and unresolved-conflict labels remain uncertain and outside known-valid/invalid calibration denominators. In the fixture table, state the source status, why the label is uncertain and what would resolve it; do not bury this only in the ledger.

## Boundaries
Do not optimize for defeating AI-writing, plagiarism, spam, safety or integrity detectors. Do not publish, send or alter production content. Do not expose private inputs in reusable fixtures. Approval to design tests does not authorize external execution, sharing, or spending.

