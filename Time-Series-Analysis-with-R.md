Time Series Analysis (ARIMA) with R
================
Leopoldine Mirtil

### Disclaimer

This analysis was done as part of the “Time Series Analysis (ARIMA) with
R” guided project offered on Coursera.com and taught by instructor
Barsha Saha.

### Objective

Understand the pattern of the time series data, select the best fit
model and forecast

### Load Data

``` r
data('EuStockMarkets')
```

### Convert Data to Time Series Format

![](Time-Series-Analysis-with-R_files/figure-gfm/unnamed-chunk-2-1.png)<!-- -->

### ARIMA Model

#### Exploratory Analysis for Time Series Components

![](Time-Series-Analysis-with-R_files/figure-gfm/unnamed-chunk-3-1.png)<!-- -->

#### Unit Root Test

    ## 
    ## ####################### 
    ## # KPSS Unit Root Test # 
    ## ####################### 
    ## 
    ## Test is of type: tau with 8 lags. 
    ## 
    ## Value of test-statistic is: 3.6982 
    ## 
    ## Critical value for a significance level of: 
    ##                 10pct  5pct 2.5pct  1pct
    ## critical values 0.119 0.146  0.176 0.216

![](Time-Series-Analysis-with-R_files/figure-gfm/unnamed-chunk-4-1.png)<!-- -->

#### Remove Seasonality

![](Time-Series-Analysis-with-R_files/figure-gfm/unnamed-chunk-5-1.png)<!-- -->

### Model Fit

![](Time-Series-Analysis-with-R_files/figure-gfm/unnamed-chunk-6-1.png)<!-- -->![](Time-Series-Analysis-with-R_files/figure-gfm/unnamed-chunk-6-2.png)<!-- -->

#### Sample Test

![](Time-Series-Analysis-with-R_files/figure-gfm/unnamed-chunk-7-1.png)<!-- -->

#### Best Fit Model

![](Time-Series-Analysis-with-R_files/figure-gfm/unnamed-chunk-9-1.png)<!-- -->

### Forecast

![](Time-Series-Analysis-with-R_files/figure-gfm/unnamed-chunk-10-1.png)<!-- -->
