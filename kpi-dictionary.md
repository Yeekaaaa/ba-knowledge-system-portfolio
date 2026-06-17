# KPI Dictionary

## Definition

A controlled list of business metrics: definitions, formulas, data sources, owners, units, thresholds, and interpretation rules.

## When to use

When teams calculate or interpret the same metric inconsistently — common before dashboard programmes.

## Minimum viable structure

| Field | Description |
|---|---|
| KPI name | Standard name |
| Business meaning | Decision it supports |
| Formula | Unambiguous calculation |
| Data source | System / file / field |
| Grain | Store, region, day, month |
| Owner | Role accountable for definition |
| Thresholds | Optional RAG rules |
| Caveats | Known data gaps |

## Quality checklist

- Formula and unit explicit
- Time period defined (e.g. calendar month)
- Edge cases documented (returns, closures, partial months)
- Stakeholders agree in sign-off workshop

## Example (SYNTHETIC)

| KPI | Formula (sample) |
|---|---|
| Revenue | Sum of recognised sales in period |
| Operating cost | Sum of mapped cost lines |
| Margin | Revenue − operating cost |
| Budget variance | Actual − budget |

Fictional context: `sample-raw/synthetic-project-note.md`.

## Transformation KPI layer

For digital programmes, extend with themes from [[digital-transformation-framework]]:

- **Value creation** — e.g. reporting cycle time
- **Team health** — e.g. validation error rate
- **Change progress** — e.g. % periods using standard import

## Sources / Evidence

- [[public-article-digital-transformation-summary]]
- `sample-raw/synthetic-project-note.md` (SYNTHETIC)
