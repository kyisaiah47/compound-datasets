# ShipWall: launched products and the badge check behind each one

One row per product that has launched on the board: what it is, where it lives, what it was built with, and whether the embed badge was actually found on the site it points at.

| | |
|---|---|
| Rows in this cut | 43 |
| One row is | one launched product |
| Cut | 2026-09-04 |
| Refreshed | Monthly, on the first of the month |
| Measured by | [ShipWall](https://shipwall.thecompound.tech) |
| Method | [https://toolproof.thecompound.tech/methodology](https://toolproof.thecompound.tech/methodology) |
| Licence | [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/) |
| Publisher | [Compound Labs](https://thecompound.tech) |

## How it is measured

The badge check fetches the product's own site and looks for the badge it claims to carry, storing the HTTP status and the time it was last found. A claim about a live site is checked against the live site.

## What a citer needs to know

- Only launched rows publish. Pending and scheduled submissions are not public and are not exported.
- The submitter's email address, IP hash, edit token, moderation notes and payment references are never exported. `maker_handle` is a public handle and is the only identity field in the file.

## Files

| File | Format | Size |
|---|---|---|
| `shipwall-products-2026-09-04.csv` | CSV | 0.02 MB |
| `shipwall-products-2026-09-04.json` | JSON | 0.04 MB |

Every cut is also a [GitHub release](https://github.com/kyisaiah47/compound-datasets/releases) with the same files attached, so a
citation can pin the exact edition it quoted.

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
| `category_slug` | string | 62.8% |
| `built_with` | array | 0.0% |
| `human_edited` | string | 0.0% |
| `pricing` | string | 37.2% |
| `maker_handle` | string | 0.0% |
| `launch_date` | string | 0.0% |
| `launch_slot` | number | 0.0% |
| `launched_at` | string | 0.0% |
| `featured` | boolean | 0.0% |
| `upvote_count` | number | 0.0% |
| `badge_found_at` | string | 97.7% |
| `badge_last_checked_at` | string | 0.0% |
| `badge_http_status` | number | 0.0% |

## Cite it

```
Compound Labs (2026). ShipWall: launched products and the badge check behind each one. ShipWall, https://shipwall.thecompound.tech. Cut of 2026-09-04. Creative Commons Attribution 4.0 International (CC BY 4.0). https://github.com/kyisaiah47/compound-datasets/tree/main/shipwall-products
```

```bibtex
@dataset{compound_shipwall_products_2026,
  title     = {ShipWall: launched products and the badge check behind each one},
  author    = {{Compound Labs}},
  year      = {2026},
  publisher = {Compound Labs},
  url       = {https://github.com/kyisaiah47/compound-datasets/tree/main/shipwall-products},
  note      = {Cut of 2026-09-04. Measured by ShipWall, https://shipwall.thecompound.tech},
  license   = {CC-BY-4.0}
}
```

Attribution is the licence condition, and it is the only one. Quote a figure with the publisher,
the product that measured it and the cut date, and there is nothing else to ask.
