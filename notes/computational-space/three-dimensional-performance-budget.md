# Turn a 3D performance budget into a testable contract

A new engineering exercise for balancing rendering cost and useful interaction. The proposed budgets are provisional test targets, not measured results or guarantees for the referenced projects.

> Retrospective study note compiled 2026-10-27. Archive dates are editorial slots; this is an unexecuted design exercise, not a historical activity claim.

## External project context

- [mrdoob/three.js — external upstream reference for a new exercise](https://github.com/mrdoob/three.js)
- [pmndrs/react-three-fiber — external upstream reference for a new exercise](https://github.com/pmndrs/react-three-fiber)

## Question

Which visual costs should be reduced first when a spatial interface becomes difficult to operate on a modest device? This exercise treats performance as part of interaction rather than a final optimization pass. It asks how to maintain responsive selection, readable labels, and predictable camera movement while controlling geometry, texture, and effect costs. The relevant question is not the highest possible frame rate, but whether the essential task remains usable under a clearly documented workload.

## Design proposal

Propose separate budgets for initial loading, steady rendering, and interaction response. Begin with a provisional target of a 33 millisecond frame time during a representative camera route, then revise it against actual measurements and task requirements. Identify essential content and optional effects before reducing quality. Provide explicit quality presets and record which features each preset changes. An automatic adjustment should expose its current setting and avoid changing geometry needed to interpret the task.

## Procedure

Choose one repeatable scene route and a fixed sequence of selection actions. Record the device, browser, viewport, asset versions, and quality preset for every run. Measure a baseline before changing anything. Then vary one cost category at a time: texture resolution, visible object count, shadows, or postprocessing. Include a cold load and a repeated load. Save timing distributions and screenshots so a faster variant can also be checked for lost information.

## Evaluation

Compare median and slow frame times, input response during motion, initial transfer size, and the duration until essential controls become usable. Inspect visual differences at the same camera positions. Reject a performance improvement that removes a necessary label or makes a selectable object ambiguous. Repeat promising changes to distinguish stable gains from a lucky run. Report the tested device conditions alongside the numbers instead of describing one machine's result as universal performance.
