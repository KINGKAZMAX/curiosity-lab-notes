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

## Procedure

Build the exercise using original placeholder graphics and links rather than copying third party game files. Define example entries for original work, an adapted interface, a forked project, and an external reference. Verify that each gallery card reaches the relevant provenance record in one clear path. Follow the source link manually and record what was actually checked, leaving uncertain terms unresolved. Test export and offline views to ensure that the provenance records remain attached to the corresponding entries.

## Evaluation plan

Ask future reviewers to identify who created an included item, what the archive author changed, and where the recorded reuse information came from. Count misattributions, broken source links, missing manifest entries, and credits that disappear in a secondary view. Inspect whether unknown information is visible rather than silently replaced with a default license label. Measure the effort needed to update a credit when an item changes. Treat this as a documentation evaluation, not a legal determination about any particular asset.

## Limitations and next steps

A manifest can preserve recorded information but cannot establish authorship or resolve ambiguous permissions by itself. Source pages and repository histories may also change over time. Next, record the date and version of each source check and seek clarification before distributing material with unresolved reuse conditions. Keep upstream software attribution and the source of every later third party asset explicit, while using only original placeholders in this first exercise. The exercise proposes an archive workflow; it does not claim that every asset in the referenced projects has been independently audited.
