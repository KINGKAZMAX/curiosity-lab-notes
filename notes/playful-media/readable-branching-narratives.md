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
