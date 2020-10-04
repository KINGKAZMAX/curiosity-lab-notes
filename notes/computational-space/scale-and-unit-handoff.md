# Make scale and coordinate conventions travel with the model

A new model handoff exercise that uses explicit units, reference geometry, and transformation records. It proposes validation fixtures rather than reporting interoperability results.

> Retrospective study note compiled 2026-10-27. Archive dates are editorial slots; this is an unexecuted design exercise, not a historical activity claim.

## External project context

- [mrdoob/three.js — external upstream reference for a new exercise](https://github.com/mrdoob/three.js)
- [google-deepmind/mujoco — external upstream reference for a new exercise](https://github.com/google-deepmind/mujoco)

## Question

How can a model move between a design tool and an interactive scene without silently changing its physical meaning? This exercise focuses on units, axis directions, origin, and scale rather than visual resemblance. A model can appear convincing while a container is interpreted in meters instead of millimeters or a vertical axis becomes horizontal. The question is whether a recipient can detect and explain such errors before performing measurements or arranging objects around the imported geometry.
