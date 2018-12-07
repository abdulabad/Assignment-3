Assignment 3 Submission
================
Abdul Abad
October 10, 2018

Part 1
======

``` r
getwd()
```

    ## [1] "C:/Users/Grimp/OneDrive/Documents/Assignment-3-Submission"

``` r
library(dplyr)
```

    ## 
    ## Attaching package: 'dplyr'

    ## The following objects are masked from 'package:stats':
    ## 
    ##     filter, lag

    ## The following objects are masked from 'package:base':
    ## 
    ##     intersect, setdiff, setequal, union

``` r
library(tidyr)
library(ggplot2)
```

``` r
K1 <- read.csv("Class_Motivation.csv", header = TRUE)
```

``` r
K2 <- dplyr::select(K1, 2:6)
```

``` r
K3 <- na.omit(K2)
```

``` r
K3 <- scale(K3)
```

``` r
fit <- kmeans(K3, 2)
```

``` r
K4 <- data.frame(K3, fit$cluster)
```

``` r
names(K4) <- c("1", "2", "3", "4", "5", "cluster")
```

``` r
K5 <- tidyr::gather(K4, "week", "motivation", 1:5)
```

``` r
K6 <- K5 %>% group_by(week, cluster)
K6 <- summarise(K6, avg = mean(motivation))
```

``` r
K6$week <- as.numeric(K6$week)
K6$cluster <- as.factor(K6$cluster)
```

``` r
K7 <- dplyr::count(K4, cluster)
```

Part 2
======

``` r
library(tidyverse)
```

    ## -- Attaching packages ----------------------------------------------------------------------------------------- tidyverse 1.2.1 --

    ## v tibble  1.4.2     v purrr   0.2.5
    ## v readr   1.1.1     v stringr 1.3.1
    ## v tibble  1.4.2     v forcats 0.3.0

    ## -- Conflicts -------------------------------------------------------------------------------------------- tidyverse_conflicts() --
    ## x dplyr::filter() masks stats::filter()
    ## x dplyr::lag()    masks stats::lag()

``` r
M1 <- read.csv("HUDK405018-cluster.csv", header = TRUE)
#Create a dataframe that only includes the surevy questions about hours
M2 <- M1[3:47, 20:26]
# Deal with missing values now
# Convert the blank cells to NAs and convert all columns to numeric
M2[M2==""] <- NA
M2 <- M2 %>% mutate_all(funs(as.numeric(levels(.))[.]))
```

    ## Warning in evalq(as.numeric(levels(Q2_1))[Q2_1], <environment>): NAs
    ## introduced by coercion

    ## Warning in evalq(as.numeric(levels(Q2_2))[Q2_2], <environment>): NAs
    ## introduced by coercion

    ## Warning in evalq(as.numeric(levels(Q2_3))[Q2_3], <environment>): NAs
    ## introduced by coercion

    ## Warning in evalq(as.numeric(levels(Q2_4))[Q2_4], <environment>): NAs
    ## introduced by coercion

    ## Warning in evalq(as.numeric(levels(Q2_5))[Q2_5], <environment>): NAs
    ## introduced by coercion

    ## Warning in evalq(as.numeric(levels(Q2_6))[Q2_6], <environment>): NAs
    ## introduced by coercion

    ## Warning in evalq(as.numeric(levels(Q2_7))[Q2_7], <environment>): NAs
    ## introduced by coercion

``` r
#Recode as zero - but missing is not the same as recording zero hours
M2[is.na(M2)] <- 0
#Generate clusters for survey questions
fit2 <- kmeans(M2, 3)
#Create a dataframe that only includes location data
L1 <- M1[3:47, 18:19]
L1 <- unite(L1, place, Q1_1, Q1_2, sep = ",")
#Request lattitude and longitude from Google Maps API
library(ggmap)
L2 <- geocode(as.character(L1$place), output = "latlon", source = "dsk")
```

    ## Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Melbourne,Australia&sensor=false

    ## Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Boston,US&sensor=false

    ## Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Columbus,%20OH,U.S&sensor=false

    ## Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Los%20Angeles,USA&sensor=false

    ## Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Berkeley,USA&sensor=false

    ## Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=San%20Francisco,USA&sensor=false

    ## Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Jakarta,Indonesia&sensor=false

    ## Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Shanghai,China&sensor=false

    ## Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Pittsburgh,USA&sensor=false

    ## Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Brooklyn,US&sensor=false

    ## Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Eugene,U.S&sensor=false

    ## Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Hangzhou,China&sensor=false

    ## Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Madison,US&sensor=false

    ## Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Appleton,United%20States%20of%20America&sensor=false

    ## Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Las%20Vegas,United%20States&sensor=false

    ## Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Brooklyn,USA&sensor=false

    ## Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Champaign,%20IL,USA&sensor=false

    ## Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Hong%20Kong,China&sensor=false

    ## Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=NYC,US&sensor=false

    ## Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=San%20Diego,USA&sensor=false

    ## Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=State%20College,USA&sensor=false

    ## Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Santa%20Barbara,US&sensor=false

    ## Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Santo%20Domingo,Dominican%20Republic&sensor=false

    ## Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=New%20York,USA&sensor=false

    ## Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Chengdu,China&sensor=false

    ## Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Bangkok,Thailand&sensor=false

    ## Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=BEIJING,CHINA&sensor=false

    ## Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=State%20college,USA&sensor=false

    ## Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Berkeley,US&sensor=false

    ## Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=New%20York,United%20States&sensor=false

    ## Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=West%20Lafayette,USA&sensor=false

    ## Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Hubei,China&sensor=false

    ## Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Pittsburgh,U.S.&sensor=false

    ## Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Taipei,Taiwan&sensor=false

    ## Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Minneapolis,USA&sensor=false

    ## Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Changsha,China&sensor=false

    ## Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Seattle,U.S.&sensor=false

    ## Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=wuhan,china&sensor=false

    ## Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Shenzhen,China&sensor=false

``` r
#Generate clusters for lat/lon
fit3 <- kmeans(L2, 2)
```

Part 3
======

``` r
library(vcd)
```

    ## Loading required package: grid

``` r
P1 <- structable(fit2$cluster ~ fit3$cluster)
mosaic(P1, shade=TRUE, legend=TRUE) 
```

![](Assignment_3_Abdul_Abad_Final_Submission_files/figure-markdown_github/unnamed-chunk-15-1.png)

``` r
#This shows how much overlap there are between the groups of clusters
```
