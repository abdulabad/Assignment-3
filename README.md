# Assignment-3
Assignment 3 by Abdul Abad
Show in New WindowClear OutputExpand/Collapse Output Error: Incomplete expression: K2 <-

ConsoleD:/Core Methods in Educational Data Mining/assignment3-master/

R version 3.5.1 (2018-07-02) -- "Feather Spray" Copyright (C) 2018 The R Foundation for Statistical Computing Platform: x86_64-w64-mingw32/x64 (64-bit)

R is free software and comes with ABSOLUTELY NO WARRANTY. You are welcome to redistribute it under certain conditions. Type 'license()' or 'licence()' for distribution details.

R is a collaborative project with many contributors. Type 'contributors()' for more information and 'citation()' on how to cite R or R packages in publications.

Type 'demo()' for some demos, 'help()' for on-line help, or 'help.start()' for an HTML browser interface to help. Type 'q()' to quit R.

library() getwd() [1] "C:/Users/Grimp/OneDrive/Documents/Assignment-3" setwd(D:/Core Methods in Educational Data Mining/assignment3-master) Error: unexpected '/' in "setwd(D:/" setwd("D:/Core Methods in Educational Data Mining/assignment3-master") K1 <- read.csv("Class_Motivation.csv, header=TRUE") Error in file(file, "rt") : cannot open the connection In addition: Warning message: In file(file, "rt") : cannot open file 'Class_Motivation.csv, header=TRUE': No such file or directory K1 <- read.csv(Class_Motivation.csv, header=TRUE) Error in read.table(file = file, header = header, sep = sep, quote = quote, : object 'Class_Motivation.csv' not found getwd() [1] "D:/Core Methods in Educational Data Mining/assignment3-master" K1 <- read.csv("Class_Motivation.csv, header = TRUE") Error in file(file, "rt") : cannot open the connection In addition: Warning message: In file(file, "rt") : cannot open file 'Class_Motivation.csv, header = TRUE': No such file or directory K1 <- read.csv("Class_Motivation.csv", header = TRUE)

K2 <- + Error: Incomplete expression: K2 <- library(dplyr)
Attaching package: ‘dplyr’

The following objects are masked from ‘package:stats’:

filter, lag
The following objects are masked from ‘package:base’:

intersect, setdiff, setequal, union
library(tidyr) Error in library(tidyr) : there is no package called ‘tidyr’ install.packages(tidyr) Error in install.packages : object 'tidyr' not found install.packages(ggplot2) Error in install.packages : object 'ggplot2' not found library(ggplot2) Error in library(ggplot2) : there is no package called ‘ggplot2’ library("ggplot2") Error in library("ggplot2") : there is no package called ‘ggplot2’ install.packages("tidyr") Installing package into ‘C:/Users/Grimp/OneDrive/Documents/R/win-library/3.5’ (as ‘lib’ is unspecified) trying URL 'https://cran.rstudio.com/bin/windows/contrib/3.5/tidyr_0.8.2.zip' Content type 'application/zip' length 948618 bytes (926 KB) downloaded 926 KB
package ‘tidyr’ successfully unpacked and MD5 sums checked

The downloaded binary packages are in C:8_packages > install.packages("dplyr") Error in install.packages : Updating loaded packages

Restarting R session...

install.packages("dplyr") Installing package into ‘C:/Users/Grimp/OneDrive/Documents/R/win-library/3.5’ (as ‘lib’ is unspecified) trying URL 'https://cran.rstudio.com/bin/windows/contrib/3.5/dplyr_0.7.8.zip' Content type 'application/zip' length 3069237 bytes (2.9 MB) downloaded 2.9 MB
package ‘dplyr’ successfully unpacked and MD5 sums checked

The downloaded binary packages are in C:_packages > install.packages("ggplot2") Installing package into ‘C:/Users/Grimp/OneDrive/Documents/R/win-library/3.5’ (as ‘lib’ is unspecified) also installing the dependencies ‘colorspace’, ‘labeling’, ‘munsell’, ‘RColorBrewer’, ‘gtable’, ‘lazyeval’, ‘plyr’, ‘reshape2’, ‘scales’, ‘viridisLite’

trying URL 'https://cran.rstudio.com/bin/windows/contrib/3.5/colorspace_1.3-2.zip' Content type 'application/zip' length 527783 bytes (515 KB) downloaded 515 KB

trying URL 'https://cran.rstudio.com/bin/windows/contrib/3.5/labeling_0.3.zip' Content type 'application/zip' length 61841 bytes (60 KB) downloaded 60 KB

trying URL 'https://cran.rstudio.com/bin/windows/contrib/3.5/munsell_0.5.0.zip' Content type 'application/zip' length 243626 bytes (237 KB) downloaded 237 KB

trying URL 'https://cran.rstudio.com/bin/windows/contrib/3.5/RColorBrewer_1.1-2.zip' Content type 'application/zip' length 55444 bytes (54 KB) downloaded 54 KB

trying URL 'https://cran.rstudio.com/bin/windows/contrib/3.5/gtable_0.2.0.zip' Content type 'application/zip' length 85078 bytes (83 KB) downloaded 83 KB

trying URL 'https://cran.rstudio.com/bin/windows/contrib/3.5/lazyeval_0.2.1.zip' Content type 'application/zip' length 166885 bytes (162 KB) downloaded 162 KB

trying URL 'https://cran.rstudio.com/bin/windows/contrib/3.5/plyr_1.8.4.zip' Content type 'application/zip' length 1297630 bytes (1.2 MB) downloaded 1.2 MB

trying URL 'https://cran.rstudio.com/bin/windows/contrib/3.5/reshape2_1.4.3.zip' Content type 'application/zip' length 625975 bytes (611 KB) downloaded 611 KB

trying URL 'https://cran.rstudio.com/bin/windows/contrib/3.5/scales_1.0.0.zip' Content type 'application/zip' length 1064417 bytes (1.0 MB) downloaded 1.0 MB

trying URL 'https://cran.rstudio.com/bin/windows/contrib/3.5/viridisLite_0.3.0.zip' Content type 'application/zip' length 60488 bytes (59 KB) downloaded 59 KB

trying URL 'https://cran.rstudio.com/bin/windows/contrib/3.5/ggplot2_3.1.0.zip' Content type 'application/zip' length 3622746 bytes (3.5 MB) downloaded 3.5 MB

package ‘colorspace’ successfully unpacked and MD5 sums checked package ‘labeling’ successfully unpacked and MD5 sums checked package ‘munsell’ successfully unpacked and MD5 sums checked package ‘RColorBrewer’ successfully unpacked and MD5 sums checked package ‘gtable’ successfully unpacked and MD5 sums checked package ‘lazyeval’ successfully unpacked and MD5 sums checked package ‘plyr’ successfully unpacked and MD5 sums checked package ‘reshape2’ successfully unpacked and MD5 sums checked package ‘scales’ successfully unpacked and MD5 sums checked package ‘viridisLite’ successfully unpacked and MD5 sums checked package ‘ggplot2’ successfully unpacked and MD5 sums checked

The downloaded binary packages are in C:_packages > K1 id motivation1 motivation2 motivation3 motivation4 motivation5 1 10005216 2 2 2 2 2 2 10033216 3 NA 3 NA NA 3 10004216 1 2 1 2 2 4 10008216 1 2 1 2 NA 5 10026216 3 NA 3 NA NA 6 10014216 2 NA 2 NA 2 7 10021216 2 2 2 2 2 8 10013216 2 NA 2 NA 1 9 10035216 2 3 2 3 NA 10 10015216 2 2 2 2 2 11 10031216 1 1 1 1 NA 12 10007216 2 1 2 1 2 13 10010216 2 2 2 2 NA 14 10020216 2 3 2 3 1 15 10002216 1 1 1 1 4 16 10011216 2 2 2 2 NA 17 10023216 1 1 1 1 3 18 10028216 1 1 1 1 1 19 10028216 1 1 1 1 1 20 10034216 3 2 3 2 2 21 10003216 2 NA 2 NA NA 22 10029216 2 2 2 2 5 23 10022216 1 3 1 3 NA 24 10006216 1 1 1 1 NA 25 10009216 1 1 1 1 2 26 10018216 1 2 1 2 4 27 10018216 1 2 1 2 3 28 10018216 1 2 1 2 4 29 10018216 1 2 1 2 3 30 10018216 1 2 1 2 4 31 10018216 1 2 1 2 3 32 10018216 1 2 1 2 4 33 10018216 1 2 1 2 3 34 10027216 1 1 1 1 1 35 10025216 2 2 2 2 2 36 10019216 1 NA 1 NA NA 37 10032216 3 NA 3 NA NA 38 10017216 3 NA 3 NA 3 > > K3 <- na.omit(K2) #This command create a data frame with only those people with no missing values. It "omits" all rows with missing values, also known as a "listwise deletion". EG - It runs down the list deleting rows as it goes. Error in na.omit(K2) : object 'K2' not found > > K2 <- dplyr :: select(K1, 2:6) > > K3 <- na.omit(K2) #This command create a data frame with only those people with no missing values. It "omits" all rows with missing values, also known as a "listwise deletion". EG - It runs down the list deleting rows as it goes. > > > K3 <- scale(K3) > > fit <- kmeans(K3, 2) > fitcluster137101214151718192022252627282930313233343522221211112212222222212 > K4 < −*data.frame(K3, fi**t*cluster) > names(K4) <- c("1", "2", "3", "4", "5", "cluster") > K5 <-tidyr :: gather(K4, "week", "motivation", 1:5) > K6 <- K5 %>% group_by(week, cluster) Error in K5 %>% group_by(week, cluster) : could not find function "%>%" > K6 <- summarise(K6, avg = mean(motivation)) Error in summarise(K6, avg = mean(motivation)) : could not find function "summarise" > K6 <- K5 %>% group_by(week, cluster) Error in K5 %>% group_by(week, cluster) : could not find function "%>%" > K6 <- summarize(K6, avg = mean(motivation)) Error in summarize(K6, avg = mean(motivation)) : could not find function "summarize" > install.packages("plyr") Installing package into ‘C:/Users/Grimp/OneDrive/Documents/R/win-library/3.5’ (as ‘lib’ is unspecified) trying URL 'https://cran.rstudio.com/bin/windows/contrib/3.5/plyr_1.8.4.zip' Content type 'application/zip' length 1297630 bytes (1.2 MB) downloaded 1.2 MB

package ‘plyr’ successfully unpacked and MD5 sums checked

The downloaded binary packages are in C:_packages > K6 <- summarise(K6, avg = mean(motivation)) Error in summarise(K6, avg = mean(motivation)) : could not find function "summarise" > library(dplyr)

Attaching package: ‘dplyr’

The following objects are masked from ‘package:stats’:

filter, lag
The following objects are masked from ‘package:base’:

intersect, setdiff, setequal, union
library(ggplot2) library(tidyr) K6 <- summarise(K6, avg = mean(motivation)) Error in summarise(K6, avg = mean(motivation)) : object 'K6' not found K6 <- K5 %>% group_by(week, cluster) K6 <- summarise(K6, avg = mean(motivation)) K6week < −as.numeric(K6week) K6cluster < −as.factor(K6cluster) ggplot(K6, aes(week, avg, colour = cluster)) + geom_line() + xlab("Week") + ylab("Average Motivation")

K7 <- dplyr::count(K4, cluster) library(tidyverse) Error in library(tidyverse) : there is no package called ‘tidyverse’ install.packages("tidyverse") Installing package into ‘C:/Users/Grimp/OneDrive/Documents/R/win-library/3.5’ (as ‘lib’ is unspecified) also installing the dependencies ‘ps’, ‘processx’, ‘generics’, ‘DBI’, ‘callr’, ‘clipr’, ‘fs’, ‘selectr’, ‘broom’, ‘dbplyr’, ‘forcats’, ‘haven’, ‘lubridate’, ‘modelr’, ‘reprex’, ‘rvest’, ‘xml2’
There are binary versions available but the source versions are later: binary source needs_compilation processx 3.2.0 3.2.1 TRUE broom 0.5.0 0.5.1 FALSE

Binaries will be installed trying URL 'https://cran.rstudio.com/bin/windows/contrib/3.5/ps_1.2.1.zip' Content type 'application/zip' length 302519 bytes (295 KB) downloaded 295 KB

trying URL 'https://cran.rstudio.com/bin/windows/contrib/3.5/processx_3.2.0.zip' Content type 'application/zip' length 300367 bytes (293 KB) downloaded 293 KB

trying URL 'https://cran.rstudio.com/bin/windows/contrib/3.5/generics_0.0.2.zip' Content type 'application/zip' length 63713 bytes (62 KB) downloaded 62 KB

trying URL 'https://cran.rstudio.com/bin/windows/contrib/3.5/DBI_1.0.0.zip' Content type 'application/zip' length 887657 bytes (866 KB) downloaded 866 KB

trying URL 'https://cran.rstudio.com/bin/windows/contrib/3.5/callr_3.0.0.zip' Content type 'application/zip' length 201143 bytes (196 KB) downloaded 196 KB

trying URL 'https://cran.rstudio.com/bin/windows/contrib/3.5/clipr_0.4.1.zip' Content type 'application/zip' length 37400 bytes (36 KB) downloaded 36 KB

trying URL 'https://cran.rstudio.com/bin/windows/contrib/3.5/fs_1.2.6.zip' Content type 'application/zip' length 954784 bytes (932 KB) downloaded 932 KB

trying URL 'https://cran.rstudio.com/bin/windows/contrib/3.5/selectr_0.4-1.zip' Content type 'application/zip' length 458519 bytes (447 KB) downloaded 447 KB

trying URL 'https://cran.rstudio.com/bin/windows/contrib/3.5/dbplyr_1.2.2.zip' Content type 'application/zip' length 533175 bytes (520 KB) downloaded 520 KB

trying URL 'https://cran.rstudio.com/bin/windows/contrib/3.5/forcats_0.3.0.zip' Content type 'application/zip' length 209541 bytes (204 KB) downloaded 204 KB

trying URL 'https://cran.rstudio.com/bin/windows/contrib/3.5/haven_2.0.0.zip' Content type 'application/zip' length 995534 bytes (972 KB) downloaded 972 KB

trying URL 'https://cran.rstudio.com/bin/windows/contrib/3.5/lubridate_1.7.4.zip' Content type 'application/zip' length 1569099 bytes (1.5 MB) downloaded 1.5 MB

trying URL 'https://cran.rstudio.com/bin/windows/contrib/3.5/modelr_0.1.2.zip' Content type 'application/zip' length 196957 bytes (192 KB) downloaded 192 KB

trying URL 'https://cran.rstudio.com/bin/windows/contrib/3.5/reprex_0.2.1.zip' Content type 'application/zip' length 405165 bytes (395 KB) downloaded 395 KB

trying URL 'https://cran.rstudio.com/bin/windows/contrib/3.5/rvest_0.3.2.zip' Content type 'application/zip' length 881335 bytes (860 KB) downloaded 860 KB

trying URL 'https://cran.rstudio.com/bin/windows/contrib/3.5/xml2_1.2.0.zip' Content type 'application/zip' length 3605403 bytes (3.4 MB) downloaded 3.4 MB

trying URL 'https://cran.rstudio.com/bin/windows/contrib/3.5/tidyverse_1.2.1.zip' Content type 'application/zip' length 92570 bytes (90 KB) downloaded 90 KB

package ‘ps’ successfully unpacked and MD5 sums checked package ‘processx’ successfully unpacked and MD5 sums checked package ‘generics’ successfully unpacked and MD5 sums checked package ‘DBI’ successfully unpacked and MD5 sums checked package ‘callr’ successfully unpacked and MD5 sums checked package ‘clipr’ successfully unpacked and MD5 sums checked package ‘fs’ successfully unpacked and MD5 sums checked package ‘selectr’ successfully unpacked and MD5 sums checked package ‘dbplyr’ successfully unpacked and MD5 sums checked package ‘forcats’ successfully unpacked and MD5 sums checked package ‘haven’ successfully unpacked and MD5 sums checked package ‘lubridate’ successfully unpacked and MD5 sums checked package ‘modelr’ successfully unpacked and MD5 sums checked package ‘reprex’ successfully unpacked and MD5 sums checked package ‘rvest’ successfully unpacked and MD5 sums checked package ‘xml2’ successfully unpacked and MD5 sums checked package ‘tidyverse’ successfully unpacked and MD5 sums checked

The downloaded binary packages are in C:_packages installing the source package ‘broom’

trying URL 'https://cran.rstudio.com/src/contrib/broom_0.5.1.tar.gz' Content type 'application/x-gzip' length 1230196 bytes (1.2 MB) downloaded 1.2 MB

installing source package 'broom' ... ** package 'broom' successfully unpacked and MD5 sums checked ** R ** data *** moving datasets to lazyload DB ** inst ** byte-compile and prepare package for lazy loading ** help *** installing help indices converting help for package 'broom' finding HTML links ... done argument_glossary html
augment.Mclust html
augment.betareg html
augment.coxph html
augment.decomposed.ts html
augment.factanal html
augment.felm html
augment.glm html
Rd warning: C:/Users/Grimp/AppData/Local/Temp/RtmpQFcLK1/R.INSTALL54ac18161c98/broom/man/augment.glm.Rd:28: file link 'residuals.glm' in package 'stats' does not exist and so has been treated as a topic augment.glmRob html
Rd warning: C:/Users/Grimp/AppData/Local/Temp/RtmpQFcLK1/R.INSTALL54ac18161c98/broom/man/augment.glmRob.Rd:28: file link 'residuals.glm' in package 'stats' does not exist and so has been treated as a topic augment.htest html
augment.ivreg html
augment.kmeans html
augment.lm html
Rd warning: C:/Users/Grimp/AppData/Local/Temp/RtmpQFcLK1/R.INSTALL54ac18161c98/broom/man/augment.lm.Rd:30: file link 'residuals.glm' in package 'stats' does not exist and so has been treated as a topic augment.lmRob html
Rd warning: C:/Users/Grimp/AppData/Local/Temp/RtmpQFcLK1/R.INSTALL54ac18161c98/broom/man/augment.lmRob.Rd:28: file link 'residuals.glm' in package 'stats' does not exist and so has been treated as a topic augment.loess html
augment.mjoint html
augment.nlrq html
augment.nls html
augment.plm html
augment.poLCA html
augment.prcomp html
augment.rlm html
Rd warning: C:/Users/Grimp/AppData/Local/Temp/RtmpQFcLK1/R.INSTALL54ac18161c98/broom/man/augment.rlm.Rd:28: file link 'residuals.glm' in package 'stats' does not exist and so has been treated as a topic augment.rq html
augment.rqs html
augment.smooth.spline html
augment.speedlm html
augment.stl html
augment.survreg html
augment_columns html
bootstrap html
brms_tidiers html
broom html
column_glossary html
confint_tidy html
data.frame_tidiers html
durbinWatsonTest_tidiers html
emmeans_tidiers html
finish_glance html
fix_data_frame html
geeglm_tidiers html
glance.Arima html
glance.Gam html
glance.Mclust html
glance.aareg html
glance.betareg html
glance.biglm html
glance.binDesign html
glance.cch html
glance.coxph html
glance.cv.glmnet html
glance.ergm html
glance.factanal html
glance.felm html
glance.fitdistr html
glance.garch html
glance.glm html
glance.glmRob html
glance.glmnet html
glance.gmm html
glance.ivreg html
glance.kmeans html
glance.lavaan html
glance.lm html
glance.lmRob html
glance.lmodel2 html
glance.mjoint html
glance.muhaz html
glance.multinom html
glance.nlrq html
glance.nls html
glance.orcutt html
glance.plm html
glance.poLCA html
glance.pyears html
glance.ridgelm html
Rd warning: C:/Users/Grimp/AppData/Local/Temp/RtmpQFcLK1/R.INSTALL54ac18161c98/broom/man/glance.ridgelm.Rd:48: file link 'select.ridgelm' in package 'MASS' does not exist and so has been treated as a topic glance.rlm html
glance.rq html
glance.smooth.spline html
glance.speedlm html
glance.survdiff html
glance.survexp html
glance.survfit html
glance.survreg html
glance_optim html
insert_NAs html
list_tidiers html
lme4_tidiers html
matrix_tidiers html
mcmc_tidiers html
mgcv_glance_gam html
mgcv_tidy_gam html
nlme_tidiers html
null_tidiers html
Rd warning: C:/Users/Grimp/AppData/Local/Temp/RtmpQFcLK1/R.INSTALL54ac18161c98/broom/man/null_tidiers.Rd:28: file link 'map_df' in package 'purrr' does not exist and so has been treated as a topic ordinal_tidiers html
reexports html
rowwise_df_tidiers html
rstanarm_tidiers html
sp_tidiers html
sparse_tidiers html
summary_tidiers html
tidy.Arima html
tidy.Gam html
tidy.Kendall html
tidy.Mclust html
tidy.TukeyHSD html
tidy.aareg html
tidy.acf html
Rd warning: C:/Users/Grimp/AppData/Local/Temp/RtmpQFcLK1/R.INSTALL54ac18161c98/broom/man/tidy.acf.Rd:10: file link 'pacf' in package 'stats' does not exist and so has been treated as a topic Rd warning: C:/Users/Grimp/AppData/Local/Temp/RtmpQFcLK1/R.INSTALL54ac18161c98/broom/man/tidy.acf.Rd:11: file link 'ccf' in package 'stats' does not exist and so has been treated as a topic Rd warning: C:/Users/Grimp/AppData/Local/Temp/RtmpQFcLK1/R.INSTALL54ac18161c98/broom/man/tidy.acf.Rd:45: file link 'pacf' in package 'stats' does not exist and so has been treated as a topic Rd warning: C:/Users/Grimp/AppData/Local/Temp/RtmpQFcLK1/R.INSTALL54ac18161c98/broom/man/tidy.acf.Rd:45: file link 'ccf' in package 'stats' does not exist and so has been treated as a topic tidy.anova html
tidy.aov html
tidy.aovlist html
tidy.betareg html
tidy.biglm html
tidy.binDesign html
tidy.binWidth html
tidy.boot html
tidy.btergm html
tidy.cch html
tidy.cld html
tidy.coeftest html
tidy.confint.glht html
tidy.confusionMatrix html
tidy.coxph html
tidy.cv.glmnet html
tidy.density html
tidy.dist html
tidy.ergm html
tidy.factanal html
tidy.felm html
tidy.fitdistr html
tidy.ftable html
tidy.gamlss html
tidy.garch html
tidy.glht html
tidy.glm html
tidy.glmRob html
tidy.glmnet html
tidy.gmm html
tidy.htest html
tidy.ivreg html
tidy.kappa html
tidy.kde html
tidy.kmeans html
tidy.lavaan html
tidy.lm html
tidy.lmRob html
tidy.lmodel2 html
tidy.manova html
tidy.map html
tidy.mjoint html
tidy.mle2 html
tidy.muhaz html
tidy.multinom html
tidy.nlrq html
tidy.nls html
tidy.orcutt html
tidy.pairwise.htest html
tidy.plm html
tidy.poLCA html
tidy.power.htest html
tidy.prcomp html
tidy.pyears html
tidy.rcorr html
tidy.ridgelm html
tidy.rlm html
tidy.roc html
tidy.rq html
tidy.rqs html
tidy.spec html
tidy.speedlm html
tidy.summary.glht html
tidy.survdiff html
tidy.survexp html
tidy.survfit html
tidy.survreg html
tidy.table html
finding level-2 HTML links ... done

tidy.ts html
tidy.zoo html
tidy_irlba html
tidy_optim html
tidy_svd html
tidy_xyz html
vector_tidiers html
*** copying figures ** building package indices ** installing vignettes ** testing if installed package can be loaded *** arch - i386 *** arch - x64
DONE (broom) In R CMD INSTALL

The downloaded source packages are in ‘C:_packages’ > library(tidyverse) -- Attaching packages --------------------------------------- tidyverse 1.2.1 -- v tibble 1.4.2 v purrr 0.2.5 v readr 1.1.1 v stringr 1.3.1 v tibble 1.4.2 v forcats 0.3.0 -- Conflicts ------------------------------------------ tidyverse_conflicts() -- x dplyr::filter() masks stats::filter() x dplyr::lag() masks stats::lag() > > library(tidyverse) > M1 <- read.csv("HUDK405018-cluster.csv") > M2 <- M1[3:47, 20:26] > M2[M2==""] <- NA > M2 <- M2 %>% mutate_all(funs(as.numeric(levels(.))[.])) Warning messages: 1: In evalq(as.numeric(levels(Q2_1))[Q2_1], ) : NAs introduced by coercion 2: In evalq(as.numeric(levels(Q2_2))[Q2_2], ) : NAs introduced by coercion 3: In evalq(as.numeric(levels(Q2_3))[Q2_3], ) : NAs introduced by coercion 4: In evalq(as.numeric(levels(Q2_4))[Q2_4], ) : NAs introduced by coercion 5: In evalq(as.numeric(levels(Q2_5))[Q2_5], ) : NAs introduced by coercion 6: In evalq(as.numeric(levels(Q2_6))[Q2_6], ) : NAs introduced by coercion 7: In evalq(as.numeric(levels(Q2_7))[Q2_7], ) : NAs introduced by coercion > M2 <- na.omit(M2) > fit2 <- kmeans(M2, 3) > L1 <- M1[3:47, 18:19] > L1 <- unite(L1, place, Q1_1, Q1_2, sep = ",") > install.packages("ggmap") Installing package into ‘C:/Users/Grimp/OneDrive/Documents/R/win-library/3.5’ (as ‘lib’ is unspecified) also installing the dependencies ‘maps’, ‘sp’, ‘proto’, ‘RgoogleMaps’, ‘png’, ‘rjson’, ‘mapproj’, ‘jpeg’, ‘geosphere’

trying URL 'https://cran.rstudio.com/bin/windows/contrib/3.5/maps_3.3.0.zip' Content type 'application/zip' length 3694065 bytes (3.5 MB) downloaded 3.5 MB

trying URL 'https://cran.rstudio.com/bin/windows/contrib/3.5/sp_1.3-1.zip' Content type 'application/zip' length 1869183 bytes (1.8 MB) downloaded 1.8 MB

trying URL 'https://cran.rstudio.com/bin/windows/contrib/3.5/proto_1.0.0.zip' Content type 'application/zip' length 471969 bytes (460 KB) downloaded 460 KB

trying URL 'https://cran.rstudio.com/bin/windows/contrib/3.5/RgoogleMaps_1.4.3.zip' Content type 'application/zip' length 903500 bytes (882 KB) downloaded 882 KB

trying URL 'https://cran.rstudio.com/bin/windows/contrib/3.5/png_0.1-7.zip' Content type 'application/zip' length 292444 bytes (285 KB) downloaded 285 KB

trying URL 'https://cran.rstudio.com/bin/windows/contrib/3.5/rjson_0.2.20.zip' Content type 'application/zip' length 577826 bytes (564 KB) downloaded 564 KB

trying URL 'https://cran.rstudio.com/bin/windows/contrib/3.5/mapproj_1.2.6.zip' Content type 'application/zip' length 90414 bytes (88 KB) downloaded 88 KB

trying URL 'https://cran.rstudio.com/bin/windows/contrib/3.5/jpeg_0.1-8.zip' Content type 'application/zip' length 230437 bytes (225 KB) downloaded 225 KB

trying URL 'https://cran.rstudio.com/bin/windows/contrib/3.5/geosphere_1.5-7.zip' Content type 'application/zip' length 977912 bytes (954 KB) downloaded 954 KB

trying URL 'https://cran.rstudio.com/bin/windows/contrib/3.5/ggmap_2.6.1.zip' Content type 'application/zip' length 4673455 bytes (4.5 MB) downloaded 4.5 MB

package ‘maps’ successfully unpacked and MD5 sums checked package ‘sp’ successfully unpacked and MD5 sums checked package ‘proto’ successfully unpacked and MD5 sums checked package ‘RgoogleMaps’ successfully unpacked and MD5 sums checked package ‘png’ successfully unpacked and MD5 sums checked package ‘rjson’ successfully unpacked and MD5 sums checked package ‘mapproj’ successfully unpacked and MD5 sums checked package ‘jpeg’ successfully unpacked and MD5 sums checked package ‘geosphere’ successfully unpacked and MD5 sums checked package ‘ggmap’ successfully unpacked and MD5 sums checked

The downloaded binary packages are in C:_packages > library(ggmap) Google Maps API Terms of Service: http://developers.google.com/maps/terms. Please cite ggmap if you use it: see citation('ggmap') for details. > L2 <- geocode(as.character(L1$place), output = "latlon", source = "dsk") Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Melbourne,Australia&sensor=false Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Boston,US&sensor=false Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Columbus,%20OH,U.S&sensor=false Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Los%20Angeles,USA&sensor=false Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Berkeley,USA&sensor=false Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=San%20Francisco,USA&sensor=false Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Jakarta,Indonesia&sensor=false Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Shanghai,China&sensor=false Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Pittsburgh,USA&sensor=false Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Brooklyn,US&sensor=false Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Eugene,U.S&sensor=false Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Hangzhou,China&sensor=false Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Madison,US&sensor=false Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Appleton,United%20States%20of%20America&sensor=false Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Las%20Vegas,United%20States&sensor=false Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Brooklyn,USA&sensor=false Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Champaign,%20IL,USA&sensor=false Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Hong%20Kong,China&sensor=false Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=NYC,US&sensor=false Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=San%20Diego,USA&sensor=false Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=State%20College,USA&sensor=false Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Santa%20Barbara,US&sensor=false Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Santo%20Domingo,Dominican%20Republic&sensor=false Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=New%20York,USA&sensor=false Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Chengdu,China&sensor=false Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Bangkok,Thailand&sensor=false Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=BEIJING,CHINA&sensor=false Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=State%20college,USA&sensor=false Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Berkeley,US&sensor=false Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=New%20York,United%20States&sensor=false Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=West%20Lafayette,USA&sensor=false Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Hubei,China&sensor=false Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Pittsburgh,U.S.&sensor=false Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Taipei,Taiwan&sensor=false Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Minneapolis,USA&sensor=false Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Changsha,China&sensor=false Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Seattle,U.S.&sensor=false Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=wuhan,china&sensor=false Information from URL : http://www.datasciencetoolkit.org/maps/api/geocode/json?address=Shenzhen,China&sensor=false > fit3 <- kmeans(L2, 2) > install.packages("vcd") Installing package into ‘C:/Users/Grimp/OneDrive/Documents/R/win-library/3.5’ (as ‘lib’ is unspecified) also installing the dependencies ‘zoo’, ‘lmtest’

trying URL 'https://cran.rstudio.com/bin/windows/contrib/3.5/zoo_1.8-4.zip' Content type 'application/zip' length 1098882 bytes (1.0 MB) downloaded 1.0 MB

trying URL 'https://cran.rstudio.com/bin/windows/contrib/3.5/lmtest_0.9-36.zip' Content type 'application/zip' length 359375 bytes (350 KB) downloaded 350 KB

trying URL 'https://cran.rstudio.com/bin/windows/contrib/3.5/vcd_1.4-4.zip' Content type 'application/zip' length 1554888 bytes (1.5 MB) downloaded 1.5 MB

package ‘zoo’ successfully unpacked and MD5 sums checked package ‘lmtest’ successfully unpacked and MD5 sums checked package ‘vcd’ successfully unpacked and MD5 sums checked

The downloaded binary packages are in C:_packages > library(vcd) Loading required package: grid > P1 <- structable(fit2cluster fit3cluster) Error in model.frame.default(formula = ~fit3cluster + fit2cluster) : variable lengths differ (found for 'fit2cluster′) > library(vcd)>P1 < −structable(fit2cluster ~ fit3cluster)Errorinmodel.frame.default(formula =  fit3cluster + fit2cluster):variablelengthsdiffer(*foundfor′fi**t*2cluster')
