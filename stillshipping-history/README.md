# StillShipping: the daily verdict history

One row per tool per captured day: the verdict it held that day and the activity figures behind it. This is the series a reader needs to see a project slow down rather than to see where it stands today.

| | |
|---|---|
| Rows in this cut | 10,142 |
| One row is | one tool on one day |
| Cut | 2026-09-04 |
| Refreshed | Monthly, on the first of the month |
| Measured by | [StillShipping](https://stillshipping.thecompound.tech) |
| Method | [https://toolproof.thecompound.tech/methodology](https://toolproof.thecompound.tech/methodology) |
| Licence | [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/) |
| Publisher | [Compound Labs](https://thecompound.tech) |

## How it is measured

A snapshot is written every night after the verdicts are recomputed, from the same GitHub API reads. Nothing is backfilled and nothing is revised, so a day that was measured wrong stays in the series and is corrected by a later day rather than overwritten.

## What a citer needs to know

- The series starts when a tool was first tracked, not when the project started. A short series means a recent addition.

## Files

| File | Format | Size |
|---|---|---|
| `stillshipping-history-2026-09-04.csv` | CSV | 6.9 MB |
| `stillshipping-history-2026-09-04.json` | JSON | 8.4 MB |

Every cut is also a [GitHub release](https://github.com/kyisaiah47/compound-datasets/releases) with the same files attached, so a
citation can pin the exact edition it quoted.

## Schema

| Column | Type | Empty in sample |
|---|---|---|
| `tool_slug` | string | 0.0% |
| `captured_on` | string | 0.0% |
| `verdict` | string | 0.0% |
| `freshness` | number | 0.0% |
| `days_since_push` | number | 0.0% |
| `recent_commits` | number | 0.0% |
| `release_gap_days` | number | 13.9% |
| `issue_response_hours` | number | 77.5% |
| `contributors_90d` | number | 0.0% |
| `stars` | number | 0.0% |
| `open_issues` | number | 0.0% |
| `archived` | boolean | 0.0% |
| `reasons` | array | 0.0% |
| `captured_at` | string | 0.0% |

## Cite it

```
Compound Labs (2026). StillShipping: the daily verdict history. StillShipping, https://stillshipping.thecompound.tech. Cut of 2026-09-04. Creative Commons Attribution 4.0 International (CC BY 4.0). https://github.com/kyisaiah47/compound-datasets/tree/main/stillshipping-history
```

```bibtex
@dataset{compound_stillshipping_history_2026,
  title     = {StillShipping: the daily verdict history},
  author    = {{Compound Labs}},
  year      = {2026},
  publisher = {Compound Labs},
  url       = {https://github.com/kyisaiah47/compound-datasets/tree/main/stillshipping-history},
  note      = {Cut of 2026-09-04. Measured by StillShipping, https://stillshipping.thecompound.tech},
  license   = {CC-BY-4.0}
}
```

Attribution is the licence condition, and it is the only one. Quote a figure with the publisher,
the product that measured it and the cut date, and there is nothing else to ask.
