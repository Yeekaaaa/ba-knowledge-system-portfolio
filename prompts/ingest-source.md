# Prompt: Ingest Source

Use the agent schema in [AGENTS.md](../AGENTS.md) and [CLAUDE.md](../CLAUDE.md).

Ingest this source:

`sample-raw/<file-name>.md`

## Tasks

1. Confirm source metadata: title, type, URL/DOI, date accessed, synthetic flag.
2. Treat the raw file as immutable.
3. Create or update a source summary in `sample-wiki/07-sources/`.
4. Integrate reusable knowledge into existing wiki pages.
5. Add `[[wiki-links]]` between summaries and synthesis pages.
6. For job-market signals, update `sample-wiki/06-career/role-taxonomy.md` and `keyword-bank.md`.
7. Update `sample-wiki/index.md`.
8. Append `sample-wiki/log.md` with `## [YYYY-MM-DD] ingest | <title>`.
9. Run privacy/copyright checklist from [docs/privacy-copyright-and-sanitisation.md](../docs/privacy-copyright-and-sanitisation.md).

## Hard rules

- No full job ad text. No publisher PDFs. No private personal data.
- Paraphrase articles and papers in own words.
- Label synthetic content.
- Separate fact, interpretation, and recommendation.
- Do not invent employment history or metrics.

## Report

- Changed files
- Open questions
- Sanitisation confirmation
