# RuleStack: the agent config formats and what each one supports

Each row records one agent config format, including AGENTS.md, CLAUDE.md and the rest. The row states which tools read the format and whether it supports frontmatter, globs, imports, nesting, multiple files and user scope. The row also stores the specification URL used for each verification.

| | |
|---|---|
| Rows in this cut | 8 |
| One row is | one config format |
| Cut | 2026-10-01 |
| Refreshed | Monthly, on the first of the month |
| Measured by | [RuleStack](https://rulestack.thecompound.tech) |
| Method | [https://toolproof.thecompound.tech/methodology](https://toolproof.thecompound.tech/methodology) |
| Licence | [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/) |
| Publisher | [Compound Labs](https://thecompound.tech) |
| Also on | [Hugging Face](https://huggingface.co/datasets/kyisaiah47/rulestack-formats) · [Kaggle](https://www.kaggle.com/datasets/kyisaiah47/rulestack-formats) · [Zenodo](https://zenodo.org/records/22844097) |

## How it is measured

The format's published specification or documentation supplies every support flag. The dataset stores the source URL and verification date beside each flag. The dataset does not infer support from general knowledge of a format.

## What a citer needs to know

- `verified_at` records the date when the support matrix was last checked against the specification. A format can change if its specification moves after that date.

## Files

| File | Format | Size |
|---|---|---|
| `rulestack-formats-2026-10-01.csv` | CSV | 0.01 MB |
| `rulestack-formats-2026-10-01.json` | JSON | 0.01 MB |

Every cut is also published as a [GitHub release](https://github.com/kyisaiah47/compound-datasets/releases). The release attaches
the same files. A citation can use the release to pin the exact edition it quoted.

## Schema

| Column | Type | Empty in sample |
|---|---|---|
| `slug` | string | 0.0% |
| `name` | string | 0.0% |
| `filename` | string | 0.0% |
| `artifact_kind` | string | 0.0% |
| `vendor` | string | 12.5% |
| `status` | string | 0.0% |
| `spec_url` | string | 87.5% |
| `docs_url` | string | 0.0% |
| `first_released` | string | 0.0% |
| `tools` | array | 0.0% |
| `cross_tool` | boolean | 0.0% |
| `supports_frontmatter` | boolean | 0.0% |
| `supports_globs` | boolean | 0.0% |
| `supports_imports` | boolean | 0.0% |
| `supports_nested` | boolean | 0.0% |
| `supports_multifile` | boolean | 0.0% |
| `supports_user_scope` | boolean | 0.0% |
| `activation` | string | 0.0% |
| `size_limit` | string | 87.5% |
| `summary` | string | 0.0% |
| `strengths` | array | 0.0% |
| `weaknesses` | array | 0.0% |
| `verified_at` | string | 0.0% |
| `sort_order` | number | 0.0% |

## Cite it

```
Compound Labs (2026). RuleStack: the agent config formats and what each one supports. RuleStack, https://rulestack.thecompound.tech. Cut of 2026-10-01. Creative Commons Attribution 4.0 International (CC BY 4.0). https://github.com/kyisaiah47/compound-datasets/tree/main/rulestack-formats
```

```bibtex
@dataset{compound_rulestack_formats_2026,
  title     = {RuleStack: the agent config formats and what each one supports},
  author    = {{Compound Labs}},
  year      = {2026},
  publisher = {Compound Labs},
  url       = {https://github.com/kyisaiah47/compound-datasets/tree/main/rulestack-formats},
  note      = {Cut of 2026-10-01. Measured by RuleStack, https://rulestack.thecompound.tech},
  license   = {CC-BY-4.0}
}
```

The whole collection has the DOI 10.5281/zenodo.22844096 at [https://doi.org/10.5281/zenodo.22844096](https://doi.org/10.5281/zenodo.22844096). The DOI resolves
to the newest Zenodo version. Cite 10.5281/zenodo.22844097 to pin the exact deposit for this cut.

Attribution is the licence condition. Attribution is the only condition. Cite the publisher, the
product that measured the figure, and the cut date when you quote a figure. You do not need to
ask for anything else.
