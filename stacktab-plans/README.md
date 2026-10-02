# StackTab records every plan, its price and the page that supplied the price.

Each row records one published plan. The row stores its base monthly price in USD, the plan's contents, its restrictions, and the URL that supplied the figure. The row also stores the date when that URL was last checked.

| | |
|---|---|
| Rows in this cut | 64 |
| One row is | one plan |
| Cut | 2026-10-01 |
| Refreshed | Monthly, on the first of the month |
| Measured by | [StackTab](https://stacktab.thecompound.tech) |
| Method | [https://toolproof.thecompound.tech/methodology](https://toolproof.thecompound.tech/methodology) |
| Licence | [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/) |
| Publisher | [Compound Labs](https://thecompound.tech) |
| Also on | [Hugging Face](https://huggingface.co/datasets/kyisaiah47/stacktab-plans) · [Kaggle](https://www.kaggle.com/datasets/kyisaiah47/stacktab-plans) · [Zenodo](https://zenodo.org/records/22844097) |

## How it is measured

StackTab re-checks each plan against its pricing page on a schedule. `price_status` states whether the check could read a number. A plan priced by sales contact is published as unpriced, not as zero.

## What a citer needs to know

- `verified_at` records the last time the page confirmed the figure. `last_check_note` records what happened when a check could not confirm it.
- `probes` stores the strings that the check searched for on the page. The dataset publishes those strings so a reader can re-derive a disputed price.

## Files

| File | Format | Size |
|---|---|---|
| `stacktab-plans-2026-10-01.csv` | CSV | 0.02 MB |
| `stacktab-plans-2026-10-01.json` | JSON | 0.03 MB |

Every cut is also published as a [GitHub release](https://github.com/kyisaiah47/compound-datasets/releases). The release attaches
the same files. A citation can use the release to pin the exact edition it quoted.

## Schema

| Column | Type | Empty in sample |
|---|---|---|
| `service_slug` | string | 0.0% |
| `plan_slug` | string | 0.0% |
| `name` | string | 0.0% |
| `rank` | number | 0.0% |
| `base_monthly_usd` | number | 0.0% |
| `price_status` | string | 0.0% |
| `included` | object | 0.0% |
| `restrictions` | object | 0.0% |
| `notes` | string | 7.8% |
| `source_url` | string | 0.0% |
| `probes` | array | 0.0% |
| `check_status` | string | 0.0% |
| `verified_at` | string | 0.0% |
| `last_checked_at` | string | 0.0% |
| `last_check_note` | string | 90.6% |

## Cite it

```
Compound Labs (2026). StackTab: every plan, its price, and the page the price was read from. StackTab, https://stacktab.thecompound.tech. Cut of 2026-10-01. Creative Commons Attribution 4.0 International (CC BY 4.0). https://github.com/kyisaiah47/compound-datasets/tree/main/stacktab-plans
```

```bibtex
@dataset{compound_stacktab_plans_2026,
  title     = {StackTab: every plan, its price, and the page the price was read from},
  author    = {{Compound Labs}},
  year      = {2026},
  publisher = {Compound Labs},
  url       = {https://github.com/kyisaiah47/compound-datasets/tree/main/stacktab-plans},
  note      = {Cut of 2026-10-01. Measured by StackTab, https://stacktab.thecompound.tech},
  license   = {CC-BY-4.0}
}
```

The whole collection has the DOI 10.5281/zenodo.22844096 at [https://doi.org/10.5281/zenodo.22844096](https://doi.org/10.5281/zenodo.22844096). The DOI resolves
to the newest Zenodo version. Cite 10.5281/zenodo.22844097 to pin the exact deposit for this cut.

Attribution is the licence condition. Attribution is the only condition. Cite the publisher, the
product that measured the figure, and the cut date when you quote a figure. You do not need to
ask for anything else.
