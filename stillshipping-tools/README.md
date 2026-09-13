# StillShipping: maintenance verdict for every tracked agent tool

One row per tracked AI agent tool, with the nightly maintenance verdict (maintained, slowing or dead), the 0-100 freshness behind it, and every GitHub signal the verdict was computed from.

| | |
|---|---|
| Rows in this cut | 340 |
| One row is | one tool |
| Cut | 2026-09-04 |
| Refreshed | Monthly, on the first of the month |
| Measured by | [StillShipping](https://stillshipping.thecompound.tech) |
| Method | [https://toolproof.thecompound.tech/methodology](https://toolproof.thecompound.tech/methodology) |
| Licence | [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/) |
| Publisher | [Compound Labs](https://thecompound.tech) |

## How it is measured

Commit, release, issue and contributor activity is pulled from the GitHub API nightly and turned into one of three verdicts. The verdict is recomputed every night rather than recorded once, so a project that goes quiet changes its own row without anybody editing it.

## What a citer needs to know

- `reasons` is the JSON the verdict was derived from, kept so a verdict can be argued with on its inputs.
- `refreshed_at` is the nightly run that last touched the row. A row whose repository has gone private or been deleted stops refreshing and keeps its last verdict.

## Files

| File | Format | Size |
|---|---|---|
| `stillshipping-tools-2026-09-04.csv` | CSV | 0.41 MB |
| `stillshipping-tools-2026-09-04.json` | JSON | 0.58 MB |

Every cut is also a [GitHub release](https://github.com/kyisaiah47/compound-datasets/releases) with the same files attached, so a
citation can pin the exact edition it quoted.

## Schema

| Column | Type | Empty in sample |
|---|---|---|
| `slug` | string | 0.0% |
| `name` | string | 0.0% |
| `repo_full_name` | string | 0.0% |
| `category` | string | 0.0% |
| `vendor` | string | 93.8% |
| `tagline` | string | 0.0% |
| `homepage` | string | 13.5% |
| `aliases` | array | 0.0% |
| `verdict` | string | 0.0% |
| `freshness` | number | 0.0% |
| `reasons` | array | 0.0% |
| `verdict_at` | string | 0.0% |
| `previous_verdict` | string | 93.8% |
| `verdict_changed_at` | string | 93.8% |
| `stars` | number | 0.0% |
| `forks` | number | 0.0% |
| `open_issues` | number | 0.0% |
| `language` | string | 1.2% |
| `license` | string | 17.1% |
| `archived` | boolean | 0.0% |
| `disabled` | boolean | 0.0% |
| `description` | string | 0.6% |
| `created_at` | string | 0.0% |
| `pushed_at` | string | 0.0% |
| `days_since_push` | number | 0.0% |
| `recent_commits` | number | 0.0% |
| `last_release_at` | string | 14.1% |
| `last_release_tag` | string | 14.1% |
| `releases_365d` | number | 0.0% |
| `release_gap_days` | number | 14.1% |
| `median_release_gap` | number | 19.4% |
| `issue_response_hours` | number | 61.8% |
| `issues_sampled` | number | 0.0% |
| `stale_issue_ratio` | number | 4.4% |
| `contributors_90d` | number | 0.0% |
| `contributors_total` | null | 100.0% |
| `bus_factor` | number | 0.0% |
| `first_seen` | string | 0.0% |
| `refreshed_at` | string | 0.0% |

## Cite it

```
Compound Labs (2026). StillShipping: maintenance verdict for every tracked agent tool. StillShipping, https://stillshipping.thecompound.tech. Cut of 2026-09-04. Creative Commons Attribution 4.0 International (CC BY 4.0). https://github.com/kyisaiah47/compound-datasets/tree/main/stillshipping-tools
```

```bibtex
@dataset{compound_stillshipping_tools_2026,
  title     = {StillShipping: maintenance verdict for every tracked agent tool},
  author    = {{Compound Labs}},
  year      = {2026},
  publisher = {Compound Labs},
  url       = {https://github.com/kyisaiah47/compound-datasets/tree/main/stillshipping-tools},
  note      = {Cut of 2026-09-04. Measured by StillShipping, https://stillshipping.thecompound.tech},
  license   = {CC-BY-4.0}
}
```

Attribution is the licence condition, and it is the only one. Quote a figure with the publisher,
the product that measured it and the cut date, and there is nothing else to ask.
