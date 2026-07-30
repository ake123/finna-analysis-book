# Finnish Cultural Heritage Metadata — Analysis Notebook

A Quarto book covering two `finna`-based analyses:

- **Chapter 1** — Fennica, nineteenth-century publication metadata (1809–1917)
- **Chapter 2** — Viola, music collection metadata (1900–2025)

## Requirements

- [Quarto](https://quarto.org/docs/get-started/) (CLI)
- R with: `dplyr`, `ggplot2`, `scales`, `forcats`, `patchwork`, `stringr`,
  `tidyr`, `grid`

## Data

Place (or symlink) the following files at:

```
~/finna/inst/extras/nineteen_cen.rds
~/finna/inst/extras/viola_collection.rds
```

or edit the `readRDS()` call in the first code chunk of each chapter to
point at your own copies.

## Render locally

```bash
quarto render
```

Output is written to `docs/`. Preview with:

```bash
quarto preview
```

## Publish online

Once `docs/` is built, either:

- **GitHub Pages**: `quarto publish gh-pages` (from a git repo), or
- push the `docs/` folder to any static host (Netlify, Quarto Pub, etc.)

## Project layout

```
_quarto.yml       # book configuration
index.qmd         # overview / landing page
01-fennica.qmd     # Chapter 1: Fennica analysis
02-viola.qmd       # Chapter 2: Viola analysis
```
