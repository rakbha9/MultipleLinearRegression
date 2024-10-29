# Project Name
Prediction of rental bikes using Multiple Linear Regression

## Introduction
BoomBikes has recently suffered considerable dips in their revenues. In order to make a business plan to accelerate its revenue we have to model the demand for shared bikes with the available independent variables.

## Table of Contents
* [General Info](#general-information)
* [Approach](#approach)
* [Conclusions](#conclusions)
* [Recommendations](#recommendations)
* [Technologies Used](#technologies-used)
* [Acknowledgements](#acknowledgements)
* [Contact](#contact)

## General Information
To build a multiple linear regression model for the prediction of demand for shared bikes.

- Background of the Project: A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues.The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue.

- Business Problem: To understand the factors on which the demand for the shared bikes depends.Specifically, they want to understand the factors affecting the demand for these shared bikes in the American market. The company wants to know the below 
    a) Which variables are significant in predicting the demand for shared bikes.
    b) How well those variables describe the bike demands
	
- Dataset: The dataset has fields related to bike rentals. It has the count of casual, registered users who rented the bike, date of rental, temperature, feels like temperature, humidity, weather on the day of rental, windspeed , season. This data helps in performing both univariate, bivariate, multivariate analysis and then perform a Multiple Linear Regression model to find the variables in predicting the demand for shared bikes.

## Approach:
The below are the high level steps that will be performed to do the Multiple Linear Regression model to find the variables in predicting the demand for shared bikes. 
- Understanding Problem Statement
- Importing necessary libraries
- Loading Dataset
- Data Understanding & Preparing Data
- Missing Value Check
- EDA
- Preprocessing - Dummy Creation
- Train-Test Split
- Scaling
- Feature Selection - RFE
- Modelling
- Manual Feature Selection
- Evaluation

## Conclusions
We can see that the equation of our best fitted line is:

cnt = 4510.7685 + (869.1712 * atemp) − (414.8227 * season_spring) + (220.5369 * season_winter) 
     + (1043.7114 * yr_1) + (101.9642 * mnth_May) + (147.7071 * mnth_Sept) − (381.7904 * weathersit_L)  
	 - (272.3049 * weathersit_M)
	 
Based on final model the below features explain the demand for bike rentals as :

- yr_1 - Year 2019 (1043.7114) - Rental growth has increased significantly from 2018 to 2019 
- atemp - Feeling Temperature (869.1712) - It has very high impact on the bike rentals as many people tend to rent bikes when the feeling temperature is good and not too cold or too hot.This suggests that people are more likely to rent bikes when the weather feels warmer, which aligns with expected seasonality.
- Season -
     a) season_spring (-414.8227) - Rentals decrease significantly in the spring probably because of rains.
     b) season_winter (220.5369) - Winter shows a positive impact on rentals.
This could indicate that certain weather factors (like rain in spring) discourage bike usage, while other conditions (like clear, cold winter days) may not impact rentals as negatively as expected.
- Months -
     a) mnth_Sept (147.7071) - 
     b) mnth_May  (101.9642) - 
Bike rentals increased slightly in May,September probably because of pleasant weather.
- Weather - 
     a) weathersit_L (-381.7904) - 
	 b) weathersit_M (-272.3049)- 
Weather conditions negatively impact bike rentals, particularly when conditions include mist, clouds, or light rain. 

## Recommendations

- Promotions and campaigns should be increased during warmer seasons or favorable weather periods to capitalize on increased demand. Also, forecasting demand based on expected temperature changes could improve bike availability management.
- Understanding seasonal preferences allows for seasonal marketing adjustments. Discounts can be provided on off-season to generate more bike rentals.
- The bike rental growth has increased significantly from 2018 to 2019 and if this trend continues, new locations can be added and increasing the no of bikes will increase revenue in future.
- Different promotional campaigns during the months May and September can be run to add more rentals. The promotional campaign for September should be different than May as Summer is followed after May and September comes in Fall season.
- Given that bad weather reduces rentals, it could be useful to develop a flexible pricing model, multi-month discount programs that offers discounts on rainy or misty days. 

## Technologies Used
Jupyter version: 7.0.8
python version: 3.11.7
numpy version: 1.26.4
pandas version: 2.1.4
matplotlib version: 3.8.0
seaborn version: 0.13.2
statsmodels version: 0.14.0
sklearn version: 1.2.2

## Acknowledgements

## Contact
Created by [@rakbha9] - feel free to contact me!

https://github.com/rakbha9/MultipleLinearRegression
