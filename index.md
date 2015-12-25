---
title       : Project for Developing Data Products Coursera Course
subtitle    : Your chances of surviving at the Titanic disaster
author      : Irene Monfalcone
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

Overview
================

This presentation has been created as a course project in the Developing Data Products course by Coursera

Project Summary
================
The idea was to develop a very simple App to predict, the chances of surviving the Titanic disaster based on a series of evaluations on values present in the R dataset "Titanic".
This data set provides information on the fate of passengers on the fatal maiden voyage of the ocean liner ‘Titanic’, summarized by economic status (class), sex, age and survival.
For do this we use:

1. The R dataset "Titanic";
2. The Age field in Titanic is "Adult" or "Child". For the App Usability, the dataset was modified and Age was considered: MinAge=0 and MaxAge=16 for Age="Child"; MinAge=17 and MaxAge=100 for Age="Adult";
3. The UI allows the user to indicate their Age, Sex and in which Class their journey on the Titanic would be.
4. Based on this information, the application finds the Survival rate in the modified dataset and return: the selected fields; the Survival Rate

---
Some information about Titanic Survival Probability 1/2
========================================================
In the Titanic dataset we discovered that the general probability to survive the Titanic disaster was:


```
##   SurvivalRate NotSurvivalRate
## 1        32.3%           67.7%
```

![plot of chunk unnamed-chunk-2](assets/fig/unnamed-chunk-2-1.png) 

---
Some information about Titanic Survival Probability 2/2
========================================================
Grouped by Sex the survival probability was:


```
##      Sex SurvivalRate
## 1 Female       73.19%
## 2   Male        21.2%
```

Grouped by Age the survival probability was:


```
##     Age SurvivalRate
## 1 Adult       31.26%
## 2 Child       52.29%
```
Grouped by Class the survival probability was:


```
##   Class SurvivalRate
## 1   1st       62.46%
## 2   2nd        41.4%
## 3   3rd       25.21%
## 4  Crew       23.95%
```

---
Application location
=====================
The application may be found at:
"https://irek978.shinyapps.io/TitanicSurvival"

The code for the application and the project my be found at:
"https://github.com/irek978/TitanicSurvival"
