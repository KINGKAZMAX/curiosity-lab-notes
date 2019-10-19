# Guide the camera while preserving user control

A proposed camera behavior study for explaining spatial content without disorienting the viewer. It describes a new interaction experiment rather than completed interface behavior.

> Retrospective study note compiled 2026-10-27. Archive dates are editorial slots; this is an unexecuted design exercise, not a historical activity claim.

## External project context

- [mrdoob/three.js — external upstream reference for a new exercise](https://github.com/mrdoob/three.js)
- [godotengine/godot — external upstream reference for a new exercise](https://github.com/godotengine/godot)

## Question

When an interface moves the camera toward a selected object, does the movement explain context or take control away from the viewer? This exercise examines short transitions between a whole scene and a selected detail. It asks whether people can predict the destination, interrupt the movement, and return to their previous view. Camera behavior should support interpretation of scale and position; a visually attractive flight is not enough to demonstrate that the transition helps.

## Design proposal

Propose a preview outline around the selected object before movement begins. Offer an explicit focus action, a persistent cancel control, and a return action that restores the previous camera state. Preserve a consistent vertical direction unless the task requires another orientation. Provide an immediate transition option alongside animation. Camera destinations should be derived from object bounds and an adjustable margin, with a clear fallback for objects whose bounds are missing or unreasonable.
