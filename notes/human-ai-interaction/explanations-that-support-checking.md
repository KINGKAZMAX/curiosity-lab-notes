# Explanations That Support Checking

A new interface plan for concise, verifiable explanations of AI assisted recommendations using explicit observations and assumptions rather than unverifiable accounts of internal reasoning.

> Retrospective study note compiled 2026-10-27. Archive dates are editorial slots; this is an unexecuted design exercise, not a historical activity claim.

## External project context

- [huggingface/transformers — external upstream reference for a new exercise](https://github.com/huggingface/transformers)
- [d3/d3 — external upstream reference for a new exercise](https://github.com/d3/d3)

## Research question

What information helps someone check a recommendation without forcing them to read a long narrative about how it was generated? Use a fictional exhibition recommendation based on stated interests, available time, and accessibility preferences. The research question is whether users can identify the inputs that matter, notice an unsupported assumption, and request a meaningful revision. The explanation should support inspection of the output and its evidence, rather than claiming to reveal hidden internal model reasoning or a complete causal account.

## Design proposal

Offer a compact explanation containing relevant inputs, the applicable selection rule, the supporting source card, and one unresolved assumption when present. Let users edit an input directly from the explanation and preview how the recommendation changes. Distinguish a documented rule from a model generated justification. Keep the original recommendation visible while the explanation is expanded. A source link should open the specific supporting passage in the prototype dataset, not an unrelated homepage that merely appears authoritative.

## Procedure

Construct eight fictional recommendation cases using a transparent rule table. Include two cases where a source does not support the displayed claim and two where a changed preference should alter the result. Build short and expanded explanation views with identical underlying data. Have reviewers check that every cited passage matches its claim before the walkthrough. Then introduce the planned inconsistencies in a separate test fixture. Label all case materials as synthetic and preserve the clean fixture for comparison.

## Evaluation plan

Ask future participants to identify why an item was suggested, detect unsupported claims, and revise one preference to obtain an appropriate alternative. Score answers against the rule table and source passages. Measure explanation openings, successful corrections, and instances where a polished explanation increases acceptance of an incorrect result. Compare short and expanded views without assuming that more text is better. Collect comments about what information was missing, and distinguish accurate understanding from confidence in the system.

## Limitations and next steps

A rule based fixture makes evaluation possible but does not represent the complexity of open ended model outputs. Explanations generated after a recommendation may be plausible without faithfully describing its production. Next, separate factual provenance from explanatory wording in the data model and require explicit labels for unsupported assumptions. Evaluate whether edited inputs actually affect subsequent recommendations. This notebook proposes a checking interface and controlled study; it does not claim interpretability guarantees or existing functionality in the reference projects.
