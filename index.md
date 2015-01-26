---
title       : Smart Phone Cover Glass Scratch Test
subtitle    : A Shiny App for Accurate Data Reporting and Reproducible Statistical Analysis
author      : Jun Xie, Data Scientist
job         : Touch Panel Product Engineering
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Motivation

1. Scratch damage of smart phone cover glass is one of the major issues for both users and vendors. 
2. Novel materials are under development to improve anti-scratch performance. Scratch tests being conducted in various locales around the world generate constant streams of data. 
3. A shiny app is being developed in order to record scratch-test data accurately along with test conditions and provide statistical data analysis instantly to guide R&D efforts. 

--- .class #id 

## Shiny App
### The user interface consists of two parts 

1. A Sidebar panel for recording tests conditions and taking other user inputs. 
2. A Main panal with multiple tabs that display data plots or analysis results.


<img src = "scratchtest_app_small.jpg" width=500>

--- .class #id

## Data Analysis
### Data analysis results are reported under the "Summary" tab.

At present the app only performs simple statiscal data analysis, reporting the results under the "Summary" tab. With additional develpment time, advanced analysis features will be incorporated.


```
## $`1`
##    Min. 1st Qu.  Median    Mean 3rd Qu.    Max. 
##   49.03   55.55   59.86   61.17   66.65   78.39 
## 
## $`2`
##    Min. 1st Qu.  Median    Mean 3rd Qu.    Max. 
##   46.22   55.60   60.34   60.59   64.03   87.92 
## 
## $`3`
##    Min. 1st Qu.  Median    Mean 3rd Qu.    Max. 
##   38.65   52.22   59.04   58.63   65.87   79.01
```

--- .class #id

## Future Development
### Plan to incorporate advanced features such as

1. Bootstrapping to study noisy data sets
2. Unsupervised learning to provide better understanding of test performance
3. Anormaly detection to support high-volume production
