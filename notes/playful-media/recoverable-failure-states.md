# Recoverable Failure States in Small Games

A prospective prototype exercise distinguishing intended game failure from technical interruption, with clear checkpoints, reversible recovery, and honest save status.

> Retrospective study note compiled 2026-10-27. Archive dates are editorial slots; this is an unexecuted design exercise, not a historical activity claim.

## External project context

- [godotengine/godot — external upstream reference for a new exercise](https://github.com/godotengine/godot)
- [affaan-m/ECC — external upstream reference for a new exercise](https://github.com/affaan-m/ECC)

## Research question

When a game stops unexpectedly, can the player understand what happened and recover without confusing a technical problem with an intended challenge? Use a fictional maze with a short sequence of rooms and explicit checkpoints. The research question concerns distinguishing a lost round, a canceled session, and unavailable saved data. It also asks whether recovery messages accurately describe what will be restored. The exercise studies comprehension and state continuity rather than claiming that failure should always be removed from play.

## Design proposal

Display separate messages for game outcomes and technical interruptions. A lost round can offer retry from the last checkpoint, while a loading problem should explain that progress has not yet been read. Show the checkpoint name and its recorded time before a recovery action. Preserve the current session until a replacement has been confirmed. Offer a fresh start as a separate choice, and avoid using a generic retry button for operations that have different effects on saved progress.

## Procedure

Create a deterministic maze state and three synthetic checkpoint files: valid, outdated, and deliberately incomplete. Simulate a lost round, interrupted save, failed load, and browser restart. Record the expected restored position and collected items for each case. Verify that repeated recovery clicks do not advance or duplicate state. Test cancellation while a recovery confirmation is open. Keep faulty files in a labeled test fixture and capture the actual message displayed alongside the state that the prototype restores.
