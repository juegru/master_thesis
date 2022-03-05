# Master's Thesis Project

[![lifecycle](https://img.shields.io/badge/lifecycle-maturing-blue.svg)](https://www.tidyverse.org/lifecycle/#maturing)
[![lifecycle](https://img.shields.io/badge/version-2021-red.svg)]()

## Meta-Information

* Name: Your Name (`@yourGHhandle`)
* Thesis Title: Your title
* Link to code that runs analysis: [click here](Your link)

## Installation Instructions

To use this template for you thesis you need to have the following `R` packages installed:

* `tisemdown`
* `bookdown` 
* `rmarkdown`

and a LaTeX installation. 

Here's the minimum instructions to get those installed:

### `R` packages

-   Open RStudio
-   Enter the following lines into the console and press `RETURN`:

``` r
# install rmarkdown and bookdown from CRAN
install.packages(c('rmarkdown', 'bookdown'))
# install tisemdown from GitHub
if (!require("remotes")) 
  install.packages("remotes", repos = "https://cran.rstudio.org")
  remotes::install_github("deer-marketing-lab/tisemdown")
```

### LaTeX

There's many ways to do this. 
Here's the easiest way:

-   Open RStudio
-   Enter the following lines into the console and press `RETURN`:

``` r
install.packages('tinytex')
# below installs latex
tinytex::install_tinytex()
# after restarting RStudio, confirm that you have LaTeX with
tinytex:::is_tinytex()
```

## Day to Day Work

Students write their thesis by editing and/or creating `.Rmd` files in the project's main directory:

* `index.Rmd` has the meta information for the title page
* `prelims/00-managementsummary.Rmd` should contain your max 1 page management summary. 
* Chapters of your thesis can be written using files `01-chap1.Rmd`, `02-chap2.Rmd` etc. One should remove the content in the current files and create their own.
* Additional chapters can be created by creating new `.Rmd` files, for example `05-chap5.Rmd`
* Appendix material should be added to `90-appendix.Rmd`
* For bibliography management, you should put bibtex for each article you cite in `bib/thesis.bib`. If you cite those references in the text, they will be automatically added to the references section.

## Template Meta-Information

* Module Maintainer: Lachlan Deer (`@lachlandeer`)
* Institute: Dept of Marketing, Tilburg University
