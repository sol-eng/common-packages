# Common Packages

This repository contains a list of common R packages that can be helpful for
establishing a new R environment.

### Packages
* [`tidyverse`](https://www.tidyverse.org/) - A collection of packages that
  provide tools for solving common data science tasks
* [`tidymodels`](https://www.tidymodels.org/) - A collection of packages that
  provide tools for solving common statistical modeling tasks
* [`rmarkdown`](https://rmarkdown.rstudio.com/) - A package for creating static
  and dynamic documents
* [`shiny`](https://shiny.rstudio.com/) - A package for building interactive
  web applications
* [`DBI`](https://dbi.r-dbi.org/) - A package for connecting to external data
  sources
* [`odbc`](https://github.com/r-dbi/odbc) - A package for connecting to
  external data sources via ODBC
* [`sparklyr`](https://spark.rstudio.com/) - A package for interacting with
  Spark
* [`data.table`](https://rdatatable.gitlab.io/data.table/) - A high-performance
  version of base R's `data.frame`.
* [`dtplyr`](https://dtplyr.tidyverse.org/) - A `data.table` backend for
  `dplyr`.

### Installation
R packages can be installed via the `install.packages()` command. By default,
users install packages to a user library within their home directory. In order
to install packages to the system library so they are accessible to all users,
the R session must be run as a root / admin account.

R packages will install by default from [CRAN](https://cran.rstudio.com/). CRAN
provides pre-built Windows and MacOS package binaries, but it does not provide
linux binaries. If you want to install these packages on linux without building
them from source, you can install them from [RStudio Public Package
Manager](https://packagemanager.rstudio.com/client/#/).

```r
packages <- c("tidyverse",
              "tidymodels",
              "rmarkdown",
              "shiny",
              "DBI",
              "odbc",
              "sparklyr",
	      "data.table",
	      "dtplyr"
)

# Install from CRAN
install.packages(packages, repos = "https://cran.rstudio.com/")

# Install from Package Manager for CentOS 7 / RHEL 7
install.packages(packages, repos = "https://packagemanager.rstudio.com/all/__linux__/centos7/latest")

# Install from Package Manager for CentOS 8 / RHEL 8
install.packages(packages, repos = "https://packagemanager.rstudio.com/all/__linux__/centos8/latest")

# Install from Package Manager for OpenSUSE 15 / SLES 15
install.packages(packages, repos = "https://packagemanager.rstudio.com/all/__linux__/opensuse15/latest")

# Install from Package Manager for OpenSUSE 42.3 / SLES 12
install.packages(packages, repos = "https://packagemanager.rstudio.com/all/__linux__/opensuse42/latest")

# Install from Package Manager for Ubuntu 16.04 (Xenial)
install.packages(packages, repos = "https://packagemanager.rstudio.com/all/__linux__/xenial/latest")

# Install from Package Manager for Ubuntu 18.04 (Bionic)
install.packages(packages, repos = "https://packagemanager.rstudio.com/all/__linux__/bionic/latest")

# Install from Package Manager for Ubuntu 20.04 (Focal)
install.packages(packages, repos = "https://packagemanager.rstudio.com/all/__linux__/focal/latest")
```
