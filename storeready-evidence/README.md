# StoreReady: the cited evidence behind every verdict

One row per piece of evidence: which builder it is about, which claim it supports, the source it came from with its title and date, the quoted passage, and the HTTP status that source last returned.

| | |
|---|---|
| Rows in this cut | 47 |
| One row is | one piece of evidence |
| Cut | 2026-09-04 |
| Refreshed | Monthly, on the first of the month |
| Measured by | [StoreReady](https://storeready.thecompound.tech) |
| Method | [https://toolproof.thecompound.tech/methodology](https://toolproof.thecompound.tech/methodology) |
| Licence | [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/) |
| Publisher | [Compound Labs](https://thecompound.tech) |

## How it is measured

Evidence is a policy clause, a rejection thread or a shipped binary, recorded with the URL it was read from. Every source URL is re-checked and its status stored, so a citation resting on a page that has gone can be found rather than assumed live.

## What a citer needs to know

- `link_status` is the last HTTP status the source returned. A non-200 does not remove the evidence; it publishes the fact that the source moved.
- `quote` is the passage as it appeared. It is the primary source for the claim beside it.

## Files

| File | Format | Size |
|---|---|---|
| `storeready-evidence-2026-09-04.csv` | CSV | 0.01 MB |
| `storeready-evidence-2026-09-04.json` | JSON | 0.02 MB |

Every cut is also a [GitHub release](https://github.com/kyisaiah47/compound-datasets/releases) with the same files attached, so a
citation can pin the exact edition it quoted.

## Schema

| Column | Type | Empty in sample |
|---|---|---|
| `builder_slug` | string | 0.0% |
| `supports` | string | 0.0% |
| `claim` | string | 0.0% |
| `kind` | string | 0.0% |
| `source_url` | string | 0.0% |
| `source_title` | string | 0.0% |
| `source_date` | string | 0.0% |
| `quote` | string | 38.3% |
| `link_status` | null | 100.0% |
| `link_checked_at` | null | 100.0% |

## Cite it

```
Compound Labs (2026). StoreReady: the cited evidence behind every verdict. StoreReady, https://storeready.thecompound.tech. Cut of 2026-09-04. Creative Commons Attribution 4.0 International (CC BY 4.0). https://github.com/kyisaiah47/compound-datasets/tree/main/storeready-evidence
```

```bibtex
@dataset{compound_storeready_evidence_2026,
  title     = {StoreReady: the cited evidence behind every verdict},
  author    = {{Compound Labs}},
  year      = {2026},
  publisher = {Compound Labs},
  url       = {https://github.com/kyisaiah47/compound-datasets/tree/main/storeready-evidence},
  note      = {Cut of 2026-09-04. Measured by StoreReady, https://storeready.thecompound.tech},
  license   = {CC-BY-4.0}
}
```

Attribution is the licence condition, and it is the only one. Quote a figure with the publisher,
the product that measured it and the cut date, and there is nothing else to ask.
