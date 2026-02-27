---
name: kodo-log-writer
description: Generate or update KODO/PROJECT.md and KODO/YYYYMMDD.md in the required KODO^ format. Use when asked to create daily logs, draft project summaries, or convert chat progress into KODO markdown files while enforcing required headings and a no-sensitive-data note.
---

# KODO Log Writer (OpenClaw)

Generate KODO markdown files in a consistent, publish-safe format.

## Output files

- `KODO/PROJECT.md`
- `KODO/YYYYMMDD.md` (today by default, or requested date)

## Required structure

Both files must keep this structure exactly:

```md
# title
...

# desc
...

# body
...
```

## Security note rule (mandatory)

When generating `YYYYMMDD.md`, append this note at the end of `# body`:

```md
---
Note: Do not include secrets or sensitive data (passwords, API keys, tokens, private keys, personal data, internal-only credentials).
```

If user-provided content contains sensitive values, redact and replace with placeholders such as `[REDACTED]`.

## Workflow

1. Summarize user input into `title`, `desc`, and `body`.
2. Preserve concise, factual progress logs.
3. Write or update the target file.
4. Keep existing sections unless full overwrite is explicitly requested.
5. Ensure the security note exists in `YYYYMMDD.md`.

## Templates

Read `references/templates.md` for copy-ready templates.
