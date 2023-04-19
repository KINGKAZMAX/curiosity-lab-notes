# Visible Human Override in Robot Controls

A simulation only design exercise for clear command ownership, cancellation, and recovery in a newly designed robot control interface. External simulation and diagramming tools provide context, not validation.

> Retrospective study note compiled 2026-10-27. Archive dates are editorial slots; this is an unexecuted design exercise, not a historical activity claim.

## External project context

- [google-deepmind/mujoco — external upstream reference for a new exercise](https://github.com/google-deepmind/mujoco)
- [mermaid-js/mermaid — external upstream reference for a new exercise](https://github.com/mermaid-js/mermaid)

## Research question

How can a control interface make it obvious whether a person or an automated routine currently has permission to issue commands? Use a simulated robot represented by a marker on a blank canvas. The exercise studies interface comprehension, not physical robot operation. Focus on moments when an automated path is queued, a person requests control, or communication is lost. The central question is whether users can predict which commands remain active and what a cancel action will actually affect.

## Design proposal

Build an explicit state display with manual control, automation requested, automation active, cancellation pending, and disconnected states. Show the current command owner beside a timestamped acknowledgment from the simulator. A visible cancel control requests cancellation, while a separate confirmed status reports when the simulator has stopped applying queued commands. Do not imply that an interface button is a certified emergency stop. Require a fresh manual acknowledgment before resuming automation after a simulated disconnect or ownership change.
