# KitGrade: the component scores behind every kit grade

Each row represents one kit. The row carries the six component scores that compose the total, the method version that produced them, and the full breakdown JSON.

| | |
|---|---|
| Rows in this cut | 39 |
| One row is | one kit |
| Cut | 2026-10-01 |
| Refreshed | Monthly, on the first of the month |
| Measured by | [KitGrade](https://kitgrade.thecompound.tech) |
| Method | [https://toolproof.thecompound.tech/methodology](https://toolproof.thecompound.tech/methodology) |
| Licence | [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/) |
| Publisher | [Compound Labs](https://thecompound.tech) |
| Also on | [Hugging Face](https://huggingface.co/datasets/kyisaiah47/kitgrade-scores) · [Kaggle](https://www.kaggle.com/datasets/kyisaiah47/kitgrade-scores) · [Zenodo](https://zenodo.org/records/22844097) |

## How it is measured

A versioned scoring function computes each component from the measured facts in the kits table. `method_version` changes when the function changes. A score from one edition is never silently compared with a score from another edition.

## What a citer needs to know

- A total is comparable only within one `method_version`. A comparison across versions compares two different functions.

## Files

| File | Format | Size |
|---|---|---|
| `kitgrade-scores-2026-10-01.csv` | CSV | 0.02 MB |
| `kitgrade-scores-2026-10-01.json` | JSON | 0.03 MB |

Every cut is also published as a [GitHub release](https://github.com/kyisaiah47/compound-datasets/releases). The release attaches
the same files. A citation can use the release to pin the exact edition it quoted.

## Schema

| Column | Type | Empty in sample |
|---|---|---|
| `kit_slug` | string | 0.0% |
| `method_version` | string | 0.0% |
| `total` | number | 0.0% |
| `normalised` | number | 0.0% |
| `coverage` | number | 0.0% |
| `maintenance` | number | 43.6% |
| `completeness` | number | 0.0% |
| `transparency` | number | 0.0% |
| `documentation` | number | 0.0% |
| `support` | number | 0.0% |
| `breakdown` | object | 0.0% |
| `computed_at` | string | 0.0% |

## Cite it

```
Compound Labs (2026). KitGrade: the component scores behind every kit grade. KitGrade, https://kitgrade.thecompound.tech. Cut of 2026-10-01. Creative Commons Attribution 4.0 International (CC BY 4.0). https://github.com/kyisaiah47/compound-datasets/tree/main/kitgrade-scores
```

```bibtex
@dataset{compound_kitgrade_scores_2026,
  title     = {KitGrade: the component scores behind every kit grade},
  author    = {{Compound Labs}},
  year      = {2026},
  publisher = {Compound Labs},
  url       = {https://github.com/kyisaiah47/compound-datasets/tree/main/kitgrade-scores},
  note      = {Cut of 2026-10-01. Measured by KitGrade, https://kitgrade.thecompound.tech},
  license   = {CC-BY-4.0}
}
```

The whole collection has the DOI 10.5281/zenodo.22844096 at [https://doi.org/10.5281/zenodo.22844096](https://doi.org/10.5281/zenodo.22844096). The DOI resolves
to the newest Zenodo version. Cite 10.5281/zenodo.22844097 to pin the exact deposit for this cut.

Attribution is the licence condition. Attribution is the only condition. Cite the publisher, the
product that measured the figure, and the cut date when you quote a figure. You do not need to
ask for anything else.
