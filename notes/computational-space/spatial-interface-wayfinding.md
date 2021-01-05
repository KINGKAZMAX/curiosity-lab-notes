# Use landmarks to test spatial wayfinding

A new navigation exercise inspired by public spatial projects. Proposed routes, controls, and observations are a study plan rather than descriptions of existing repository features.

> Retrospective study note compiled 2026-10-27. Archive dates are editorial slots; this is an unexecuted design exercise, not a historical activity claim.

## External project context

- [mrdoob/three.js — external upstream reference for a new exercise](https://github.com/mrdoob/three.js)
- [godotengine/godot — external upstream reference for a new exercise](https://github.com/godotengine/godot)

## Question

What information helps someone recover their orientation after entering an unfamiliar digital environment? This exercise focuses on a short route between three named destinations rather than open exploration. It asks whether persistent landmarks, a visible destination label, and a return point reduce uncertainty about where to go next. The study should distinguish a wrong turn from a control mistake, because difficulty moving the camera can otherwise be mistaken for difficulty understanding the space.

## Design proposal

Propose a navigation layer with three independent aids: recognizable landmarks in the scene, a compact overview showing current position, and a route list written in plain language. Each destination receives one stable name across all views. Add a clearly labeled return action that restores a known orientation. Avoid revealing every aid at once during comparison; the interface should support controlled variants so the contribution of each aid can be inspected separately.

## Procedure

Construct a small test environment with two junctions, one plausible wrong turn, and three visually distinct landmarks. Write a destination task that does not disclose the route. Verify the task first with keyboard controls and then with pointer controls. Run a rehearsal using landmarks alone, followed by variants adding the overview or route list. Log position, destination changes, recovery actions, and requests for assistance without collecting unrelated browsing activity or personal information.

## Evaluation

Measure successful arrival, incorrect junction choices, time spent stationary at decisions, and use of the return action. Review these traces together with a short explanation of the route from the participant. A faster completion time alone is insufficient if the participant cannot describe their location afterward. Mark control failures separately from orientation failures. Compare variants only when task distance, destination wording, and starting camera position remain equivalent across the planned trials.
