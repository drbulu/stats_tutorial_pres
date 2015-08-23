---
title       : Shiny App Pitch
subtitle    : Reproducible data products in motion
author      : drbulu
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
--- 

## Presenting...

<div align="center">
<b style="color:blue;font-size:300%;">Stats Tutorial</b><br/><br/>
<b>https://drbulu.shinyapps.io/stats_tutorial</b><br/><br/>
</div>

<p>This is an interactive web application that is an introductory tutorial 
into regression modelling that explores how a linear model is affected by the data that it describes.</p>

<p>This app will also introduce users to some of the tools (statistical approaches) that can be used to measure the quality and usefulness of a regression model. These concepts also apply to other types of linear models.</p>

--- .class #id  

## Basic App structure

<b style="color:blue;">Stats Tutorial</b> consists of the a number of key components.

<b>1.</b> <b style="color:blue;">Data:</b> A simple set of 40 observations, each consisting of two measurements x and y.  

<b>2.</b> <b style="color:blue;">Side panel tab:</b> A series of checkboxes that enable users to create a "User" model by selecting or deselecting observations.  

<b>3.</b> <b style="color:blue;">Visualisation tab:</b> A pair of scatter plots representing the "User" and "Reference" data sets. Each plot has a regression line representing the linear model created by the data.  

<b>4.</b> <b style="color:blue;">Statistics tabs:</b> Three tabs contain summary statistics of both the User" and "Reference" data sets. These allow the user to observe characteristics of the data and refine their model.  

--- .class #id

## Data Visualisation



```r
# Visualisation of the "Reference" data set that drives "Stats Tutorial"!
refdataModel = lm(y ~ x, data=projectData)    
plot(projectData$x, projectData$y, xlab = "data points (x)", ylab = "data values (y)")
abline(a = refdataModel)
```

![plot of chunk unnamed-chunk-2](assets/fig/unnamed-chunk-2-1.png) 

--- .class #id

## Getting Started

How do you get started with <b style="color:blue;">Stats Tutorial</b>?

Step 1: Go to the app website

<div align="center">
<b style="color:blue;font-size:120%;">https://drbulu.shinyapps.io/stats_tutorial</b>
</div>
<br/>

Step 2: Read the README page (especially the app <b>walkthrough</b>!)

Step 3: Explore the data... change the model... change the <b style="color:blue;">WORLD</b>!

<div align="center"><b style="color:red;font-size:150%;">..........</b></div>
<div align="center">
<b style="color:blue;font-size:300%;">Thank YOU!</b>
</div>
<div align="center"><b style="color:red;font-size:150%;">..........</b></div>
