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

## Security rule (mandatory)

Do not append a boilerplate security note inside generated markdown files.

Instead, enforce safety in generation:

- If user-provided content contains sensitive values, redact and replace with placeholders such as `[REDACTED]`.
- Generalize internal-only identifiers and private infrastructure details.
- Prefer safe summaries over raw confidential strings.

## Workflow

1. Summarize user input into `title`, `desc`, and `body`.
2. Preserve concise, factual progress logs.
3. Write or update the target file.
4. Keep existing sections unless full overwrite is explicitly requested.

## Templates

Read `references/templates.md` for copy-ready templates.
