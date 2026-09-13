# StoreReady: AI app builders and whether their output ships

One row per AI app builder: what it actually outputs, whether the source leaves the platform, whether it submits to the store for you, what it costs, and the review verdict on whether the App Store accepts what it produces.

| | |
|---|---|
| Rows in this cut | 14 |
| One row is | one app builder |
| Cut | 2026-09-04 |
| Refreshed | Monthly, on the first of the month |
| Measured by | [StoreReady](https://storeready.thecompound.tech) |
| Method | [https://toolproof.thecompound.tech/methodology](https://toolproof.thecompound.tech/methodology) |
| Licence | [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/) |
| Publisher | [Compound Labs](https://thecompound.tech) |

## How it is measured

Every verdict is attached to numbered evidence in the companion evidence dataset. A builder nobody has evidence for is published as unknown rather than given the benefit of the doubt.

## What a citer needs to know

- `risk_guidelines` names the App Review guideline clauses the output is exposed to, by number.
- A verdict is about the output, not about the company. It moves when the output changes.

## Files

| File | Format | Size |
|---|---|---|
| `storeready-builders-2026-09-04.csv` | CSV | 0.02 MB |
| `storeready-builders-2026-09-04.json` | JSON | 0.02 MB |

Every cut is also a [GitHub release](https://github.com/kyisaiah47/compound-datasets/releases) with the same files attached, so a
citation can pin the exact edition it quoted.

## Schema

| Column | Type | Empty in sample |
|---|---|---|
| `slug` | string | 0.0% |
| `name` | string | 0.0% |
| `tagline` | string | 0.0% |
| `url` | string | 0.0% |
| `category` | string | 0.0% |
| `output_type` | string | 0.0% |
| `output_detail` | string | 0.0% |
| `exports_source` | string | 0.0% |
| `exports_source_detail` | string | 0.0% |
| `submits_for_you` | string | 0.0% |
| `price_free` | boolean | 14.3% |
| `price_from_usd` | number | 7.1% |
| `price_note` | string | 0.0% |
| `review_verdict` | string | 0.0% |
| `review_summary` | string | 0.0% |
| `risk_guidelines` | array | 0.0% |
| `rank` | number | 0.0% |
| `updated_at` | string | 0.0% |

## Cite it

```
Compound Labs (2026). StoreReady: AI app builders and whether their output ships. StoreReady, https://storeready.thecompound.tech. Cut of 2026-09-04. Creative Commons Attribution 4.0 International (CC BY 4.0). https://github.com/kyisaiah47/compound-datasets/tree/main/storeready-builders
```

```bibtex
@dataset{compound_storeready_builders_2026,
  title     = {StoreReady: AI app builders and whether their output ships},
  author    = {{Compound Labs}},
  year      = {2026},
  publisher = {Compound Labs},
  url       = {https://github.com/kyisaiah47/compound-datasets/tree/main/storeready-builders},
  note      = {Cut of 2026-09-04. Measured by StoreReady, https://storeready.thecompound.tech},
  license   = {CC-BY-4.0}
}
```

Attribution is the licence condition, and it is the only one. Quote a figure with the publisher,
the product that measured it and the cut date, and there is nothing else to ask.
