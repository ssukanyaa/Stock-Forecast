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
