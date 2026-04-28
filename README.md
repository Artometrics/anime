# Artometrics — Anime

**The Artometrics of Japanese Animation**
Published at [artometrics.com/anime](https://artometrics.com/anime)

---

## About This Report

A data analysis of 13,631 anime titles from the MyAnimeList TidyTuesday
dataset (April 2019). The report examines how the anime industry
industrialized and diversified across a century, which studios produce
consistent quality at scale, and how genre positioning maps onto
popularity vs. critical reception.

**Three charts:**

1. **Releases by Year by Type** — Faceted line chart tracing the
   rise and fall of each format (TV, Movie, OVA, Special, ONA, Music)
   from the 1920s through 2018.

2. **Studio Consistency** — Dot plot with IQR bars ranking the top 20
   studios (min 20 titles) by median MAL score, colored by TV share.

3. **Genre Map** — Bubble scatter plotting median popularity rank vs.
   median score for every major genre (min 80 titles), with size
   encoding volume.

---

## Data Source

MyAnimeList via TidyTuesday (April 23, 2019)
https://github.com/rfordatascience/tidytuesday/tree/main/data/2019/2019-04-23

Data is loaded directly from the TidyTuesday GitHub raw URL — no local
CSV dependency.

---

## File Structure

```
anime/
├── anime.qmd           # Main Quarto report
├── artometrics.css     # Shared Artometrics stylesheet
├── art-head.html       # Quarto header include (progress bar, fonts)
├── art-body.html       # Quarto body include (sidebar toggle, copy button)
├── charts/             # Generated chart PNGs (created on render)
│   ├── chart1_releases_by_year.png
│   ├── chart2_studio_consistency.png
│   └── chart3_genre_map.png
└── README.md
```

---

## How to Render

Open `anime.qmd` in RStudio. Always use **Source mode** — never Visual
mode (Visual mode corrupts Quarto documents by converting sections into
pipe tables).

Required packages:

```r
install.packages(c(
  "tidyverse", "lubridate", "scales",
  "ggrepel", "ggtext", "ggridges"
))
```

Run → Render. Charts output to `charts/` automatically via `ggsave()`.

---

## Part of the Artometrics Series

Artometrics is a data-forward content brand analyzing creative
industries. "The Economist for Artists."

- Website: [artometrics.com](https://artometrics.com)
- GitHub: [github.com/Artometrics](https://github.com/Artometrics)
