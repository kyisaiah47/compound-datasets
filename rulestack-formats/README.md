# RuleStack: the agent config formats and what each one supports

One row per agent config format (AGENTS.md, CLAUDE.md and the rest): which tools read it, whether it supports frontmatter, globs, imports, nesting, multiple files and user scope, and the specification URL each of those was verified against.

| | |
|---|---|
| Rows in this cut | 8 |
| One row is | one config format |
| Cut | 2026-09-04 |
| Refreshed | Monthly, on the first of the month |
| Measured by | [RuleStack](https://rulestack.thecompound.tech) |
| Method | [https://toolproof.thecompound.tech/methodology](https://toolproof.thecompound.tech/methodology) |
| Licence | [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/) |
| Publisher | [Compound Labs](https://thecompound.tech) |

## How it is measured

Every support flag is read from the format's own published specification or documentation, with the URL stored beside it and a verification date. Nothing is inferred from what a format is generally understood to do.

## What a citer needs to know

- `verified_at` is the date the support matrix was last confirmed against the spec. A format whose spec has moved since then may have changed.

## Files

| File | Format | Size |
|---|---|---|
| `rulestack-formats-2026-09-04.csv` | CSV | 0.01 MB |
| `rulestack-formats-2026-09-04.json` | JSON | 0.01 MB |

Every cut is also a [GitHub release](https://github.com/kyisaiah47/compound-datasets/releases) with the same files attached, so a
citation can pin the exact edition it quoted.

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
Compound Labs (2026). RuleStack: the agent config formats and what each one supports. RuleStack, https://rulestack.thecompound.tech. Cut of 2026-09-04. Creative Commons Attribution 4.0 International (CC BY 4.0). https://github.com/kyisaiah47/compound-datasets/tree/main/rulestack-formats
```

```bibtex
@dataset{compound_rulestack_formats_2026,
  title     = {RuleStack: the agent config formats and what each one supports},
  author    = {{Compound Labs}},
  year      = {2026},
  publisher = {Compound Labs},
  url       = {https://github.com/kyisaiah47/compound-datasets/tree/main/rulestack-formats},
  note      = {Cut of 2026-09-04. Measured by RuleStack, https://rulestack.thecompound.tech},
  license   = {CC-BY-4.0}
}
```

Attribution is the licence condition, and it is the only one. Quote a figure with the publisher,
the product that measured it and the cut date, and there is nothing else to ask.
