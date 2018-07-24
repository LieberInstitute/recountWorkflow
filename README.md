# recount workflow: accessing over 70,000 human RNA-seq samples with Bioconductor

## Abstract

The recount2 resource is composed of over 70,000 uniformly processed human RNA-seq samples spanning TCGA and SRA, including GTEx. The processed data can be accessed via the recount2 website and the `recount` Bioconductor package. This workflow explains in detail how to use the `recount` package and how to integrate it with other Bioconductor packages for several analyses that can be carried out with the recount2 resource. In particular, we describe how the coverage count matrices were computed in recount2 as well as different ways of obtaining public metadata, which can facilitate downstream analyses. Step-by-step directions show how to do a gene level differential expression analysis, visualize base-level genome coverage data, and perform an analyses at multiple feature levels. This workflow thus provides further information to understand the data in recount2 and a compendium of R code to use the data.

## Bioconductor installation 

The workflow is available on Bioconductor at https://www.bioconductor.org/help/workflows/recountWorkflow/ and F1000Research at https://f1000research.com/articles/6-1558/v1.

All the packages used in this workflow get installed by installing the workflow corresponding package:

```{r}
## You will need R 3.5.x or newer
install.packages("BiocManager")
BiocManager::install("recountWorkflow")
```

## Feedback and bug reports

For feedback and bug reports, please create a new post in the Bioconductor support website using the `recountWorkflow` tag at https://support.bioconductor.org/t/recountWorkflow/. Remember to check the posting guidelines before submitting your new post. Thank you.
