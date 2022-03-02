# Data Mining

# Final Project

## Predicting the trend on SPY
## Context for this project

As an investor, your goal is to reduce risk. If you can obtain a forecast on the upcoming trend, your risk will be lower than normal and increase the probability of being profitable.

## The Problem

What trend will the largest 500 public companies take in the stock market?

Data Source: Yahoo Finance
Retrieve Data from Yahoo Finance ranged from January 23, 2012, to February 23, 2022

## Methods Used:

### Linear Regression using Stepwise Variable Selection

Linear regression attempts to model the relationship between variables by fitting a linear equation to observed data. One variable is considered a dependent variable as it depends on others to be predicted, and the other are considered to be independent variables or predictors. Stepwise regression is the step-by-step iterative construction of a regression model that involves the selection of independent variables to be used in a final model.
Results:
Linear Regression RMSE: 0.9839
Stepwise Backward RMSE: 0.9839 
Stepwise Forward RMSE: 0.9839 
Stepwise Both RMSE: 0.9839

### KNN Model
KNN is a clustering model that will group categories depending on numeric values. We created two models: 

Model 1 – (Low, High)
Accuracy: 50%
Model 2 – (Open – Close) 
Accuracy: 83% 

### Time Series 

A Time Series model hopes to forecast a trend from dates and numbers. We are using dates when the market was opened and closing prices to determine the trend. We created to models, Auto Arima model with a log (2,1,3) with a drift and a custom Arima with a log of (1,1,1).

Auto Arima (2,1,2) with a drift
RMSE: 2.057
Custom Arima with a log of (1,1,1)
RMSE: 2.061



