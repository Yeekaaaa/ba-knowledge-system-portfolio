# Sample Lint Report

Date: 2026-06-16  
Scope: `sample-wiki/` public portfolio sample

## Summary

| Severity | Count |
|---|---|
| Critical | 0 |
| High | 0 |
| Medium | 3 |
| Low | 4 |

**Privacy / copyright:** PASS — no full JD text, no publisher PDFs, no PII detected.

## Findings

### Medium

1. **Point-in-time job-market stats** — Salary (~$115K) and role volume may stale. Add review date on [[role-taxonomy]] and [[job-market-signal-business-analyst-summary]].
2. **Synthetic project not in `07-sources/`** — Fictional project referenced across wiki but only exists in `sample-raw/`. Consider optional source summary for traceability.
3. **Agile keyword** — Listed in [[keyword-bank]] secondary list without deep wiki method page. Avoid over-claiming until evidence added.

### Low

1. **No `05-projects/` layer** — Intentional for public repo; document in README (done).
2. **McKinsey concepts paraphrased** — Ensure future edits do not drift into full article paste.
3. **Broken link risk** — Run periodic `[[wiki-link]]` audit against `index.md`.
4. **Second hospitality paper** — Li et al. (2026) service robots paper not yet in sample; optional future public metadata ingest.

## Orphan check

All pages listed in [[index]] — no orphans detected at initial publish.

## Recommended next sources (public-safe)

1. Open Agile / user story guide (Atlassian or similar — paraphrase only)
2. IIBA BABOK study notes (own notes, not copyrighted text)
3. Second paper metadata: service robots and workplace impacts (DOI summary only)

## Recommended wiki improvements

1. Add `stakeholder-matrix` deliverable page
2. Add `traceability-matrix` deliverable page
3. Add optional `07-sources` entry for SYNTHETIC project
4. Add CI script for markdown link checking
5. Publish static site from `sample-wiki/`

## Actions taken

- Initial lint at repository creation — no critical issues.
- Logged in [[log]].
