# Interruptible Voice Turns Without Losing Intent

A prospective voice interaction experiment separating stopping playback, replacing a request, and preserving a draft response in a fictional character conversation.

> Retrospective study note compiled 2026-10-27. Archive dates are editorial slots; this is an unexecuted design exercise, not a historical activity claim.

## External project context

- [huggingface/transformers — external upstream reference for a new exercise](https://github.com/huggingface/transformers)
- [ollama/ollama — external upstream reference for a new exercise](https://github.com/ollama/ollama)

## Research question

When someone interrupts a spoken response, are they asking the system to stop, correct a detail, or begin a different task? This exercise examines how a voice interface can acknowledge interruption while keeping these intentions distinct. Use a fictional character describing an imaginary exhibition. The question is whether people can regain conversational control without repeating their entire request or wondering whether the assistant is still speaking, listening, or preparing another response behind the visible interface.

## Design proposal

Represent listening, preparing, speaking, and interrupted states with text labels as well as visual indicators. Offer a persistent stop playback control that works independently from speech recognition. After interruption, retain the previous request as a visible draft and let the person choose to correct it or start again. Show when audio capture is active and provide a text input alternative. Do not automatically interpret every sound as an instruction, or treat silence as permission to resume a canceled response.

## Procedure

Build a local playback prototype with prerecorded synthetic speech and scripted transcript inputs. Test interruptions near the beginning, middle, and end of a response. Inject acknowledgment delays of different lengths and label them as experimental conditions rather than measured service performance. Include a correction, a complete topic change, and a noninstruction sound. Verify that stop playback works without microphone permission. Store event timestamps and selected actions; avoid collecting real microphone recordings by default during the initial exercise.
