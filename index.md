--- 
title       : Shiny Crime Map 
subtitle    : Downtown Houston Texas Violent Crimes Interactive Map
author      : James C. Fielding
job         : JHU Developing Data Products - Project 1
framework   : io2012   # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : solarized_light      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides

--- .segue .quote .dark

<q> Shiny Crime Map an interactive map that allows the user to view the locations of different types of violent crimes in the Houston, Texas downtown area from January 2010 through August 2010.</q>

<style>
.dark q {
  color: white;
}
</style>

---

<iframe src = 'https://jcfielding.shinyapps.io/ShinyCrimeMap' height='600px'></iframe>

--- .segue .quote bg:yellow

<q> Shiny Crime Map is simple to use. Just select the Crime Type you would like to map in the drop down menu. You can also toggle the radio buttons to change Map Type.</q>

---

## Built in R...



```r
violent.crimes %>% group_by(offense) %>% summarize(count = n())
```

```
## Source: local data frame [4 x 2]
## 
##              offense count
## 1            robbery   312
## 2 aggravated assault   362
## 3               rape    22
## 4             murder     5
```
<br/>
## Try Shiny Crime Map today...
https://jcfielding.shinyapps.io/ShinyCrimeMap
