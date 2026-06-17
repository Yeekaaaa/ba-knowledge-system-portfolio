# Knowledge Architecture

## LLM Wiki pattern

The LLM Wiki pattern treats the knowledge base as a **compiled layer** on top of immutable sources. LLM chats are ephemeral; the wiki is persistent.

```
┌─────────────────────────────────────────────────────────┐
│  Schema (AGENTS.md / CLAUDE.md / prompts / templates)   │
└──────────────────────────┬──────────────────────────────┘
                           │ governs
┌──────────────────────────▼──────────────────────────────┐
│  Wiki (sample-wiki/)                                     │
│  - frameworks, methods, deliverables, domains, career    │
│  - source summaries (07-sources)                         │
│  - index.md, log.md, maintenance                         │
└──────────────────────────┬──────────────────────────────┘
                           │ ingested from
┌──────────────────────────▼──────────────────────────────┐
│  Raw (sample-raw/)                                       │
│  - job-market signals, paper metadata, article metadata  │
│  - synthetic project notes (clearly labelled)            │
└─────────────────────────────────────────────────────────┘
```

## Wiki taxonomy (sample)

| Folder | Content type | Example |
|---|---|---|
| `01-frameworks/` | Durable BA / transformation concepts | Business analysis overview, digital transformation |
| `02-methods/` | How-to procedures | Requirements analysis, stakeholder analysis |
| `03-deliverables/` | Artefact definitions and checklists | Dashboard spec, UAT plan |
| `04-domains/` | Industry or role context | AI automation BA, digital transformation BA |
| `06-career/` | Job-market alignment | Role taxonomy, keyword bank |
| `07-sources/` | One summary per important raw source | Job signal summary, paper summary |
| `09-maintenance/` | Lint and audit reports | Sample lint report |

> Note: `05-projects/` is omitted from this public sample to avoid mixing synthetic demos with implied real client work. Private vaults may include a projects layer with real evidence.

## Page linking

Use Obsidian-style links: `[[page-name]]`. The index page is the entry point for humans and agents.

## Index and log

- **`index.md`** — curated map of the wiki (updated after ingests).
- **`log.md`** — chronological audit trail: date, source, pages touched, career value.

## Agent responsibilities

When ingesting or querying, agents should:

1. Read the schema first.
2. Read `index.md` before deep synthesis.
3. Update existing pages when concepts already exist.
4. Never copy full copyrighted JD or article text into the public wiki.
5. Record uncertainty instead of inventing metrics.

## Extension points

Private vaults can add:

- `raw/00-inbox/` for Web Clipper landing zone
- `wiki/05-projects/` for portfolio evidence
- `wiki/08-outputs/` for reusable query results
- `raw/assets/` for images (with rights check)
