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
Ordinary Least Squares (OLS) fits a line to the data with the goal of finding a relationship between one or more independent variables (x-axis, z-axis, and so on) and a continuous dependent variable (y-axis). OLS chooses the line that minimizes the squared residuals (squared difference) between the fitted line, which represents the prediction of the dependent variable, and the actual value of the dependent variable. 
## Intuition
In the graph below, think of the data points (dots) as pegs fixed into the wall. The line is a stick hovering within the lines. See those dotted lines connecting the pegs to the stick? Imagine that those are rubber bands. The angle and location of the stick, which moves freely, is determined entirely by the position of the fixed pegs. 
![alt text](assets/linear_regression.png "Logo Title Text 1")

## Assumptions
### Linearity
- There is a linear relationship between the independent and dependent variables. Real world relationships are often messy, so this assumption is frequently violated.
- Detection - Look for non-linear relationships in scatterplots of the dependent variables vs independent variable. If you're feeling fancy, look for a relationship in the plotted residuals. 
- Fix - Consider transforming the dependent variable to reflect the non-linear relationship (X^2, log(X), sqrt(X)) or use a non-parametric model
### Non-correlation of error terms (residuals)
- Assumes that error terms aren't correlated. Put differently, OLS assumes that the fitted line does not systematically over or under-estimate the dependent variable. This assumption is often violated in time series analyses, where adjacent time points will have correlated errors. Correlated error terms mean result in underestimation of the true standard errors, leading to artificially narrower confidence prediction intervals. 
- Detection - Plot the residuals 
