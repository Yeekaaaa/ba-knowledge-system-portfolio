# UAT Plan

## Definition

A structured plan for **User Acceptance Testing** — validating that a solution meets business requirements before release.

## When to use

Before production release of reporting workflows, dashboards, or system changes.

## Minimum viable structure

- Scope and objectives
- In-scope / out-of-scope features
- Roles (testers, BA, product owner, sign-off approver)
- Entry / exit criteria
- Test environment and data rules
- Test scenarios mapped to requirements / user stories
- Defect severity definitions
- Sign-off process
- Schedule

## Quality checklist

- Scenarios trace to acceptance criteria — [[user-stories]]
- Includes negative and edge cases (validation failures, empty data)
- Sign-off owners named
- Entry criteria include stable build and test data

## Example scenarios (SYNTHETIC)

| ID | Scenario | Expected result |
|---|---|---|
| UAT-01 | Import file with missing mandatory field | Rejected with clear message |
| UAT-02 | Valid file for Store A, Month M | Dashboard totals match import |
| UAT-03 | Budget line missing for one store | Variance shows data gap flag |

Fictional context: `sample-raw/synthetic-project-note.md`.

## Portfolio relevance

UAT is among top employer-sought skills in AU BA market signals — [[keyword-bank]].

## Related pages

- [[user-stories]]
- [[dashboard-specification]]
- [[requirements-analysis]]

## Sources / Evidence

- [[job-market-signal-business-analyst-summary]]
