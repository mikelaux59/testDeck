---
title       : Temperature Conversion
subtitle    : Johns Hopkins Data Products Coursera Course
author      : Mike Laux
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [mathjax,bootstrap,quiz]            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Temperature Converter Overview

1. Demonstrates calculation in server.R
2. Demonstrates user input control
3. Is simple and does not solve all of the worl'd problems

--- .class #id 

## Conversion computation

Farenheight to Celsius  $$N = (T - 32)*\frac{5}{9}$$<br/>
Celsius to Farenheight  $$N = \frac{9}{5}*T + 32$$<br/>

--- .class #id 

## R code for conversion
R code is used for the conversion.  For example:
```{R}
conversionFunc <- function(convType, deg) {
  if (convType == "Farenheight to Celsius") 
  {
    (5.0/9.0) * (deg - 32.0);
  }
  else
  {
    deg* (9.0/5.0) + 32.0;
  }
}
T <- 20;
N <- T* (9.0/5.0) + 32.0;
```

--- .class #id 
## Summary

This submission is

1.  Simple
2.  Direct
3.  Useful to convert from one temperature system to another, for example, if you are visiting a country under one system and you are familiar with the other.
