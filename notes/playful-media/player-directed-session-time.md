# Player Directed Session Time

A new game interface exercise supporting optional session awareness, comfortable stopping points, and transparent local timing without pressure to continue or return.

> Retrospective study note compiled 2026-10-27. Archive dates are editorial slots; this is an unexecuted design exercise, not a historical activity claim.

## External project context

- [processing/p5.js — external upstream reference for a new exercise](https://github.com/processing/p5.js)
- [godotengine/godot — external upstream reference for a new exercise](https://github.com/godotengine/godot)

## Research question

How can a game help players manage their own session time without turning a reminder into another demand? Use a fictional short puzzle with clear round boundaries. The research question concerns whether players can understand elapsed active time, set an optional stopping intention, and leave with progress preserved. It does not aim to maximize retention or assume that a longer session is better. Focus on transparency of timing and the player's ability to dismiss, change, or disable the feature.

## Design proposal

Offer an optional session panel showing elapsed active play time and a player chosen reminder. Explain whether paused time is included and keep that rule consistent. At a reminder, provide equally visible continue, save and leave, and change reminder actions. Avoid countdown pressure, lost streak messages, or rewards tied to ignoring a break. Show the next natural stopping point when the game has one. Keep timing data local in the prototype and provide a clear reset control.

## Procedure

Implement the timing model with a controllable test clock. Walk through active play, pause, a hidden window, a completed round, and a restored session. Verify that the displayed duration matches the documented inclusion rule in each case. Test reminder cancellation and disablement before and after a trigger. Use short simulated intervals during the walkthrough so participants do not need to wait. Confirm that saving and leaving preserves the intended state and does not silently schedule an external notification.
