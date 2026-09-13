# StackTab: every plan, its price, and the page the price was read from

One row per published plan: its base monthly price in USD, what the plan includes, the restrictions attached to it, and the URL the figure was read from with the date it was last checked.

| | |
|---|---|
| Rows in this cut | 64 |
| One row is | one plan |
| Cut | 2026-09-04 |
| Refreshed | Monthly, on the first of the month |
| Measured by | [StackTab](https://stacktab.thecompound.tech) |
| Method | [https://toolproof.thecompound.tech/methodology](https://toolproof.thecompound.tech/methodology) |
| Licence | [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/) |
| Publisher | [Compound Labs](https://thecompound.tech) |

## How it is measured

Each plan is re-checked on a schedule against its own pricing page. `price_status` says whether a number was readable at all, so a plan priced by sales contact is published as unpriced rather than as zero.

## What a citer needs to know

- `verified_at` is the last time the figure was confirmed against the page. `last_check_note` carries what happened when a check could not confirm it.
- `probes` are the strings the check looked for on the page. They are published so a disputed price can be re-derived.

## Files

| File | Format | Size |
|---|---|---|
| `stacktab-plans-2026-09-04.csv` | CSV | 0.02 MB |
| `stacktab-plans-2026-09-04.json` | JSON | 0.03 MB |

Every cut is also a [GitHub release](https://github.com/kyisaiah47/compound-datasets/releases) with the same files attached, so a
citation can pin the exact edition it quoted.

## Schema

| Column | Type | Empty in sample |
|---|---|---|
| `service_slug` | string | 0.0% |
| `plan_slug` | string | 0.0% |
| `name` | string | 0.0% |
| `rank` | number | 0.0% |
| `base_monthly_usd` | number | 0.0% |
| `price_status` | string | 0.0% |
| `included` | object | 0.0% |
| `restrictions` | object | 0.0% |
| `notes` | string | 7.8% |
| `source_url` | string | 0.0% |
| `probes` | array | 0.0% |
| `check_status` | string | 0.0% |
| `verified_at` | string | 0.0% |
| `last_checked_at` | string | 0.0% |
| `last_check_note` | string | 98.4% |

## Cite it

```
Compound Labs (2026). StackTab: every plan, its price, and the page the price was read from. StackTab, https://stacktab.thecompound.tech. Cut of 2026-09-04. Creative Commons Attribution 4.0 International (CC BY 4.0). https://github.com/kyisaiah47/compound-datasets/tree/main/stacktab-plans
```

```bibtex
@dataset{compound_stacktab_plans_2026,
  title     = {StackTab: every plan, its price, and the page the price was read from},
  author    = {{Compound Labs}},
  year      = {2026},
  publisher = {Compound Labs},
  url       = {https://github.com/kyisaiah47/compound-datasets/tree/main/stacktab-plans},
  note      = {Cut of 2026-09-04. Measured by StackTab, https://stacktab.thecompound.tech},
  license   = {CC-BY-4.0}
}
```

Attribution is the licence condition, and it is the only one. Quote a figure with the publisher,
the product that measured it and the cut date, and there is nothing else to ask.
