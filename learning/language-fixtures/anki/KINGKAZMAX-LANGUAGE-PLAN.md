# KINGKAZMAX language-learning adaptation plan

Upstream: [ankitects/anki](https://github.com/ankitects/anki)  
Prepared: 2026-10-27  
Status: planned adaptation; original fixtures prepared, runtime integration pending.

## Personal learning context

English and Japanese are being rebuilt from fundamentals. Long-term goals are IELTS 7.5 and JLPT N2, with no exam date set. The first twelve weeks focus on a sustainable foundation; neither target is promised within that period. Personal recordings, scores, and detailed study history belong in the private second brain.

## Why this upstream

A mature spaced-repetition program for a small personal English/Japanese card workflow; choose it for repeatable review and editable note structure, not as a promise of exam success. Metadata snapshot: 32,311 stars on 2026-10-27. Stars indicate popularity, not a standardized quality rating.

## First small adaptation

Define a personal note type and inspect a 12-row original bilingual TSV fixture before any import. Map fields, retain stable record IDs, and design a Markdown export for the second brain.

## Acceptance checks

- [ ] All 12 fixture rows have unique record IDs and all required fields.
- [ ] An import trial into a disposable test deck preserves the IDs and handles a repeated import without unintended duplication; this runtime test remains pending.
- [ ] A future Markdown export preserves expression, reading, self-authored example, source, and actual creation date.
- [ ] No private performance history or copyrighted deck is placed in the public fork.

## Working method

Start by reading the upstream documentation and contribution instructions. Inspect the bundled original fixtures before touching a personal collection. Make one small change, record the upstream revision and environment, then retain the exact command or manual steps and observed result. A written plan or passing file-format check does not establish that the application integration works.

## Second-brain record

Keep a stable record ID, the actual study date, the source URL, the original answer, the correction, and the relevant commit URL in the private Obsidian record. The public fork contains reusable examples and adaptation code only. Mark work as planned, attempted, verified locally, or merged upstream; these states have different meanings.

## Attribution and resources

Retain upstream authorship and license files. GitHub reports `NOASSERTION` for the repository; review the actual license and bundled notices before redistributing any component. Dictionary data, audio, models, and media can have separate licenses.

- [Official documentation](https://docs.ankiweb.net/)

The examples are newly authored study fixtures. They are not official IELTS/JLPT questions, historical learning records, or evidence that a past experiment occurred.
