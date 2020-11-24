# EXAM-2

# First Part ( calculator used )
1)
a- 0.5398
b-4.1348E^-7
c-0.1770
d-(24.45,3.55)
e-0.122681
f-1.418596


2)
there is no significance
the t-stat = 1.027322654
the p-value= 0.3056922123
df = 174.2878548

3) tstat = 7.3385
   pvalue = 2.175951E^-13






attach(acs2017_ny)
The following objects are masked from datuse (pos = 4):

    AfAm, AGE, Amindian, ANCESTR1, ANCESTR1D, ANCESTR2, ANCESTR2D,
    Asian, below_150poverty, below_200poverty, below_povertyline,
    BPL, BPLD, BUILTYR2, CITIZEN, CLASSWKR, CLASSWKRD, Commute_bus,
    Commute_car, Commute_other, Commute_rail, Commute_subway,
    COSTELEC, COSTFUEL, COSTGAS, COSTWATR, DEGFIELD, DEGFIELD2,
    DEGFIELD2D, DEGFIELDD, DEPARTS, EDUC, educ_advdeg, educ_college,
    educ_hs, educ_nohs, educ_somecoll, EDUCD, EMPSTAT, EMPSTATD,
    FAMSIZE, female, foodstamps, FOODSTMP, FTOTINC, FUELHEAT, GQ,
    has_AnyHealthIns, has_PvtHealthIns, HCOVANY, HCOVPRIV, HHINCOME,
    Hisp_Cuban, Hisp_DomR, Hisp_Mex, Hisp_PR, HISPAN, HISPAND,
    Hispanic, in_Bronx, in_Brooklyn, in_Manhattan, in_Nassau, in_NYC,
    in_Queens, in_StatenI, in_Westchester, INCTOT, INCWAGE, IND,
    LABFORCE, LINGISOL, MARST, MIGCOUNTY1, MIGPLAC1, MIGPUMA1,
    MIGRATE1, MIGRATE1D, MORTGAGE, NCHILD, NCHLT5, OCC, OWNCOST,
    OWNERSHP, OWNERSHPD, POVERTY, PUMA, PWPUMA00, RACE, race_oth,
    RACED, RELATE, RELATED, RENT, ROOMS, SCHOOL, SEX, SSMC, TRANTIME,
    TRANWORK, UHRSWORK, UNITSSTR, unmarried, veteran, VETSTAT,
    VETSTATD, white, WKSWORK2, YRSUSA1

The following objects are masked from datuse (pos = 5):

    AfAm, AGE, Amindian, ANCESTR1, ANCESTR1D, ANCESTR2, ANCESTR2D,
    Asian, below_150poverty, below_200poverty, below_povertyline,
    BPL, BPLD, BUILTYR2, CITIZEN, CLASSWKR, CLASSWKRD, Commute_bus,
    Commute_car, Commute_other, Commute_rail, Commute_subway,
    COSTELEC, COSTFUEL, COSTGAS, COSTWATR, DEGFIELD, DEGFIELD2,
    DEGFIELD2D, DEGFIELDD, DEPARTS, EDUC, educ_advdeg, educ_college,
    educ_hs, educ_nohs, educ_somecoll, EDUCD, EMPSTAT, EMPSTATD,
    FAMSIZE, female, foodstamps, FOODSTMP, FTOTINC, FUELHEAT, GQ,
    has_AnyHealthIns, has_PvtHealthIns, HCOVANY, HCOVPRIV, HHINCOME,
    Hisp_Cuban, Hisp_DomR, Hisp_Mex, Hisp_PR, HISPAN, HISPAND,
    Hispanic, in_Bronx, in_Brooklyn, in_Manhattan, in_Nassau, in_NYC,
    in_Queens, in_StatenI, in_Westchester, INCTOT, INCWAGE, IND,
    LABFORCE, LINGISOL, MARST, MIGCOUNTY1, MIGPLAC1, MIGPUMA1,
    MIGRATE1, MIGRATE1D, MORTGAGE, NCHILD, NCHLT5, OCC, OWNCOST,
    OWNERSHP, OWNERSHPD, POVERTY, PUMA, PWPUMA00, RACE, race_oth,
    RACED, RELATE, RELATED, RENT, ROOMS, SCHOOL, SEX, SSMC, TRANTIME,
    TRANWORK, UHRSWORK, UNITSSTR, unmarried, veteran, VETSTAT,
    VETSTATD, white, WKSWORK2, YRSUSA1

