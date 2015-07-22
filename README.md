# The family of R packages containing TCGA data

[Contribution: Adding a new package to the `RTCGA.data` family](https://github.com/mi2-warsaw/RTCGA.data/wiki/Contribution:-Adding-a-new-package-to-the-%60RTCGA.data%60-family)

### Installation of packages from the `RTCGA.data` family: 

Make sure you have [rtools](http://cran.r-project.org/bin/windows/Rtools/) installed on your computer.

```{Ruby}
if (!require(devtools)) {
   install.packages("devtools")
   require(devtools)
}
install_github(paste0("mi2-warsaw/RTCGA.data/", 
                  subdir = paste0("RTCGA.", 
                                  c("clinical",
                                    "rnaseq",
                                    "mutations",
                                    "cnv",
                                    "PANCAN12")
                                 )
               )
)
```

<h5> The list of available datasets: </h5>
```{Ruby}
library(RTCGA.clinical)
library(RTCGA.rnaseq)
library(RTCGA.mutations)
library(RTCGA.PANCAN12)
library(RTCGA.cnv)
?clinical
?rnaseq
?mutations
?pancan12
?cnv
```

# Packages from the `RTCGA.data`-family are based on the `RTCGA` package


### Installation of the [`RTCGA`](https://github.com/MarcinKosinski/RTCGA) package: 
To get started, install the latest version of **RTCGA** from GitHub:

```{Ruby}
if (!require(devtools)) {
    install.packages("devtools")
    require(devtools)
}
install_github("MarcinKosinski/RTCGA")
```

<h4> Authors: </h4>

>
> Marcin Kosiński, m.p.kosinski@gmail.com
>
> Przemysław Biecek, przemyslaw.biecek@gmail.com
>
