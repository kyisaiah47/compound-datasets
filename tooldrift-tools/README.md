# ToolDrift: the AI coding tools under watch

One row per AI coding tool watched nightly: its layer in the stack, its vendor, its licence and pricing model, its default model, and the GitHub maintenance signals beside the OpenRouter usage rank.

| | |
|---|---|
| Rows in this cut | 36 |
| One row is | one tool |
| Cut | 2026-09-04 |
| Refreshed | Monthly, on the first of the month |
| Measured by | [ToolDrift](https://tooldrift.thecompound.tech) |
| Method | [https://toolproof.thecompound.tech/methodology](https://toolproof.thecompound.tech/methodology) |
| Licence | [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/) |
| Publisher | [Compound Labs](https://thecompound.tech) |
| Also on | [Hugging Face](https://huggingface.co/datasets/kyisaiah47/tooldrift-tools) · [Kaggle](https://www.kaggle.com/datasets/kyisaiah47/tooldrift-tools) · [Zenodo](https://zenodo.org/records/22844097) |

## How it is measured

Vendor changelogs, pricing pages and store rankings are fetched on a schedule and diffed against the previous capture. A price is recorded from the page that states it, and a page that has moved is followed and the redirect published rather than silently followed.

## What a citer needs to know

- `status` carries a tool that has been acquired, renamed or shut down. `acquired_by` and `status_changed_on` say which and when.
- `or_rank` and `or_tokens_week` come from OpenRouter's public rankings and are absent for a tool that does not route through it.

## Files

| File | Format | Size |
|---|---|---|
| `tooldrift-tools-2026-09-04.csv` | CSV | 0.02 MB |
| `tooldrift-tools-2026-09-04.json` | JSON | 0.03 MB |

Every cut is also a [GitHub release](https://github.com/kyisaiah47/compound-datasets/releases) with the same files attached, so a
citation can pin the exact edition it quoted.

## Schema

| Column | Type | Empty in sample |
|---|---|---|
| `slug` | string | 0.0% |
| `name` | string | 0.0% |
| `layer` | string | 0.0% |
| `vendor` | string | 0.0% |
| `homepage` | string | 0.0% |
| `pricing_url` | string | 8.3% |
| `docs_url` | string | 0.0% |
| `github_full_name` | string | 66.7% |
| `openrouter_app_slug` | string | 83.3% |
| `status` | string | 0.0% |
| `status_note` | string | 80.6% |
| `status_changed_on` | string | 83.3% |
| `acquired_by` | string | 91.7% |
| `default_model` | string | 77.8% |
| `default_model_note` | string | 50.0% |
| `byo_key` | boolean | 0.0% |
| `open_source` | boolean | 0.0% |
| `license` | string | 69.4% |
| `pricing_model` | string | 0.0% |
| `description` | string | 0.0% |
| `tags` | array | 0.0% |
| `gh_stars` | number | 66.7% |
| `gh_forks` | number | 66.7% |
| `gh_archived` | boolean | 66.7% |
| `gh_pushed_at` | string | 66.7% |
| `gh_days_since_push` | number | 66.7% |
| `gh_maintenance` | number | 66.7% |
| `gh_dead` | boolean | 66.7% |
| `gh_star_delta_30d` | number | 66.7% |
| `or_rank` | number | 88.9% |
| `or_tokens_week` | number | 88.9% |
| `last_pricing_check` | string | 8.3% |
| `last_change_at` | string | 33.3% |
| `curated_on` | string | 0.0% |

## Cite it

```
Compound Labs (2026). ToolDrift: the AI coding tools under watch. ToolDrift, https://tooldrift.thecompound.tech. Cut of 2026-09-04. Creative Commons Attribution 4.0 International (CC BY 4.0). https://github.com/kyisaiah47/compound-datasets/tree/main/tooldrift-tools
```

```bibtex
@dataset{compound_tooldrift_tools_2026,
  title     = {ToolDrift: the AI coding tools under watch},
  author    = {{Compound Labs}},
  year      = {2026},
  publisher = {Compound Labs},
  url       = {https://github.com/kyisaiah47/compound-datasets/tree/main/tooldrift-tools},
  note      = {Cut of 2026-09-04. Measured by ToolDrift, https://tooldrift.thecompound.tech},
  license   = {CC-BY-4.0}
}
```

The whole collection has a DOI, 10.5281/zenodo.22844096, at [https://doi.org/10.5281/zenodo.22844096](https://doi.org/10.5281/zenodo.22844096). It resolves to the
newest Zenodo version. To pin the exact deposit this cut belongs to, cite 10.5281/zenodo.22844097 instead.

Attribution is the licence condition, and it is the only one. Quote a figure with the publisher,
the product that measured it and the cut date, and there is nothing else to ask.
