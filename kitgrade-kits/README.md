# KitGrade: SaaS starter kits and what is measurably in the box

One row per graded SaaS starter kit: its stack, licence and pricing, the release and commit activity behind it, what its own documentation says ships in the box, and the evidence level the grade rests on.

| | |
|---|---|
| Rows in this cut | 36 |
| One row is | one starter kit |
| Cut | 2026-09-04 |
| Refreshed | Monthly, on the first of the month |
| Measured by | [KitGrade](https://kitgrade.thecompound.tech) |
| Method | [https://toolproof.thecompound.tech/methodology](https://toolproof.thecompound.tech/methodology) |
| Licence | [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/) |
| Publisher | [Compound Labs](https://thecompound.tech) |
| Also on | [Hugging Face](https://huggingface.co/datasets/kyisaiah47/kitgrade-kits) · [Zenodo](https://zenodo.org/records/22844097) |

## How it is measured

Kits are graded from measured facts rather than from their own landing pages. A price is recorded from the page that states it, with the quote in `price_evidence`. `evidence_level` separates a kit somebody installed and ran from a kit somebody read about, because those are different claims and merging them is how starter-kit comparisons become useless.

## What a citer needs to know

- `price_unmeasurable` is true where a kit publishes no price a machine can read. That is published as a finding rather than as a null.
- `includes` and `price_points` are JSON, kept whole so a reader can recompute a grade from the inputs.

## Files

| File | Format | Size |
|---|---|---|
| `kitgrade-kits-2026-09-04.csv` | CSV | 0.08 MB |
| `kitgrade-kits-2026-09-04.json` | JSON | 0.09 MB |

Every cut is also a [GitHub release](https://github.com/kyisaiah47/compound-datasets/releases) with the same files attached, so a
citation can pin the exact edition it quoted.

## Schema

| Column | Type | Empty in sample |
|---|---|---|
| `slug` | string | 0.0% |
| `name` | string | 0.0% |
| `vendor` | string | 0.0% |
| `homepage` | string | 0.0% |
| `pricing_url` | string | 61.1% |
| `docs_url` | string | 22.2% |
| `repo` | string | 38.9% |
| `ecosystem` | string | 0.0% |
| `stack` | array | 0.0% |
| `license` | string | 0.0% |
| `license_source` | string | 0.0% |
| `open_source` | boolean | 0.0% |
| `pricing_model` | string | 0.0% |
| `price_min_usd` | number | 5.6% |
| `price_max_usd` | number | 5.6% |
| `price_evidence` | string | 66.7% |
| `price_checked_at` | string | 61.1% |
| `price_points` | array | 0.0% |
| `price_unmeasurable` | boolean | 0.0% |
| `last_commit_at` | string | 38.9% |
| `last_release_at` | string | 55.6% |
| `last_release_tag` | string | 52.8% |
| `releases_12mo` | number | 38.9% |
| `stars` | number | 38.9% |
| `forks` | number | 38.9% |
| `open_issues` | number | 38.9% |
| `contributors` | number | 38.9% |
| `includes` | object | 0.0% |
| `support_model` | string | 8.3% |
| `support_source` | string | 8.3% |
| `docs_pages` | number | 61.1% |
| `docs_kind` | string | 0.0% |
| `evidence_level` | string | 0.0% |
| `active` | boolean | 0.0% |
| `archived` | boolean | 0.0% |
| `logo_url` | string | 0.0% |
| `summary` | string | 2.8% |
| `summary_source` | string | 0.0% |
| `changelog_url` | string | 97.2% |
| `changelog_source` | string | 97.2% |
| `edition_of` | string | 97.2% |
| `edition_label` | string | 94.4% |
| `refreshed_at` | string | 0.0% |

## Cite it

```
Compound Labs (2026). KitGrade: SaaS starter kits and what is measurably in the box. KitGrade, https://kitgrade.thecompound.tech. Cut of 2026-09-04. Creative Commons Attribution 4.0 International (CC BY 4.0). https://github.com/kyisaiah47/compound-datasets/tree/main/kitgrade-kits
```

```bibtex
@dataset{compound_kitgrade_kits_2026,
  title     = {KitGrade: SaaS starter kits and what is measurably in the box},
  author    = {{Compound Labs}},
  year      = {2026},
  publisher = {Compound Labs},
  url       = {https://github.com/kyisaiah47/compound-datasets/tree/main/kitgrade-kits},
  note      = {Cut of 2026-09-04. Measured by KitGrade, https://kitgrade.thecompound.tech},
  license   = {CC-BY-4.0}
}
```

The whole collection has a DOI, 10.5281/zenodo.22844096, at [https://doi.org/10.5281/zenodo.22844096](https://doi.org/10.5281/zenodo.22844096). It resolves to the
newest Zenodo version. To pin the exact deposit this cut belongs to, cite 10.5281/zenodo.22844097 instead.

Attribution is the licence condition, and it is the only one. Quote a figure with the publisher,
the product that measured it and the cut date, and there is nothing else to ask.
