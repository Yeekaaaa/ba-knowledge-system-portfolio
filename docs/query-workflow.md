# Query Workflow

## Purpose

Answer BA questions using the wiki as the **primary source**, not one-off chat memory.

## Steps

1. **Read** [sample-wiki/index.md](../sample-wiki/index.md).
2. **Open whole pages** most relevant to the question (framework, method, deliverable, source summary).
3. **Synthesise** an answer:
   - Separate **confirmed facts** (from sources) from **interpretation**.
   - Cite wiki pages with `[[page-name]]` links.
4. **Do not fabricate** experience, metrics, certifications, or employment claims.
5. **Write back** if the answer is reusable:
   - Update an existing wiki page, or
   - Add a short note to a maintenance / outputs area in a private vault.

## Example queries

| Question | Start pages |
|---|---|
| What skills do AU BA employers seek? | [[keyword-bank]], [[job-market-signal-business-analyst-summary]] |
| How should a BA scope digital transformation? | [[digital-transformation-framework]] |
| What deliverables support a dashboard initiative? | [[dashboard-specification]], [[kpi-dictionary]] |
| How do service robots affect employees? | [[public-paper-ai-service-work-summary]], [[change-impact-analysis]] |

## Prompt

Use [prompts/query-wiki.md](../prompts/query-wiki.md).

## Output format (recommended)

```markdown
## Answer
<synthesis>

## Evidence
- [[page]] — <what it contributed>

## Interpretation
<your BA reading>

## Gaps
<what the wiki does not yet cover>
```

## Public repo caution

Query answers in this portfolio must not pull from private vaults or invent personal project metrics.
