# ToolDrift: OpenRouter app usage rankings, captured daily

Each row records one app for one ranking window and one capture, with the ToolDrift tool mapping when one exists. The data uses the same series as the model rankings and reads it from the consumer side.

| | |
|---|---|
| Rows in this cut | 1,181 |
| One row is | one app in one ranking window on one capture day |
| Cut | 2026-10-01 |
| Refreshed | Monthly, on the first of the month |
| Measured by | [ToolDrift](https://tooldrift.thecompound.tech) |
| Method | [https://toolproof.thecompound.tech/methodology](https://toolproof.thecompound.tech/methodology) |
| Licence | [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/) |
| Publisher | [Compound Labs](https://thecompound.tech) |
| Also on | [Hugging Face](https://huggingface.co/datasets/kyisaiah47/tooldrift-app-rankings) · [Kaggle](https://www.kaggle.com/datasets/kyisaiah47/tooldrift-app-rankings) · [Zenodo](https://zenodo.org/records/22844097) |

## How it is measured

The dataset fetches the public OpenRouter app rankings on a schedule and stores them as captured. It fills `tool_slug` only when an app maps to a tool that ToolDrift already tracks; otherwise, it leaves the field empty rather than guessing.

## What a citer needs to know

- The `categories` field contains OpenRouter's own classification of the app, passed through unchanged.

## Files

| File | Format | Size |
|---|---|---|
| `tooldrift-app-rankings-2026-10-01.csv` | CSV | 0.10 MB |
| `tooldrift-app-rankings-2026-10-01.json` | JSON | 0.24 MB |

Every cut is also published as a [GitHub release](https://github.com/kyisaiah47/compound-datasets/releases). The release attaches
the same files. A citation can use the release to pin the exact edition it quoted.

## Schema

| Column | Type | Empty in sample |
|---|---|---|
| `captured_on` | string | 0.0% |
| `time_window` | string | 0.0% |
| `app_slug` | string | 0.0% |
| `app_title` | string | 0.0% |
| `tool_slug` | string | 80.0% |
| `categories` | array | 0.0% |
| `rank` | number | 0.0% |
| `total_tokens` | number | 0.0% |
| `total_requests` | number | 0.0% |

## Cite it

```
Compound Labs (2026). ToolDrift: OpenRouter app usage rankings, captured daily. ToolDrift, https://tooldrift.thecompound.tech. Cut of 2026-10-01. Creative Commons Attribution 4.0 International (CC BY 4.0). https://github.com/kyisaiah47/compound-datasets/tree/main/tooldrift-app-rankings
```

```bibtex
@dataset{compound_tooldrift_app_rankings_2026,
  title     = {ToolDrift: OpenRouter app usage rankings, captured daily},
  author    = {{Compound Labs}},
  year      = {2026},
  publisher = {Compound Labs},
  url       = {https://github.com/kyisaiah47/compound-datasets/tree/main/tooldrift-app-rankings},
  note      = {Cut of 2026-10-01. Measured by ToolDrift, https://tooldrift.thecompound.tech},
  license   = {CC-BY-4.0}
}
```

The whole collection has the DOI 10.5281/zenodo.22844096 at [https://doi.org/10.5281/zenodo.22844096](https://doi.org/10.5281/zenodo.22844096). The DOI resolves
to the newest Zenodo version. Cite 10.5281/zenodo.22844097 to pin the exact deposit for this cut.

Attribution is the licence condition. Attribution is the only condition. Cite the publisher, the
product that measured the figure, and the cut date when you quote a figure. You do not need to
ask for anything else.
