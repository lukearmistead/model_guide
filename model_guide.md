# Structure
## Overview
## Intuition 
## Assumptions
## Pros
## Cons
## Reading

# Contents
- linear regression
- logistic regression
- decision tree regressor/classifier
- knn
- k-means
- heirarchical clustering
- naive bayes
- random forest regressor/classifier
- adaboost regressor/classifier
- svm/svc
- PCA/PCR

# Linear Regression
## Overview
Ordinary Least Squares (OLS) fits a line to the data with the goal of finding a relationship between one or more independent variables (x-axis, z-axis, and so on) and a continuous dependent variable (y-axis). OLS chooses the line that minimizes the squared residuals (squared difference) between the line, which is essentially the prediction of the dependent variable given a set of dependent variables. 
## Intuition
In the graph below, think of the data points (dots) as pegs fixed into the wall. The line is a stick hovering within the lines. See those dotted lines connecting the pegs to the stick? Imagine that those are rubber bands. The angle and location of the stick, which moves freely, is determined entirely by the position of the fixed pegs. 
## Assumptions
### Linearity
Problem - There is a linear relationship between the independent and dependent variables. Real world relationships are often messy, so this assumption is frequently violated.
Fix - Consider transforming the dependent variable to reflect the non-linear relationship (X^2, log(X), sqrt(X)) or use a non-parametric model
### Correlation of error terms

