# Interruptible Voice Turns Without Losing Intent

A prospective voice interaction experiment separating stopping playback, replacing a request, and preserving a draft response in a fictional character conversation.

> Retrospective study note compiled 2026-10-27. Archive dates are editorial slots; this is an unexecuted design exercise, not a historical activity claim.

## External project context

- [huggingface/transformers — external upstream reference for a new exercise](https://github.com/huggingface/transformers)
- [ollama/ollama — external upstream reference for a new exercise](https://github.com/ollama/ollama)

## Research question

When someone interrupts a spoken response, are they asking the system to stop, correct a detail, or begin a different task? This exercise examines how a voice interface can acknowledge interruption while keeping these intentions distinct. Use a fictional character describing an imaginary exhibition. The question is whether people can regain conversational control without repeating their entire request or wondering whether the assistant is still speaking, listening, or preparing another response behind the visible interface.
