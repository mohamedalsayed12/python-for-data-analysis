# Data files

This folder contains the three CSV files used in the notebook.

| File | Purpose |
|---|---|
| `netflix_weekly_top10.csv` | Weekly global Netflix Top 10 viewing, rank and title information |
| `imdb_ratings.csv` | IMDb title, rating, vote count and descriptive metadata |
| `netflix_titles.csv` | Historical Netflix catalogue metadata for television shows |

## Provenance note

These files were exported from the local educational database used to develop this portfolio project. The original download URLs and licences were not stored with that database, so they should not be guessed.

Before reusing the raw data outside this portfolio, confirm the original source and licence. The analysis itself makes the following scope distinctions:

- weekly Netflix viewing is global Top 10 activity rather than UK title-level viewing;
- the catalogue is historical and cannot prove current platform or rights status;
- IMDb title matching is based on cleaned titles and can require manual checking for remakes;
- no file contains licence cost, confirmed rights, Google Trends or original UK audience data.

## Notes added in version 2

- `imdb_ratings.csv` mixes series, individual episodes **and films**. It also looks like a snapshot from about 2022, because almost no series in it start after 2022. The notebook removes films and episodes before matching.
- `title_match_overrides.csv` is analyst-maintained. It records reviewed accept/reject decisions for IMDb matches that the matching rule flags (for example, remakes that share a title with an older show). Each row has a reason.
