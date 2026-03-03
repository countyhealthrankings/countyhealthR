# countyhealthR
an R package to quickly pull CHR&amp;R data into R, modeled after tidycensus

[![CRAN Version](https://www.r-pkg.org/badges/version/countyhealhtR)](https://cran.r-project.org/package=countyhealthR)
[![CRAN Downloads](https://cranlogs.r-pkg.org/badges/grand-total/countyhealthR)](https://cran.r-project.org/package=countyhealthR)

To use the development version (ie from GitHub) run the following R code to quickly install and load `countyhealthR` into your local environment: 
```r
# Quick Start 
library(devtools)
devtools::install_github("County-Health-Rankings-and-Roadmaps/countyhealthR")
library(countyhealthR)

# Example: load county-level premature death data for release year 2024
get_chrr_measure_data("county", "premature death", 2024)
``` 
