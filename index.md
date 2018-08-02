---
title       : 
subtitle    : 
author      : 
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Slide 1


The Stock Analysis app is used to provide a graphical representation of the
price changes and the closing price for a particular stock.

- First graph plots price change percent with upper and lower confidence intervals
 - Also includes fitted line
- Second graph plots closing price with a simple moving average.
 - This plot can change the number of days lag
- Both graphs can be adjusted for the date range

---

## Slide 2



```r
direc <- paste0(getwd(),"/","tickerFunction.R")
direc2 <- paste0(getwd(),"/","appAPI.R")

source(direc)
```

```
## Warning in file(filename, "r", encoding = encoding): cannot open file
## '/Users/michaelgarcia/stock-trend-shiny-app/Stock Analysis Shiny App/
## tickerFunction.R': No such file or directory
```

```
## Error in file(filename, "r", encoding = encoding): cannot open the connection
```

```r
source(direc2)
```

```
## Warning in file(filename, "r", encoding = encoding): cannot open file
## '/Users/michaelgarcia/stock-trend-shiny-app/Stock Analysis Shiny App/
## appAPI.R': No such file or directory
```

```
## Error in file(filename, "r", encoding = encoding): cannot open the connection
```

```r
head(stockdf,2)
```

```
## Error in head(stockdf, 2): object 'stockdf' not found
```

---

## Slide 3

![Plot1](plot1.png)

- Includes upper and lower confidence intervals
- Includes fitted line

---

## Slide 4

![Plot2](plot2.png)
- Closing Price plot
- Includes simple moving average

---

## Slide 5

![reactiveoptions](reactiveoptions.png)
- Closing Price plot
- Includes simple moving average





