# Separate offshore scene context from operational claims

A new information design exercise for a fictional offshore scene built with external graphics and visualization libraries. Proposed statuses and tasks use synthetic data and are not operational or safety guidance.

> Retrospective study note compiled 2026-10-27. Archive dates are editorial slots; this is an unexecuted design exercise, not a historical activity claim.

## External project context

- [mrdoob/three.js — external upstream reference for a new exercise](https://github.com/mrdoob/three.js)
- [d3/d3 — external upstream reference for a new exercise](https://github.com/d3/d3)

## Question

How can a visually rich offshore scene communicate the difference between environmental context, equipment identity, and a time sensitive status? This exercise uses synthetic information to explore interface hierarchy. It asks whether a viewer can tell what an indicator represents, when it was updated, and whether it is a simulation value. The target is clarity in a demonstration interface, not advice for managing offshore equipment or evidence that a visualization is suitable for operational decisions.

## Design proposal

Propose three independently controlled layers: scene context, named assets, and synthetic status records. Use restrained labels for identity and reserve stronger emphasis for the selected record. Every status should include a source label, a timestamp, and a visible simulation designation. Missing or stale values need their own states rather than borrowing a normal color. Provide an accompanying table so viewers can inspect records without searching through occluded objects in the scene.

## Procedure

Create a small synthetic dataset with normal values, a deliberately stale record, a missing value, and two conflicting records for the same asset. Assign stable identifiers to scene objects and table rows. Walk through tasks that locate an asset, inspect its source, and compare update times. Toggle each information layer and rotate the scene to create occlusion. Verify that selecting a table row identifies the intended asset without altering the underlying records.
