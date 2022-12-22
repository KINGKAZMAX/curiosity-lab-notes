# Evidence Logs for Interaction Experiments

A practical documentation plan for separating observations, proposals, synthetic examples, and retrospective notes in small interaction experiments and future research records.

> Retrospective study note compiled 2026-10-27. Archive dates are editorial slots; this is an unexecuted design exercise, not a historical activity claim.

## External project context

- [n8n-io/n8n — external upstream reference for a new exercise](https://github.com/n8n-io/n8n)
- [mermaid-js/mermaid — external upstream reference for a new exercise](https://github.com/mermaid-js/mermaid)
- [affaan-m/ECC — external upstream reference for a new exercise](https://github.com/affaan-m/ECC)

## Research question

How can a small interaction project keep enough evidence to reconstruct a claim without creating an unmanageable archive? This exercise focuses on a single prototype revision and a fictional walkthrough. The research question concerns traceability: whether another reader can distinguish an observed event, an interpretation, a proposed change, and a synthetic example. It also asks how retrospective documentation should be labeled when the original activity date or supporting artifact is missing, instead of filling those gaps with plausible details.

## Design proposal

Design an evidence entry with a stable identifier, record type, artifact link, capture time, documentation time, author, and verification status. Keep observations separate from interpretations and proposed actions. Allow an unknown activity date and explain why it is unknown. Link a claim to the exact artifact version that supports it, and mark generated examples as synthetic. Provide a supersedes relationship for corrections so readers can follow changes without silently replacing the earlier record or overstating its certainty.

## Procedure

Create a miniature evidence bundle containing one interface screenshot, one scripted event log, one design proposal, and one intentionally incomplete note. Use fictional data and label the bundle as an exercise. Write entries that connect each claim to its supporting material. Change the prototype once, preserve both artifact versions, and update the relevant entry through a correction record. Ask a future reviewer to reconstruct what changed and identify which statements remain unverified using only the bundle.
