# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a personal website built with [Quarto](https://quarto.org/), a scientific/technical publishing system. Source files are `.qmd` (Quarto Markdown) and the site is rendered to the `_site/` directory.

## Key Commands

```bash
# Start live preview server (auto-reloads on file changes)
quarto preview

# Render the full site to _site/
quarto render

# Render a single page
quarto render index.qmd
```

## Architecture

- `_quarto.yml` — Site-wide configuration: navbar, theme, CSS, output format
- `index.qmd` — Home/landing page (hero section, 3-column feature grid, CTA buttons)
- `about.qmd` — Bio page (experience, education, skills)
- `coding-projects.qmd` — Coding projects portfolio page
- `research-projects.qmd` — Research projects portfolio page
- `styles.css` — Custom CSS layered on top of the Bootstrap/Cosmo theme
- `_site/` — Build output (git-ignored via `_site/` entry in `.gitignore`)

The site uses the `cosmo` Bootstrap theme plus a `brand` theme layer, with `toc: true` enabled globally. Adding a new page requires creating a `.qmd` file and registering it in `_quarto.yml` under `website.navbar`.

## Adding Projects

To add a project to `coding-projects.qmd` or `research-projects.qmd`, use a `::: {.project-card}` div block. Each file contains a commented-out template showing the expected structure, including how to embed a Shiny app via `<iframe src="https://yourusername.shinyapps.io/app-name/">`.

## Navbar Structure

Home | About | Projects ▾ (Coding Projects / Research Projects) | LinkedIn icon | GitHub icon
