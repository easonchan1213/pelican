Title: HelloWorld
Date: 2014-12-03 10:20
Modified: 2014-12-05 19:30
Category: Python
Tags: pelican, publishing
Slug: my-super-post
Authors: YSChan(Eason)
Summary: Just some lil post

This is the content of my super blog post.
```r
library(datasets)
data(airquality)
summary(airquality)
```

```
##      Ozone          Solar.R         Wind            Temp     
##  Min.   :  1.0   Min.   :  7   Min.   : 1.70   Min.   :56.0  
##  1st Qu.: 18.0   1st Qu.:116   1st Qu.: 7.40   1st Qu.:72.0  
##  Median : 31.5   Median :205   Median : 9.70   Median :79.0  
##  Mean   : 42.1   Mean   :186   Mean   : 9.96   Mean   :77.9  
##  3rd Qu.: 63.2   3rd Qu.:259   3rd Qu.:11.50   3rd Qu.:85.0  
##  Max.   :168.0   Max.   :334   Max.   :20.70   Max.   :97.0  
##  NA's   :37      NA's   :7                                   
##      Month           Day      
##  Min.   :5.00   Min.   : 1.0  
##  1st Qu.:6.00   1st Qu.: 8.0  
##  Median :7.00   Median :16.0  
##  Mean   :6.99   Mean   :15.8  
##  3rd Qu.:8.00   3rd Qu.:23.0  
##  Max.   :9.00   Max.   :31.0  
## 
```


Let's first examine how r code being implemented using RMarkdown


```r
pairs(airquality)
```

![plot of chunk unnamed-chunk-2](figure/unnamed-chunk-2.png) 


Here's a lil regression model


```r
library(stats)
fit <- lm(Ozone ~ Wind + Temp + Solar.R, data = airquality)
summary(fit)
```

```
## 
## Call:
## lm(formula = Ozone ~ Wind + Temp + Solar.R, data = airquality)
## 
## Residuals:
##    Min     1Q Median     3Q    Max 
## -40.48 -14.22  -3.55  10.10  95.62 
## 
## Coefficients:
##             Estimate Std. Error t value Pr(>|t|)    
## (Intercept) -64.3421    23.0547   -2.79   0.0062 ** 
## Wind         -3.3336     0.6544   -5.09  1.5e-06 ***
## Temp          1.6521     0.2535    6.52  2.4e-09 ***
## Solar.R       0.0598     0.0232    2.58   0.0112 *  
## ---
## Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1
## 
## Residual standard error: 21.2 on 107 degrees of freedom
##   (42 observations deleted due to missingness)
## Multiple R-squared:  0.606,	Adjusted R-squared:  0.595 
## F-statistic: 54.8 on 3 and 107 DF,  p-value: <2e-16
```


* first
* second
* third






