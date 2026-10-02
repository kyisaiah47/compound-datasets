# BlockDex: every component, block and theme inside those registries

Each row represents one item in every crawled registry. The row records the item's type, dependencies, shipped files, install command, and first-seen and last-seen dates.

| | |
|---|---|
| Rows in this cut | 116,147 |
| One row is | one registry item |
| Cut | 2026-10-01 |
| Refreshed | Monthly, on the first of the month |
| Measured by | [BlockDex](https://blockdex.thecompound.tech) |
| Method | [https://toolproof.thecompound.tech/methodology](https://toolproof.thecompound.tech/methodology) |
| Licence | [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/) |
| Publisher | [Compound Labs](https://thecompound.tech) |
| Also on | [Hugging Face](https://huggingface.co/datasets/kyisaiah47/blockdex-items) · [Kaggle](https://www.kaggle.com/datasets/kyisaiah47/blockdex-items) · [Zenodo](https://zenodo.org/records/22844097) |

## How it is measured

The crawl reads each registry item individually from the registry JSON. When an item disappears between crawls, the dataset records it as removed on a date. The dataset does not forget that item. The dataset records the dependencies declared by the item. It does not infer dependencies from the item's name.

## What a citer needs to know

- An item with a `status` of `removed` and a `removed_on` date was present before and is no longer present. Those rows make this dataset more than a snapshot of a directory.
- The `registry_slug` field identifies the registry that owns a row. That field joins the registries dataset.

## Files

| File | Format | Size |
|---|---|---|
| `blockdex-items-2026-10-01.csv.gz` | CSV, gzipped | 7.1 MB |
| `blockdex-items-2026-10-01.json.gz` | JSON, gzipped | 7.8 MB |

Every cut is also published as a [GitHub release](https://github.com/kyisaiah47/compound-datasets/releases). The release attaches
the same files. A citation can use the release to pin the exact edition it quoted.

## Schema

| Column | Type | Empty in sample |
|---|---|---|
| `id` | string | 0.0% |
| `registry_slug` | string | 0.0% |
| `name` | string | 0.0% |
| `title` | string | 41.5% |
| `description` | string | 37.8% |
| `type` | string | 0.0% |
| `kind` | string | 0.0% |
| `categories` | array | 0.0% |
| `dependencies` | array | 0.0% |
| `registry_dependencies` | array | 0.0% |
| `dev_dependencies` | array | 0.0% |
| `file_paths` | array | 0.0% |
| `file_count` | number | 0.0% |
| `primary_file` | string | 1.1% |
| `has_tailwind_config` | boolean | 0.0% |
| `has_css_vars` | boolean | 0.0% |
| `item_url` | string | 0.0% |
| `install_cmd` | string | 0.0% |
| `docs_url` | string | 63.9% |
| `preview_url` | string | 65.9% |
| `preview_embeddable` | boolean | 65.9% |
| `access` | string | 0.0% |
| `status` | string | 0.0% |
| `first_seen` | string | 0.0% |
| `last_seen` | string | 0.0% |
| `removed_on` | string | 75.8% |
| `registry_stars` | number | 54.7% |

## Cite it

```
Compound Labs (2026). BlockDex: every component, block and theme inside those registries. BlockDex, https://blockdex.thecompound.tech. Cut of 2026-10-01. Creative Commons Attribution 4.0 International (CC BY 4.0). https://github.com/kyisaiah47/compound-datasets/tree/main/blockdex-items
```

```bibtex
@dataset{compound_blockdex_items_2026,
  title     = {BlockDex: every component, block and theme inside those registries},
  author    = {{Compound Labs}},
  year      = {2026},
  publisher = {Compound Labs},
  url       = {https://github.com/kyisaiah47/compound-datasets/tree/main/blockdex-items},
  note      = {Cut of 2026-10-01. Measured by BlockDex, https://blockdex.thecompound.tech},
  license   = {CC-BY-4.0}
}
```

The whole collection has the DOI 10.5281/zenodo.22844096 at [https://doi.org/10.5281/zenodo.22844096](https://doi.org/10.5281/zenodo.22844096). The DOI resolves
to the newest Zenodo version. Cite 10.5281/zenodo.22844097 to pin the exact deposit for this cut.

Attribution is the licence condition. Attribution is the only condition. Cite the publisher, the
product that measured the figure, and the cut date when you quote a figure. You do not need to
ask for anything else.
