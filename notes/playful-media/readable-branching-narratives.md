# Readable Branching Narratives

A new narrative interface plan for making choices, consequences, and revisitable branches understandable without revealing every future event or erasing player intent.

> Retrospective study note compiled 2026-10-27. Archive dates are editorial slots; this is an unexecuted design exercise, not a historical activity claim.

## External project context

- [godotengine/godot — external upstream reference for a new exercise](https://github.com/godotengine/godot)
- [mermaid-js/mermaid — external upstream reference for a new exercise](https://github.com/mermaid-js/mermaid)

## Research question

How can a branching story let players understand the consequences of a choice without spoiling every future event? Use a fictional journey with three locations and two decisions about whom to accompany. The question concerns readability of the path already taken: whether players remember what they selected, recognize why a scene changed, and know whether revisiting a choice will replace or preserve progress. This exercise addresses interface comprehension rather than claiming a particular emotional or literary effect.

## Design proposal

Create a compact journey map showing visited scenes and the choices that connect them. Hide undiscovered content behind neutral placeholders instead of suggestive spoilers. At each decision, describe the immediate action clearly while leaving its later narrative consequences open. Provide a revisit control that explains whether it creates a new branch or replaces the active path. Keep a visible current path marker and allow players to compare their earlier choice text with the dialogue that followed.

## Procedure

Write a short original story with six scenes, two branching decisions, and one shared ending. Build a transition table before presenting the story. Test the forward route, revisit route, and return to the active branch with deterministic state. Introduce one delayed consequence to examine whether its connection is understandable. Ask a future reader to reconstruct the visited path using the map. Preserve both branch states during the exercise so an accidental revisit cannot silently erase the comparison material.

## Evaluation plan

Measure correct reconstruction of choices, recognition of the active branch, and successful return after revisiting an earlier scene. Ask readers to explain one delayed consequence using evidence from the story. Track accidental overwrites and repeated clicks caused by unclear labels. Compare a map with a simple chronological history using the same narrative. Record comments about spoilers separately from navigation errors. The evaluation should distinguish a deliberately ambiguous story event from an interface that fails to communicate saved state.

## Limitations and next steps

A small authored story may not reveal problems in long narratives with many variables or procedurally generated dialogue. A map can also change the experience by making structure more prominent than characters. Next, test whether optional history views help without interrupting reading, and specify how accessibility tools announce a branch change. Keep the story original and label the prototype as an exercise. The references motivate narrative exploration but do not verify that these branch controls exist in their implementations.
