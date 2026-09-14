# Anatomy & Physiology — Semester 1 Image Repository

Standalone image repo for the HS Anatomy & Physiology (Florida 2000350) Semester 1 revision pass. Created so images can be referenced from Canvas lesson/reading pages the same way the Optima owl logo already is — via a raw GitHub URL — instead of living only as local files nobody can embed.

## Status

**Live at `https://github.com/optimaondemand/hsanatomy-physiology-images`, branch `main`.** Raw file URLs resolve at:

```
https://raw.githubusercontent.com/optimaondemand/hsanatomy-physiology-images/main/<module-folder>/<filename>
```

e.g. `https://raw.githubusercontent.com/optimaondemand/hsanatomy-physiology-images/main/module-03-skeletal/3.01-01-bone-biology-tissue-shapes-markings-bone.jpg` — confirmed resolving 2026-09-14. This is the base URL to use in `<img src="...">` tags going forward, the same pattern the Optima owl logo uses from `optima-assets`.

## Contents

- **327 images** total, organized into one folder per module (`module-0X-*/`, matching the folder names under `semester-1/`).
- **38 are flagged** for manual review before use (19 `LOW-RES` — tiny placeholder graphics that need to be re-sourced from the URL in their caption, not used directly; 21 `NO CAPTION TEXT FOUND` — placement could not be automatically correlated with reading text and needs to be verified against the original docx before use). Flag status is recorded per-image in each module's `INDEX.md` — flagged files are **not** separated into a different folder, so check the index before using any file.

## Naming convention

`<lesson>-<sequence>-<slug>.<ext>`

- `<lesson>` is the **current, post-renumbering** lesson number (e.g. `3.02`), matching what `semester-1/module-03-skeletal/week-01/reading-2.html` etc. actually use today — not the old numbering used in the original source docx. Translating old→new numbering (including Module 2's and Module 4's lesson-level restructuring, not just the module-number shift) was done automatically from each module's own revision history in `plan.md`; a small number of images were reassigned by keyword (e.g. sarcomere-related Module 4 images moved from old 3.02 to new 4.03, matching the actual content move documented in `plan.md`).
- `<sequence>` is a two-digit counter, starting at `01`, for images within that same lesson.
- `<slug>` is a short, auto-generated description from the original caption — good enough to eyeball in a directory listing, not guaranteed to be polished prose. **The full original caption is always in that module's `INDEX.md`** — treat the slug as a finding aid, the index as the source of truth.

## Per-module indexes

- [`module-01-intro/INDEX.md`](module-01-intro/INDEX.md) — Module 1, Introduction to Anatomy & Physiology (32 images)
- [`module-02-tissues-integument/INDEX.md`](module-02-tissues-integument/INDEX.md) — Module 2, Tissues & the Integumentary System (28 images)
- [`module-03-skeletal/INDEX.md`](module-03-skeletal/INDEX.md) — Module 3, Skeletal System (69 images)
- [`module-04-muscular/INDEX.md`](module-04-muscular/INDEX.md) — Module 4, Muscular System (54 images)
- [`module-05-nervous/INDEX.md`](module-05-nervous/INDEX.md) — Module 5, Nervous System (63 images)
- [`module-06-endocrine/INDEX.md`](module-06-endocrine/INDEX.md) — Module 6, Endocrine System (16 images)
- [`module-07-cardiovascular/INDEX.md`](module-07-cardiovascular/INDEX.md) — Module 7, Cardiovascular System (65 images)

## Known placement uncertainty

- **Module 2** (`module-02-tissues-integument`): this module's lessons were restructured (old Lesson 1.05 removed except its Cancer section, which now opens Reading 1.08; old 1.06→1.05; old 1.07→1.06; old 1.08 split into 1.07 Day 1 / 1.08 Day 2). Most images were reassigned automatically by keyword matching (epidermis/dermis/hypodermis → Day 1 / 1.07; accessory structures/burns/cancer → Day 2 / 1.08), and 3 images were hand-corrected against the actual recommendations docx text where the automatic correlation picked the wrong lesson. Spot-check against `INDEX.md` captions before use, especially for anything near the Day 1/Day 2 boundary.
- **Module 4** (`module-04-muscular`): this module had the most restructuring of the whole semester (sarcomere content moved lessons, Back+Thorax merged, Upper/Lower Limb shifted weeks, a new Lesson 4.12 was created). Old→new lesson mapping used an explicit table built from this module's `plan.md` history, plus keyword detection for sarcomere-related and Duchenne-muscular-dystrophy-related images (which moved lessons independently of the general restructure). This is the module most worth double-checking against `INDEX.md` before trusting a placement.
- All other modules (1, 3, 5, 6, 7) had no lesson-level restructuring, so old→new lesson mapping was a straightforward module-number swap and should be reliable.

## Source

Extracted from the `Suggested Images/*.docx` files (see the main course directory's `CLAUDE.md`). Original extraction + manifests live in `../images/module-0X-*/manifest.md` — this repo is a reorganized, renamed, current-numbering copy of those same files, built for embedding rather than reference.

