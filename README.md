# Demand-forecasting-using-sarimax
## Introduction
Organizations like superstores use demand forecasting for adequate planning. In this project, using Python, a SARIMAX model is developed to help a superstore anticipate the demand for a product in a particular store location on a daily basis.

## Project Overview

Given the relevant sales data, exploratory data analysis was performed. This helped to identify outliers and other key information.

Subsequently, time-series analysis techniques were used to identify key time series features like seasonality, trend, and auto-correlation.

Appropriate transformations were carried out to make the timeseries suitable for forecasting using a sarimax model (sarimax was used due to the identified seasonality).

Exogenous variables were also created using the following:
- month
- day of the week
- weekend day or not
- first-year lag
- mid-year lag

To determine model parameters, two methods were used:
- An automatic parameter search using auto arima.
- Based on the ACF and PACF plots as well as their seasonal counterparts, model parameters were tested.

The best-performing model was observed to have a SMAPE of 18% on two months of unseen data.


