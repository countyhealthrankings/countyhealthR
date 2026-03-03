# countyhealthR
An R package for programmatic access to archived County Health Rankings & Roadmaps (CHR&R) data, modeled after the simplicity of the `tidycensus` package.

[![CRAN Version](https://www.r-pkg.org/badges/version/countyhealthR)](https://cran.r-project.org/package=countyhealthR)
[![CRAN Downloads](https://cranlogs.r-pkg.org/badges/grand-total/countyhealthR)](https://cran.r-project.org/package=countyhealthR)

### Reference Manual: https://cran.r-project.org/web/packages/countyhealthR/countyhealthR.pdf 
---

## Install

### Install the stable CRAN version

```r
install.packages("countyhealthR")
```

### Install the development version (GitHub) 
```r
# install.packages("devtools") # if needed 
devtools::install_github("countyhealthrankings/countyhealthR")
``` 

## Quick Start 
```r
library(countyhealthR)

# Example: Load county-level premature death data for the 2024 release
get_chrr_measure_data(
  geography = "county",
  measure = "premature death",
  year = 2024
)
``` 
