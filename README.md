[<img src="https://www.bioconductor.org/images/logo/jpg/bioconductor_logo_rgb.jpg" width="200" align="right"/>](https://bioconductor.org/)

_Biobase_ is an R/Bioconductor package that implements base functions for Bioconductor.

See https://bioconductor.org/packages/Biobase for more information including how to install the release version of the package (please refrain from installing directly from GitHub).

**Note of the current repository**: this repository is a clone of https://github.com/crhisto/Biobase. It contains some modifications related with compatibility with sparse matrices using: dgCMatrix objects in R. This has been done as part of a project: https://github.com/crhisto/thymus_NPM-ALK_notebook. 

If you want to install the Biobase library with sparse support you can use: 

``` r
if("Biobase" %in% rownames(installed.packages())){
  library(Biobase)
}else{
  devtools::install_github( repo = "crhisto/Biobase")
  library(Biobase)
}
```
