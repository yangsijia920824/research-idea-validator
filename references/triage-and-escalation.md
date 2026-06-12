# Literature Triage and Escalation

## Keep the Current Goal Visible

Write the validation target at the top of the working document. Judge every group, query, title, abstract, and full text against that target. Classification and reading are operations, not outcomes.

## Triage Existing Groups

Classify groups into:

- **direct** - the group name clearly matches the validation target;
- **uncertain** - relevance cannot be decided from the group name;
- **defer** - the group concerns work needed only after validation;
- **skip** - the group is clearly outside the current decision.

Start with direct groups. Visit uncertain groups only if the direct evidence is insufficient or if omission risk matters.

Begin with the groups most closely aligned to the decisive validation target. Do not try to make every field-mapping group exhaustive before the project direction is chosen. Once a direction is selected, enrich only its target groups and nearby alternatives.

## Record Group Formation History

When a group name does not explain where its records came from, add a short group-formation note. Record:

- search expression and fields searched;
- whether records came from automated retrieval or manual title/abstract screening;
- date or library state;
- inclusion rule;
- processing already completed;
- next action.

This enables later incremental updates and prevents re-reading records without knowing what has already been screened or extracted.

## Escalate Gradually

For each record:

1. Judge from title when possible.
2. Search the abstract for target terms and inspect the surrounding sentence.
3. Queue for full text only when title and abstract cannot decide.
4. Download full texts in a batch.
5. Extract the predefined evidence targets in a separate batch.

Do not interrupt title screening to download and deeply read individual papers.

Locate the search expression inside the title or abstract and read the surrounding phrase first. Then inspect nearby subject terms to determine what entity the expression describes. A morphology term, for example, may describe the wrong material or may appear only in a routine characterization sentence.

Use negative wording and relation words as evidence. Expressions such as `rather than`, the orientation of a core-shell structure, or a modifier attached to a different component can make a superficially matching record irrelevant.

## Use Action-Specific Queues

Rename or tag groups by the next action:

- `topic-download-full-text`
- `topic-extract-validation-method-and-readout`
- `topic-extract-introduction`
- `topic-review-abstract`
- `topic-defer-one-to-ten`

This prevents repeatedly deciding what to do with the same record.

Keep the source group visible in the action-group name when useful. After moving records to an action group, optionally remove them from the unprocessed source view so the remaining queue represents unfinished work. Preserve provenance through tags or history rather than destroying it.

## Expand Search Scope with a Trial

When a target group was initially built from title searching, test whether the expression should also be searched in abstracts.

1. Run the title-plus-abstract expansion.
2. Inspect a small sample of newly added records, typically about 10.
3. Estimate whether the expression is used in the intended sense.
4. Keep the expansion when the added queue is manageable or the relevant proportion is useful.
5. Retain title-only searching when the added set is large and relevance is very low.

The source method used a rough working heuristic: accept small result sets directly; for result sets above roughly 200, sample the additions and avoid expansion when fewer than about 1 in 10 are relevant. Treat these as adjustable workload heuristics, not universal scientific thresholds.

Store search-derived records in a group named after the expression. Store manually discovered records separately or document the difference in group history.

## Adjust the Screening Threshold Dynamically

Raise the inclusion threshold when dozens or hundreds of strong candidates already await processing. Prefer records whose titles or abstracts explicitly connect the target component, feature, and intended relation.

Lower the threshold when the first batch fails to provide enough information or the pilot does not work. Revisit previously deferred records, broaden to weaker groups, expand title searches to abstracts, and run a more precise follow-up search.

Do not demand exhaustive retrieval when a sufficient set of reproducible routes already supports the pilot.

## Choose Exclusive or Nonexclusive Tags

Use nonexclusive tagging when:

- mapping a field broadly;
- terminology overlaps;
- missing a relevant paper is costly;
- the same paper can inform several validation routes.

Use more exclusive grouping when:

- the target expression is already clear;
- a narrow, well-defined subset is needed;
- repeated overlap creates more work than protection.

Do not over-optimize this choice. Records remain searchable, and tags can be revised.

## Preserve Redundancy Intentionally

Allow relevant records to appear in multiple groups. Redundancy protects against imperfect search terms and earlier classification mistakes. It is especially useful when morphology, mechanism, material, application, or method terms overlap.

## Stop Rules

Stop expanding the evidence queue when:

- a feasible pilot can be specified;
- essential settings and controls are supported by multiple credible sources;
- at least one alternative route exists for a likely implementation failure;
- further papers repeat known patterns without changing the decision;
- the validation budget would be exceeded before added reading could alter the design.

Before execution, run a narrow novelty check for work that may already test the same idea. This is different from broad exploratory searching.
