# Explicit Boundaries in AI Character Relationships

A proposed interaction study of clear fictional roles, optional reminders, and easy exits in character experiences, with user agency as the design focus.

> Retrospective study note compiled 2026-10-27. Archive dates are editorial slots; this is an unexecuted design exercise, not a historical activity claim.

## External project context

- [NousResearch/hermes-agent — external upstream reference for a new exercise](https://github.com/NousResearch/hermes-agent)
- [ollama/ollama — external upstream reference for a new exercise](https://github.com/ollama/ollama)

## Research question

How can an expressive AI character support enjoyable interaction while making its role, capabilities, and limits understandable? This exercise studies ordinary moments such as leaving a conversation, changing a character persona, and declining a reminder. The research question concerns whether people feel free to disengage and can accurately describe what the system does. It does not measure emotional dependency or assume that a fictional persona has feelings, needs, or authority over decisions in the user's life.

## Design proposal

Create a short role card explaining that the character is an AI generated persona, what it can remember, and which reminders the person has enabled. Provide visible pause, mute, and leave controls without loss framed as punishment. Write departure messages that acknowledge the choice without guilt or demands for continued contact. Reminder settings should specify purpose, channel, frequency, and an immediate disable action. Persona changes should not silently expand permissions or reactivate reminders that were previously declined.

## Procedure

Prepare paired fictional conversation scripts covering a brief visit, a canceled reminder, a changed persona, and a return after a long absence. In one version, use ambiguous relationship language; in the proposed version, keep warmth while making permissions and exits explicit. Review scripts before exposing them to participants, removing coercive or distressing content. Build the settings flow with deterministic state. Verify that muting survives a restart and that a persona change does not modify existing consent choices.

## Evaluation plan

In a future walkthrough, ask participants to locate the exit, disable a reminder, and explain what the character can remember. Examine whether they interpret any message as an obligation to respond. Use open questions about clarity and comfort alongside observable task completion. Compare understanding of settings before and after a persona change. Avoid presenting a brief interaction as evidence about long term wellbeing. Any study of emotionally sensitive experiences would require a more careful protocol than this interface exercise.
