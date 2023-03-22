# Uncertainty in Rehabilitation Prototype Feedback

A nonclinical interface exercise for distinguishing observation quality, simulated signals, and unsupported interpretations in a movement related demonstration.

> Retrospective study note compiled 2026-10-27. Archive dates are editorial slots; this is an unexecuted design exercise, not a historical activity claim.

## External project context

- [d3/d3 — external upstream reference for a new exercise](https://github.com/d3/d3)
- [excalidraw/excalidraw — external upstream reference for a new exercise](https://github.com/excalidraw/excalidraw)

## Research question

How should a movement related prototype communicate that an observation is incomplete without turning uncertainty into a diagnosis? Use prerecorded synthetic landmark sequences and fictional device states. The research question concerns what users understand about the display: whether it is showing a captured observation, a simulated signal, or an unavailable result. The exercise excludes treatment decisions, exercise prescriptions, and claims about recovery. It asks whether the interface supports accurate interpretation of its own limited data quality.

## Design proposal

Separate the screen into observation status, signal provenance, and interface guidance. Display clear states such as visible landmarks, insufficient visibility, and simulation mode. Show the time of the latest usable sample and avoid substituting a reassuring score when data are absent. Guidance should concern operating the demonstration, such as checking camera permission or selecting a sample recording. Keep any simulated sensor channel visibly labeled throughout the interaction, including charts, exports, and error states.

## Procedure

Create a synthetic sequence library covering complete observations, occlusion, missing frames, and frozen input. Label every sequence as simulated and attach its intended interface state. Run each through a local visualization without making clinical classifications. Capture what appears when the input changes abruptly or stops. Test the same sequence in the main view, compact view, and exported report. Check that labels survive those transitions and that no default placeholder appears as a measured value.
