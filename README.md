
<!-- README.md is generated from README.Rmd. Please edit that file -->

# recountWorkflow

<!-- badges: start -->

[![Lifecycle:
stable](https://img.shields.io/badge/lifecycle-stable-brightgreen.svg)](https://www.tidyverse.org/lifecycle/#stable)
[![BioC
status](https://master.bioconductor.org/shields/build/release/workflows/recountWorkflow.svg)](http://bioconductor.org/checkResults/release/workflows-LATEST/recountWorkflow/)
[![R build
status](https://github.com/LieberInstitute/recountWorkflow/workflows/R-CMD-check-bioc/badge.svg)](https://github.com/LieberInstitute/recountWorkflow/actions)
<!-- badges: end -->

# recount workflow: accessing over 70,000 human RNA-seq samples with Bioconductor

## Abstract

The recount2 resource is composed of over 70,000 uniformly processed
human RNA-seq samples spanning TCGA and SRA, including GTEx. The
processed data can be accessed via the recount2 website and the
`recount` Bioconductor package. This workflow explains in detail how to
use the `recount` package and how to integrate it with other
Bioconductor packages for several analyses that can be carried out with
the recount2 resource. In particular, we describe how the coverage count
matrices were computed in recount2 as well as different ways of
obtaining public metadata, which can facilitate downstream analyses.
Step-by-step directions show how to do a gene level differential
expression analysis, visualize base-level genome coverage data, and
perform an analyses at multiple feature levels. This workflow thus
provides further information to understand the data in recount2 and a
compendium of R code to use the data.

## Workflow locations

The workflow is available on Bioconductor at
<https://www.bioconductor.org/help/workflows/recountWorkflow/> and
F1000Research at <https://f1000research.com/articles/6-1558/v1>.

## Documentation

For more information about `recountWorkflow` check the vignettes
[through Bioconductor](http://bioconductor.org/packages/recountWorkflow)
or at the [documentation
website](http://LieberInstitute.github.io/recountWorkflow).

## Installation instructions

Get the latest stable `R` release from
[CRAN](http://cran.r-project.org/). Then install `recountWorkflow` using
from [Bioconductor](http://bioconductor.org/) the following code:

``` r
if (!requireNamespace("BiocManager", quietly = TRUE))
    install.packages("BiocManager")

BiocManager::install("recountWorkflow")
```

## Citation

Below is the citation output from using `citation('recountWorkflow')` in
R. Please run this yourself to check for any updates on how to cite
**recountWorkflow**.

``` r
print(citation('recountWorkflow'), bibtex = TRUE)
#> 
#> Collado-Torres L, Nellore A, Jaffe AE (2017). "recount workflow:
#> Accessing over 70,000 human RNA-seq samples with Bioconductor [version
#> 1; referees: 1 approved, 2 approved with reservations]."
#> _F1000Research_. doi: 10.12688/f1000research.12223.1 (URL:
#> https://doi.org/10.12688/f1000research.12223.1), <URL:
#> https://f1000research.com/articles/6-1558/v1>.
#> 
#> A BibTeX entry for LaTeX users is
#> 
#>   @Article{,
#>     title = {recount workflow: Accessing over 70,000 human RNA-seq samples with Bioconductor [version 1; referees: 1 approved, 2 approved with reservations]},
#>     author = {Leonardo Collado-Torres and Abhinav Nellore and Andrew E. Jaffe},
#>     year = {2017},
#>     journal = {F1000Research},
#>     doi = {10.12688/f1000research.12223.1},
#>     url = {https://f1000research.com/articles/6-1558/v1},
#>   }
#> 
#> Collado-Torres L, Nellore A, Jaffe AE (2020). _recount workflow:
#> accessing over 70,000 human RNA-seq samples with Bioconductor_. doi:
#> 10.18129/B9.bioc.recountWorkflow (URL:
#> https://doi.org/10.18129/B9.bioc.recountWorkflow),
#> https://github.com/LieberInstitute/recountWorkflow - R package version
#> 1.11.4, <URL: http://www.bioconductor.org/packages/recountWorkflow>.
#> 
#> A BibTeX entry for LaTeX users is
#> 
#>   @Manual{,
#>     title = {recount workflow: accessing over 70,000 human RNA-seq samples with Bioconductor},
#>     author = {Leonardo Collado-Torres and Abhinav Nellore and Andrew E. Jaffe},
#>     year = {2020},
#>     url = {http://www.bioconductor.org/packages/recountWorkflow},
#>     note = {https://github.com/LieberInstitute/recountWorkflow - R package version 1.11.4},
#>     doi = {10.18129/B9.bioc.recountWorkflow},
#>   }
```

Please note that the `recountWorkflow` was only made possible thanks to
many other R and bioinformatics software authors, which are cited either
in the vignettes and/or the paper(s) describing this package.

## Code of Conduct

Please note that the recountWorkflow project is released with a
[Contributor Code of
Conduct](https://contributor-covenant.org/version/2/0/CODE_OF_CONDUCT.html).
By contributing to this project, you agree to abide by its terms.

## Development tools

  - Continuous code testing is possible thanks to [GitHub
    actions](https://www.tidyverse.org/blog/2020/04/usethis-1-6-0/)
    through *[usethis](https://CRAN.R-project.org/package=usethis)*,
    *[remotes](https://CRAN.R-project.org/package=remotes)*,
    *[sysreqs](https://github.com/r-hub/sysreqs)* and
    *[rcmdcheck](https://CRAN.R-project.org/package=rcmdcheck)*
    customized to use [Bioconductor’s docker
    containers](https://www.bioconductor.org/help/docker/) and
    *[BiocCheck](https://bioconductor.org/packages/3.11/BiocCheck)*.
  - Code coverage assessment is possible thanks to
    [codecov](https://codecov.io/gh) and
    *[covr](https://CRAN.R-project.org/package=covr)*.
  - The [documentation
    website](http://LieberInstitute.github.io/recountWorkflow) is
    automatically updated thanks to
    *[pkgdown](https://CRAN.R-project.org/package=pkgdown)*.
  - The code is styled automatically thanks to
    *[styler](https://CRAN.R-project.org/package=styler)*.
  - The documentation is formatted thanks to
    *[devtools](https://CRAN.R-project.org/package=devtools)* and
    *[roxygen2](https://CRAN.R-project.org/package=roxygen2)*.

For more details, check the `dev` directory.
