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

## Procedure

Implement the state machine entirely in a local simulator with no network connection to hardware. Prepare scenarios involving a delayed acknowledgment, duplicate command, lost connection, and rejected ownership request. Execute each scenario while recording state transitions and rendered labels. Try keyboard and pointer cancellation paths. Reload the interface while a request is pending to test whether stale UI state is mistakenly restored as active authority. Maintain an expected outcome table for every injected fault before conducting a walkthrough.

## Evaluation plan

In future task sessions, ask users to identify the command owner and predict the next movement before allowing the simulation to proceed. Measure incorrect ownership judgments, duplicate commands, cancellation requests without acknowledgment, and time to recognize a disconnect. Inspect event logs to distinguish interface latency from simulated controller delay. Count a successful cancellation only when the simulator confirms the intended state transition. Qualitative feedback can reveal confusing terminology, but it cannot establish physical safety or readiness for real deployment.
