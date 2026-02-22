# Todd Iodice — Personal Website

Source code for my personal portfolio site, built with [Quarto](https://quarto.org/). The site is used to share my background, coding projects, and research work as part of my job search.

## Site Structure

| File | Page | Description |
|---|---|---|
| `index.qmd` | Home | Landing page with intro and links to key sections |
| `about.qmd` | About | Full bio: work experience, education, and skills |
| `coding-projects.qmd` | Coding Projects | Portfolio of coding and software projects |
| `research-projects.qmd` | Research Projects | Quantitative research and data science write-ups |
| `_quarto.yml` | — | Site-wide config: navbar, theme, CSS |
| `styles.css` | — | Custom CSS on top of the Bootstrap/Cosmo theme |

## Local Development

Requires [Quarto](https://quarto.org/docs/get-started/) to be installed.

```bash
# Live preview with auto-reload
quarto preview

# Build the full site to _site/
quarto render
```

## Tech Stack

- **Framework:** [Quarto](https://quarto.org/) (`.qmd` source files → static HTML)
- **Theme:** Bootstrap Cosmo + custom CSS
- **Hosting:** GitHub Pages *(or update as applicable)*
