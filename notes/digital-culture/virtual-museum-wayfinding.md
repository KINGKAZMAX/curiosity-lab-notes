# Let visitors choose a path through a virtual exhibition

A new navigation exercise for separating exhibition structure from movement through a fictional simulated building. External engines are implementation references, with no institutional affiliation implied.

> Retrospective study note compiled 2026-10-27. Archive dates are editorial slots; this is an unexecuted design exercise, not a historical activity claim.

## External project context

- [mrdoob/three.js — external upstream reference for a new exercise](https://github.com/mrdoob/three.js)
- [godotengine/godot — external upstream reference for a new exercise](https://github.com/godotengine/godot)

## Question

Does a visitor understand the exhibition's organization, or are they merely learning how to move through its digital rooms? This exercise distinguishes thematic orientation from camera navigation. It asks whether a person can find a named object, return to a previous section, and choose another interpretive route without traversing every corridor. Spatial exploration may be enjoyable, but it should not make essential cultural information dependent on mastering a game like movement system.

## Design proposal

Propose three connected navigation routes: a room overview, a thematic contents list, and direct object search. Use consistent names across all routes and show the current section in ordinary text. Provide a return link to the previous object and a route back to the exhibition overview. Suggested sequences should remain optional. Distinguish visited items from recommended items so the interface does not imply that one linear path is the only valid interpretation.

## Procedure

Prepare a small exhibition outline with several objects distributed across two themes and three rooms. Create tasks that locate an object by name, follow a theme across rooms, and return to an earlier label. Run the tasks with movement controls, then repeat using only the contents list. Intentionally enter through a deep link to test orientation without an introductory tour. Record where room names, theme names, or object titles become inconsistent.

## Evaluation

Check task completion, incorrect destinations, recovery actions, and whether visitors can describe the exhibition's thematic structure afterward. Compare the information available through direct links with the information encountered during spatial movement. Inspect keyboard reachability and the usefulness of text orientation when the scene is unavailable. Do not judge a route solely by speed: deliberate exploration may be valuable. Record whether the interface allows that choice while keeping requested information easy to locate.