> usevar<- (AGE>=18) & ( AGE<=55) & (LABFORCE==1)
> datuse<- subset(acs2017_ny,usevar)
> detach()
> attach(datuse)
The following objects are masked from datuse (pos = 4):

    AfAm, AGE, Amindian, ANCESTR1, ANCESTR1D, ANCESTR2, ANCESTR2D,
    Asian, below_150poverty, below_200poverty, below_povertyline,
    BPL, BPLD, BUILTYR2, CITIZEN, CLASSWKR, CLASSWKRD, Commute_bus,
    Commute_car, Commute_other, Commute_rail, Commute_subway,
    COSTELEC, COSTFUEL, COSTGAS, COSTWATR, DEGFIELD, DEGFIELD2,
    DEGFIELD2D, DEGFIELDD, DEPARTS, EDUC, educ_advdeg, educ_college,
    educ_hs, educ_nohs, educ_somecoll, EDUCD, EMPSTAT, EMPSTATD,
    FAMSIZE, female, foodstamps, FOODSTMP, FTOTINC, FUELHEAT, GQ,
    has_AnyHealthIns, has_PvtHealthIns, HCOVANY, HCOVPRIV, HHINCOME,
    Hisp_Cuban, Hisp_DomR, Hisp_Mex, Hisp_PR, HISPAN, HISPAND,
    Hispanic, in_Bronx, in_Brooklyn, in_Manhattan, in_Nassau, in_NYC,
    in_Queens, in_StatenI, in_Westchester, INCTOT, INCWAGE, IND,
    LABFORCE, LINGISOL, MARST, MIGCOUNTY1, MIGPLAC1, MIGPUMA1,
    MIGRATE1, MIGRATE1D, MORTGAGE, NCHILD, NCHLT5, OCC, OWNCOST,
    OWNERSHP, OWNERSHPD, POVERTY, PUMA, PWPUMA00, RACE, race_oth,
    RACED, RELATE, RELATED, RENT, ROOMS, SCHOOL, SEX, SSMC, TRANTIME,
    TRANWORK, UHRSWORK, UNITSSTR, unmarried, veteran, VETSTAT,
    VETSTATD, white, WKSWORK2, YRSUSA1

The following objects are masked from datuse (pos = 5):

    AfAm, AGE, Amindian, ANCESTR1, ANCESTR1D, ANCESTR2, ANCESTR2D,
    Asian, below_150poverty, below_200poverty, below_povertyline,
    BPL, BPLD, BUILTYR2, CITIZEN, CLASSWKR, CLASSWKRD, Commute_bus,
    Commute_car, Commute_other, Commute_rail, Commute_subway,
    COSTELEC, COSTFUEL, COSTGAS, COSTWATR, DEGFIELD, DEGFIELD2,
    DEGFIELD2D, DEGFIELDD, DEPARTS, EDUC, educ_advdeg, educ_college,
    educ_hs, educ_nohs, educ_somecoll, EDUCD, EMPSTAT, EMPSTATD,
    FAMSIZE, female, foodstamps, FOODSTMP, FTOTINC, FUELHEAT, GQ,
    has_AnyHealthIns, has_PvtHealthIns, HCOVANY, HCOVPRIV, HHINCOME,
    Hisp_Cuban, Hisp_DomR, Hisp_Mex, Hisp_PR, HISPAN, HISPAND,
    Hispanic, in_Bronx, in_Brooklyn, in_Manhattan, in_Nassau, in_NYC,
    in_Queens, in_StatenI, in_Westchester, INCTOT, INCWAGE, IND,
    LABFORCE, LINGISOL, MARST, MIGCOUNTY1, MIGPLAC1, MIGPUMA1,
    MIGRATE1, MIGRATE1D, MORTGAGE, NCHILD, NCHLT5, OCC, OWNCOST,
    OWNERSHP, OWNERSHPD, POVERTY, PUMA, PWPUMA00, RACE, race_oth,
    RACED, RELATE, RELATED, RENT, ROOMS, SCHOOL, SEX, SSMC, TRANTIME,
    TRANWORK, UHRSWORK, UNITSSTR, unmarried, veteran, VETSTAT,
    VETSTATD, white, WKSWORK2, YRSUSA1

