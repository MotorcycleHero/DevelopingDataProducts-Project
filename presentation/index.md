---
title       : Iris-o-Matic
subtitle    : Using Data Science to Identify Iris Species
author      : Jeremy Peach
job         : Developing Data Products
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## The Problem

Every day, people come across iris flowers as they go about their day-to-day lives.
All of these people have the same question:  <b>What is the species of this iris?</b>

<img src="http://vignette2.wikia.nocookie.net/fantendo/images/b/bb/Royalty-free-confused-clipart-illustration-215196.png" style="width: 45%;" />
<img src="http://www.twofrog.com/images/iris38a.jpg" style="width: 45%;" />

--- .class #id 

## The Solution

Using data science, we can help people solve this daunting problem that has wrecked so many lives.

We can use data that has been gathered about different species of irises
to build a prediction model.

Users will enter the length and width of the iris they've found.  These
measurements will be put into the model, and the species of the iris
will be determined based on irises that have similar measurements.

You can test out this solution at:  
https://motorcyclehero.shinyapps.io/Iris-o-Matic

--- .class #id 

## The Data

The R programming language already contains a data set with iris measurements.
This data was collected and published by Edgar Anderson in 1935.



The dataset contains 150 observations of data.

The following table shows which species are included in the data set and how
many observations there are for each species:

```r
table(iris$Species)
```

```
## 
##     setosa versicolor  virginica 
##         50         50         50
```

--- .class #id 

## Potential Pitfalls

Unfortunately, this solution will not be perfect.  Here are some potential
pitfalls that might prevent the application from being as successful as we hope.

1. The data is 80 years old, and the
world has changed a great deal since the data was gathered.  Nuclear weapons
have been invented, and they may have released radiation into the atmosphere.
This could cause the modern irises to mutate and become much larger than members
of the same species many years ago.  This would mean that today's irises cannot
be identified using the old data.

2. The data set only includes information for 3 different
species. People are likely to encounter irises of a species not included in the
data set. In those cases, the Iris-o-Matic application will not be able to help
them, and they will have to spend the rest of their lives wondering what the
species of the iris is.

3. The iris measurements in the data set are recorded in centimeters.  Most
people in the U.S. do not know how to use the Metric System so this application
will not be able to help them.

