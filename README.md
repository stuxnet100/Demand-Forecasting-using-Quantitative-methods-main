# Demand-Forecasting-using-Quantitative-methods

## Project Description:
The purpose of this project is to observe trend and seasonality in the sales of products and applying different timeseries and causal models to predict sales for future periods and to choose the best model that has lower mean absolute percentage error.

## Tools Used
1. Seaborn, matplotlib for visualizing graphs.
2. Statsmodels for **exponentioal smoothing**, **ARIMA**.
3. Sklearn for regression.

## Data:
Data was taken from kaggle. CSV file is present in this repository.

## Data Visualization:
1. Lineplot to visualize trend in the data.
2. **ACF** and **PACF** plots for identifying autocorrelation.
3. **Heat map** for identifying correlation in the new created features.

## Quantitative Methods Implemented:
1. **Holt Winters** Model
2. **ARIMA** - Autoregressive integrated Moving Average
3. **SARIMA** - Seasonal ARIMA
4. **Causal Model** - Linear Regression Model

## Conclusions:
| Method  | MSE |MAPE|
| ------------- | ------------- |-----------|
| Holt's winter  | 12.43  |24.44|
| SARIMAX  | 10.46  | 20.56 |
| Regression | 8.86 | 15.74|

Model is trained on the data of first 10 months and tested on 2 months data. MAPE for holt winter is 24.44%, for SARIMA is 20.55% and regression is 15.74%. New features are created using different lags and rolling mean, max and min and amongst them best 5 features are selected using recursive feature elimination technique and the regression model is trained based on those 5 features.
