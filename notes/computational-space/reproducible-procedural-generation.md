# Package a procedural result so it can be regenerated

A new reproducibility exercise for procedural spatial studies. It separates deterministic generation checks from judgments about design quality and makes no claim of completed replication.

> Retrospective study note compiled 2026-10-27. Archive dates are editorial slots; this is an unexecuted design exercise, not a historical activity claim.

## External project context

- [processing/p5.js — external upstream reference for a new exercise](https://github.com/processing/p5.js)
- [mrdoob/three.js — external upstream reference for a new exercise](https://github.com/mrdoob/three.js)

## Question

What must accompany a generated spatial form so that another person can recreate it and understand an intentional variation? Saving a screenshot or a random seed alone may omit dependencies, input geometry, and generator settings. This exercise asks how to build a compact generation record that distinguishes a repeated run from a new experiment. It also separates reproducibility of the process from the unrelated question of whether the resulting form is useful or desirable.
