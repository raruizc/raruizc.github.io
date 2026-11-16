# raruizc.github.io

Personal website of Ricardo Antonio Ruiz-Cardozo, built with [Quarto](https://quarto.org) and published with GitHub Pages.

## Work on the site locally

```bash
quarto preview      # live preview in the browser, reloads on save
quarto render       # build the full site into _site/
```

## Structure

| File / folder | Content |
|---|---|
| `_quarto.yml` | Site settings: navbar, footer, theme |
| `styles.scss`, `styles-dark.scss` | Colours and custom styles (light / dark mode) |
| `index.qmd` | Home page |
| `about.qmd`, `research.qmd`, `open-science.qmd`, `teaching.qmd` | Main pages |
| `projects/<name>/index.qmd` | One page per project; the Projects page lists them automatically |
| `images/` | Profile photo and project figures |
| `.github/workflows/publish.yml` | Builds and deploys the site on every push to `main` |

## Add a new project

1. Copy a folder in `projects/`, e.g. `projects/agriraster/`, to `projects/new-project/`.
2. Edit the YAML header (`title`, `description`, `image`, `categories`, `order`) and the text.
3. Run `quarto preview`; the card appears on the Projects page.
