# Explaining Card Sampling Without Mystique

A prospective card toy exercise showing how deck composition and replacement rules shape draws, using original geometric cards and transparent arithmetic.

> Retrospective study note compiled 2026-10-27. Archive dates are editorial slots; this is an unexecuted design exercise, not a historical activity claim.

## External project context

- [processing/p5.js — external upstream reference for a new exercise](https://github.com/processing/p5.js)
- [d3/d3 — external upstream reference for a new exercise](https://github.com/d3/d3)

## Research question

Can a card toy help players understand why the chance of a particular draw changes without implying that a random system owes them a favorable outcome? Use an original twelve card deck containing five red, four blue, and three gold cards. The question concerns the difference between drawing with replacement and drawing without replacement. Ask whether players can relate the next draw to the remaining deck rather than to a vague feeling that one color is due.

## Design proposal

Show the remaining deck counts beside a plainly labeled draw rule. In the version without replacement, reduce the displayed count when a card is drawn; in the replacement version, return it before the next draw. Explain the next red draw as five of twelve initially and four of eleven after a red card is removed. Provide an inspectable draw history and a reset action. Keep visual celebration consistent across colors so presentation does not imply that a rarer card has greater worth.

## Procedure

Create geometric card art and a deterministic set of sample sequences for interface testing. Mark those sequences as scripted rather than random. Verify displayed counts after every draw, reset, and rule change. Then add a separately labeled random mode and check that its interface follows the same accounting rules. Prepare prediction questions before and after a red card is removed. Do not mix the two modes silently, and preserve the selected rule in any exported explanation or screenshot.

## Evaluation plan

Ask future participants to calculate or describe the next red draw in both modes, then explain why the answers differ after a removal. Score comprehension of the rule separately from arithmetic fluency. Check whether players interpret a long run of one color as a guarantee about the next draw. Inspect count consistency as a software property rather than relying on participant judgment. Treat any perceived fairness ratings as subjective observations, not proof of the random generator's statistical or security properties.

## Limitations and next steps

A twelve card toy simplifies larger games with hidden information, strategic actions, and changing deck composition. Scripted sequences cannot validate randomness, and a transparent display does not prevent every mistaken intuition about chance. Next, add an explanation for switching modes partway through a session and decide whether that action resets the deck. Use original assets throughout the exercise. The linked projects supply a playful presentation context, not evidence that this sampling model or educational effect already exists.
