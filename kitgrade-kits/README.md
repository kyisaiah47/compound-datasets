# KitGrade: SaaS starter kits and what is measurably in the box

Each row represents one graded SaaS starter kit. The row records its stack, licence, pricing, release activity, commit activity, documented contents, and the evidence level supporting the grade.

| | |
|---|---|
| Rows in this cut | 39 |
| One row is | one starter kit |
| Cut | 2026-10-01 |
| Refreshed | Monthly, on the first of the month |
| Measured by | [KitGrade](https://kitgrade.thecompound.tech) |
| Method | [https://toolproof.thecompound.tech/methodology](https://toolproof.thecompound.tech/methodology) |
| Licence | [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/) |
| Publisher | [Compound Labs](https://thecompound.tech) |
| Also on | [Hugging Face](https://huggingface.co/datasets/kyisaiah47/kitgrade-kits) · [Kaggle](https://www.kaggle.com/datasets/kyisaiah47/kitgrade-kits) · [Zenodo](https://zenodo.org/records/22844097) |

## How it is measured

KitGrade grades kits from measured facts rather than their landing pages. The dataset records a price from the page that states it. The dataset stores the quotation in `price_evidence`. `evidence_level` separates a kit that somebody installed and ran from a kit that somebody only read about. Those are different claims. Combining them makes starter-kit comparisons useless.

## What a citer needs to know

- `price_unmeasurable` is true when a kit publishes no price that a machine can read. The dataset publishes that result as a finding rather than as a null.
- The dataset keeps `includes` and `price_points` as whole JSON values. A reader can recompute a grade from those inputs.

## Files

| File | Format | Size |
|---|---|---|
| `kitgrade-kits-2026-10-01.csv` | CSV | 0.09 MB |
| `kitgrade-kits-2026-10-01.json` | JSON | 0.10 MB |

Every cut is also published as a [GitHub release](https://github.com/kyisaiah47/compound-datasets/releases). The release attaches
the same files. A citation can use the release to pin the exact edition it quoted.

## Schema

| Column | Type | Empty in sample |
|---|---|---|
| `slug` | string | 0.0% |
| `name` | string | 0.0% |
| `vendor` | string | 0.0% |
| `homepage` | string | 0.0% |
| `pricing_url` | string | 56.4% |
| `docs_url` | string | 17.9% |
| `repo` | string | 43.6% |
| `ecosystem` | string | 0.0% |
| `stack` | array | 0.0% |
| `license` | string | 0.0% |
| `license_source` | string | 0.0% |
| `open_source` | boolean | 0.0% |
| `pricing_model` | string | 0.0% |
| `price_min_usd` | number | 5.1% |
| `price_max_usd` | number | 5.1% |
| `price_evidence` | string | 61.5% |
| `price_checked_at` | string | 56.4% |
| `price_points` | array | 0.0% |
| `price_unmeasurable` | boolean | 0.0% |
| `last_commit_at` | string | 43.6% |
| `last_release_at` | string | 53.8% |
| `last_release_tag` | string | 53.8% |
| `releases_12mo` | number | 43.6% |
| `stars` | number | 43.6% |
| `forks` | number | 43.6% |
| `open_issues` | number | 43.6% |
| `contributors` | number | 43.6% |
| `includes` | object | 0.0% |
| `support_model` | string | 12.8% |
| `support_source` | string | 12.8% |
| `docs_pages` | number | 56.4% |
| `docs_kind` | string | 0.0% |
| `evidence_level` | string | 0.0% |
| `active` | boolean | 0.0% |
| `archived` | boolean | 0.0% |
| `logo_url` | string | 0.0% |
| `summary` | string | 2.6% |
| `summary_source` | string | 0.0% |
| `changelog_url` | string | 92.3% |
| `changelog_source` | string | 92.3% |
| `edition_of` | string | 97.4% |
| `edition_label` | string | 94.9% |
| `refreshed_at` | string | 0.0% |

## Cite it

```
Compound Labs (2026). KitGrade: SaaS starter kits and what is measurably in the box. KitGrade, https://kitgrade.thecompound.tech. Cut of 2026-10-01. Creative Commons Attribution 4.0 International (CC BY 4.0). https://github.com/kyisaiah47/compound-datasets/tree/main/kitgrade-kits
```

```bibtex
@dataset{compound_kitgrade_kits_2026,
  title     = {KitGrade: SaaS starter kits and what is measurably in the box},
  author    = {{Compound Labs}},
  year      = {2026},
  publisher = {Compound Labs},
  url       = {https://github.com/kyisaiah47/compound-datasets/tree/main/kitgrade-kits},
  note      = {Cut of 2026-10-01. Measured by KitGrade, https://kitgrade.thecompound.tech},
  license   = {CC-BY-4.0}
}
```

The whole collection has the DOI 10.5281/zenodo.22844096 at [https://doi.org/10.5281/zenodo.22844096](https://doi.org/10.5281/zenodo.22844096). The DOI resolves
to the newest Zenodo version. Cite 10.5281/zenodo.22844097 to pin the exact deposit for this cut.

Attribution is the licence condition. Attribution is the only condition. Cite the publisher, the
product that measured the figure, and the cut date when you quote a figure. You do not need to
ask for anything else.
