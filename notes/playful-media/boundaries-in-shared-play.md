# Boundaries in Shared Play

A new cooperative game interface plan for legible action ownership, shared decisions, and respectful pause behavior in a small local two player scenario.

> Retrospective study note compiled 2026-10-27. Archive dates are editorial slots; this is an unexecuted design exercise, not a historical activity claim.

## External project context

- [godotengine/godot — external upstream reference for a new exercise](https://github.com/godotengine/godot)
- [excalidraw/excalidraw — external upstream reference for a new exercise](https://github.com/excalidraw/excalidraw)

## Research question

How can a shared play space make clear which actions belong to one player and which affect both? Use a fictional two player puzzle in which each person moves a different piece toward a common arrangement. The research question concerns control boundaries around movement, pausing, resetting, and changing shared settings. Focus on whether players can recognize another person's pending choice and recover from disagreement. This exercise does not assume that collaboration requires both players to act identically or at equal speed.

## Design proposal

Label each piece and its controls with both a shape and a player identifier. Let either player request a pause, with the pause affecting the whole local session. Require both players to acknowledge a full board reset, while allowing each to undo a personal move that has no shared consequence. Display pending shared actions in a neutral banner. Provide a cancel route and a visible timeout state, avoiding messages that blame one player for taking longer to decide.
