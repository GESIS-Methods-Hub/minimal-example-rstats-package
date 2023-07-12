# Minimal Example of Tutorial as R package vignette

[`vignettes/example.Rmd`](vignettes/example.Rmd) shows all **required** metadata used by [`methodshub`](https://github.com/GESIS-Methods-Hub/methodshub).

## Supported Features

[`methodshub`](https://github.com/GESIS-Methods-Hub/methodshub) uses [Quarto](https://quarto.org/) and [`pkgdown`](https://pkgdown.r-lib.org/) uses [R Markdown](https://rmarkdown.rstudio.com/). Quarto and R Markdown are not 100% compatible.

| Feature | [`methodshub`](https://github.com/GESIS-Methods-Hub/methodshub) | [`pkgdown`](https://pkgdown.r-lib.org/) | Notes |
| --- | --- | --- | --- |
| Pandoc’s Markdown | 👍 | 👍 | |
| Callout Blocks | 👍 | 😥 | `pkgdown` does **not** have the CSS for callout blocks. |
| Cross References | 👍 | 😭 | |
| Citations and Bibliographies | 👍 | 👍 | |
| [Code Annotation](https://quarto.org/docs/authoring/code-annotation.html) | 👍 | 😭 | Requires Quarto >= 1.3 |
| Computation of [Code Chunks](https://rmarkdown.rstudio.com/lesson-3.html) | 👍 | 👍 | |
| Computation of [Inline Code](https://rmarkdown.rstudio.com/lesson-4.html) | 👍 | 👍 | |
| [Title Blocks](https://quarto.org/docs/authoring/title-blocks.html) | 👍 | 👍 | Generated by Quarto based on YAML header |
| How to cite in the appendix | 👍 | 😥 | Generated by Quarto based on YAML header |

## GitHub Actions

[`.github/workflows/pkgdown.yaml`](.github/workflows/pkgdown.yaml) is the [GitHub Actions](https://docs.github.com/en/actions) used to create the R package website with [`pkgdown`](https://pkgdown.r-lib.org/). Ensure that GitHub Pages' source in `Settings > Pages > Build and deployment` is `GitHub Actions`.
