# ToolDrift: the AI coding tools under watch

Each row records one AI coding tool watched nightly, including its layer in the stack, vendor, licence and pricing model, default model, and the GitHub maintenance signals beside the OpenRouter usage rank.

| | |
|---|---|
| Rows in this cut | 36 |
| One row is | one tool |
| Cut | 2026-10-01 |
| Refreshed | Monthly, on the first of the month |
| Measured by | [ToolDrift](https://tooldrift.thecompound.tech) |
| Method | [https://toolproof.thecompound.tech/methodology](https://toolproof.thecompound.tech/methodology) |
| Licence | [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/) |
| Publisher | [Compound Labs](https://thecompound.tech) |
| Also on | [Hugging Face](https://huggingface.co/datasets/kyisaiah47/tooldrift-tools) · [Kaggle](https://www.kaggle.com/datasets/kyisaiah47/tooldrift-tools) · [Zenodo](https://zenodo.org/records/22844097) |

## How it is measured

The dataset fetches vendor changelogs, pricing pages and store rankings on a schedule and compares them with the previous capture. It records a price from the page that states it. When a page has moved, it follows the page and publishes the redirect instead of silently following it.

## What a citer needs to know

- The `status` field records when a tool has been acquired, renamed or shut down. The `acquired_by` and `status_changed_on` fields record which change occurred and when.
- The `or_rank` and `or_tokens_week` fields come from OpenRouter's public rankings. They are absent for a tool that does not route through OpenRouter.

## Files

| File | Format | Size |
|---|---|---|
| `tooldrift-tools-2026-10-01.csv` | CSV | 0.02 MB |
| `tooldrift-tools-2026-10-01.json` | JSON | 0.04 MB |

Every cut is also published as a [GitHub release](https://github.com/kyisaiah47/compound-datasets/releases). The release attaches
the same files. A citation can use the release to pin the exact edition it quoted.

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
| `last_change_at` | string | 30.6% |
| `curated_on` | string | 0.0% |

## Cite it

```
Compound Labs (2026). ToolDrift: the AI coding tools under watch. ToolDrift, https://tooldrift.thecompound.tech. Cut of 2026-10-01. Creative Commons Attribution 4.0 International (CC BY 4.0). https://github.com/kyisaiah47/compound-datasets/tree/main/tooldrift-tools
```

```bibtex
@dataset{compound_tooldrift_tools_2026,
  title     = {ToolDrift: the AI coding tools under watch},
  author    = {{Compound Labs}},
  year      = {2026},
  publisher = {Compound Labs},
  url       = {https://github.com/kyisaiah47/compound-datasets/tree/main/tooldrift-tools},
  note      = {Cut of 2026-10-01. Measured by ToolDrift, https://tooldrift.thecompound.tech},
  license   = {CC-BY-4.0}
}
```

The whole collection has the DOI 10.5281/zenodo.22844096 at [https://doi.org/10.5281/zenodo.22844096](https://doi.org/10.5281/zenodo.22844096). The DOI resolves
to the newest Zenodo version. Cite 10.5281/zenodo.22844097 to pin the exact deposit for this cut.

Attribution is the licence condition. Attribution is the only condition. Cite the publisher, the
product that measured the figure, and the cut date when you quote a figure. You do not need to
ask for anything else.
