Rendering a basic R script
================
Jared Parrish
September 11, 2020

When we add the special characters and select our output style we can
render markdowns to GitHub.  
For this example we will use the VADeaths dataset dataset `VADeaths`.

``` r
print(VADeaths)
```

    ##       Rural Male Rural Female Urban Male Urban Female
    ## 50-54       11.7          8.7       15.4          8.4
    ## 55-59       18.1         11.7       24.3         13.6
    ## 60-64       26.9         20.3       37.0         19.3
    ## 65-69       41.0         30.9       54.6         35.1
    ## 70-74       66.0         54.3       71.1         50.0

``` r
## We can add comments to the code directly - Let's summarize these data.
summary(VADeaths)
```

    ##    Rural Male     Rural Female     Urban Male     Urban Female  
    ##  Min.   :11.70   Min.   : 8.70   Min.   :15.40   Min.   : 8.40  
    ##  1st Qu.:18.10   1st Qu.:11.70   1st Qu.:24.30   1st Qu.:13.60  
    ##  Median :26.90   Median :20.30   Median :37.00   Median :19.30  
    ##  Mean   :32.74   Mean   :25.18   Mean   :40.48   Mean   :25.28  
    ##  3rd Qu.:41.00   3rd Qu.:30.90   3rd Qu.:54.60   3rd Qu.:35.10  
    ##  Max.   :66.00   Max.   :54.30   Max.   :71.10   Max.   :50.00

We can use usual markdown syntax to make things **bold** or *italics*.
We can even make inline statments. Let’s use an example`dotchart()` from
the `VADeaths` data to add a visual.

``` r
dotchart(VADeaths, main = "Death Rates in Virginia - 1940")
```

![](Rmkdwn_eg_files/figure-gfm/dotchart-1.png)<!-- -->

to knit this we can select File \> Knit Document or Cntl+Shift+K
