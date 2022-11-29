# Decision Records for AI Co-Creation

A new design plan for documenting alternatives, human selections, and unresolved tradeoffs during an AI assisted spatial concept exercise.

> Retrospective study note compiled 2026-10-27. Archive dates are editorial slots; this is an unexecuted design exercise, not a historical activity claim.

## External project context

- [mermaid-js/mermaid — external upstream reference for a new exercise](https://github.com/mermaid-js/mermaid)
- [Comfy-Org/ComfyUI — external upstream reference for a new exercise](https://github.com/Comfy-Org/ComfyUI)

## Research question

When a design emerges through repeated exchanges with an AI system, how can a later reader understand which decisions a person actually made? This exercise uses a fictional reading room concept with three competing priorities: quiet, circulation, and informal gathering. The question is whether a compact decision record preserves meaningful human choices without requiring a transcript of every interaction. Particular attention goes to rejected alternatives, changed criteria, and cases where the team intentionally leaves a tradeoff unresolved.

## Design proposal

Create a decision panel containing the current question, candidate options, evaluation criteria, selected option, and a short rationale entered or confirmed by the designer. Link each candidate to a visible artifact version rather than only to a chat message. Provide an explicit undecided status and permit a decision to be superseded without deleting its predecessor. AI generated suggestions should carry an origin label; the record should distinguish generating an option, modifying it, and approving it for the next iteration.

## Procedure

Construct three rounds of a fictional design exercise. Begin with a room arrangement, introduce a circulation constraint, then change the intended group size. Save each artifact with a stable identifier. After every round, create one decision record and link it to the relevant alternatives. Deliberately revisit an earlier decision to test supersession. Ask a collaborator in a future walkthrough to reconstruct the sequence from the records alone, with the full transcript withheld until the reconstruction is complete.

## Evaluation plan

Assess whether the reader can identify the current decision, the person who approved it, the rejected alternative, and the constraint that motivated a revision. Measure missing links and contradictory statuses as concrete documentation defects. Track the time required to create records so the system does not turn minor edits into administrative work. Compare reconstruction with and without the panel using matched scenarios. Treat subjective satisfaction as supplementary information, separate from the accuracy of reconstructed decision history.

## Limitations and next steps

A decision panel can record stated reasons but cannot prove that those reasons caused a choice. Designers may also rationalize decisions after the event, especially when a record is created retrospectively. Next, add separate fields for the decision date and documentation date, allowing either to remain unknown. Explore lightweight capture at natural review points rather than after every keystroke. The exercise should preserve disagreement between collaborators instead of compressing all perspectives into a single authoritative account.
