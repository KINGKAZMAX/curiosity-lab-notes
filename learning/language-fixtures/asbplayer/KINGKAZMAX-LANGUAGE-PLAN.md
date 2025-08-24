# KINGKAZMAX language-learning adaptation plan

Upstream: [asbplayer/asbplayer](https://github.com/asbplayer/asbplayer)  
Prepared: 2026-10-27  
Status: planned adaptation; original fixtures prepared, runtime integration pending.

## Personal learning context

English and Japanese are being rebuilt from fundamentals. Long-term goals are IELTS 7.5 and JLPT N2, with no exam date set. The first twelve weeks focus on a sustainable foundation; neither target is promised within that period. Personal recordings, scores, and detailed study history belong in the private second brain.

## Why this upstream

A focused subtitle and sentence-mining project for small listening exercises; the current canonical repository is asbplayer/asbplayer, redirected from killergerbah/asbplayer. Metadata snapshot: 1,494 stars on 2026-10-27. Stars indicate popularity, not a standardized quality rating.

## First small adaptation

Use a four-cue original SRT and a provenance manifest to design a short listening-to-card workflow. Record a matching original audio/video clip later; no media has been produced or imported by this task.

## Acceptance checks

- [ ] SRT cue numbers are sequential and times are monotonic and non-overlapping.
- [ ] The manifest explicitly states that this is a text-only fixture with no recorded media yet.
- [ ] Every future card can be traced to a clip ID, cue, source rights, and actual learning date.
- [ ] A real playback/import test is documented only after it is executed.

## Working method

Start by reading the upstream documentation and contribution instructions. Inspect the bundled original fixtures before touching a personal collection. Make one small change, record the upstream revision and environment, then retain the exact command or manual steps and observed result. A written plan or passing file-format check does not establish that the application integration works.

## Second-brain record

Keep a stable record ID, the actual study date, the source URL, the original answer, the correction, and the relevant commit URL in the private Obsidian record. The public fork contains reusable examples and adaptation code only. Mark work as planned, attempted, verified locally, or merged upstream; these states have different meanings.

## Attribution and resources

Retain upstream authorship and license files. GitHub reports `AGPL-3.0` for the repository; review the actual license and bundled notices before redistributing any component. Dictionary data, audio, models, and media can have separate licenses.

- [Official documentation](https://docs.asbplayer.dev/)

The examples are newly authored study fixtures. They are not official IELTS/JLPT questions, historical learning records, or evidence that a past experiment occurred.
