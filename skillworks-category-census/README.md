# SkillWorks: Claude Code artefacts by category and kind

A structural census of the public Claude Code artefact ecosystem, aggregated to one row per category and artefact kind: how many listings the index holds, how many distinct repositories they came from, how many do not parse into something Claude Code could load, and the mean of the 0-100 score.

| | |
|---|---|
| Rows in this cut | 74 |
| One row is | one category and artefact kind |
| Cut | 2026-09-10 |
| Refreshed | Monthly, on the first of the month |
| Measured by | [SkillWorks](https://skillworks.thecompound.tech) |
| Method | [https://toolproof.thecompound.tech/methodology](https://toolproof.thecompound.tech/methodology) |
| Licence | [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/) |
| Publisher | [Compound Labs](https://thecompound.tech) |
| Also on | [Hugging Face](https://huggingface.co/datasets/kyisaiah47/skillworks-category-census) · [Kaggle](https://www.kaggle.com/datasets/kyisaiah47/skillworks-category-census) · [Zenodo](https://zenodo.org/records/22844097) |

## How it is measured

Each listing's files are read from the repository that publishes them and scored on four weighted components. A listing that does not parse into a loadable artefact is counted as broken rather than dropped from the denominator, which is the number that decides whether a failure rate means anything.

## What a citer needs to know

- This is an aggregate. The underlying listing rows carry author handles at a scale nobody consented to being redistributed, so the row level is not published in any form.
- The ecosystem is heavily forked and vendored, so the same file is counted once per repository carrying it. The failure RATE is the citable figure; the population count is not a claim about how many distinct artefacts exist.

The aggregate is a database view, and this is its definition:

```sql
select coalesce(category, 'uncategorised') as category, kind, count(*) as listings,
       count(distinct repo_full_name) as repositories,
       count(*) filter (where works is false) as listings_that_do_not_load,
       count(*) filter (where works is true)  as listings_that_load,
       round(avg(score)::numeric, 2) as mean_score,
       count(*) filter (where official) as official,
       count(*) filter (where archived) as archived_repository,
       count(*) filter (where license is not null) as with_a_license,
       sum(stars) as total_repository_stars
from sw_listings group by 1, 2
```

## Files

| File | Format | Size |
|---|---|---|
| `skillworks-category-census-2026-09-10.csv` | CSV | 0.00 MB |
| `skillworks-category-census-2026-09-10.json` | JSON | 0.02 MB |

Every cut is also a [GitHub release](https://github.com/kyisaiah47/compound-datasets/releases) with the same files attached, so a
citation can pin the exact edition it quoted.

## Schema

| Column | Type | Empty in sample |
|---|---|---|
| `category` | string | 0.0% |
| `kind` | string | 0.0% |
| `listings` | number | 0.0% |
| `repositories` | number | 0.0% |
| `listings_that_do_not_load` | number | 0.0% |
| `listings_that_load` | number | 0.0% |
| `mean_score` | number | 0.0% |
| `official` | number | 0.0% |
| `archived_repository` | number | 0.0% |
| `with_a_license` | number | 0.0% |
| `total_repository_stars` | number | 0.0% |

## Cite it

```
Compound Labs (2026). SkillWorks: Claude Code artefacts by category and kind. SkillWorks, https://skillworks.thecompound.tech. Cut of 2026-09-10. Creative Commons Attribution 4.0 International (CC BY 4.0). https://github.com/kyisaiah47/compound-datasets/tree/main/skillworks-category-census
```

```bibtex
@dataset{compound_skillworks_category_census_2026,
  title     = {SkillWorks: Claude Code artefacts by category and kind},
  author    = {{Compound Labs}},
  year      = {2026},
  publisher = {Compound Labs},
  url       = {https://github.com/kyisaiah47/compound-datasets/tree/main/skillworks-category-census},
  note      = {Cut of 2026-09-10. Measured by SkillWorks, https://skillworks.thecompound.tech},
  license   = {CC-BY-4.0}
}
```

The whole collection has a DOI, 10.5281/zenodo.22844096, at [https://doi.org/10.5281/zenodo.22844096](https://doi.org/10.5281/zenodo.22844096). It resolves to the
newest Zenodo version. To pin the exact deposit this cut belongs to, cite 10.5281/zenodo.22844097 instead.

Attribution is the licence condition, and it is the only one. Quote a figure with the publisher,
the product that measured it and the cut date, and there is nothing else to ask.
