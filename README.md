# geosocial-outbreaker: Integrating geographical and social contact data to reconstruct transmission chains

o2geosocial infer probabilistic transmission trees from routinely-collected epidemiological data. It combines the age group, location, onset date and genotype of cases to infer their import status, and their likely infector. o2geosocial is adapted from the R package "outbreaker2" (https://github.com/reconhub/outbreaker2), it is designed to study datasets that do not include genetic sequences but genotype of the cases. o2geosocial will cluster cases from different genotypes in different trees, without computing the genetic distance between cases.

o2geosocial was originally designed to study measles outbreaks, as the evolution rate of the measles virus is slow and the genetic diversity minimal. It can be also applied to other viruses.

Installation
-------------

To install the development version from github (requires Rtools on windows and GSL headers on all platforms):

```{r, eval = FALSE}
devtools::install_github("alxsrobert/o2geosocial")
```

To add local copies of the vignettes, you will need to specify:
```{r, eval = FALSE}
devtools::install_github("alxsrobert/o2geosocial", build_vignettes = TRUE)
```

Then, to load the package, use:

```{r, eval = FALSE}
library("o2geosocial")
```


