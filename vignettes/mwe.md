---
title: "Minimal Example of Tutorial as R package vignette"
author:
- Raniere Silva
bibliography: references.bib
output: rmarkdown::html_vignette
vignette: >
  %\VignetteIndexEntry{example}
  %\VignetteEngine{knitr::rmarkdown}
  %\VignetteEncoding{UTF-8}
---

This example demonstrates the required metadata by
[`methodshub`](https://github.com/GESIS-Methods-Hub/methodshub).

## Markdown {#sec-markdown}

::: callout-important
[`methodshub`](https://github.com/GESIS-Methods-Hub/methodshub) uses
[Quarto](https://quarto.org/) and
[`pkgdown`](https://pkgdown.r-lib.org/) uses [R
Markdown](https://rmarkdown.rstudio.com/) to convert Markdown to HTML.
:::

R Markdown does **not** support cross-references like @sec-markdown.

R Markdown supports code execution [@xie2018r].

## Execution of R code

``` r
1 + 1
#> [1] 2
```

## Execution of R code from package

``` r
library(mwe)
```

``` r
hello()
#> [1] "Hello"
```

## Creation of figure with R

``` r
plot(rnorm(10), rnorm(10))
```

![](mwe_files/figure-markdown/unnamed-chunk-4-1.png)

## mybinder.org

[mybinder.org](https://mybinder.org/) uses the [`DESCRIPTION` file](https://github.com/GESIS-Methods-Hub/minimal-example-rstats-package/blob/main/DESCRIPTION) to install the R package but dependencies are not installed. Authors **must** use [`install.R`](https://repo2docker.readthedocs.io/en/latest/config_files.html#install-r-install-an-r-rstudio-environment) and [`apt.txt`](https://repo2docker.readthedocs.io/en/latest/config_files.html#apt-txt-install-packages-with-apt-get) to install the packages dependencies for the user.

## References
