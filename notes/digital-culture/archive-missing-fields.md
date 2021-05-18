# Make missing archive information useful rather than invisible

A new archive quality exercise for distinguishing unknown, unrecorded, disputed, and inapplicable information. It proposes practical review queues without inventing facts about works or artists.

> Retrospective study note compiled 2026-10-27. Archive dates are editorial slots; this is an unexecuted design exercise, not a historical activity claim.

## External project context

- [d3/d3 — external upstream reference for a new exercise](https://github.com/d3/d3)
- [firecrawl/firecrawl — external upstream reference for a new exercise](https://github.com/firecrawl/firecrawl)

## Question

How should an artwork archive behave when dates, materials, dimensions, attribution, or exhibition context are incomplete? This exercise asks whether missing information can guide careful follow up instead of being hidden behind a polished presentation. It distinguishes an unknown value from a field that was never reviewed and from a field that does not apply. The objective is an honest, workable record, not a complete looking catalogue assembled through plausible guesses.

## Design proposal

Propose explicit states for missing values: unknown, not yet reviewed, not applicable, and disputed. Pair each state with an optional reason and a source needed for resolution. Keep these states separate from actual field values so search and export do not confuse a missing date with a literal date string. Provide a review queue organized by the practical effect of the gap, such as blocked attribution or an ambiguous version, rather than a universal completeness score.

## Procedure

Create a small set of fictional archive records with deliberately missing fields and inspect only the information their fixture sources support. Mark absent fields without filling them from visual inference. Create a documented follow up task for each important gap, naming the evidence that could resolve it. Test how the records appear in a list, a detail page, and an exported caption. Add a disputed attribution fixture to check that two competing claims are preserved with their sources.

## Evaluation

Evaluate whether reviewers can distinguish the missing states and choose a sensible next action. Count cases where an export hides uncertainty or a filter incorrectly excludes incomplete records. Check that resolving a field records the supporting source and does not erase the previous uncertainty. Review usefulness of the task queue rather than rewarding the largest number of populated fields. A smaller archive with traceable facts can be more informative than a fuller one with unsupported values.
