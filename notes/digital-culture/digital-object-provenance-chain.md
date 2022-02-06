# Make the provenance chain visible for each digital object

A new documentation exercise for connecting a digital exhibit to its sources and later transformations. It proposes an auditable record rather than asserting provenance for any particular collection item.

> Retrospective study note compiled 2026-10-27. Archive dates are editorial slots; this is an unexecuted design exercise, not a historical activity claim.

## External project context

- [microsoft/markitdown — external upstream reference for a new exercise](https://github.com/microsoft/markitdown)
- [firecrawl/firecrawl — external upstream reference for a new exercise](https://github.com/firecrawl/firecrawl)

## Question

What should a visitor be able to trace when encountering a digital object whose appearance has changed through scanning, editing, translation, or reconstruction? This exercise asks how to distinguish the physical or documentary source from the digital derivative currently displayed. It focuses on understandable links between records rather than a single authoritative label. The question is whether a reader can see where information came from, what was changed, and which parts remain uncertain.

## Design proposal

Propose a provenance panel containing the source record, capture or acquisition event, transformation history, and current presentation version. Give each stage a stable identifier and identify the responsible role without publishing unnecessary personal information. Keep rights information separate from historical provenance, since knowing a source does not establish permission to reuse it. Display uncertainty at the relevant stage instead of placing one vague disclaimer at the bottom of the page.

## Procedure

Select a small set of materials already appropriate for public reference and create a record for each source. Describe one proposed derivative, such as a resized image or translated label, and connect it to its parent record. Record the transformation method and date. Introduce a deliberately missing source link in a test copy. Follow the chain from exhibit to origin and back, checking that both directions remain understandable without inspecting filenames.
