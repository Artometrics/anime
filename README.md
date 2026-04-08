# ANIME: The Artometrics of Japanese Animation

A data analysis of 13,631 anime titles spanning 1917–2019, built on the [MyAnimeList TidyTuesday dataset](https://github.com/rfordatascience/tidytuesday/blob/master/data/2019/2019-04-23/readme.md).

## What's in this repo

- `anime.qmd` — Quarto markdown file containing all R code, analysis, and write-up
- `tidy_anime.xlsx` — raw dataset export
- `chart1_releases_by_year.png` — anime releases per year by format
- `chart2_hitrate_by_format.png` — hit-rate of 8+ titles by format
- `chart3_popularity_vs_score.png` — popularity rank vs MAL score (decile analysis)
- `chart4_studio_rankings.png` — studio rankings by median score
- `chart5_genre_map.png` — genre map: popularity vs rating

## What the analysis covers

Five charts working through what the MAL archive actually shows:

1. How the industry grew — format by format, decade by decade
2. Which formats produce the best odds of finding a great title
3. Why popular shows score higher (and what lives in the back rooms)
4. Which studios are the most consistent
5. Where the hidden gems are hiding by genre

## Read the full article

[artometrics.com](https://artometrics.com)

## Tools

- R / Quarto
- tidyverse, ggplot2, ggrepel, lubridate, scales

## Disclosure

This analysis is based on original data work (R / TidyTuesday). AI was used to assist in analysis, research, and writing.