> #the criteria put into play is the AGE. we chose AGE and limited between 18 and 15 to ensure that the population be able pertain to the Labor Market. Although it is 16 but we chose 18 to maake sure that the individual is up to chose for his own.
> also we added Labor force constraint to make sure that those inside are those who are in 
Error: unexpected symbol in "also we"
> t.test(female)

	One Sample t-test

data:  female
t = 167.06, df = 21604, p-value < 2.2e-16
alternative hypothesis: true mean is not equal to 0
95 percent confidence interval:
 0.5570524 0.5702792
sample estimates:
mean of x 
0.5636658 

> model1<-lm(UHRSWORK~AGE+I(AGE^2) +female+  AfAm+ I(female*AfAm)+ I(female*educ_college) +NCHILD + educ_nohs+educ_hs+educ_college +educ_advdeg, data = datuse)
> summary(model1)

Call:
lm(formula = UHRSWORK ~ AGE + I(AGE^2) + female + AfAm + I(female * 
    AfAm) + I(female * educ_college) + NCHILD + educ_nohs + educ_hs + 
    educ_college + educ_advdeg, data = datuse)

Residuals:
    Min      1Q  Median      3Q     Max 
-12.494  -6.667  -3.986  -1.390  92.400 

Coefficients:
                           Estimate Std. Error t value Pr(>|t|)    
(Intercept)              16.7108074  0.8921230  18.732  < 2e-16 ***
AGE                      -0.3927106  0.0562387  -6.983 2.97e-12 ***
I(AGE^2)                  0.0034988  0.0007762   4.508 6.58e-06 ***
female                   -2.0949684  0.2083633 -10.054  < 2e-16 ***
AfAm                     -1.7545933  0.3146411  -5.576 2.48e-08 ***
I(female * AfAm)          1.0308215  0.4508810   2.286 0.022250 *  
I(female * educ_college) -1.4898454  0.5717319  -2.606 0.009171 ** 
NCHILD                   -0.3129426  0.0823715  -3.799 0.000146 ***
educ_nohs                -3.3396713  0.2656798 -12.570  < 2e-16 ***
educ_hs                  -1.3390936  0.2159637  -6.201 5.73e-10 ***
educ_college              1.9814533  0.4959988   3.995 6.49e-05 ***
educ_advdeg               1.8674210  0.4272750   4.371 1.25e-05 ***
---
Signif. codes:  0 ‘***’ 0.001 ‘**’ 0.01 ‘*’ 0.05 ‘.’ 0.1 ‘ ’ 1

Residual standard error: 12.42 on 21593 degrees of freedom
Multiple R-squared:  0.04958,	Adjusted R-squared:  0.0491 
F-statistic: 102.4 on 11 and 21593 DF,  p-value: < 2.2e-16

> 
> anova(model1)
Analysis of Variance Table

Response: UHRSWORK
                            Df  Sum Sq Mean Sq  F value    Pr(>F)    
AGE                          1   93970   93970 609.0399 < 2.2e-16 ***
I(AGE^2)                     1    6001    6001  38.8908 4.565e-10 ***
female                       1   16417   16417 106.4015 < 2.2e-16 ***
AfAm                         1    8450    8450  54.7637 1.409e-13 ***
I(female * AfAm)             1    1034    1034   6.7045 0.0096237 ** 
I(female * educ_college)     1    3370    3370  21.8441 2.975e-06 ***
NCHILD                       1    2326    2326  15.0775 0.0001035 ***
educ_nohs                    1   24479   24479 158.6536 < 2.2e-16 ***
educ_hs                      1   13001   13001  84.2614 < 2.2e-16 ***
educ_college                 1    1813    1813  11.7499 0.0006096 ***
educ_advdeg                  1    2947    2947  19.1016 1.245e-05 ***
Residuals                21593 3331621     154                       
---
Signif. codes:  0 ‘***’ 0.001 ‘**’ 0.01 ‘*’ 0.05 ‘.’ 0.1 ‘ ’ 1

