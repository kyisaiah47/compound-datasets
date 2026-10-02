# StillShipping records a maintenance verdict for every tracked agent tool.

Each row records one tracked AI agent tool. The row stores the nightly maintenance verdict, which is maintained, slowing or dead. The row stores the 0-100 freshness score and every GitHub signal used to compute the verdict.

| | |
|---|---|
| Rows in this cut | 362 |
| One row is | one tool |
| Cut | 2026-10-01 |
| Refreshed | Monthly, on the first of the month |
| Measured by | [StillShipping](https://stillshipping.thecompound.tech) |
| Method | [https://toolproof.thecompound.tech/methodology](https://toolproof.thecompound.tech/methodology) |
| Licence | [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/) |
| Publisher | [Compound Labs](https://thecompound.tech) |
| Also on | [Hugging Face](https://huggingface.co/datasets/kyisaiah47/stillshipping-tools) · [Kaggle](https://www.kaggle.com/datasets/kyisaiah47/stillshipping-tools) · [Zenodo](https://zenodo.org/records/22844097) |

## How it is measured

StillShipping pulls commit, release, issue and contributor activity from the GitHub API nightly. It converts those signals into one of three verdicts. It recomputes the verdict every night instead of recording it once. A project that goes quiet therefore changes its own row without manual editing.

## What a citer needs to know

- `reasons` stores the JSON used to derive the verdict. The field preserves the inputs for disputing that verdict.
- `refreshed_at` records the nightly run that last changed the row. A row stops refreshing when its repository becomes private or is deleted. The row keeps its last verdict.

## Files

| File | Format | Size |
|---|---|---|
| `stillshipping-tools-2026-10-01.csv` | CSV | 0.44 MB |
| `stillshipping-tools-2026-10-01.json` | JSON | 0.62 MB |

Every cut is also published as a [GitHub release](https://github.com/kyisaiah47/compound-datasets/releases). The release attaches
the same files. A citation can use the release to pin the exact edition it quoted.

## Schema

| Column | Type | Empty in sample |
|---|---|---|
| `slug` | string | 0.0% |
| `name` | string | 0.0% |
| `repo_full_name` | string | 0.0% |
| `category` | string | 0.0% |
| `vendor` | string | 94.2% |
| `tagline` | string | 0.0% |
| `homepage` | string | 13.8% |
| `aliases` | array | 0.0% |
| `verdict` | string | 0.0% |
| `freshness` | number | 0.0% |
| `reasons` | array | 0.0% |
| `verdict_at` | string | 0.0% |
| `previous_verdict` | string | 90.1% |
| `verdict_changed_at` | string | 90.1% |
| `stars` | number | 0.0% |
| `forks` | number | 0.0% |
| `open_issues` | number | 0.0% |
| `language` | string | 1.4% |
| `license` | string | 17.4% |
| `archived` | boolean | 0.0% |
| `disabled` | boolean | 0.0% |
| `description` | string | 0.5% |
| `created_at` | string | 0.0% |
| `pushed_at` | string | 0.0% |
| `days_since_push` | number | 0.0% |
| `recent_commits` | number | 0.0% |
| `last_release_at` | string | 14.1% |
| `last_release_tag` | string | 14.1% |
| `releases_365d` | number | 0.0% |
| `release_gap_days` | number | 14.1% |
| `median_release_gap` | number | 20.7% |
| `issue_response_hours` | number | 64.4% |
| `issues_sampled` | number | 0.0% |
| `stale_issue_ratio` | number | 4.4% |
| `contributors_90d` | number | 0.0% |
| `contributors_total` | null | 100.0% |
| `bus_factor` | number | 0.0% |
| `first_seen` | string | 0.0% |
| `refreshed_at` | string | 0.0% |

## Cite it

```
Compound Labs (2026). StillShipping: maintenance verdict for every tracked agent tool. StillShipping, https://stillshipping.thecompound.tech. Cut of 2026-10-01. Creative Commons Attribution 4.0 International (CC BY 4.0). https://github.com/kyisaiah47/compound-datasets/tree/main/stillshipping-tools
```

```bibtex
@dataset{compound_stillshipping_tools_2026,
  title     = {StillShipping: maintenance verdict for every tracked agent tool},
  author    = {{Compound Labs}},
  year      = {2026},
  publisher = {Compound Labs},
  url       = {https://github.com/kyisaiah47/compound-datasets/tree/main/stillshipping-tools},
  note      = {Cut of 2026-10-01. Measured by StillShipping, https://stillshipping.thecompound.tech},
  license   = {CC-BY-4.0}
}
```

The whole collection has the DOI 10.5281/zenodo.22844096 at [https://doi.org/10.5281/zenodo.22844096](https://doi.org/10.5281/zenodo.22844096). The DOI resolves
to the newest Zenodo version. Cite 10.5281/zenodo.22844097 to pin the exact deposit for this cut.

Attribution is the licence condition. Attribution is the only condition. Cite the publisher, the
product that measured the figure, and the cut date when you quote a figure. You do not need to
ask for anything else.
