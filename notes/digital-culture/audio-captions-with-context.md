# Make audio meaning available in synchronized text

A new captioning workflow exercise for cultural audio. It proposes timing, attribution, and review checks without claiming that any referenced archive currently contains verified captions.

> Retrospective study note compiled 2026-10-27. Archive dates are editorial slots; this is an unexecuted design exercise, not a historical activity claim.

## External project context

- [huggingface/transformers — external upstream reference for a new exercise](https://github.com/huggingface/transformers)
- [microsoft/markitdown — external upstream reference for a new exercise](https://github.com/microsoft/markitdown)

## Question

What information is lost when an audio element is unavailable, difficult to hear, or presented in an unfamiliar language? This exercise treats captions and transcripts as part of the exhibit record rather than an optional afterthought. It asks how to preserve spoken content, relevant sounds, speaker changes, and meaningful uncertainty. The goal is equivalent access to the intended information, not a claim that text can reproduce every aesthetic or cultural quality of the recording.

## Design proposal

Propose synchronized captions for the playback experience and a separate readable transcript for searching and reference. Identify speakers only when the record supports that identification. Describe relevant non speech sounds concisely, and mark uncertain words instead of silently guessing. Keep translation distinct from transcription. Connect both text versions to the exact audio revision and provide a visible way to report a correction without exposing personal contact details in the public exhibit.

## Procedure

Use an audio sample that is appropriate for the intended review and establish its version identifier. Prepare a first transcription, review unclear segments, and add timestamps after the wording is stable. Check speaker changes and sounds that affect interpretation. Test playback with sound disabled and with the transcript alone. If translation is required, preserve the original language text and record the translator or review role according to the agreed attribution practice.
