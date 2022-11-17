# Bike Sharing Demand Prediction

<img src="http://static1.squarespace.com/static/5bcfc8c07a1fbd730b2ba933/5cc102ea971a180a4c6a1dbf/5cc110457817f7e445a690a6/1567474883972/IMG_1235.jpg?format=1500w" width="800" height="500"/>

## Introduction

Currently Rental bikes are introduced in many urban cities for the enhancement of mobility comfort. It is important to make the rental bike available and accessible to the public at the right time as it lessens the waiting time. Eventually, providing the city with a stable supply of rental bikes becomes a major concern. The crucial part is the prediction of bike count required at each hour for the stable supply of rental bikes. People use bike-share for various reasons. Some
who would otherwise use their own bicycle have concerns about theft or vandalism, parking or storage, and maintenance. The typical bike-share has several defining
characteristics and features, including station-based bikes and payment systems, membership and pass fees, and per-hour usage fees.

## Project Objectives

* To highlight the main variables/factors influencing rental bike count.
* To predict bike count required at each hour for the stable supply of rental bikes.
* To compare the various machine learning models and find out best model for the above task.

## Data Description

The dataset contains weather information (Temperature, Humidity, Windspeed, Visibility, Dewpoint, Solar radiation, Snowfall, Rainfall), the number of bikes rented per hour and date information.

### Attribute Information:

* Date : year-month-day
* Rented Bike count - Count of bikes rented at each hour
* Hour - Hour of he day
* Temperature-Temperature in Celsius
* Humidity - %
* Windspeed - m/s
* Visibility - 10m
* Dew point temperature - Celsius
* Solar radiation - MJ/m2
* Rainfall - mm
* Snowfall - cm
* Seasons - Winter, Spring, Summer, Autumn
* Holiday - Holiday/No holiday
* Functional Day - NoFunc(Non Functional Hours), Fun(Functional hours)

## Steps involved

* Reading and understanding data
* Data cleaning
* Exploratory Data Analysis(EDA)
* Feature engineering
* Data preparation
* Model building
* Hyperparameter tuning

## Feature engineering

We have extracted month and year from the date column. To select the most relevant features we have used correlation matrix and VIF to remove multi-collinear features. We have also dropped some features like rainfall and snowfall which contain most of the zero values and also these features are slightly correlated with the dependent variable.

## List of models

* Linear Regression
* Polynomial Regression
* Regularized Linear Regression
* Decision Tree
* Random Forest
* Gradient Boosting
* XGBoost

## Conclusion

The data analysis and prediction provides a thought-provoking outcome for both the data exploration and the prediction models. The generated plots based on their
correlation, certainly show different parameter relationships that can be concealed in the most used prediction models. 

Simple linear regression model certainly underfits the data whereas nonlinear model (3-degree polynomial model) with regularization gives accurate fit. Other complex models like Random forest, Gradient boosting, and XGBoost gave better accuracy than other models but they tend to over fit the data slightly. Temperature, hour and humidity are the three most important features given by all the models except XGBoost.
