# Lint Workflow

## Purpose

Keep the wiki **accurate, linked, and maintainable** — especially after multiple ingests.

## When to lint

- After a batch ingest (3+ sources)
- Monthly for active vaults
- Before a portfolio or interview push

## Checks

| Check | Question |
|---|---|
| Stale claims | Are job-market stats dated? |
| Duplicates | Same concept on many pages without cross-links? |
| Orphans | Pages not linked from `index.md`? |
| Broken links | `[[wiki-links]]` to missing pages? |
| Missing metrics | Placeholder `___` never filled? |
| Contradictions | New source conflicts with old synthesis? |
| Privacy leak | Private names, employers, or full JD text? |
| Copyright | Full article text or PDFs in repo? |
| Synthetic labelling | Fictional examples clearly marked? |
| Deliverable gaps | Methods without deliverable examples? |

## Steps

1. Run [prompts/lint-wiki.md](../prompts/lint-wiki.md).
2. Produce a short report in `sample-wiki/09-maintenance/`.
3. Propose edits — do not silently overwrite contradictory claims; add `Contradictions / updates` sections.
4. Update `log.md` with a lint entry.

## Example report

See [sample-wiki/09-maintenance/sample-lint-report.md](../sample-wiki/09-maintenance/sample-lint-report.md).

## Severity guide

| Severity | Example | Action |
|---|---|---|
| Critical | Private data in public repo | Remove immediately |
| High | Full copyrighted JD pasted | Replace with signal extract |
| Medium | Orphan page | Link from index |
| Low | Stale salary statistic | Add date qualifier |
