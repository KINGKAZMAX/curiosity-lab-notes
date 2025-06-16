# Virtual Pet Rhythms Without Pressure

A proposed virtual pet interaction study emphasizing optional routines, visible state changes, and comfortable return after an absence without guilt or punitive mechanics.

> Retrospective study note compiled 2026-10-27. Archive dates are editorial slots; this is an unexecuted design exercise, not a historical activity claim.

## External project context

- [godotengine/godot — external upstream reference for a new exercise](https://github.com/godotengine/godot)
- [processing/p5.js — external upstream reference for a new exercise](https://github.com/processing/p5.js)

## Research question

How can a virtual pet suggest a gentle rhythm while leaving the player free to stop interacting? This exercise examines a fictional companion with play, rest, and observe actions. The question is whether state changes feel understandable without implying that the player has harmed a dependent creature by leaving. Focus on short visits, interrupted sessions, and returns after an absence. The design should support playful attachment while making clear that the pet's displayed states are part of a simulation.

## Design proposal

Use a small state model with active, resting, and ready states. Make transitions visible through a short caption and an optional animation. Let the player choose when to rest the pet and resume later without losing progress. Avoid escalating warnings, negative messages about absence, or automatic reminders. If reminders are added in a later version, require a separate opt in setting. A compact activity log should describe actions neutrally and allow players to clear their local history.

## Procedure

Implement a deterministic companion prototype with placeholder shapes and manually adjustable time. Walk through a brief visit, a browser close, a return the next day, and a longer absence. Check that the interface never invents an obligation to compensate for missed visits. Compare a continuous activity meter with a simpler descriptive state label. Keep the underlying transition rules identical between versions. Record expected state after each scenario and make the simulated time control visible during evaluation sessions.

## Evaluation plan

In a future walkthrough, ask players to predict what will happen if they leave and to explain the meaning of the pet's current state. Track whether anyone searches for a recovery payment, penalty reversal, or urgent care action that the design does not intend. Use open questions about perceived pressure and freedom to stop. Evaluate clarity of the return message separately from aesthetic preference. A short session cannot establish long term wellbeing, attachment quality, or sustained use patterns.

## Limitations and next steps

People bring different expectations to virtual pets, and even neutral state changes can acquire personal meaning. The proposed prototype also removes many economic and social features found in larger games. Next, inspect notification language and persistence rules across repeated sessions, then test whether the chosen rhythm remains understandable without a visible meter. Keep any reminder feature optional and reversible. The source projects inspire a companion context; they do not provide evidence that the proposed pressure reducing design has been implemented.
