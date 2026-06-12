# Failure Diagnosis and Decision Logic

## Do Not Equate a Failed Run with a Failed Idea

A negative or weak result can arise from:

- the central scientific relation being false;
- the input material, sample, model, or dataset being unsuitable;
- preparation or assembly failure;
- an assay or instrument problem;
- incorrect software, test mode, parameter, threshold, or preprocessing;
- insufficient sensitivity, power, duration, or dose;
- a missing boundary condition;
- contamination, confounding, or uncontrolled variation.

Require controls that separate these explanations.

## Build a Failure Tree Before Execution

For each required link, define:

1. what evidence confirms the link worked;
2. what failure would look like;
3. the cheapest diagnostic;
4. the corrective action;
5. whether the result still permits judgment of the central claim.

Example structure:

`known-good input? -> assembly valid? -> test system valid? -> intervention delivered? -> decisive response observed?`

If an upstream check fails, classify the run as inconclusive rather than as evidence against the idea.

## Use Positive and Process Controls

- A **positive control** shows that the system can produce the expected signal.
- A **negative control** estimates background or alternative explanations.
- A **process control** confirms that a preparation, assembly, data pipeline, or measurement step worked.
- A **reference benchmark** shows whether the observed magnitude is meaningful.

Controls should map to named branches in the failure tree.

## Make Bounded Revisions

Revise when:

- the test was interpretable;
- a specific, evidence-supported parameter or component is likely responsible;
- the next iteration can discriminate between explanations;
- the revision stays within the preset budget.

Avoid indefinite optimization. After the budget is exhausted, decide whether to pivot or stop.

## Recognize Productive Surprises

An unexpected material, response, pattern, or dataset may support a different valuable question. A pivot is justified when:

- the unexpected result is reproducible;
- it has scientific or practical value;
- it can be framed as a new load-bearing claim;
- a new zero-to-one validation contract can be written.

## Decision Matrix

| Status | Conditions |
|---|---|
| Go | Controls pass, decisive threshold is met, and the effect supports the intended value |
| Revise | Controls pass, claim remains plausible, and a bounded change can resolve the gap |
| Pivot | Original claim is weak, but a reproducible alternative opportunity appears |
| Stop | Interpretable evidence contradicts the claim or expected value does not justify further work |
| Inconclusive | Controls, execution, or measurement failed, so the claim was not tested |

Record the evidence behind the classification and the next action. Do not use ambiguous labels such as "promising" without explicit criteria.
