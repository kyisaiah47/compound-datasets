# Toolproof: the nine indexes and what each one currently measures

Each row records one index under the Toolproof masthead, including what it measures, the method behind it, the public endpoint that supplies its figures, and the headline figure that endpoint returned at the cut.

| | |
|---|---|
| Rows in this cut | 9 |
| One row is | one index |
| Cut | 2026-10-01 |
| Refreshed | Monthly, on the first of the month |
| Measured by | [Toolproof](https://toolproof.thecompound.tech) |
| Method | [https://toolproof.thecompound.tech/methodology](https://toolproof.thecompound.tech/methodology) |
| Licence | [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/) |
| Publisher | [Compound Labs](https://thecompound.tech) |
| Also on | [Hugging Face](https://huggingface.co/datasets/kyisaiah47/toolproof-indexes) · [Kaggle](https://www.kaggle.com/datasets/kyisaiah47/toolproof-indexes) · [Zenodo](https://zenodo.org/records/22844097) |

## How it is measured

Read from https://toolproof.thecompound.tech/api/index.json, which builds itself by calling each index's own public stats endpoint at request time. An index that did not answer is kept in the file with ok=false and the reason it gave, because a consumer has to be able to tell a missing index from an index that measured nothing.

## What a citer needs to know

- The headline figures can change between cuts. A citation of one figure should include the cut date, which appears in the filename and in `as_of`.
- The `as_of` field records the run that produced the figure. The `fetched_at` field records when this export read it. These are different dates, and both matter.

## Files

| File | Format | Size |
|---|---|---|
| `toolproof-indexes-2026-10-01.csv` | CSV | 0.00 MB |
| `toolproof-indexes-2026-10-01.json` | JSON | 0.01 MB |

Every cut is also published as a [GitHub release](https://github.com/kyisaiah47/compound-datasets/releases). The release attaches
the same files. A citation can use the release to pin the exact edition it quoted.

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
Compound Labs (2026). Toolproof: the nine indexes and what each one currently measures. Toolproof, https://toolproof.thecompound.tech. Cut of 2026-10-01. Creative Commons Attribution 4.0 International (CC BY 4.0). https://github.com/kyisaiah47/compound-datasets/tree/main/toolproof-indexes
```

```bibtex
@dataset{compound_toolproof_indexes_2026,
  title     = {Toolproof: the nine indexes and what each one currently measures},
  author    = {{Compound Labs}},
  year      = {2026},
  publisher = {Compound Labs},
  url       = {https://github.com/kyisaiah47/compound-datasets/tree/main/toolproof-indexes},
  note      = {Cut of 2026-10-01. Measured by Toolproof, https://toolproof.thecompound.tech},
  license   = {CC-BY-4.0}
}
```

The whole collection has the DOI 10.5281/zenodo.22844096 at [https://doi.org/10.5281/zenodo.22844096](https://doi.org/10.5281/zenodo.22844096). The DOI resolves
to the newest Zenodo version. Cite 10.5281/zenodo.22844097 to pin the exact deposit for this cut.

Attribution is the licence condition. Attribution is the only condition. Cite the publisher, the
product that measured the figure, and the cut date when you quote a figure. You do not need to
ask for anything else.
