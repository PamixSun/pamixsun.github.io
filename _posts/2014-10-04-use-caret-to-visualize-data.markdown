---
layout: post
title:  "Using caret to visualize data"
date:   2014-10-04
categories: update
output: html_document
published: true
status: publish
 
---
 
The **caret** package (short for Classification And Regression Training) is a set of functions that attempt to streamline the process for creating predictive models. The package contains tools for:
 
- data splitting
- pre-processing
- feature selection
- model turning using resampling
- variable importance estimation

as well as other functionality.
 
In this post, I will show how to use this package to visualize our data set.
 
To install this package, type the code below in the R evirernment:
 

    install.packages('caret')
 
The **iris** data are used here for investigation, whose basic information is describe below:
 

    str(iris)

    ## 'data.frame':	150 obs. of  5 variables:
    ##  $ Sepal.Length: num  5.1 4.9 4.7 4.6 5 5.4 4.6 5 4.4 4.9 ...
    ##  $ Sepal.Width : num  3.5 3 3.2 3.1 3.6 3.9 3.4 3.4 2.9 3.1 ...
    ##  $ Petal.Length: num  1.4 1.4 1.3 1.5 1.4 1.7 1.4 1.5 1.4 1.5 ...
    ##  $ Petal.Width : num  0.2 0.2 0.2 0.2 0.2 0.4 0.3 0.2 0.2 0.1 ...
    ##  $ Species     : Factor w/ 3 levels "setosa","versicolor",..: 1 1 1 1 1 1 1 1 1 1 ...
 
Next, we will load **caret** in and use it to visualize **iris** as a scatter plot matrix.
 

    library(caret)

    ## Loading required package: lattice
    ## Loading required package: ggplot2
    ## Loading required package: methods

    featurePlot(x = iris[, 1:4],
                y = iris$Species,
                plot = "pairs",
                ## Add a key at the top
                auto.key = list(columns = 3))

![plot of chunk unnamed-chunk-3](/images/figure/unnamed-chunk-3.png) 
 
Furture more, we can get also the overlayed density plots:

    featurePlot(x = iris[, 1:4],
                      y = iris$Species,
                      plot = "density",
                      ## Pass in options to xyplot() to 
                      ## make it prettier
                      scales = list(x = list(relation="free"),
                                    y = list(relation="free")),
                      adjust = 1.5,
                      pch = "|",
                      layout = c(4, 1),
                      auto.key = list(columns = 3))

![plot of chunk unnamed-chunk-4](/images/figure/unnamed-chunk-4.png) 
 
and the box plots:

    featurePlot(x = iris[, 1:4],
                      y = iris$Species,
                      plot = "box",
                      ## Pass in options to bwplot() 
                      scales = list(y = list(relation="free"),
                                    x = list(rot = 90)),
                      layout = c(4,1 ),
                      auto.key = list(columns = 2))

![plot of chunk unnamed-chunk-5](/images/figure/unnamed-chunk-5.png) 
 
 
 
