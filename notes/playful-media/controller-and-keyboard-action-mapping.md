# Controller and Keyboard Action Mapping

A new design exercise for discoverable, reversible input mappings across keyboard and game controller use, with device transitions treated as part of the interface.

> Retrospective study note compiled 2026-10-27. Archive dates are editorial slots; this is an unexecuted design exercise, not a historical activity claim.

## External project context

- [godotengine/godot — external upstream reference for a new exercise](https://github.com/godotengine/godot)
- [mermaid-js/mermaid — external upstream reference for a new exercise](https://github.com/mermaid-js/mermaid)

## Research question

Can a player understand and change the controls without confusing an in game action with the physical button assigned to it? Use a fictional two action toy with move and interact controls. The question concerns switching between keyboard and controller while preserving an understandable mapping. Particular cases include a disconnected device, a conflicting assignment, and a held button during reconnection. This is an interface design exercise and does not assume any specific input API or device implementation in the references.

## Design proposal

Represent actions independently from hardware labels. A controls panel lists each action, its current keyboard assignment, and its controller assignment. Selecting an action enters a clearly marked capture state with cancel and restore defaults options. Warn about conflicting mappings before applying them, and show which action would be displaced. Display the active input route near the play area. When a device disappears, pause the toy and require a fresh neutral input before resuming movement.

## Procedure

Create a local input simulator that emits named actions and device connection events. Use it to test assignment, cancellation, conflict handling, disconnect, and reconnect flows before adding real hardware. Prepare a small matrix of keyboard only, controller only, and mixed input scenarios. Verify that opening the mapping panel cannot trigger a game action accidentally. Save mappings in a visible test profile and reload it. Document expected behavior for held inputs so the reconnect case has a clear acceptance criterion.

## Evaluation plan

Ask future participants to perform an action, remap it, resolve one conflict, and recover from a simulated disconnect. Track incorrect mappings, unintended actions, and time spent searching for the active device label. Test whether users can describe which assignment changed after resolving a conflict. Compare displayed labels with the simulator log to identify interface defects. Include a successful restoration to defaults as part of the task, and avoid claiming support for hardware that has not been tested.
