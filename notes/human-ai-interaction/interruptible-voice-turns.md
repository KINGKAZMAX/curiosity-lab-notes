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

## Evaluation plan

Measure time from an interruption action to audible playback stopping, then separately measure time to a visible acknowledgment. Ask future participants whether the prior request remains active and what will happen if they press continue. Count unintended resumptions, repeated requests, and corrections applied to the wrong draft. Compare speech interruption with the dedicated stop control. Review transcripts only when participants have explicitly agreed to recording, and keep conversational usability findings separate from claims about speech recognition accuracy.

## Limitations and next steps

Synthetic voices and scripted input cannot capture overlapping speakers, accents, background noise, or the social awkwardness of interrupting a character. The prototype also cannot establish end to end performance for a production service. Next, test the state transitions with assistive input methods and clarify whether interrupted responses are retained or discarded. Any later microphone study should define recording consent and deletion procedures. The linked projects provide a character interaction context, not evidence that these interruption controls already exist.
