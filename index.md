---
title       : Derbies Premier League
subtitle    : Final Project - Developing Data Products
author      : Brais Lopez, Software Engineer
job         : 
logo        : premier-league.png
framework   : io2012       # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [mathjax, quiz, bootstrap]            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Index




1. Objectives of the project

2. Explanation of the project

3. Future improvements

![Caption for the picture.](premier_league.png)



--- .class #id 

## 1. Objectives of the project

**Objectives:** 
  * The most important thing is to use Shiny to present data to the users.
  * To show relevant data this project shows the derbies in the Premier League. Their results and the results of the teams that they play a derby.
  * The final user has the possibility to select the season that he wants to check the results. In this first version, there are only available the seasons: 2012/2013, 2013/2014 and 2014/2015. 

**Data:** the project extracts data from a .csv file that it is in the same folder of the project.  

**Test Url:** [https://blytest.shinyapps.io/4-ShinyProject/](https://blytest.shinyapps.io/4-ShinyProject/) 

**Project Url:** [https://github.com/Braisly/ShinyProject_DerbiesPremier](https://github.com/Braisly/ShinyProject_DerbiesPremier) 


--- .class #id 

## 2. Explanation of the project

**Explanation:** the operations that the project does at this moment are extract the data from a csv file with the results of the derbies. There is a previous project that download all data from internet and extract the required information.
Once we have all data stored in memory we will see the data and results of the selected season. Here, the reactive component of year is the key to load the different data in the table.


**For Example:**


```r
year <- 2013
dateSeason <- as.Date(paste("30/06/", year, sep = ""), format='%d/%m/%Y')
dateSeason
```

```
## [1] "2013-06-30"
```

Right now, the only thing to filter the results is to compare the dates that you want to show. 

--- .class #id 

## 3. Future improvements

**Improvements:** until this moment the project offers different data to the user but the one way to improve the information that the user can be interested is to show of an statistical way. Indeed showing different charts or plots can be an advantage to see what happens when there is a derby.

### Thanks for your time!

--- .class #id 
