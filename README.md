# kodo-skills

Public skill repository for KODO markdown workflows.

## What is KODO^?

KODO^ is a build-in-public workflow that turns repository activity into readable progress narratives.
By keeping a `KODO/` directory in your repo (for example `PROJECT.md` and `YYYYMMDD.md`), you can publish progress while keeping implementation details private.

- Website: https://kodo.pw/

## Why this repository exists

This repository provides reusable skills that help agents generate KODO markdown files in a consistent format.

## Structure

- `codex/` - skills and usage notes for Codex
- `claude-code/` - skills and usage notes for Claude Code
- `openclaw/` - skills and usage notes for OpenClaw
- `shared/` - shared templates and common guidance

## Included skill

- `kodo-log-writer`
  - Generates or updates `KODO/PROJECT.md` and `KODO/YYYYMMDD.md`
  - Enforces required headings: `# title`, `# desc`, `# body`
  - Uses narrative-style daily logs (what changed, why, outcome, next)
  - Enforces sensitive-data safety via redaction/generalization rules

## Security

Never include secrets or sensitive data in generated markdown files.

## Output samples

- `shared/samples/PROJECT.sample.md`
- `shared/samples/YYYYMMDD.sample.md`

These are copy-ready examples for registering content into KODO.
