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
