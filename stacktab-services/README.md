# StackTab: the developer services under price watch

One row per developer service whose pricing StackTab reads: its category, its homepage and the pricing page the plan figures were read from.

| | |
|---|---|
| Rows in this cut | 29 |
| One row is | one service |
| Cut | 2026-09-04 |
| Refreshed | Monthly, on the first of the month |
| Measured by | [StackTab](https://stacktab.thecompound.tech) |
| Method | [https://toolproof.thecompound.tech/methodology](https://toolproof.thecompound.tech/methodology) |
| Licence | [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/) |
| Publisher | [Compound Labs](https://thecompound.tech) |

## How it is measured

The pricing page is fetched and the plan figures are read from the page that states them. Nothing is taken from a comparison site or a press release.

## What a citer needs to know

- `attrs` is JSON carrying the service-level facts that are not plan-level.

## Files

| File | Format | Size |
|---|---|---|
| `stacktab-services-2026-09-04.csv` | CSV | 0.01 MB |
| `stacktab-services-2026-09-04.json` | JSON | 0.01 MB |

Every cut is also a [GitHub release](https://github.com/kyisaiah47/compound-datasets/releases) with the same files attached, so a
citation can pin the exact edition it quoted.

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
Compound Labs (2026). StackTab: the developer services under price watch. StackTab, https://stacktab.thecompound.tech. Cut of 2026-09-04. Creative Commons Attribution 4.0 International (CC BY 4.0). https://github.com/kyisaiah47/compound-datasets/tree/main/stacktab-services
```

```bibtex
@dataset{compound_stacktab_services_2026,
  title     = {StackTab: the developer services under price watch},
  author    = {{Compound Labs}},
  year      = {2026},
  publisher = {Compound Labs},
  url       = {https://github.com/kyisaiah47/compound-datasets/tree/main/stacktab-services},
  note      = {Cut of 2026-09-04. Measured by StackTab, https://stacktab.thecompound.tech},
  license   = {CC-BY-4.0}
}
```

Attribution is the licence condition, and it is the only one. Quote a figure with the publisher,
the product that measured it and the cut date, and there is nothing else to ask.
