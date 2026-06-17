# Dashboard Specification

## Definition

A dashboard specification defines what a dashboard should show, why each metric matters, how it is calculated, where data comes from, and how users should act on the information.

## When to use

When translating business reporting needs into a buildable BI or operational dashboard requirement.

## Minimum viable structure

- Business objective and decision questions
- Users / stakeholders
- KPI list with owners
- Metric definitions (link to [[kpi-dictionary]])
- Data sources and grain
- Filters and dimensions
- Visual layout (wireframe or description)
- Refresh frequency
- Data quality rules
- Acceptance criteria
- Open questions

## Quality checklist

- Every KPI has a definition and owner
- Every visual answers a decision question
- Calculation rules are testable
- Users know what action to take on red/amber/green states
- Acceptance criteria cover totals, filters, and edge cases

## Example (SYNTHETIC)

Fictional Northline Retail Group regional dashboard: store comparison for revenue, cost, margin, budget variance; monthly grain; drill-down by store. See `sample-raw/synthetic-project-note.md` in `sample-raw/`.

## Portfolio relevance

Demonstrates connecting business questions → metrics → layout → tests — a core BA artefact for reporting and transformation roles.

## Related pages

- [[kpi-dictionary]]
- [[requirements-analysis]]
- [[uat-plan]]

## Sources / Evidence

- [[job-market-signal-business-analyst-summary]] — reporting and data presentation
- `sample-raw/synthetic-project-note.md` (SYNTHETIC)
