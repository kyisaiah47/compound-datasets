# Toolproof: the nine indexes and what each one currently measures

One row per index under the Toolproof masthead: what it measures, the method behind it, the public endpoint its figures come from, and the headline figure that endpoint returned at the moment of the cut.

| | |
|---|---|
| Rows in this cut | 9 |
| One row is | one index |
| Cut | 2026-09-04 |
| Refreshed | Monthly, on the first of the month |
| Measured by | [Toolproof](https://toolproof.thecompound.tech) |
| Method | [https://toolproof.thecompound.tech/methodology](https://toolproof.thecompound.tech/methodology) |
| Licence | [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/) |
| Publisher | [Compound Labs](https://thecompound.tech) |
| Also on | [Hugging Face](https://huggingface.co/datasets/kyisaiah47/toolproof-indexes) · [Zenodo](https://zenodo.org/records/22844097) |

## How it is measured

Read from https://toolproof.thecompound.tech/api/index.json, which builds itself by calling each index's own public stats endpoint at request time. An index that did not answer is kept in the file with ok=false and the reason it gave, because a consumer has to be able to tell a missing index from an index that measured nothing.

## What a citer needs to know

- The headline figures move between cuts. A citation of one of them should carry the cut date, which is in the filename and in `as_of`.
- `as_of` is the run that produced the figure. `fetched_at` is when this export read it. Those are different dates and both matter.

## Files

| File | Format | Size |
|---|---|---|
| `toolproof-indexes-2026-09-04.csv` | CSV | 0.00 MB |
| `toolproof-indexes-2026-09-04.json` | JSON | 0.01 MB |

Every cut is also a [GitHub release](https://github.com/kyisaiah47/compound-datasets/releases) with the same files attached, so a
citation can pin the exact edition it quoted.

## Schema

| Column | Type | Empty in sample |
|---|---|---|
| `slug` | string | 0.0% |
| `name` | string | 0.0% |
| `url` | string | 0.0% |
| `answering` | boolean | 0.0% |
| `measures` | string | 0.0% |
| `method` | string | 0.0% |
| `source_endpoint` | string | 0.0% |
| `headline_label` | string | 0.0% |
| `headline_value` | number | 0.0% |
| `detail_1` | string | 0.0% |
| `detail_2` | string | 0.0% |
| `detail_3` | string | 11.1% |
| `as_of` | string | 0.0% |
| `stale` | boolean | 44.4% |
| `error` | null | 100.0% |
| `fetched_at` | string | 0.0% |

## Cite it

```
Compound Labs (2026). Toolproof: the nine indexes and what each one currently measures. Toolproof, https://toolproof.thecompound.tech. Cut of 2026-09-04. Creative Commons Attribution 4.0 International (CC BY 4.0). https://github.com/kyisaiah47/compound-datasets/tree/main/toolproof-indexes
```

```bibtex
@dataset{compound_toolproof_indexes_2026,
  title     = {Toolproof: the nine indexes and what each one currently measures},
  author    = {{Compound Labs}},
  year      = {2026},
  publisher = {Compound Labs},
  url       = {https://github.com/kyisaiah47/compound-datasets/tree/main/toolproof-indexes},
  note      = {Cut of 2026-09-04. Measured by Toolproof, https://toolproof.thecompound.tech},
  license   = {CC-BY-4.0}
}
```

The whole collection has a DOI, 10.5281/zenodo.22844096, at [https://doi.org/10.5281/zenodo.22844096](https://doi.org/10.5281/zenodo.22844096). It resolves to the
newest Zenodo version. To pin the exact deposit this cut belongs to, cite 10.5281/zenodo.22844097 instead.

Attribution is the licence condition, and it is the only one. Quote a figure with the publisher,
the product that measured it and the cut date, and there is nothing else to ask.
