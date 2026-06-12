---
name: research-idea-validator
description: Reduce a research idea to its minimum decisive zero-to-one test, design a focused evidence-gathering and validation plan, extract only decision-relevant literature, compare methods and readouts across sources, diagnose failed validation, and issue a go, revise, pivot, or stop decision. Use when Codex needs to assess whether an idea is feasible before building a full study; turn a vague hypothesis into a pilot experiment or proof of concept; decide what literature, methods, controls, measurements, or data are essential; avoid premature full-text reading or large experimental programs; troubleshoot whether failure comes from the idea, implementation, material, assay, model, or test settings; or determine when a project is ready to move from zero-to-one validation into full one-to-ten development.
---

# Research Idea Validator

## Overview

Validate the load-bearing claim of a research idea before investing in a complete study. Work backward from the decision the result must support, remove or substitute nonessential steps, gather only the literature evidence needed to execute and interpret the decisive test, and preserve an explicit path to revise or stop.

## Core Rules

- Treat zero-to-one validation and one-to-ten development as different stages.
- Do not follow the chronological research sequence by default. Find the earliest test that can decide whether the central relation is worth pursuing.
- Delete, simplify, outsource, or replace steps that are not required for the decision. Prefer known-good or commercial components when they isolate the uncertain claim.
- Read literature by information target, not article order. Extract the same kind of evidence across multiple papers before expanding scope.
- Use the minimum readout that can distinguish success from failure. Add measurements only when they resolve a named ambiguity.
- Keep provenance for every extracted method, result, threshold, and caveat.
- Distinguish idea failure from execution failure. A failed run is not automatically a falsified idea.
- Stop refining when the evidence supports the next action.

## Workflow

### 1. Define the decision

State:

- the proposed idea in one sentence;
- the real-world or scientific problem it is meant to address;
- the claim that must be true for the project to remain worthwhile;
- the decisions available after the pilot: `go`, `revise`, `pivot`, or `stop`.

If the useful phenomenon is already guaranteed to exist, classify the work as one-to-ten development and explain why a separate zero-to-one gate is unnecessary.

### 2. Draw the causal chain

Represent the idea as:

`inputs/intervention -> mechanism or intermediate state -> decisive observable -> intended value`

Mark every uncertain link. Separate:

- assumptions already supported by reliable evidence;
- components that can be bought, borrowed, simulated, or replaced with known-good versions;
- project-specific claims that require direct validation.

Read [references/zero-to-one-design.md](references/zero-to-one-design.md) when decomposing a multi-step idea or choosing a decisive gate.

### 3. Apply the deletion test

Remove one step at a time and ask whether the central idea can still be judged.

- If yes, omit or simplify that step in the pilot.
- If no, retain it as part of the minimum validation chain.
- If removing a step makes failure easier to localize, prefer the reduced design.
- If a custom component creates avoidable uncertainty, test first with a validated substitute.

Do not optimize the full system during this stage.

### 4. Specify the validation contract

Before gathering more literature, define:

- test unit, model, material, dataset, or population;
- intervention and comparator;
- positive, negative, and process controls;
- minimum decisive readout;
- success threshold and failure threshold;
- replication or robustness requirement;
- confounders that would make the result uninterpretable;
- maximum time, cost, or iteration budget;
- next action for each plausible outcome.

Use ranges or sensitivity analyses when a defensible threshold is unavailable. Label assumptions rather than inventing precision.

### 5. Build the evidence queue

Create three queues:

1. `extract-now`: likely to contain required methods, settings, controls, thresholds, or representative outcomes;
2. `need-full-text`: relevance is plausible but cannot be judged from title or abstract;
3. `defer`: useful only after the idea passes the zero-to-one gate.

Start from the most relevant existing groups or tags. Skip clearly off-target groups. Inspect uncertain groups by title, then abstract, then full text only as needed.

Encode both provenance and next action in group names or metadata. Keep a short group-formation history when a label alone does not reveal how records entered the group. Separate evidence for validating the study from material intended for later introduction writing or other one-to-ten tasks.

Read [references/triage-and-escalation.md](references/triage-and-escalation.md) for grouping choices, nonexclusive tagging, and stopping rules.

### 6. Extract evidence by target

Create a validation evidence file or structured table. Organize it by source, but extract only predefined targets such as:

- method or preparation steps needed for the decisive test;
- essential settings and parameters;
- minimum characterization needed to verify the input or intermediate state;
- decisive outcome and its measurement method;
- controls, failure modes, and reported thresholds;
- representative figures and captions;
- source identifier and exact location.

Batch the same extraction task across papers. Do not polish formatting during capture.

Read [references/evidence-extraction.md](references/evidence-extraction.md) for the extraction schema and comparison workflow.

### 7. Synthesize a pilot

Compare the extracted evidence side by side. Identify:

- consensus steps;
- parameters with meaningful variation;
- incompatible methods or definitions;
- easiest known-good starting configuration;
- alternative route if the first approach fails;
- measurements needed to separate competing failure explanations.

Produce the smallest executable pilot, not a publication-complete protocol.

### 8. Interpret without overclaiming

Classify the result:

- `go`: the decisive claim passes and the path to one-to-ten development is credible;
- `revise`: the test was interpretable, but a bounded modification is justified;
- `pivot`: an unexpected result supports a different worthwhile question or implementation;
- `stop`: adequate evidence contradicts the load-bearing claim or the remaining uncertainty is not worth resolving;
- `inconclusive`: controls or execution do not permit judgment.

Read [references/failure-diagnosis.md](references/failure-diagnosis.md) before labeling an idea false.

## Required Output

Return a compact validation dossier with:

1. **Idea and decision** - the claim, intended value, and decision options.
2. **Minimum decisive chain** - retained steps, deleted steps, and substitutions.
3. **Validation contract** - model, controls, readout, thresholds, budget, and interpretation rules.
4. **Evidence plan** - search targets, queues, extraction fields, and provenance method.
5. **Pilot protocol** - ordered actions for the minimum test.
6. **Failure tree** - how to distinguish idea failure from material, method, assembly, assay, code, data, or parameter failure.
7. **Decision matrix** - `go`, `revise`, `pivot`, `stop`, and `inconclusive` conditions.
8. **Deferred work** - characterization, optimization, mechanism, performance, presentation, and writing tasks reserved for one-to-ten development.

## Guardrails

- Do not treat one paper, one mentor, or one inherited protocol as ground truth.
- Do not expand reading merely because more literature exists.
- Do not confuse a representative readout with comprehensive characterization.
- Do not let grouping, downloading, extraction, or formatting become the goal.
- Do not interpret absence of evidence as evidence of absence.
- For medical, human-subject, animal, environmental, or otherwise high-risk studies, identify required ethics, safety, regulatory, and expert-review gates before proposing execution.
