# Calibrating Trust When Evidence Is Incomplete

A proposed interface study of appropriate reliance on AI suggestions using fictional planning tasks and deliberately varied evidence quality. References motivate the topic only.

> Retrospective study note compiled 2026-10-27. Archive dates are editorial slots; this is an unexecuted design exercise, not a historical activity claim.

## External project context

- [huggingface/transformers — external upstream reference for a new exercise](https://github.com/huggingface/transformers)
- [excalidraw/excalidraw — external upstream reference for a new exercise](https://github.com/excalidraw/excalidraw)

## Research question

Can an interface help people distinguish a useful suggestion from a suggestion that lacks enough evidence? Use a fictional exhibition planning task rather than a consequential real decision. Some recommendations have complete source cards, while others depend on missing room dimensions or outdated schedules. The research question concerns appropriate reliance: accepting supported suggestions, checking uncertain ones, and declining unsuitable ones. It does not ask whether participants simply report liking the assistant or believing that it sounds confident.

## Design proposal

Design a recommendation card that separates the suggestion, supporting observations, assumptions, and unresolved inputs. Avoid an invented numerical confidence score. Instead, show concrete statements such as a missing dimension or a source date that needs checking. Place a verify action beside each unresolved input and a revise action beside the proposed plan. Keep the visual weight of the recommendation consistent across evidence conditions, so stronger typography does not accidentally become a substitute for stronger support.

## Procedure

Prepare twelve fictional planning cases with an answer key describing which inputs are sufficient. Build two interface variants: a concise recommendation alone and the same recommendation with structured evidence. Keep wording, task complexity, and available actions consistent. Counterbalance case order in a future study, and provide a practice case first. Log which source cards are opened and whether the final plan incorporates an unsupported assumption. Do not introduce real venue information or represent fabricated sources as authentic records.

## Evaluation plan

Evaluate supported acceptance, unsupported acceptance, appropriate checking, and unnecessary checking separately. Report completion time alongside these outcomes because slowing every decision is not automatically an improvement. Ask participants to explain one accepted and one rejected recommendation in their own words. Compare those explanations with the case evidence rather than judging their attitude toward AI. A later analysis should disclose sample size and task order, and should treat exploratory differences as hypotheses until an adequately planned study is conducted.

## Limitations and next steps

The controlled cases simplify how people evaluate expertise, deadlines, and conflicting sources in everyday work. Evidence cards may also invite superficial scanning instead of thoughtful verification. Next, test whether participants can notice a contradiction between two sources and whether the interface clearly communicates that the conflict remains unresolved. The linked repositories inspire questions about interaction and evidence; they do not establish that this particular calibration interface exists or has already improved decision quality.
