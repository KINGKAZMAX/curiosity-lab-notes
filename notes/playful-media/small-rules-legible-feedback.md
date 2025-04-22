# Small Rules, Legible Feedback

A prospective microgame exercise examining whether a simple rule can be learned from immediate, understandable feedback without relying on elaborate instructions.

> Retrospective study note compiled 2026-10-27. Archive dates are editorial slots; this is an unexecuted design exercise, not a historical activity claim.

## External project context

- [godotengine/godot — external upstream reference for a new exercise](https://github.com/godotengine/godot)
- [processing/p5.js — external upstream reference for a new exercise](https://github.com/processing/p5.js)

## Research question

How quickly can a player discover a small game rule when feedback clearly connects an action to its consequence? Design a fictional microgame in which moving one token changes the state of an adjacent tile. The question concerns understanding the local relationship, not increasing engagement time or maximizing reward frequency. Compare whether players can predict the next state after a few examples, explain an unsuccessful move, and apply the same rule when the board arrangement changes.

## Design proposal

Use a compact board with one rule, one action, and three visible outcomes: changed tile, blocked move, and completed pattern. Each outcome receives a brief text label alongside a restrained visual response. Show the affected tile immediately so players can connect cause and effect. Keep score optional and avoid adding bonuses during the first experiment. Provide a replay action that repeats the last transition without changing the board, allowing the feedback itself to become an inspectable teaching tool.
