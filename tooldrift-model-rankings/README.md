# ToolDrift: OpenRouter model usage rankings, captured daily

Each row records one model for one ranking window and one capture, including its rank, the tokens and requests behind that rank, and its share of the window. The series records which models the market routes work to each day.

| | |
|---|---|
| Rows in this cut | 84,461 |
| One row is | one model in one ranking window on one capture day |
| Cut | 2026-10-01 |
| Refreshed | Monthly, on the first of the month |
| Measured by | [ToolDrift](https://tooldrift.thecompound.tech) |
| Method | [https://toolproof.thecompound.tech/methodology](https://toolproof.thecompound.tech/methodology) |
| Licence | [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/) |
| Publisher | [Compound Labs](https://thecompound.tech) |
| Also on | [Hugging Face](https://huggingface.co/datasets/kyisaiah47/tooldrift-model-rankings) · [Kaggle](https://www.kaggle.com/datasets/kyisaiah47/tooldrift-model-rankings) · [Zenodo](https://zenodo.org/records/22844097) |

## How it is measured

The dataset fetches the public OpenRouter rankings on a schedule and stores them as captured, with one row per model per window. It does not smooth, interpolate or revise the data after capture.

## What a citer needs to know

- A gap in `captured_on` marks a day when the capture did not run. The dataset leaves that day as a gap rather than filling it, because a cited interpolated row is indistinguishable from a measured row.
- The `time_window` field contains OpenRouter's own window label, passed through unchanged.

## Files

| File | Format | Size |
|---|---|---|
| `tooldrift-model-rankings-2026-10-01.csv` | CSV | 9.4 MB |
| `tooldrift-model-rankings-2026-10-01.json` | JSON | 20.9 MB |

Every cut is also published as a [GitHub release](https://github.com/kyisaiah47/compound-datasets/releases). The release attaches
the same files. A citation can use the release to pin the exact edition it quoted.

## Schema

| Column | Type | Empty in sample |
|---|---|---|
| `captured_on` | string | 0.0% |
| `time_window` | string | 0.0% |
| `model_id` | string | 0.0% |
| `permaslug` | string | 0.0% |
| `rank` | number | 0.0% |
| `total_tokens` | number | 0.0% |
| `prompt_tokens` | number | 0.0% |
| `completion_tokens` | number | 0.0% |
| `requests` | number | 0.0% |
| `share_pct` | number | 0.0% |

## Cite it

```
Compound Labs (2026). ToolDrift: OpenRouter model usage rankings, captured daily. ToolDrift, https://tooldrift.thecompound.tech. Cut of 2026-10-01. Creative Commons Attribution 4.0 International (CC BY 4.0). https://github.com/kyisaiah47/compound-datasets/tree/main/tooldrift-model-rankings
```

```bibtex
@dataset{compound_tooldrift_model_rankings_2026,
  title     = {ToolDrift: OpenRouter model usage rankings, captured daily},
  author    = {{Compound Labs}},
  year      = {2026},
  publisher = {Compound Labs},
  url       = {https://github.com/kyisaiah47/compound-datasets/tree/main/tooldrift-model-rankings},
  note      = {Cut of 2026-10-01. Measured by ToolDrift, https://tooldrift.thecompound.tech},
  license   = {CC-BY-4.0}
}
```

The whole collection has the DOI 10.5281/zenodo.22844096 at [https://doi.org/10.5281/zenodo.22844096](https://doi.org/10.5281/zenodo.22844096). The DOI resolves
to the newest Zenodo version. Cite 10.5281/zenodo.22844097 to pin the exact deposit for this cut.

Attribution is the licence condition. Attribution is the only condition. Cite the publisher, the
product that measured the figure, and the cut date when you quote a figure. You do not need to
ask for anything else.
