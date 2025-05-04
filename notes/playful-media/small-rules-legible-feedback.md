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

## Procedure

Create six short board configurations using geometric shapes rather than borrowed artwork. Build a deterministic state table for all possible moves. Test one feedback variant that highlights the affected tile and another that shows only a general success signal. Introduce the same configurations in counterbalanced order during a future walkthrough. After two examples, ask the player to predict a move before executing it. Save the predicted and actual states, and include an unfamiliar arrangement to examine transfer.

## Evaluation plan

Measure correct state predictions, repeated invalid moves, and the number of examples needed before the player can explain the rule. Distinguish learning the rule from simply completing a memorized board. Record whether the replay control helps resolve a misunderstanding. Ask which visual or textual cue informed each prediction. Completion time can provide context but should not dominate interpretation, because deliberate exploration may produce slower play with better understanding. Report only observations from a study that has actually occurred.

## Limitations and next steps

A single rule on a small board does not capture the complexity of action games, narrative systems, or competitive play. Players may also infer patterns that accidentally work in the selected examples. Next, test counterexamples that separate the intended rule from plausible alternatives and inspect whether feedback remains legible at smaller screen sizes. The source projects supply a playful interaction context. They do not establish that this microgame, feedback treatment, or proposed learning effect already exists.
