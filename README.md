# ANIME: The Artometrics of Japanese Animation

A data analysis of 13,631 anime titles spanning 1917–2019, built on the
[MyAnimeList TidyTuesday dataset](https://github.com/rfordatascience/tidytuesday/blob/master/data/2019/2019-04-23/readme.md).

## What's in this repo

- `anime.qmd` — Quarto markdown file containing all R, SQL, and Python code, analysis, and write-up
- `tidy_anime.xlsx` — raw dataset export (convenience copy; analysis reads directly from TidyTuesday URL)
- `chart1_releases_by_year.png` — anime releases per year by format
- `chart2_hitrate_by_format.png` — hit-rate of 8+ titles by format
- `chart3_popularity_vs_score.png` — popularity rank vs MAL score (decile analysis)
- `chart4_studio_rankings.png` — studio consistency by median score and output volume
- `chart5_genre_map.png` — genre map: popularity vs rating
- `chart6_source_shift.png` — source material shift: the rise of the light novel
- `chart7_episode_collapse.png` — the 12-episode standardization by era
- `chart8_maturity_score.png` — score distributions by content rating
- `chart9_devotion_index.png` — reach vs obsession: the devotion index
- `chart10_genre_lifecycles.png` — genre lifecycles over 40 years of TV anime
- `chart11_era_scoring.png` — MAL score distributions by decade
- `chart12_survivor_bias.png` — survivor bias: episode count vs score

## What the analysis covers

Twelve charts and a polyglot Trinity analysis (R + SQL + Python) working
through what the MAL archive actually shows:

1. How the industry grew — format by format, decade by decade
2. Which formats produce the best odds of finding a great title
3. Why popular shows score higher (and what lives in the back rooms)
4. Which studios are the most consistent across volume
5. Where the hidden gems are hiding by genre
6. How studios shifted from manga to light novel source material
7. How the 1-cour standard took over TV anime
8. Whether mature content ratings actually predict better scores
9. The difference between shows people watch and shows people worship
10. The rise and fall of Mecha, and the rise of Fantasy and Slice of Life
11. Whether modern anime is actually better or just rated higher
12. Why bad shows don't run forever

## Read the full article

[artometrics.com/anime](https://www.artometrics.com/anime/)

## Tools

- R / Quarto
- tidyverse · ggplot2 · ggrepel · ggtext · ggridges · lubridate · scales · DBI · RSQLite · reticulate
- Python (pandas · numpy) · SQL (SQLite in-memory)

## Disclosure

This analysis is based on original data work (R / TidyTuesday). AI was
used to assist in analysis, research, and writing.