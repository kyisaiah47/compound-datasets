# ToolDrift: OpenRouter model usage rankings, captured daily

One row per model per ranking window per capture: its rank, the tokens and requests behind that rank, and its share of the window. The series shows which models the market actually routes work to, day by day.

| | |
|---|---|
| Rows in this cut | 44,369 |
| One row is | one model in one ranking window on one capture day |
| Cut | 2026-09-04 |
| Refreshed | Monthly, on the first of the month |
| Measured by | [ToolDrift](https://tooldrift.thecompound.tech) |
| Method | [https://toolproof.thecompound.tech/methodology](https://toolproof.thecompound.tech/methodology) |
| Licence | [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/) |
| Publisher | [Compound Labs](https://thecompound.tech) |

## How it is measured

The public OpenRouter rankings are fetched on a schedule and stored as captured, one row per model per window. Nothing is smoothed, interpolated or revised after capture.

## What a citer needs to know

- A gap in `captured_on` is a day the capture did not run. It is left as a gap rather than filled, because an interpolated row in a ranking series is indistinguishable from a measured one once it is cited.
- `time_window` is OpenRouter's own window label, passed through unchanged.

## Files

| File | Format | Size |
|---|---|---|
| `tooldrift-model-rankings-2026-09-04.csv` | CSV | 4.9 MB |
| `tooldrift-model-rankings-2026-09-04.json` | JSON | 11.0 MB |

Every cut is also a [GitHub release](https://github.com/kyisaiah47/compound-datasets/releases) with the same files attached, so a
citation can pin the exact edition it quoted.

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
Compound Labs (2026). ToolDrift: OpenRouter model usage rankings, captured daily. ToolDrift, https://tooldrift.thecompound.tech. Cut of 2026-09-04. Creative Commons Attribution 4.0 International (CC BY 4.0). https://github.com/kyisaiah47/compound-datasets/tree/main/tooldrift-model-rankings
```

```bibtex
@dataset{compound_tooldrift_model_rankings_2026,
  title     = {ToolDrift: OpenRouter model usage rankings, captured daily},
  author    = {{Compound Labs}},
  year      = {2026},
  publisher = {Compound Labs},
  url       = {https://github.com/kyisaiah47/compound-datasets/tree/main/tooldrift-model-rankings},
  note      = {Cut of 2026-09-04. Measured by ToolDrift, https://tooldrift.thecompound.tech},
  license   = {CC-BY-4.0}
}
```

Attribution is the licence condition, and it is the only one. Quote a figure with the publisher,
the product that measured it and the cut date, and there is nothing else to ask.
