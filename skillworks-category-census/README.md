# SkillWorks records Claude Code artefacts by category and kind.

The census aggregates the public Claude Code artefact ecosystem into one row per category and artefact kind. Each row states how many listings the index holds, how many distinct repositories they came from, how many listings do not parse into an artefact Claude Code could load, and the mean score from 0 to 100.

| | |
|---|---|
| Rows in this cut | 74 |
| One row is | one category and artefact kind |
| Cut | 2026-10-01 |
| Refreshed | Monthly, on the first of the month |
| Measured by | [SkillWorks](https://skillworks.thecompound.tech) |
| Method | [https://toolproof.thecompound.tech/methodology](https://toolproof.thecompound.tech/methodology) |
| Licence | [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/) |
| Publisher | [Compound Labs](https://thecompound.tech) |
| Also on | [Hugging Face](https://huggingface.co/datasets/kyisaiah47/skillworks-category-census) · [Kaggle](https://www.kaggle.com/datasets/kyisaiah47/skillworks-category-census) · [Zenodo](https://zenodo.org/records/22844097) |

## How it is measured

The dataset reads each listing's files from the repository that publishes them. It scores each listing on four weighted components. It counts a listing that does not parse into a loadable artefact as broken instead of dropping it from the denominator. The denominator determines whether a failure rate is meaningful.

## What a citer needs to know

- The dataset publishes an aggregate. The underlying listing rows contain author handles, and the dataset does not publish those rows in any form.
- The ecosystem contains many forks and vendored files, so the dataset counts the same file once for each repository that carries it. The failure RATE is the citable figure. The population count does not state how many distinct artefacts exist.

The aggregate is a database view. This file defines the view:

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
| `skillworks-category-census-2026-10-01.csv` | CSV | 0.00 MB |
| `skillworks-category-census-2026-10-01.json` | JSON | 0.02 MB |

Every cut is also published as a [GitHub release](https://github.com/kyisaiah47/compound-datasets/releases). The release attaches
the same files. A citation can use the release to pin the exact edition it quoted.

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
Compound Labs (2026). SkillWorks: Claude Code artefacts by category and kind. SkillWorks, https://skillworks.thecompound.tech. Cut of 2026-10-01. Creative Commons Attribution 4.0 International (CC BY 4.0). https://github.com/kyisaiah47/compound-datasets/tree/main/skillworks-category-census
```

```bibtex
@dataset{compound_skillworks_category_census_2026,
  title     = {SkillWorks: Claude Code artefacts by category and kind},
  author    = {{Compound Labs}},
  year      = {2026},
  publisher = {Compound Labs},
  url       = {https://github.com/kyisaiah47/compound-datasets/tree/main/skillworks-category-census},
  note      = {Cut of 2026-10-01. Measured by SkillWorks, https://skillworks.thecompound.tech},
  license   = {CC-BY-4.0}
}
```

The whole collection has the DOI 10.5281/zenodo.22844096 at [https://doi.org/10.5281/zenodo.22844096](https://doi.org/10.5281/zenodo.22844096). The DOI resolves
to the newest Zenodo version. Cite 10.5281/zenodo.22844097 to pin the exact deposit for this cut.

Attribution is the licence condition. Attribution is the only condition. Cite the publisher, the
product that measured the figure, and the cut date when you quote a figure. You do not need to
ask for anything else.
