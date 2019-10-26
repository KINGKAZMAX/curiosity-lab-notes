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

## Procedure

Prepare objects at three sizes, including one partially hidden object and one near a scene boundary. Define the same focus and return tasks for each. Test direct movement, a brief animated transition, and an immediate change of view using identical destinations. During each transition, attempt cancellation and manual navigation. Record the camera state before and after every action. Repeat with a narrow viewport and the reduced motion preference enabled.

## Evaluation

Check whether the selected object remains identifiable, whether the camera avoids clipping through geometry, and whether cancel and return behave consistently. In a planned usability session, ask the viewer to describe where the detail sits in the larger scene after focusing it. Record unexpected motion and repeated recovery actions. Assess motion discomfort through optional participant feedback rather than assuming a short animation is comfortable. Treat task understanding and control as separate evaluation dimensions.

## Limitations and next steps

Object bounds alone do not determine a meaningful viewpoint, especially for thin surfaces, interiors, or articulated objects. Automated framing may also hide the context a reviewer needs. The proposed camera behavior is a new prototype requirement, not a feature attributed to the linked engines. Next, add authored viewpoints for difficult cases and document when automatic focus should be disabled. Further evaluation should include people who prefer immediate changes and people who rely primarily on keyboard navigation.
