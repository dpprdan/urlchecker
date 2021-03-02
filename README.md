
# urlchecker

<!-- badges: start -->
[![R build status](https://github.com/r-lib/urlchecker/workflows/R-CMD-check/badge.svg)](https://github.com/r-lib/urlchecker/actions)
<!-- badges: end -->

The goal of urlchecker is to run the URL checks from R 4.1 in older versions of R and automatically update URLs as needed.

It also uses concurrent requests, so is generally much faster than the URL checks from the tools package.

``` r
library(urlchecker)

# Check all URLs in a package
url_check("path/to/pkg")

## Update any redirected URLs automatically
url_update("path/to/pkg")
```
