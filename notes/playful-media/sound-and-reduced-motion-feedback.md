# Sound and Reduced Motion Feedback

A prospective audiovisual design exercise preserving essential game information when sound is muted or motion is reduced, with independent player controls.

> Retrospective study note compiled 2026-10-27. Archive dates are editorial slots; this is an unexecuted design exercise, not a historical activity claim.

## External project context

- [processing/p5.js — external upstream reference for a new exercise](https://github.com/processing/p5.js)
- [godotengine/godot — external upstream reference for a new exercise](https://github.com/godotengine/godot)

## Research question

Can players understand an event when its usual sound or animation is unavailable? Use a fictional toy with three events: an accepted action, an invalid action, and a completed pattern. The research question concerns whether each event remains distinguishable with sound muted, motion reduced, or both settings enabled. This exercise treats those settings as ordinary player preferences and access needs. It does not assume that a single substitute cue will be equally useful for everyone or establish a medical benefit.

## Design proposal

Assign each essential event a concise text label and a stable visual state in addition to optional sound and animation. Provide independent controls for volume and motion rather than one setting that changes everything. Reduced motion mode should replace moving transitions with direct state changes and a persistent marker where needed. Keep timing consistent enough that cues remain associated with the triggering action. Display current settings clearly, and allow changes during play without resetting progress or hiding the controls.

## Procedure

Create an event simulator with original tones and geometric graphics. Test all combinations of sound enabled or muted and motion standard or reduced. Trigger events at a slow pace first, then in a short sequence to inspect overlap. Capture screenshots after each event and verify that essential information remains available after transient effects end. Ask a future reviewer to identify events using the alternative cues alone. Record any case where a label disappears before it can be understood.

## Evaluation plan

Measure event identification accuracy and the ability to locate the changed game state under each settings combination. Track settings discoverability, unintended resets, and confusion when multiple cues overlap. Ask players which cues they used rather than inferring their perception from performance alone. Compare cue effectiveness separately from aesthetic preference. Include a text enlargement check because substitute labels can introduce their own barriers. Limit conclusions to the tested prototype and participants instead of declaring a universally accessible audiovisual system.

## Limitations and next steps

The exercise uses a small event vocabulary and cannot represent dense action scenes or every sensory preference. Text labels may become distracting, while persistent markers may clutter the display. Next, test prioritization when several events occur together and examine whether players can adjust cue intensity independently. Preserve a quiet default during testing and let participants stop whenever they choose. The linked projects motivate audiovisual experimentation; they do not provide evidence for the proposed cue mappings or their effectiveness.
