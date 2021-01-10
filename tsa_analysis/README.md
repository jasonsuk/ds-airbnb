# Time series analysis for Airbnb data

The project has two objectives as following:

1. Build a ETL pipeline to extract, transform and load multiple gzips into database.

2. Perform time series analysis on the clean data, which includes

    - Descriptive analysis using moving average (plus Holt-Winter method)
    - Evaluating seasonality and stationarity with ETS decompotion and Augmented Dickey-Fuller test
    - Forecasting with ARIMA mode

## Acknowledgement

Data are downloaded from [Inside Airbnb](http://insideairbnb.com/get-the-data.html) website.

## Description on data

`calendar` file will be used to extract performance metrics such as occupancy rate and average daily rate.

The location of interest is Hong Kong for the period between 2019-01-01 and 2020-12-31.

## Objectives of the analysis

The purpose of this analysis is to evaluate how Airbnb performed in recent years (the analysis is done on Q1 2021), and also to see how vulnerable, or stable, the Airbnb business/market was amid COVID-19 pandemic.