the anovva table shows the significance of all my variabes

> predicted <-data.frame(AGE=30, female=0,AfAm=0,NCHILD=0,educ_nohs=1,educ_hs=0, educ_college=0,educ_advdeg=0)
> modelpredict<-predict(model1,newdata = predicted)
> summary(modelpredict)
   Min. 1st Qu.  Median    Mean 3rd Qu.    Max. 
  4.739   4.739   4.739   4.739   4.739   4.739 
> datafor<-data.frame(datuse$UHRSWORK,
+            datuse$AGE,
+            datuse$female,
+            datuse$AfAm,
+            datuse$educ_nohs,
+            datuse$educ_hs,
+            datuse$educ_college,
+            datuse$educ_advdeg,
+            datuse$NCHILD)
> 
> names(datafor)<-c("UHRSWORK",
+                   "female",
+                   "Afam",
+                   "educ_nohs",
+                   "educ_hs)",
+                   "educ_college",
+                   "educ_advdeg",
+                   "NCHILD")
>            
> require("standardize")
> set.seed(54321)
> NN <- length(datafor$UHRSWOK)
> restrict_1 <- (runif(NN) < 0.8) # use 10% as training data
> summary(restrict_1)
   Mode 
logical 
> dat_train <- subset(datafor, restrict_1)
> dat_test <- subset(datafor, !restrict_1)
> sobj <- standardize(UHRSWORK~AGE+I(AGE^2) +female+  AfAm+ I(female*AfAm)+ I(female*educ_college) +NCHILD + educ_nohs+educ_hs+educ_college +educ_advdeg, data = datuse)
> 
> s_dat_test <- predict(sobj, dat_test)
Error in `[<-.data.frame`(`*tmp*`, names(p)[-1], value = list(AGE = c(0.897663337279671,  : 
  replacement element 1 is a matrix/data frame of 21605 rows, need 0
> UHRSW<-UHRSWORK>=35
> 
> modellogit1<- glm(UHRSW~ AGE + I(AGE^2) + female + educ_nohs+ educ_hs + NCHILD + AfAm ,family = binomial, data= datuse)
> summary(modellogit1)

Call:
glm(formula = UHRSW ~ AGE + I(AGE^2) + female + educ_nohs + educ_hs + 
    NCHILD + AfAm, family = binomial, data = datuse)

Deviance Residuals: 
    Min       1Q   Median       3Q      Max  
-0.6184  -0.4642  -0.3695  -0.2869   2.9240  

Coefficients:
              Estimate Std. Error z value Pr(>|z|)    
(Intercept) -1.7156165  0.2682886  -6.395 1.61e-10 ***
AGE          0.0184666  0.0171821   1.075 0.282483    
I(AGE^2)    -0.0005371  0.0002439  -2.202 0.027664 *  
female      -0.5751570  0.0543272 -10.587  < 2e-16 ***
educ_nohs   -1.0067528  0.0901165 -11.172  < 2e-16 ***
educ_hs     -0.4299838  0.0551333  -7.799 6.24e-15 ***
NCHILD      -0.1302141  0.0315352  -4.129 3.64e-05 ***
AfAm        -0.2647732  0.0736156  -3.597 0.000322 ***
---
Signif. codes:  0 ‘***’ 0.001 ‘**’ 0.01 ‘*’ 0.05 ‘.’ 0.1 ‘ ’ 1

(Dispersion parameter for binomial family taken to be 1)

    Null deviance: 11956  on 21604  degrees of freedom
Residual deviance: 11461  on 21597  degrees of freedom
AIC: 11477

Number of Fisher Scoring iterations: 6

> 
> anova(modellogit1)
Analysis of Deviance Table

Model: binomial, link: logit

Response: UHRSW

Terms added sequentially (first to last)


          Df Deviance Resid. Df Resid. Dev
NULL                      21604      11956
AGE        1  171.477     21603      11784
I(AGE^2)   1    0.333     21602      11784
female     1  115.253     21601      11668
educ_nohs  1  111.519     21600      11557
educ_hs    1   66.612     21599      11490
NCHILD     1   15.687     21598      11475
AfAm       1   13.587     21597      11461
> df = 174.287854
