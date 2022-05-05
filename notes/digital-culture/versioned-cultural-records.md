# Version cultural records without erasing their revision history

A new archival design exercise for tracking source changes, editorial corrections, and revised interpretations. It specifies a proposed record structure rather than claiming a deployed preservation system.

> Retrospective study note compiled 2026-10-27. Archive dates are editorial slots; this is an unexecuted design exercise, not a historical activity claim.

## External project context

- [microsoft/markitdown — external upstream reference for a new exercise](https://github.com/microsoft/markitdown)
- [n8n-io/n8n — external upstream reference for a new exercise](https://github.com/n8n-io/n8n)

## Question

When a cultural record changes, can a reader tell whether the underlying source changed or only the presentation was corrected? This exercise separates object identity, source versions, metadata revisions, and public display versions. It asks how an archive can correct an error without making the earlier state impossible to understand. The aim is a usable account of change, not the assumption that every old version should remain publicly available under every circumstance.

## Design proposal

Propose a stable object identifier with separate version identifiers for files and descriptive records. Every revision should state what changed, why it changed, the responsible role, and its relationship to a source. Keep mechanical edits distinct from interpretive revisions. The public page can show the current version and a concise correction history, while access to earlier files follows the item's conditions. A withdrawn display should retain an appropriate explanation without exposing restricted material.
