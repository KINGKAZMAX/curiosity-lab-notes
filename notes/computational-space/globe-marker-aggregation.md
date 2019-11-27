# Keep globe clusters geographically honest

A new marker aggregation exercise using synthetic location fixtures and external visualization libraries. It specifies inspection criteria without asserting an existing clustering implementation.

> Retrospective study note compiled 2026-10-27. Archive dates are editorial slots; this is an unexecuted design exercise, not a historical activity claim.

## External project context

- [d3/d3 — external upstream reference for a new exercise](https://github.com/d3/d3)
- [mrdoob/three.js — external upstream reference for a new exercise](https://github.com/mrdoob/three.js)

## Question

How should a globe summarize many locations without implying that a cluster is a real place? Dense markers can overlap, while a single large symbol may conceal the distribution it represents. This exercise asks whether viewers can discover individual locations, understand cluster counts, and recognize geographic spread across zoom levels. Special attention goes to points near the date line and the poles, where a convenient screen based grouping can produce misleading geographic relationships.
