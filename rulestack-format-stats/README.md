# RuleStack: how much each config format is actually used, day by day

One row per format per day: how many repositories carry it, how many config files were read, how long those files are at the median and the 90th percentile, and what share of them carry runnable commands or code.

| | |
|---|---|
| Rows in this cut | 168 |
| One row is | one format on one day |
| Cut | 2026-09-04 |
| Refreshed | Monthly, on the first of the month |
| Measured by | [RuleStack](https://rulestack.thecompound.tech) |
| Method | [https://toolproof.thecompound.tech/methodology](https://toolproof.thecompound.tech/methodology) |
| Licence | [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/) |
| Publisher | [Compound Labs](https://thecompound.tech) |

## How it is measured

Config files are read out of public repositories and measured. The format shares are computed from the files found, never from a survey of what people say they use.

## What a citer needs to know

- `share_pct` is a share of the files read on that day, so it moves with the crawl as well as with the ecosystem.
- A day missing from the series is a day the crawl did not run.

## Files

| File | Format | Size |
|---|---|---|
| `rulestack-format-stats-2026-09-04.csv` | CSV | 0.01 MB |
| `rulestack-format-stats-2026-09-04.json` | JSON | 0.04 MB |

Every cut is also a [GitHub release](https://github.com/kyisaiah47/compound-datasets/releases) with the same files attached, so a
citation can pin the exact edition it quoted.

## Schema

| Column | Type | Empty in sample |
|---|---|---|
| `day` | string | 0.0% |
| `format` | string | 0.0% |
| `repo_count` | number | 0.0% |
| `config_count` | number | 0.0% |
| `median_words` | number | 0.0% |
| `p90_words` | number | 0.0% |
| `median_stars` | number | 0.0% |
| `total_stars` | number | 0.0% |
| `share_pct` | number | 0.0% |
| `with_commands_pct` | number | 0.0% |
| `with_code_pct` | number | 0.0% |
| `median_quality` | number | 0.0% |

## Cite it

```
Compound Labs (2026). RuleStack: how much each config format is actually used, day by day. RuleStack, https://rulestack.thecompound.tech. Cut of 2026-09-04. Creative Commons Attribution 4.0 International (CC BY 4.0). https://github.com/kyisaiah47/compound-datasets/tree/main/rulestack-format-stats
```

```bibtex
@dataset{compound_rulestack_format_stats_2026,
  title     = {RuleStack: how much each config format is actually used, day by day},
  author    = {{Compound Labs}},
  year      = {2026},
  publisher = {Compound Labs},
  url       = {https://github.com/kyisaiah47/compound-datasets/tree/main/rulestack-format-stats},
  note      = {Cut of 2026-09-04. Measured by RuleStack, https://rulestack.thecompound.tech},
  license   = {CC-BY-4.0}
}
```

Attribution is the licence condition, and it is the only one. Quote a figure with the publisher,
the product that measured it and the cut date, and there is nothing else to ask.
