# Accessible Task Paths in AI Interfaces

A design exercise making a small AI assisted task complete through keyboard, readable text, and multiple input routes, without assuming a particular user capability.

> Retrospective study note compiled 2026-10-27. Archive dates are editorial slots; this is an unexecuted design exercise, not a historical activity claim.

## External project context

- [NousResearch/hermes-agent — external upstream reference for a new exercise](https://github.com/NousResearch/hermes-agent)
- [excalidraw/excalidraw — external upstream reference for a new exercise](https://github.com/excalidraw/excalidraw)

## Research question

Can a person complete an AI assisted task without depending on voice input, precise pointer movement, or interpreting color alone? Use a narrow task: select a fictional sample, inspect its source information, and export a plain text summary. The question concerns completion and comprehension across interaction routes. It does not assume that accessibility is a single setting or that one simulated limitation represents a disability. Each barrier should be tied to a concrete control, message, or transition.

## Design proposal

Provide a clear task sequence with semantic labels, visible keyboard focus, and a persistent location indicator. Make every essential action available through the keyboard, while keeping pointer and text entry options. Present status changes in concise text and avoid using animation as the only signal of completion. Give generated summaries headings and a predictable reading order. Preserve the entered request after validation errors, and place an actionable explanation next to the field that requires attention.

## Procedure

Implement the task with fixed sample data so interface behavior can be tested independently from model variability. Walk through selection, inspection, export, cancellation, and recovery using only the keyboard. Inspect the reading order with a screen reader, enlarge text, and reduce motion. Create one intentional validation error and one delayed response. Record the specific point where focus moves after each action. Repeat the task from a fresh session to detect hidden dependence on prior pointer interactions.

## Evaluation plan

Use a task checklist covering successful completion, discoverability of essential controls, focus continuity, and comprehension of status messages. In a later study with consenting participants, collect descriptions of barriers in their own terms and avoid treating completion time as the sole measure. Separate an inaccessible control from unfamiliar task content. Compare the exported text with the visible summary for missing information. Report which assistive technologies and settings were actually tested rather than claiming universal accessibility from a limited walkthrough.
