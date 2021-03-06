---
title       : Housing Sales Shiny App
subtitle    : 
author      : Ryan Conger
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## The Motivation

1. Housing prices vary quite a bit over time
2. People note all kinds of trends nationwide
3. The data are accessible, so why not look at it?
3. [Go to the app!](https://raconger.shinyapps.io/housing-sales/)

--- .class #id 

## The logistics
### [Go to the app!](https://raconger.shinyapps.io/housing-sales/)

- Historical sales data was obtained from the Douglas County (NV) assessor's website
- The following parameters are used
  - Upper Kingsbury (District 430) housing sales from 2000 to 2015
  - parcel number: 131800000000:131999999999
  - date range: 0101200:05172015

The CSV file came from a query at the Douglas County, NV Assessor's office [URL](http://assessor-search.douglasnv.us:1401/cgi-bin/asw300)

--- .class #id 

## What it looks like

<img src="http://raconger.github.io/Housing-Sales-Shiny-App/media/app.png" alt="Beautiful screenshot" width="100%">

--- .class #id 

## What it calculates
### [Go to the app!](https://raconger.shinyapps.io/housing-sales/)

In addition to the year and date, these pages calculate dollars per square foot and then plots it in a few different ways.

An example can be shown below:

```r
sale_price <- 300000 # Sale price of $300k
square_footage <- 1745 # 1,745 square feet

dol_p_sqft <- sale_price / square_footage
print(dol_p_sqft) # $/ft^2
```

```
## [1] 171.9198
```

--- .class #id

## Thanks!
### [Go to the app!](https://raconger.shinyapps.io/housing-sales/)

[Go to the source! (for the app)](https://github.com/raconger/housing-sales)

[Go to the source! (for the pitch)](https://github.com/raconger/Housing-Sales-Shiny-App)


