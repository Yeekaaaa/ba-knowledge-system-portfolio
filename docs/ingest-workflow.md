# Ingest Workflow

## When to ingest

Ingest when a new source is **important enough** to influence frameworks, methods, deliverables, domains, or career alignment — not for every bookmark.

## Steps

### 1. Capture raw source

Add a file to `sample-raw/` using the appropriate format:

| Source type | Template / example |
|---|---|
| Job-market signal | [templates/job-market-signal-template.md](../templates/job-market-signal-template.md) |
| Paper metadata | [templates/paper-metadata-template.md](../templates/paper-metadata-template.md) |
| Article metadata | Paraphrased notes + URL |
| Synthetic project | Clearly labelled fictional note |

**Rule:** Raw files are immutable after capture except for missing metadata fields.

### 2. Run ingest prompt

Use [prompts/ingest-source.md](../prompts/ingest-source.md) with the agent schema in [AGENTS.md](../AGENTS.md).

### 3. Create source summary

Write `sample-wiki/07-sources/<source-slug>-summary.md` using [templates/source-summary-template.md](../templates/source-summary-template.md).

Required content:

- Source metadata (type, URL, date accessed)
- Key takeaways (own words)
- BA concepts, methods, deliverables
- Career / portfolio relevance (public-safe)
- Limitations and uncertainty
- Links to updated wiki pages

### 4. Update synthesis pages

Integrate reusable knowledge into existing wiki pages. **Do not** leave insights only in the source summary.

### 5. Update navigation

- Add links to [sample-wiki/index.md](../sample-wiki/index.md)
- Append [sample-wiki/log.md](../sample-wiki/log.md):

```markdown
## [YYYY-MM-DD] ingest | Source Title
- Raw path:
- Source type:
- Pages created:
- Pages updated:
- BA career value:
```

### 6. Report

Return: changed files, open questions, sanitisation checks passed.

## Job-market signal ingest (special rules)

Extract only:

- Title, role family, seniority, location (if non-sensitive)
- Platform, URL, date accessed
- Responsibilities, skills, deliverables (paraphrased)
- BA relevance analysis

**Do not** paste full job ad text.

## Paper / article ingest (special rules)

Include citation metadata, DOI/URL, licence if known, paraphrased summary, BA implications.

**Do not** upload publisher PDF or reproduce abstract verbatim unless licence permits.

## Quality checklist

- [ ] Raw source is metadata-first or synthetic
- [ ] Source summary created in `07-sources/`
- [ ] At least one synthesis page updated
- [ ] `index.md` and `log.md` updated
- [ ] No private personal data introduced
- [ ] Synthetic content labelled
