# OilForecast

Collaboration project of group 8 Computer Engineering

 1. Kevin Darmawan (1806148744)  
 2. Muhammad Alfi A (1806200015)  
 3. Muhammad 
Farhan Almasyhur(1806200375)  
 4. Mohammad Salman A (1806200381)

This python notebook project predicts World Oil price for 2019-2050 using data extracted each month from 1988-2018 using the ARIMA method

## Description
Included in this repository are dataset, resampled dataset and the source codes for the project.
Learn more about the auto ARIMA prediction method [here](https://github.com/kevindar/OilForecast/raw/master/Oil%20Prediction.ppt)
Screenshots of the results are accessible here
https://drive.google.com/open?id=1OI39vkXWKGWrg8Mczqm-JGm2TZIZqRPD

## Method
This project utilizes the Auto ARIMA function that is able to predict a certain time series in the future using training data from the past (in the dataset). 

## Implementation
For dataset with daily data, import to the Months.ipynb notebook to generate the max value of each month
Use the Auto ARIMA function to generate the p,d,q order of the ARIMA function by the least AIC value
Run the OilForecast.ipyb notebook, importing the oil_months.csv and run auto ARIMA
Execute the plot and see the prediction/


## Analysis
An advantage of the Auto ARIMA model is the ease of usage and eliminating the need to check the AR, I and MA order manually, just refer to the least AIC value.

Auto ARIMA model order generation may differ with data for the same time series with different data frecuencies, to fix this issue, use manual order calculation using ACF, PACF, and differentiating functions. Auto ARIMA gets more accurate for datasets with more frecuencies, with less trend slope and less moving average.
