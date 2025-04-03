# 📈 Amazon Stock Price Forecasting with Prophet

This project uses **Facebook Prophet** to forecast **Amazon stock prices** with a combination of trend, seasonality, and **exogenous regressors** like `Volume` and `Open`.  
Multiple forecasting strategies were explored — from baseline Prophet models to hybrid pipelines using Prophet to forecast regressors themselves.

## 🚀 Project Highlights

- 📅 Forecasts for future **business days** (30–60 days)
- 📊 **Prophet with and without exogenous variables** (`Volume`, `Open`)
- 🔁 **Recursive forecasting** using Prophet to estimate future regressors
- Integrated **US holiday calendar**
- 🧪 Evaluated against ARIMA, SARIMA, and SARIMAX for comparison
- 📉 RMSE & MAE error metrics, clear visualizations

## 📁 Dataset

The dataset used in this project contains daily historical Amazon stock prices from Nov 2021 to Nov 2024.
[Dataset Used](/AMZN_Historical_data.xlsx)

## 📈 Forecast Comparison

The plot below compares multiple forecasting models on Amazon stock price data:
[Forecast Comparison](/Forecast_Comparison.png)
- **Training_Data**: Actual values used for training
- **Actual_Data**: Ground truth for test period
- **ARIMA (0,1,0)**: Basic differencing-only ARIMA model
- **ARIMA (1,1,1)**: Autoregressive + Moving Average
- **SARIMA (0,1,2)(1,1,2,30)**: Seasonal ARIMA with monthly seasonality
- **SARIMAX (0,1,0)(0,1,2,30)**: Seasonal ARIMA + exogenous features
- **Prophet**: Forecast from base Prophet model (no regressors)
- **Prophet + Exog**: Forecast using Prophet with `Volume` and `Open` as regressors
