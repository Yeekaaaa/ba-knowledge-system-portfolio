# Source Selection Policy

## Allowed in this public portfolio

| Category | What to include | Format |
|---|---|---|
| Job-market signals | Patterns from public job boards and career guides | Metadata + paraphrased extracts |
| Research papers | Citation, DOI, own-words summary | Metadata file; no PDF unless OA licence |
| Articles / explainers | Publisher, URL, date, paraphrased concepts | Metadata; no full article body |
| Frameworks | BABOK, Agile, DT concepts | Own-words synthesis |
| Synthetic demos | Fictional project notes | Labelled `SYNTHETIC` |

## Not allowed in this public portfolio

- Private project notes (real client, family business, internship internals)
- Resume, work authorisation status, interview notes, personal reflections
- Full job descriptions from SEEK, LinkedIn, Indeed, or company sites
- Publisher PDFs without clear redistribution rights
- Paywalled article full text
- Screenshots with personal or confidential data
- Real company operating metrics

## Job-market sources

**Include:**

- Job title and role family
- Seniority level (junior, graduate, senior, contract)
- Industry sector (generic: healthcare ICT, transport, FinTech)
- Location at city/region level if non-sensitive
- Source platform and URL
- Date accessed
- Paraphrased responsibilities, skills, deliverables
- BA relevance analysis

**Exclude:**

- Employer names when tied to personal application tracking (optional: generic sector only)
- Full "About the role" copy-paste
- Hiring manager names, internal codes, application essays

## Academic sources

**Include:**

- Authors, year, journal, DOI/URL
- Licence if known (e.g. Elsevier — typically no PDF redistribution)
- Short summary in own words
- BA methods and implications

**Exclude:**

- Publisher PDF upload unless open access with explicit licence
- Verbatim abstract beyond fair-use quoting (prefer paraphrase)

## Synthetic sources

All synthetic files must:

1. Use fictional names (e.g. "Northline Retail Group — SYNTHETIC")
2. State `source_type: synthetic` in frontmatter
3. Avoid resemblance to real private projects

## Decision tree

```
New source
  ├─ Contains private personal data? → EXCLUDE from public repo
  ├─ Full copyrighted text? → METADATA + SUMMARY ONLY
  ├─ Open licence / public domain? → May include more, still prefer summary
  └─ Fictional demo? → LABEL SYNTHETIC
```

## Related

- [privacy-copyright-and-sanitisation.md](privacy-copyright-and-sanitisation.md)
- [ingest-workflow.md](ingest-workflow.md)
