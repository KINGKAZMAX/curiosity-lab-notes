# Keep globe clusters geographically honest

A new marker aggregation exercise using synthetic location fixtures and external visualization libraries. It specifies inspection criteria without asserting an existing clustering implementation.

> Retrospective study note compiled 2026-10-27. Archive dates are editorial slots; this is an unexecuted design exercise, not a historical activity claim.

## External project context

- [d3/d3 — external upstream reference for a new exercise](https://github.com/d3/d3)
- [mrdoob/three.js — external upstream reference for a new exercise](https://github.com/mrdoob/three.js)

## Question

How should a globe summarize many locations without implying that a cluster is a real place? Dense markers can overlap, while a single large symbol may conceal the distribution it represents. This exercise asks whether viewers can discover individual locations, understand cluster counts, and recognize geographic spread across zoom levels. Special attention goes to points near the date line and the poles, where a convenient screen based grouping can produce misleading geographic relationships.

## Design proposal

Propose clusters that always reveal their membership count and open a list of constituent locations. Make the displayed cluster position a navigation convenience rather than a claimed geographic centroid. When selected, show the member extent and offer a controlled zoom to that extent. Preserve stable location identifiers through every regrouping. Define a visible transition rule so markers do not repeatedly merge and separate when the camera makes small movements near a threshold.

## Procedure

Create synthetic datasets containing isolated points, dense city groups, duplicate coordinates, points straddling the date line, and polar locations. Give each point a stable identifier and an ordinary display name. Inspect the aggregation at a fixed set of camera distances and after small rotations. Select several clusters and confirm that their membership list is complete. Repeat with a narrow viewport, then test whether returning to a previous view restores the same grouping.
