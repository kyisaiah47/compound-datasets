# StillShipping records the daily verdict history.

Each row records one tool on one captured day. The row stores the verdict held that day and the activity figures behind it. The series shows how a project slows down instead of showing only its current state.

| | |
|---|---|
| Rows in this cut | 18,462 |
| One row is | one tool on one day |
| Cut | 2026-10-01 |
| Refreshed | Monthly, on the first of the month |
| Measured by | [StillShipping](https://stillshipping.thecompound.tech) |
| Method | [https://toolproof.thecompound.tech/methodology](https://toolproof.thecompound.tech/methodology) |
| Licence | [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/) |
| Publisher | [Compound Labs](https://thecompound.tech) |
| Also on | [Hugging Face](https://huggingface.co/datasets/kyisaiah47/stillshipping-history) · [Kaggle](https://www.kaggle.com/datasets/kyisaiah47/stillshipping-history) · [Zenodo](https://zenodo.org/records/22844097) |

## How it is measured

StillShipping writes a snapshot every night after recomputing the verdicts. The snapshot uses the same GitHub API reads. The dataset does not backfill or revise snapshots. A wrongly measured day remains in the series, and a later day provides the correction instead of overwriting it.

## What a citer needs to know

- The series starts when StillShipping first tracks a tool. It does not start when the project starts. A short series indicates a recent addition.

## Files

| File | Format | Size |
|---|---|---|
| `stillshipping-history-2026-10-01.csv` | CSV | 12.9 MB |
| `stillshipping-history-2026-10-01.json` | JSON | 15.6 MB |

Every cut is also published as a [GitHub release](https://github.com/kyisaiah47/compound-datasets/releases). The release attaches
the same files. A citation can use the release to pin the exact edition it quoted.

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
Compound Labs (2026). StillShipping: the daily verdict history. StillShipping, https://stillshipping.thecompound.tech. Cut of 2026-10-01. Creative Commons Attribution 4.0 International (CC BY 4.0). https://github.com/kyisaiah47/compound-datasets/tree/main/stillshipping-history
```

```bibtex
@dataset{compound_stillshipping_history_2026,
  title     = {StillShipping: the daily verdict history},
  author    = {{Compound Labs}},
  year      = {2026},
  publisher = {Compound Labs},
  url       = {https://github.com/kyisaiah47/compound-datasets/tree/main/stillshipping-history},
  note      = {Cut of 2026-10-01. Measured by StillShipping, https://stillshipping.thecompound.tech},
  license   = {CC-BY-4.0}
}
```

The whole collection has the DOI 10.5281/zenodo.22844096 at [https://doi.org/10.5281/zenodo.22844096](https://doi.org/10.5281/zenodo.22844096). The DOI resolves
to the newest Zenodo version. Cite 10.5281/zenodo.22844097 to pin the exact deposit for this cut.

Attribution is the licence condition. Attribution is the only condition. Cite the publisher, the
product that measured the figure, and the cut date when you quote a figure. You do not need to
ask for anything else.
