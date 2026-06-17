# BA Knowledge System — Agent Schema (Public Portfolio)

You are maintaining a **public sample** of an AI-assisted Business Analysis knowledge system.

This vault follows the **LLM Wiki pattern**: raw sources stay immutable, the LLM maintains a persistent markdown wiki, and this schema governs evolution.

> **Disclaimer:** This repository contains educational summaries and portfolio samples, not full proprietary source materials. See [docs/privacy-copyright-and-sanitisation.md](docs/privacy-copyright-and-sanitisation.md).

## Core architecture

| Layer | Folder | Role |
|---|---|---|
| Raw | `sample-raw/` | Immutable metadata, signals, synthetic notes |
| Wiki | `sample-wiki/` | LLM-maintained synthesis |
| Schema | `AGENTS.md`, `CLAUDE.md`, `prompts/`, `templates/` | Rules for every change |

## Wiki folders (sample)

- `01-frameworks/` — BA and transformation frameworks
- `02-methods/` — Requirements, stakeholder, process, change, automation discovery
- `03-deliverables/` — Dashboard spec, KPI dictionary, user stories, UAT plan
- `04-domains/` — Digital transformation BA, AI automation BA
- `06-career/` — Role taxonomy, keywords, sample bullets, interview patterns
- `07-sources/` — Source summaries
- `09-maintenance/` — Lint reports

## Operating principles

- Update existing synthesis pages instead of duplicating concepts.
- If a number is unknown, write `___` — do not invent metrics.
- Separate **fact**, **interpretation**, and **recommendation**.
- Link pages with `[[wiki-links]]`.
- On contradiction, add `Contradictions / updates` — do not silently overwrite.
- Every meaningful ingest updates `sample-wiki/index.md` and `sample-wiki/log.md`.
- **Never** add private personal data, full job ads, publisher PDFs, or paywalled article text.

## Ingest workflow

1. Read raw source in `sample-raw/`.
2. Identify type: job-market-signal, article-metadata, paper-metadata, synthetic.
3. Create/update `sample-wiki/07-sources/*-summary.md`.
4. Update relevant framework, method, deliverable, domain, career pages.
5. Update index and log.
6. Confirm [source-selection-policy](docs/source-selection-policy.md).

## Query workflow

1. Read `sample-wiki/index.md`.
2. Open relevant whole pages.
3. Synthesise; cite wiki links.
4. Propose write-back if reusable.

## Lint workflow

Produce reports in `sample-wiki/09-maintenance/` per [docs/lint-workflow.md](docs/lint-workflow.md).

## Page types

See [docs/knowledge-architecture.md](docs/knowledge-architecture.md) and `templates/`.

## Synthetic content

All fictional examples must include `SYNTHETIC` labelling in raw notes and wiki references.
