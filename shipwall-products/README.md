# ShipWall records launched products and the badge check for each product.

Each row records one product launched on the board. The row states what the product is, where it lives, what it was built with, and whether the product site contains the embed badge it claims to carry.

| | |
|---|---|
| Rows in this cut | 104 |
| One row is | one launched product |
| Cut | 2026-10-01 |
| Refreshed | Monthly, on the first of the month |
| Measured by | [ShipWall](https://shipwall.thecompound.tech) |
| Method | [https://toolproof.thecompound.tech/methodology](https://toolproof.thecompound.tech/methodology) |
| Licence | [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/) |
| Publisher | [Compound Labs](https://thecompound.tech) |
| Also on | [Hugging Face](https://huggingface.co/datasets/kyisaiah47/shipwall-products) · [Kaggle](https://www.kaggle.com/datasets/kyisaiah47/shipwall-products) · [Zenodo](https://zenodo.org/records/22844097) |

## How it is measured

The badge check fetches each product's site and searches for the badge it claims to carry. The dataset stores the site's HTTP status and the last time the badge was found. The check compares every live-site claim with the live site.

## What a citer needs to know

- The dataset publishes launched rows only. The export excludes pending and scheduled submissions.
- The export never includes the submitter's email address, IP hash, edit token, moderation notes or payment references. `maker_handle` is a public handle and the file's only identity field.

## Files

| File | Format | Size |
|---|---|---|
| `shipwall-products-2026-10-01.csv` | CSV | 0.05 MB |
| `shipwall-products-2026-10-01.json` | JSON | 0.09 MB |

Every cut is also published as a [GitHub release](https://github.com/kyisaiah47/compound-datasets/releases). The release attaches
the same files. A citation can use the release to pin the exact edition it quoted.

## Schema

| Column | Type | Empty in sample |
|---|---|---|
| `slug` | string | 0.0% |
| `name` | string | 0.0% |
| `tagline` | string | 0.0% |
| `description` | string | 0.0% |
| `website_url` | string | 0.0% |
| `website_host` | string | 0.0% |
| `repo_url` | null | 100.0% |
| `demo_url` | null | 100.0% |
| `video_url` | null | 100.0% |
| `logo_url` | string | 0.0% |
| `category_slug` | string | 68.3% |
| `built_with` | array | 0.0% |
| `human_edited` | string | 0.0% |
| `pricing` | string | 25.0% |
| `maker_handle` | string | 0.0% |
| `launch_date` | string | 0.0% |
| `launch_slot` | number | 0.0% |
| `launched_at` | string | 0.0% |
| `featured` | boolean | 0.0% |
| `upvote_count` | number | 0.0% |
| `badge_found_at` | string | 99.0% |
| `badge_last_checked_at` | string | 0.0% |
| `badge_http_status` | number | 0.0% |

## Cite it

```
Compound Labs (2026). ShipWall: launched products and the badge check behind each one. ShipWall, https://shipwall.thecompound.tech. Cut of 2026-10-01. Creative Commons Attribution 4.0 International (CC BY 4.0). https://github.com/kyisaiah47/compound-datasets/tree/main/shipwall-products
```

```bibtex
@dataset{compound_shipwall_products_2026,
  title     = {ShipWall: launched products and the badge check behind each one},
  author    = {{Compound Labs}},
  year      = {2026},
  publisher = {Compound Labs},
  url       = {https://github.com/kyisaiah47/compound-datasets/tree/main/shipwall-products},
  note      = {Cut of 2026-10-01. Measured by ShipWall, https://shipwall.thecompound.tech},
  license   = {CC-BY-4.0}
}
```

The whole collection has the DOI 10.5281/zenodo.22844096 at [https://doi.org/10.5281/zenodo.22844096](https://doi.org/10.5281/zenodo.22844096). The DOI resolves
to the newest Zenodo version. Cite 10.5281/zenodo.22844097 to pin the exact deposit for this cut.

Attribution is the licence condition. Attribution is the only condition. Cite the publisher, the
product that measured the figure, and the cut date when you quote a figure. You do not need to
ask for anything else.
