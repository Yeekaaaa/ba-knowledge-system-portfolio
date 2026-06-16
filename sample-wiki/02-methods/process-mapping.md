# Process Mapping

## Purpose

Document how work happens today and how it should work after change — exposing friction, handoffs, and automation candidates.

## Inputs

- Stakeholder interviews and observation
- Existing documents (SOPs, spreadsheets, system screenshots — rights-checked)
- Volume, frequency, error patterns

## Steps

1. Define process boundaries (start/end, in/out of scope).
2. Map **current state** (swimlanes: role, system, data).
3. Identify pain points: rework, duplicate entry, delays, inconsistent rules.
4. Classify root causes: people, process, system, data, governance.
5. Design **future state** with controls and exceptions.
6. Highlight automation opportunities — [[ai-automation-opportunity-discovery]].
7. Validate with operators.

## Outputs

- Current-state process map
- Future-state process map
- Pain point register
- Control points and exception paths

## Common mistakes

- Mapping idealised process, not actual practice
- Ignoring informal workarounds (shadow spreadsheets)
- Jumping to tooling before stabilising definitions

## Example (SYNTHETIC)

Current state: email → store Excel → manual consolidation → leadership review.

Future state: controlled monthly import with validation gate → KPI engine → dashboard. See `sample-raw/synthetic-project-note.md`.

## Interview phrasing

> I separate process, data, and system layers so we fix the right root cause before specifying dashboards or automation.

## Sources / Evidence

- [[job-market-signal-business-analyst-summary]] — process mapping among top skills
- [[public-article-digital-transformation-summary]] — domain-level process change
