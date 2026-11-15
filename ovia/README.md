# The Ovia Inc layer

This fork of [openclaw/openclaw](https://github.com/openclaw/openclaw) carries a small, self-contained layer that adapts the assistant to OVIA operations work. Everything OVIA adds lives in OVIA-owned locations, so the upstream project stays untouched and future upstream syncs stay clean.

## What the layer contains

- **This document** (`ovia/README.md`) — the map of the layer.
- **Example configuration** (`ovia/config.example.json5`) — an `openclaw.json` example, in the native JSON5 config format, that runs the assistant as an OVIA operations assistant. Placeholders only; no real names, contacts, keys, or secrets.
- **Three starter skills**, in the repository's native skill format (a directory per skill under `skills/`, one `SKILL.md` per skill, `ovia-` prefixed so the ownership is obvious):
  - [`skills/ovia-client-conversations`](../skills/ovia-client-conversations/SKILL.md) — answering and drafting client messages, tone rules, escalation to a human.
  - [`skills/ovia-scheduling-followup`](../skills/ovia-scheduling-followup/SKILL.md) — appointment reminders and no-show prevention sequences in English, French, and Spanish.
  - [`skills/ovia-quote-invoice-chase`](../skills/ovia-quote-invoice-chase/SKILL.md) — the quote and invoice follow-up rhythm, with promise-to-pay handling.

## How the layer stays separate

- **Additive only.** No upstream file is modified, renamed, or deleted by the layer. The single exception is the fork's own `README.md`, which carries a short "Ovia Inc layer" section under the fork's modification-reference note and points here.
- **OVIA-owned paths only.** New material goes under `ovia/` or into `skills/` with an `ovia-` prefix. Upstream would have to add a file at the exact same path before a sync could ever touch the layer.
- **Sync behaviour.** An upstream sync merges upstream commits as usual. Layer files ride along unchanged; after a sync, a quick check that the three `skills/ovia-*` directories and this folder survived is the whole maintenance routine. If upstream ever restructures the skills directory, the layer moves with the same names to the new location.

## Using the layer

1. Copy `ovia/config.example.json5` to `~/.openclaw/openclaw.json` and replace every placeholder with real local values, kept out of git.
2. Keep the three `skills/ovia-*` directories in place; the assistant loads skills from `skills/` by directory name.
3. Adjust the persona wording in the config example to the engagement at hand before first use, and review the escalation rules in `ovia-client-conversations` with the team that receives the hand-offs.

## Licence and credit

The fork and this layer sit under the MIT licence of the upstream project (see `LICENSE` at the repository root). Upstream credit: openclaw/openclaw and its contributors. The layer's own text is documentation and configuration for the fork, written for OVIA operations use.
