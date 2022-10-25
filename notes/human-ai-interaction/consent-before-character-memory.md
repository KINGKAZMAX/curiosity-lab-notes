# Consent Before Character Memory

A prospective design exercise separating conversational context from persistent character memory, with inspection, correction, and deletion controls. Linked projects provide thematic inspiration, not implementation evidence.

> Retrospective study note compiled 2026-10-27. Archive dates are editorial slots; this is an unexecuted design exercise, not a historical activity claim.

## External project context

- [NousResearch/hermes-agent — external upstream reference for a new exercise](https://github.com/NousResearch/hermes-agent)
- [ollama/ollama — external upstream reference for a new exercise](https://github.com/ollama/ollama)

## Research question

How might a character interface ask permission to remember something without making every conversation feel like a form? This exercise distinguishes temporary context, a suggested memory, and a confirmed memory. A fictional conversation about a preferred nickname provides a low sensitivity test case. The central question is whether people can predict what will persist after closing the session, identify who can use that information, and revoke permission without searching through unrelated account settings.

## Design proposal

Prototype a memory suggestion card beside the relevant message. It contains the exact proposed text, its intended use, a persistence period, and three equally visible actions: save, edit before saving, or keep for this session. A separate memory drawer shows confirmed items with their origin and expiration. Deletion should remove the item from subsequent retrieval in the prototype. The design must distinguish removing stored content from removing previously displayed conversation text, because those are different operations.

## Procedure

Create six scripted conversations using fictional preferences. Include an obvious preference, a passing remark, a correction, a third party detail, an explicit refusal, and an expired memory. Implement the flows with deterministic local data before connecting any model. Walk through saving, editing, refusing, inspecting, and deleting each item. Restart the interface between selected steps to test persistence boundaries. Record expected state transitions alongside screenshots, and use conspicuous sample labels so nobody mistakes the examples for personal records.

## Evaluation plan

In a future usability session, ask participants to predict the stored state before opening the drawer. Compare their predictions with the prototype state, then ask them to remove one item and explain the effect. Track prediction accuracy, time to locate deletion, unintended saves, and recovery from a mistaken save. Use a short comprehension question about the persistence period. Qualitative comments should identify ambiguous labels; they should not be presented as evidence of long term relationship outcomes.

## Limitations and next steps

A deterministic prototype cannot establish how reliably a deployed model obeys memory boundaries or how deletion propagates through backups. This exercise also excludes sensitive personal information and shared accounts. Next, specify retrieval tests that prove deleted entries cannot influence subsequent responses in the controlled environment. Review consent wording separately from interaction speed. Any later implementation should document its actual storage architecture and retention behavior before making promises about erasure or portability to users.
