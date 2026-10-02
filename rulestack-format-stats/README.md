# RuleStack: how much each config format is actually used, day by day

Each row represents one format on one day. The row records how many repositories carry the format, how many config files were read, the median file length, the 90th-percentile file length, and the share of files carrying runnable commands or code.

| | |
|---|---|
| Rows in this cut | 336 |
| One row is | one format on one day |
| Cut | 2026-10-01 |
| Refreshed | Monthly, on the first of the month |
| Measured by | [RuleStack](https://rulestack.thecompound.tech) |
| Method | [https://toolproof.thecompound.tech/methodology](https://toolproof.thecompound.tech/methodology) |
| Licence | [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/) |
| Publisher | [Compound Labs](https://thecompound.tech) |
| Also on | [Hugging Face](https://huggingface.co/datasets/kyisaiah47/rulestack-format-stats) · [Kaggle](https://www.kaggle.com/datasets/kyisaiah47/rulestack-format-stats) · [Zenodo](https://zenodo.org/records/22844097) |

## How it is measured

The crawl reads config files from public repositories and measures them. The format shares come from the files found. The shares do not come from a survey of what people say they use.

## What a citer needs to know

- `share_pct` is the share of files read on that day. The crawl changes that share as the ecosystem changes and as the crawl changes.
- A missing day in the series means that the crawl did not run.

## Files

| File | Format | Size |
|---|---|---|
| `rulestack-format-stats-2026-10-01.csv` | CSV | 0.02 MB |
| `rulestack-format-stats-2026-10-01.json` | JSON | 0.08 MB |

Every cut is also published as a [GitHub release](https://github.com/kyisaiah47/compound-datasets/releases). The release attaches
the same files. A citation can use the release to pin the exact edition it quoted.

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
Compound Labs (2026). RuleStack: how much each config format is actually used, day by day. RuleStack, https://rulestack.thecompound.tech. Cut of 2026-10-01. Creative Commons Attribution 4.0 International (CC BY 4.0). https://github.com/kyisaiah47/compound-datasets/tree/main/rulestack-format-stats
```

```bibtex
@dataset{compound_rulestack_format_stats_2026,
  title     = {RuleStack: how much each config format is actually used, day by day},
  author    = {{Compound Labs}},
  year      = {2026},
  publisher = {Compound Labs},
  url       = {https://github.com/kyisaiah47/compound-datasets/tree/main/rulestack-format-stats},
  note      = {Cut of 2026-10-01. Measured by RuleStack, https://rulestack.thecompound.tech},
  license   = {CC-BY-4.0}
}
```

The whole collection has the DOI 10.5281/zenodo.22844096 at [https://doi.org/10.5281/zenodo.22844096](https://doi.org/10.5281/zenodo.22844096). The DOI resolves
to the newest Zenodo version. Cite 10.5281/zenodo.22844097 to pin the exact deposit for this cut.

Attribution is the licence condition. Attribution is the only condition. Cite the publisher, the
product that measured the figure, and the cut date when you quote a figure. You do not need to
ask for anything else.
