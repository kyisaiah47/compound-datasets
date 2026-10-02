# StoreReady records AI app builders and whether their output ships.

Each row records one AI app builder. The row states what the builder outputs, whether the source leaves the platform, whether the builder submits to the store, what the builder costs, and whether the App Store accepts its output.

| | |
|---|---|
| Rows in this cut | 14 |
| One row is | one app builder |
| Cut | 2026-10-01 |
| Refreshed | Monthly, on the first of the month |
| Measured by | [StoreReady](https://storeready.thecompound.tech) |
| Method | [https://toolproof.thecompound.tech/methodology](https://toolproof.thecompound.tech/methodology) |
| Licence | [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/) |
| Publisher | [Compound Labs](https://thecompound.tech) |
| Also on | [Hugging Face](https://huggingface.co/datasets/kyisaiah47/storeready-builders) · [Kaggle](https://www.kaggle.com/datasets/kyisaiah47/storeready-builders) · [Zenodo](https://zenodo.org/records/22844097) |

## How it is measured

Each verdict links to numbered evidence in the companion evidence dataset. The dataset publishes a builder as unknown when it has no supporting evidence.

## What a citer needs to know

- `risk_guidelines` lists the App Review guideline clauses, identified by number, that expose the output to risk.
- The verdict evaluates the output, not the company. The verdict changes when the output changes.

## Files

| File | Format | Size |
|---|---|---|
| `storeready-builders-2026-10-01.csv` | CSV | 0.02 MB |
| `storeready-builders-2026-10-01.json` | JSON | 0.02 MB |

Every cut is also published as a [GitHub release](https://github.com/kyisaiah47/compound-datasets/releases). The release attaches
the same files. A citation can use the release to pin the exact edition it quoted.

## Schema

| Column | Type | Empty in sample |
|---|---|---|
| `slug` | string | 0.0% |
| `name` | string | 0.0% |
| `tagline` | string | 0.0% |
| `url` | string | 0.0% |
| `category` | string | 0.0% |
| `output_type` | string | 0.0% |
| `output_detail` | string | 0.0% |
| `exports_source` | string | 0.0% |
| `exports_source_detail` | string | 0.0% |
| `submits_for_you` | string | 0.0% |
| `price_free` | boolean | 14.3% |
| `price_from_usd` | number | 7.1% |
| `price_note` | string | 0.0% |
| `review_verdict` | string | 0.0% |
| `review_summary` | string | 0.0% |
| `risk_guidelines` | array | 0.0% |
| `rank` | number | 0.0% |
| `updated_at` | string | 0.0% |

## Cite it

```
Compound Labs (2026). StoreReady: AI app builders and whether their output ships. StoreReady, https://storeready.thecompound.tech. Cut of 2026-10-01. Creative Commons Attribution 4.0 International (CC BY 4.0). https://github.com/kyisaiah47/compound-datasets/tree/main/storeready-builders
```

```bibtex
@dataset{compound_storeready_builders_2026,
  title     = {StoreReady: AI app builders and whether their output ships},
  author    = {{Compound Labs}},
  year      = {2026},
  publisher = {Compound Labs},
  url       = {https://github.com/kyisaiah47/compound-datasets/tree/main/storeready-builders},
  note      = {Cut of 2026-10-01. Measured by StoreReady, https://storeready.thecompound.tech},
  license   = {CC-BY-4.0}
}
```

The whole collection has the DOI 10.5281/zenodo.22844096 at [https://doi.org/10.5281/zenodo.22844096](https://doi.org/10.5281/zenodo.22844096). The DOI resolves
to the newest Zenodo version. Cite 10.5281/zenodo.22844097 to pin the exact deposit for this cut.

Attribution is the licence condition. Attribution is the only condition. Cite the publisher, the
product that measured the figure, and the cut date when you quote a figure. You do not need to
ask for anything else.
