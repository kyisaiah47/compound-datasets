# StackTab watches prices for developer services.

Each row records one developer service whose pricing StackTab reads. The row stores the service category, homepage and pricing page that supplied the plan figures.

| | |
|---|---|
| Rows in this cut | 29 |
| One row is | one service |
| Cut | 2026-10-01 |
| Refreshed | Monthly, on the first of the month |
| Measured by | [StackTab](https://stacktab.thecompound.tech) |
| Method | [https://toolproof.thecompound.tech/methodology](https://toolproof.thecompound.tech/methodology) |
| Licence | [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/) |
| Publisher | [Compound Labs](https://thecompound.tech) |
| Also on | [Hugging Face](https://huggingface.co/datasets/kyisaiah47/stacktab-services) · [Kaggle](https://www.kaggle.com/datasets/kyisaiah47/stacktab-services) · [Zenodo](https://zenodo.org/records/22844097) |

## How it is measured

StackTab fetches each pricing page and reads plan figures from the page that states them. StackTab does not use comparison sites or press releases as sources.

## What a citer needs to know

- `attrs` stores service-level facts that do not belong to individual plans as JSON.

## Files

| File | Format | Size |
|---|---|---|
| `stacktab-services-2026-10-01.csv` | CSV | 0.01 MB |
| `stacktab-services-2026-10-01.json` | JSON | 0.01 MB |

Every cut is also published as a [GitHub release](https://github.com/kyisaiah47/compound-datasets/releases). The release attaches
the same files. A citation can use the release to pin the exact edition it quoted.

## Schema

| Column | Type | Empty in sample |
|---|---|---|
| `slug` | string | 0.0% |
| `name` | string | 0.0% |
| `category` | string | 0.0% |
| `tagline` | string | 0.0% |
| `homepage_url` | string | 0.0% |
| `pricing_url` | string | 0.0% |
| `attrs` | object | 0.0% |
| `rank` | number | 0.0% |

## Cite it

```
Compound Labs (2026). StackTab: the developer services under price watch. StackTab, https://stacktab.thecompound.tech. Cut of 2026-10-01. Creative Commons Attribution 4.0 International (CC BY 4.0). https://github.com/kyisaiah47/compound-datasets/tree/main/stacktab-services
```

```bibtex
@dataset{compound_stacktab_services_2026,
  title     = {StackTab: the developer services under price watch},
  author    = {{Compound Labs}},
  year      = {2026},
  publisher = {Compound Labs},
  url       = {https://github.com/kyisaiah47/compound-datasets/tree/main/stacktab-services},
  note      = {Cut of 2026-10-01. Measured by StackTab, https://stacktab.thecompound.tech},
  license   = {CC-BY-4.0}
}
```

The whole collection has the DOI 10.5281/zenodo.22844096 at [https://doi.org/10.5281/zenodo.22844096](https://doi.org/10.5281/zenodo.22844096). The DOI resolves
to the newest Zenodo version. Cite 10.5281/zenodo.22844097 to pin the exact deposit for this cut.

Attribution is the licence condition. Attribution is the only condition. Cite the publisher, the
product that measured the figure, and the cut date when you quote a figure. You do not need to
ask for anything else.
