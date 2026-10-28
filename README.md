# Time Series Analysis & Forecasting

## Project Overview

This project explores historical airline passenger data to identify trends, seasonality, and changes in passenger traffic over time. It also demonstrates time series forecasting using ARIMA and SARIMA models.

## Dataset

**AirPassengers.csv**

Contains 144 monthly observations from January 1949 to December 1960.

- Month: Date of observation
- #Passengers: Monthly airline passenger count in thousands

## Tools & Libraries

Python | Pandas | Matplotlib | Statsmodels

## Methodology

1. **Data Preparation:** Loaded the dataset, converted dates into datetime format, and created a time-based index.
2. **Exploratory Analysis:** Visualized passenger traffic and calculated a 12-month moving average.
3. **Seasonal Decomposition:** Separated the series into trend, seasonal, and residual components.
4. **Stationarity Testing:** Used the Augmented Dickey-Fuller (ADF) test to assess stationarity.
5. **Data Transformation:** Applied differencing and seasonal differencing.
6. **Autocorrelation Analysis:** Used ACF and PACF plots to examine relationships between observations.
7. **Forecasting:** Developed ARIMA and SARIMA models using an 80/20 chronological train-test split.

## Key Findings

- The original passenger series showed evidence of non-stationarity (ADF p-value: 0.9919).
- Two-period differencing produced an ADF p-value of 0.0386.
- Seasonal differencing produced an ADF p-value of 0.0116.
- The dataset exhibited seasonal patterns that motivated the use of SARIMA.
- ARIMA and SARIMA forecasts were generated and visualized against actual passenger counts.

## Models

**ARIMA:** (1, 1, 3)

**SARIMA:** (1, 1, 3) × (1, 1, 3, 12)

## Future Improvements

- Evaluate forecast accuracy using MAE and RMSE.
- Tune forecasting parameters.
- Investigate the SARIMA convergence warning.
- Add prediction intervals.

## Learning Outcomes

Developed practical experience in time series preparation, stationarity testing, seasonal decomposition, and forecasting.
