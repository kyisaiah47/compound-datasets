# BlockDex: every public shadcn registry

One row per public shadcn component registry: where it is served from, the repository behind it, its licence, how many items it holds and how many of those are free, and whether it is still there.

| | |
|---|---|
| Rows in this cut | 1,123 |
| One row is | one registry |
| Cut | 2026-09-04 |
| Refreshed | Monthly, on the first of the month |
| Measured by | [BlockDex](https://blockdex.thecompound.tech) |
| Method | [https://toolproof.thecompound.tech/methodology](https://toolproof.thecompound.tech/methodology) |
| Licence | [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/) |
| Publisher | [Compound Labs](https://thecompound.tech) |
| Also on | [Hugging Face](https://huggingface.co/datasets/kyisaiah47/blockdex-registries) · [Kaggle](https://www.kaggle.com/datasets/kyisaiah47/blockdex-registries) · [Zenodo](https://zenodo.org/records/22844097) |

## How it is measured

Each registry is crawled on a schedule and its item list read from the registry JSON it serves rather than from its marketing page. A registry that stops answering is marked gone with the date, not deleted.

## What a citer needs to know

- `status` is `active` or `gone`. A gone registry keeps its row so a link that used to work can be explained.
- `access` is `free`, `paid`, `mixed` or `unknown`. Unknown means the registry does not state it in a form the crawl could read, and is not a guess.

## Files

| File | Format | Size |
|---|---|---|
| `blockdex-registries-2026-09-04.csv` | CSV | 0.38 MB |
| `blockdex-registries-2026-09-04.json` | JSON | 0.80 MB |

Every cut is also a [GitHub release](https://github.com/kyisaiah47/compound-datasets/releases) with the same files attached, so a
citation can pin the exact edition it quoted.

## Schema

| Column | Type | Empty in sample |
|---|---|---|
| `slug` | string | 0.0% |
| `name` | string | 0.0% |
| `homepage` | string | 2.8% |
| `registry_url` | string | 0.0% |
| `registry_source` | string | 0.0% |
| `repo_full_name` | string | 3.2% |
| `repo_url` | string | 3.2% |
| `description` | string | 49.8% |
| `license` | string | 56.4% |
| `gh_stars` | number | 26.8% |
| `gh_forks` | number | 26.8% |
| `gh_pushed_at` | string | 26.8% |
| `gh_days_since_push` | number | 26.8% |
| `maintenance` | number | 26.8% |
| `item_count` | number | 0.0% |
| `free_item_count` | number | 0.0% |
| `paid_item_count` | number | 0.0% |
| `access` | string | 0.0% |
| `docs_url` | string | 74.9% |
| `preview_embeddable` | boolean | 83.2% |
| `status` | string | 0.0% |
| `first_seen` | string | 0.0% |
| `last_seen` | string | 0.0% |
| `last_crawled_at` | string | 0.0% |
| `gone_on` | string | 86.9% |
| `notes` | string | 99.8% |

## Cite it

```
Compound Labs (2026). BlockDex: every public shadcn registry. BlockDex, https://blockdex.thecompound.tech. Cut of 2026-09-04. Creative Commons Attribution 4.0 International (CC BY 4.0). https://github.com/kyisaiah47/compound-datasets/tree/main/blockdex-registries
```

```bibtex
@dataset{compound_blockdex_registries_2026,
  title     = {BlockDex: every public shadcn registry},
  author    = {{Compound Labs}},
  year      = {2026},
  publisher = {Compound Labs},
  url       = {https://github.com/kyisaiah47/compound-datasets/tree/main/blockdex-registries},
  note      = {Cut of 2026-09-04. Measured by BlockDex, https://blockdex.thecompound.tech},
  license   = {CC-BY-4.0}
}
```

The whole collection has a DOI, 10.5281/zenodo.22844096, at [https://doi.org/10.5281/zenodo.22844096](https://doi.org/10.5281/zenodo.22844096). It resolves to the
newest Zenodo version. To pin the exact deposit this cut belongs to, cite 10.5281/zenodo.22844097 instead.

Attribution is the licence condition, and it is the only one. Quote a figure with the publisher,
the product that measured it and the cut date, and there is nothing else to ask.
