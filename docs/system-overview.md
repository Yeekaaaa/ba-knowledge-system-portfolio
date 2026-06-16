# System Overview

## Purpose

This portfolio repository demonstrates an **AI-assisted Business Analysis knowledge system** built on the **LLM Wiki pattern**: immutable raw sources, a maintained markdown wiki, and a schema that governs how LLM agents evolve the knowledge base.

## What this repo is

- A **public architecture sample** for BA knowledge management.
- A **documentation and template bundle** for ingest, query, and lint workflows.
- A **sanitised wiki slice** with public-source metadata and synthetic examples.

## What this repo is not

- A dump of private project notes, employer data, or full job advertisements.
- A redistribution of publisher PDFs or paywalled article text.
- A claim of production deployment — it is a portfolio artefact.

## Three layers

| Layer | Folder | Responsibility |
|---|---|---|
| Raw | `sample-raw/` | Capture sources once; do not rewrite after ingest |
| Wiki | `sample-wiki/` | Synthesise frameworks, methods, deliverables, career alignment |
| Schema | `AGENTS.md`, `CLAUDE.md`, `prompts/`, `templates/` | Rules agents follow on every change |

## Primary workflows

1. **Ingest** — raw source → source summary → update wiki pages → log entry.
2. **Query** — index → relevant pages → answer → optional write-back.
3. **Lint** — health check → maintenance report → proposed fixes.

See:

- [knowledge-architecture.md](knowledge-architecture.md)
- [ingest-workflow.md](ingest-workflow.md)
- [query-workflow.md](query-workflow.md)
- [lint-workflow.md](lint-workflow.md)

## Design principles

- **Separate fact, interpretation, and recommendation.**
- **Prefer updating existing synthesis** over creating duplicate pages.
- **Mark synthetic content explicitly.**
- **Metadata-first** for job ads and academic papers.
- **Maintain index and log** on every meaningful ingest.

## Related pages

- [source-selection-policy.md](source-selection-policy.md)
- [privacy-copyright-and-sanitisation.md](privacy-copyright-and-sanitisation.md)
- [../sample-wiki/index.md](../sample-wiki/index.md)
