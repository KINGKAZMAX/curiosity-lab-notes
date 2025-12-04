# KINGKAZMAX language-learning adaptation plan

Upstream: [yomidevs/yomitan](https://github.com/yomidevs/yomitan)  
Prepared: 2026-10-27  
Status: planned adaptation; original fixtures prepared, runtime integration pending.

## Personal learning context

English and Japanese are being rebuilt from fundamentals. Long-term goals are IELTS 7.5 and JLPT N2, with no exam date set. The first twelve weeks focus on a sustainable foundation; neither target is promised within that period. Personal recordings, scores, and detailed study history belong in the private second brain.

## Why this upstream

A language-focused browser dictionary project suited to Japanese reading and a later Anki field mapping; lower stars than general readers but closer to the stated Japanese goal. Metadata snapshot: 2,902 stars on 2026-10-27. Stars indicate popularity, not a standardized quality rating.

## First small adaptation

Review a proposed dictionary-to-card field contract using six original Japanese examples. Compare the contract with the current official Anki integration documentation before producing real extension settings.

## Acceptance checks

- [ ] Expression, reading, own example, source URL, and source date have distinct fields.
- [ ] Dictionary definitions and audio retain their separate licensing and provenance; none are bundled in this fixture.
- [ ] Repeated captures of the same example have an explicit deduplication key.
- [ ] The JSON contract is labelled a study specification, not importable Yomitan settings.

## Working method

Start by reading the upstream documentation and contribution instructions. Inspect the bundled original fixtures before touching a personal collection. Make one small change, record the upstream revision and environment, then retain the exact command or manual steps and observed result. A written plan or passing file-format check does not establish that the application integration works.

## Second-brain record

Keep a stable record ID, the actual study date, the source URL, the original answer, the correction, and the relevant commit URL in the private Obsidian record. The public fork contains reusable examples and adaptation code only. Mark work as planned, attempted, verified locally, or merged upstream; these states have different meanings.

## Attribution and resources

Retain upstream authorship and license files. GitHub reports `GPL-3.0` for the repository; review the actual license and bundled notices before redistributing any component. Dictionary data, audio, models, and media can have separate licenses.

- [Official documentation](https://yomitan.wiki/anki/)

The examples are newly authored study fixtures. They are not official IELTS/JLPT questions, historical learning records, or evidence that a past experiment occurred.
