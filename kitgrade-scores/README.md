# KitGrade: the component scores behind every kit grade

One row per kit carrying the six component scores the total is composed from, the method version that produced them, and the full breakdown JSON.

| | |
|---|---|
| Rows in this cut | 36 |
| One row is | one kit |
| Cut | 2026-09-04 |
| Refreshed | Monthly, on the first of the month |
| Measured by | [KitGrade](https://kitgrade.thecompound.tech) |
| Method | [https://toolproof.thecompound.tech/methodology](https://toolproof.thecompound.tech/methodology) |
| Licence | [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/) |
| Publisher | [Compound Labs](https://thecompound.tech) |
| Also on | [Hugging Face](https://huggingface.co/datasets/kyisaiah47/kitgrade-scores) · [Zenodo](https://zenodo.org/records/22844097) |

## How it is measured

Each component is computed from the measured facts in the kits table by a versioned scoring function. `method_version` moves when the function changes, so a score from one edition is never silently compared with a score from another.

## What a citer needs to know

- A total is only comparable within one `method_version`. Comparing across versions is a comparison of two different functions.

## Files

| File | Format | Size |
|---|---|---|
| `kitgrade-scores-2026-09-04.csv` | CSV | 0.02 MB |
| `kitgrade-scores-2026-09-04.json` | JSON | 0.02 MB |

Every cut is also a [GitHub release](https://github.com/kyisaiah47/compound-datasets/releases) with the same files attached, so a
citation can pin the exact edition it quoted.

## Schema

| Column | Type | Empty in sample |
|---|---|---|
| `kit_slug` | string | 0.0% |
| `method_version` | string | 0.0% |
| `total` | number | 0.0% |
| `normalised` | number | 0.0% |
| `coverage` | number | 0.0% |
| `maintenance` | number | 38.9% |
| `completeness` | number | 0.0% |
| `transparency` | number | 0.0% |
| `documentation` | number | 0.0% |
| `support` | number | 0.0% |
| `breakdown` | object | 0.0% |
| `computed_at` | string | 0.0% |

## Cite it

```
Compound Labs (2026). KitGrade: the component scores behind every kit grade. KitGrade, https://kitgrade.thecompound.tech. Cut of 2026-09-04. Creative Commons Attribution 4.0 International (CC BY 4.0). https://github.com/kyisaiah47/compound-datasets/tree/main/kitgrade-scores
```

```bibtex
@dataset{compound_kitgrade_scores_2026,
  title     = {KitGrade: the component scores behind every kit grade},
  author    = {{Compound Labs}},
  year      = {2026},
  publisher = {Compound Labs},
  url       = {https://github.com/kyisaiah47/compound-datasets/tree/main/kitgrade-scores},
  note      = {Cut of 2026-09-04. Measured by KitGrade, https://kitgrade.thecompound.tech},
  license   = {CC-BY-4.0}
}
```

The whole collection has a DOI, 10.5281/zenodo.22844096, at [https://doi.org/10.5281/zenodo.22844096](https://doi.org/10.5281/zenodo.22844096). It resolves to the
newest Zenodo version. To pin the exact deposit this cut belongs to, cite 10.5281/zenodo.22844097 instead.

Attribution is the licence condition, and it is the only one. Quote a figure with the publisher,
the product that measured it and the cut date, and there is nothing else to ask.
