# kodo-skills

Public skill repository for KODO markdown workflows.

## Structure

- `codex/` - skills and usage notes for Codex
- `claude-code/` - skills and usage notes for Claude Code
- `openclaw/` - skills and usage notes for OpenClaw
- `shared/` - shared templates and common guidance

## Included skill

- `kodo-log-writer`
  - Generates or updates `KODO/PROJECT.md` and `KODO/YYYYMMDD.md`
  - Enforces required headings: `# title`, `# desc`, `# body`
  - Adds a mandatory security note to daily files

## Security

Never include secrets or sensitive data in generated markdown files.
