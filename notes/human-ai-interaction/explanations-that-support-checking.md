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
