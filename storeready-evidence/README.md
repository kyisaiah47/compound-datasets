# StoreReady records the cited evidence behind every verdict.

Each row records one piece of evidence. The row identifies the builder, the claim it supports, and the source title and date. The row stores the quoted passage and the HTTP status that the source last returned.

| | |
|---|---|
| Rows in this cut | 47 |
| One row is | one piece of evidence |
| Cut | 2026-10-01 |
| Refreshed | Monthly, on the first of the month |
| Measured by | [StoreReady](https://storeready.thecompound.tech) |
| Method | [https://toolproof.thecompound.tech/methodology](https://toolproof.thecompound.tech/methodology) |
| Licence | [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/) |
| Publisher | [Compound Labs](https://thecompound.tech) |
| Also on | [Hugging Face](https://huggingface.co/datasets/kyisaiah47/storeready-evidence) · [Kaggle](https://www.kaggle.com/datasets/kyisaiah47/storeready-evidence) · [Zenodo](https://zenodo.org/records/22844097) |

## How it is measured

The dataset records each evidence item as a policy clause, rejection thread or shipped binary. It stores the URL where the evidence was read. It re-checks every source URL and stores its status. A reader can find citations whose pages are gone instead of assuming that those pages remain live.

## What a citer needs to know

- The `link_status` field records the last HTTP status returned by the source. A non-200 status does not remove the evidence; it records that the source moved.
- The `quote` field contains the passage as it appeared. It is the primary source for the claim beside it.

## Files

| File | Format | Size |
|---|---|---|
| `storeready-evidence-2026-10-01.csv` | CSV | 0.02 MB |
| `storeready-evidence-2026-10-01.json` | JSON | 0.02 MB |

Every cut is also published as a [GitHub release](https://github.com/kyisaiah47/compound-datasets/releases). The release attaches
the same files. A citation can use the release to pin the exact edition it quoted.

## Schema

| Column | Type | Empty in sample |
|---|---|---|
| `builder_slug` | string | 0.0% |
| `supports` | string | 0.0% |
| `claim` | string | 0.0% |
| `kind` | string | 0.0% |
| `source_url` | string | 0.0% |
| `source_title` | string | 0.0% |
| `source_date` | string | 0.0% |
| `quote` | string | 38.3% |
| `link_status` | number | 0.0% |
| `link_checked_at` | string | 0.0% |

## Cite it

```
Compound Labs (2026). StoreReady: the cited evidence behind every verdict. StoreReady, https://storeready.thecompound.tech. Cut of 2026-10-01. Creative Commons Attribution 4.0 International (CC BY 4.0). https://github.com/kyisaiah47/compound-datasets/tree/main/storeready-evidence
```

```bibtex
@dataset{compound_storeready_evidence_2026,
  title     = {StoreReady: the cited evidence behind every verdict},
  author    = {{Compound Labs}},
  year      = {2026},
  publisher = {Compound Labs},
  url       = {https://github.com/kyisaiah47/compound-datasets/tree/main/storeready-evidence},
  note      = {Cut of 2026-10-01. Measured by StoreReady, https://storeready.thecompound.tech},
  license   = {CC-BY-4.0}
}
```

The whole collection has the DOI 10.5281/zenodo.22844096 at [https://doi.org/10.5281/zenodo.22844096](https://doi.org/10.5281/zenodo.22844096). The DOI resolves
to the newest Zenodo version. Cite 10.5281/zenodo.22844097 to pin the exact deposit for this cut.

Attribution is the licence condition. Attribution is the only condition. Cite the publisher, the
product that measured the figure, and the cut date when you quote a figure. You do not need to
ask for anything else.
