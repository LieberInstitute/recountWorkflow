# recount workflow: accessing over 70,000 human RNA-seq samples with Bioconductor

## Abstract

The recount2 resource is composed of over 70,000 uniformly processed human RNA-seq samples spanning TCGA and SRA, including GTEx. The processed data can be accessed via the recount2 website and the `recount` Bioconductor package. This workflow explains in detail how to use the `recount` package and how to integrate it with other Bioconductor packages for several analyses that can be carried out with the recount2 resource. In particular, we describe how the coverage count matrices were computed in recount2 as well as different ways of obtaining public metadata, which can facilitate downstream analyses. Step-by-step directions show how to do a gene level differential expression analysis, visualize base-level genome coverage data, and perform an analyses at multiple feature levels. This workflow thus provides further information to understand the data in recount2 and a compendium of R code to use the data.

## Workflow locations 

The workflow is available on Bioconductor at https://www.bioconductor.org/help/workflows/recountWorkflow/ and F1000Research at https://f1000research.com/articles/6-1558/v1.

## Documentation

For more information about `recountWorkflow` check the vignettes [through Bioconductor](http://bioconductor.org/packages/recountWorkflow) or at the [documentation website](http://LieberInstitute.github.io/recountWorkflow).

## Installation instructions

Get the latest stable `R` release from [CRAN](http://cran.r-project.org/). Then install `recountWorkflow` using from [Bioconductor](http://bioconductor.org/) the following code:

```{r 'install', eval = FALSE}
if (!requireNamespace("BiocManager", quietly = TRUE))
    install.packages("BiocManager")

BiocManager::install("recountWorkflow")
```

## Citation

Below is the citation output from using `citation('recountWorkflow')` in R. Please 
run this yourself to check for any updates on how to cite __recountWorkflow__.

```{r 'citation', eval = requireNamespace('recountWorkflow')}
print(citation('recountWorkflow'), bibtex = TRUE)
```

Please note that the `recountWorkflow` was only made possible thanks to many other R and bioinformatics software authors, which are cited either in the vignettes and/or the paper(s) describing this package.

## Code of Conduct
  
Please note that the recountWorkflow project is released with a [Contributor Code of Conduct](https://contributor-covenant.org/version/2/0/CODE_OF_CONDUCT.html). By contributing to this project, you agree to abide by its terms.

## Development tools

* Continuous code testing is possible thanks to [GitHub actions](https://www.tidyverse.org/blog/2020/04/usethis-1-6-0/)  through `r BiocStyle::CRANpkg('usethis')`, `r BiocStyle::CRANpkg('remotes')`, `r BiocStyle::Githubpkg('r-hub/sysreqs')` and `r BiocStyle::CRANpkg('rcmdcheck')` customized to use [Bioconductor's docker containers](https://www.bioconductor.org/help/docker/) and `r BiocStyle::Biocpkg('BiocCheck')`.
* Code coverage assessment is possible thanks to [codecov](https://codecov.io/gh) and `r BiocStyle::CRANpkg('covr')`.
* The [documentation website](http://LieberInstitute.github.io/recountWorkflow) is automatically updated thanks to `r BiocStyle::CRANpkg('pkgdown')`.
* The code is styled automatically thanks to `r BiocStyle::CRANpkg('styler')`.
* The documentation is formatted thanks to `r BiocStyle::CRANpkg('devtools')` and `r BiocStyle::CRANpkg('roxygen2')`.

For more details, check the `dev` directory.
