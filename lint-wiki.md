# Prompt: Lint Wiki

Use [AGENTS.md](../AGENTS.md) and [docs/lint-workflow.md](../docs/lint-workflow.md).

Lint the sample wiki in `sample-wiki/`.

## Checks

- Stale job-market claims (dates, salary aggregates)
- Duplicate concepts across pages
- Orphan pages not in `index.md`
- Missing cross-links
- Privacy or copyright violations (full JD text, PDFs, PII)
- Synthetic content not labelled
- Contradictions between source summaries and synthesis pages

## Output

Write a short report to `sample-wiki/09-maintenance/`:

- Findings by severity
- Proposed edits
- Recommended next sources and pages to improve

Append a lint entry to `sample-wiki/log.md`.
