# kodo-skills

Public skill repository for KODO markdown workflows.

## Structure

- `codex/` - skills and usage notes for Codex
- `claude-code/` - skills and usage notes for Claude Code
- `shared/` - shared templates and common guidance

## Included skill

- `kodo-log-writer`
  - Generates/updates `KODO/PROJECT.md` and `KODO/YYYYMMDD.md`
  - Enforces required headings: `# title`, `# desc`, `# body`
  - Adds mandatory security note to daily files

## Security

Never include secrets or sensitive data in generated markdown files.
