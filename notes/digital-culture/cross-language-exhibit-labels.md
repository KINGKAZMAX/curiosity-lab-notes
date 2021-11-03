# Translate exhibit labels while preserving terms and disagreements

A new editorial exercise for linked language versions of cultural labels. It proposes a reviewable translation process and does not claim completed expert translation or universal equivalence.

> Retrospective study note compiled 2026-10-27. Archive dates are editorial slots; this is an unexecuted design exercise, not a historical activity claim.

## External project context

- [huggingface/transformers — external upstream reference for a new exercise](https://github.com/huggingface/transformers)
- [microsoft/markitdown — external upstream reference for a new exercise](https://github.com/microsoft/markitdown)

## Question

How can an exhibit label be readable in another language while preserving the terms, uncertainty, and perspective of its source? This exercise treats translation as an editorial decision that should remain traceable. It asks how readers can move between versions without losing the identity of the object or mistaking a simplified explanation for an exact equivalent. The challenge is especially visible when a culturally specific term has several plausible translations or no direct counterpart.

## Design proposal

Propose linked language records sharing one object identifier and one source reference. Maintain a small terminology log containing the source term, chosen rendering, alternatives, and an explanation of the choice. Keep original terms visible when they carry important meaning. Distinguish a close translation from an explanatory paraphrase. If versions differ in scope, say so explicitly instead of presenting them as interchangeable text blocks solely because they occupy matching positions in the interface.

## Procedure

Choose a short label with one specialist term, one uncertain claim, and one proper name. Draft a translation and record the decisions that affect meaning. Ask a reviewer familiar with both languages to compare scope, tone, attribution, and uncertainty rather than only grammar. Test switching languages while viewing the same object and while following a source link. Preserve the original label and make revisions to each language version identifiable instead of silently replacing both.
