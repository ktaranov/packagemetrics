packagemetrics
================

About packagemetrics
--------------------

The packagemetrics project was a part of the 2017 rOpenSci Unconference. With over 10,000 packages on CRAN - and thousands more on GitHub and Bioconductor - a useR needs a way to navigate this wealth of options. There are many existing tools that are helpful for finding packages, but few ways to quickly compare differences between packages. We set out to create tools for comparing a set of related and potentially overlapping packages through a combination of standardized packagemetrics and an expert review process. More information about our project can be found in this [post](https://ropensci.org/blog/blog/2017/06/27/packagemetrics).

Team packagemetrics:
--------------------

Lori Shepherd, Hannah Frick, William Ampeh, Erin Grand, Sam Firke, Becca Krouse

Installation
------------

``` r
devtools::install_github("ropenscilabs/packagemetrics")
```

Use
---

### Here's an example using a case study of popular table-making packages.

``` r
library(packagemetrics)

pkg_df <- package_list_metrics(table_packages)
ft <- metrics_table(pkg_df)
```

![](README_files/figure-markdown_github-ascii_identifiers/unnamed-chunk-2-1.png)

Requirements
------------

`packagemetrics` requires R version &gt;= 3.4.0.
