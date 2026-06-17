# User Stories

## Definition

Short statements of functionality from a user perspective, paired with **acceptance criteria** that make requirements testable.

## When to use

Agile and hybrid delivery; translating business requirements into incremental development and test work.

## Minimum viable structure

```
As a <role>
I want <capability>
So that <business outcome>

Acceptance criteria:
- Given ... When ... Then ...
```

## Quality checklist

- Tied to a business outcome, not only UI preference
- Acceptance criteria are testable and unambiguous
- Data rules and exceptions included where relevant
- Traceable to requirement ID or process step

## Example (SYNTHETIC)

**Story:** As a store manager, I want the monthly import template to flag missing mandatory fields before submission, so that regional reports are not delayed by rework.

**Acceptance criteria:**
- Given a row with blank mandatory field X, when the user attempts submit, then block submission and show field-level message.
- Given all mandatory fields complete, when totals are calculated, then margin matches dictionary formula in [[kpi-dictionary]].

Context: fictional `sample-raw/synthetic-project-note.md`.

## Portfolio relevance

Addresses top job-market skill: user stories (see [[keyword-bank]]).

## Related pages

- [[requirements-analysis]]
- [[uat-plan]]

## Sources / Evidence

- [[job-market-signal-business-analyst-summary]]
