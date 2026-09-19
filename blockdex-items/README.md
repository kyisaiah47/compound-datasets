# BlockDex: every component, block and theme inside those registries

One row per item in every crawled registry: its type, its dependencies, the files it ships, its install command, and the dates it was first and last seen.

| | |
|---|---|
| Rows in this cut | 88,612 |
| One row is | one registry item |
| Cut | 2026-09-04 |
| Refreshed | Monthly, on the first of the month |
| Measured by | [BlockDex](https://blockdex.thecompound.tech) |
| Method | [https://toolproof.thecompound.tech/methodology](https://toolproof.thecompound.tech/methodology) |
| Licence | [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/) |
| Publisher | [Compound Labs](https://thecompound.tech) |
| Also on | [Hugging Face](https://huggingface.co/datasets/kyisaiah47/blockdex-items) · [Zenodo](https://zenodo.org/records/22844097) |

## How it is measured

Each registry is crawled and its items are read individually from the registry JSON, so an item that disappears between crawls is recorded as removed on a date rather than forgotten. Dependencies are the ones the item declares, not the ones a reader infers from its name.

## What a citer needs to know

- A `status` of `removed` with a `removed_on` date is an item that was there and is not any more. Those rows are the reason this dataset is more than a snapshot of a directory.
- The registry a row belongs to is `registry_slug`, which joins the registries dataset.

## Files

| File | Format | Size |
|---|---|---|
| `blockdex-items-2026-09-04.csv.gz` | CSV, gzipped | 5.4 MB |
| `blockdex-items-2026-09-04.json.gz` | JSON, gzipped | 6.0 MB |

Every cut is also a [GitHub release](https://github.com/kyisaiah47/compound-datasets/releases) with the same files attached, so a
citation can pin the exact edition it quoted.

## Schema

| Column | Type | Empty in sample |
|---|---|---|
| `id` | string | 0.0% |
| `registry_slug` | string | 0.0% |
| `name` | string | 0.0% |
| `title` | string | 42.0% |
| `description` | string | 39.0% |
| `type` | string | 0.0% |
| `kind` | string | 0.0% |
| `categories` | array | 0.0% |
| `dependencies` | array | 0.0% |
| `registry_dependencies` | array | 0.0% |
| `dev_dependencies` | array | 0.0% |
| `file_paths` | array | 0.0% |
| `file_count` | number | 0.0% |
| `primary_file` | string | 1.2% |
| `has_tailwind_config` | boolean | 0.0% |
| `has_css_vars` | boolean | 0.0% |
| `item_url` | string | 0.0% |
| `install_cmd` | string | 0.0% |
| `docs_url` | string | 63.9% |
| `preview_url` | string | 65.8% |
| `preview_embeddable` | boolean | 65.8% |
| `access` | string | 0.0% |
| `status` | string | 0.0% |
| `first_seen` | string | 0.0% |
| `last_seen` | string | 0.0% |
| `removed_on` | string | 75.8% |
| `registry_stars` | number | 57.0% |

## Cite it

```
Compound Labs (2026). BlockDex: every component, block and theme inside those registries. BlockDex, https://blockdex.thecompound.tech. Cut of 2026-09-04. Creative Commons Attribution 4.0 International (CC BY 4.0). https://github.com/kyisaiah47/compound-datasets/tree/main/blockdex-items
```

```bibtex
@dataset{compound_blockdex_items_2026,
  title     = {BlockDex: every component, block and theme inside those registries},
  author    = {{Compound Labs}},
  year      = {2026},
  publisher = {Compound Labs},
  url       = {https://github.com/kyisaiah47/compound-datasets/tree/main/blockdex-items},
  note      = {Cut of 2026-09-04. Measured by BlockDex, https://blockdex.thecompound.tech},
  license   = {CC-BY-4.0}
}
```

The whole collection has a DOI, 10.5281/zenodo.22844096, at [https://doi.org/10.5281/zenodo.22844096](https://doi.org/10.5281/zenodo.22844096). It resolves to the
newest Zenodo version. To pin the exact deposit this cut belongs to, cite 10.5281/zenodo.22844097 instead.

Attribution is the licence condition, and it is the only one. Quote a figure with the publisher,
the product that measured it and the cut date, and there is nothing else to ask.
