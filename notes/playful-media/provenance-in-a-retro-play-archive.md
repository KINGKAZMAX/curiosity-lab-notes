# Provenance in a Retro Play Archive

A practical design plan for keeping creators, upstream projects, asset origins, and recorded reuse terms visible throughout a retro inspired game archive.

> Retrospective study note compiled 2026-10-27. Archive dates are editorial slots; this is an unexecuted design exercise, not a historical activity claim.

## External project context

- [GraphiteEditor/Graphite — external upstream reference for a new exercise](https://github.com/GraphiteEditor/Graphite)
- [godotengine/godot — external upstream reference for a new exercise](https://github.com/godotengine/godot)

## Research question

How can a playful archive help visitors distinguish original interface work from included games, adapted code, and referenced assets? This exercise uses placeholder entries for a fictional retro collection. The research question concerns whether provenance remains easy to find before launching an item and after entering the play view. It also asks how to represent missing information honestly. A polished presentation should not make a third party contribution appear to have been created by the person assembling the archive.

## Design proposal

Create a provenance card for each item with its title, credited creator, source link, relationship to the archive, and recorded reuse terms. Keep unknown fields explicitly marked as unknown. Separate credits for the surrounding interface from credits for embedded content. Include a persistent credits link in the play view and a compact source label in gallery cards. Use an asset manifest to connect files to their provenance entries, and keep original notices with material whenever they are available.
