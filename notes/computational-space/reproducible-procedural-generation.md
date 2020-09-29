# Package a procedural result so it can be regenerated

A new reproducibility exercise for procedural spatial studies. It separates deterministic generation checks from judgments about design quality and makes no claim of completed replication.

> Retrospective study note compiled 2026-10-27. Archive dates are editorial slots; this is an unexecuted design exercise, not a historical activity claim.

## External project context

- [processing/p5.js — external upstream reference for a new exercise](https://github.com/processing/p5.js)
- [mrdoob/three.js — external upstream reference for a new exercise](https://github.com/mrdoob/three.js)

## Question

What must accompany a generated spatial form so that another person can recreate it and understand an intentional variation? Saving a screenshot or a random seed alone may omit dependencies, input geometry, and generator settings. This exercise asks how to build a compact generation record that distinguishes a repeated run from a new experiment. It also separates reproducibility of the process from the unrelated question of whether the resulting form is useful or desirable.

## Design proposal

Propose a run manifest containing the generator revision, input identifiers and hashes, units, parameter values, random seed, dependency versions, and output filenames. Give every run a stable identifier and keep its manifest beside the geometry and preview. Record any manual edits as subsequent steps with their own files. Define whether reproducibility means identical bytes, equivalent geometry within a tolerance, or matching derived measurements, because these are different promises.

## Procedure

Start with a generator using a small parameter set and one explicit source of randomness. Run it twice with the same manifest in a clean working directory, then vary exactly one parameter for a third run. Compare geometry and derived measurements using the declared equivalence rule. Repeat after restarting the host application. Deliberately remove an input and change a dependency version to inspect whether the workflow reports an actionable failure instead of producing an unexplained difference.

## Evaluation

Evaluate whether another person can identify every required input and execute the documented process without relying on the original author's memory. Report exact matches, tolerance based matches, and unexplained differences separately. Check that the intentionally changed parameter produces a traceable new run identifier and manifest difference. Review error messages for missing inputs. Successful regeneration is evidence about the recorded process only; it should not be presented as validation of the design's environmental or social effects.

## Limitations and next steps

Floating point operations, geometry kernels, dependency updates, and platform differences can prevent byte identical output even when the underlying method is stable. Seeds also fail to control randomness introduced outside the generator. The next step is to locate those sources explicitly and define tolerances for the measurements that matter. Preserve earlier manifests instead of overwriting them, and document any conversion needed to reopen an archived model in a newer application version.
