# Amazon Stock Price Forecasting using ARIMA and ARIMAX

This project uses classical time series models — **ARIMA** and **ARIMAX** — to forecast the closing stock prices of **Amazon Inc.**, integrating **Google Trends** as an exogenous variable in the ARIMAX model.

---

## Objective

- Predict Amazon's daily closing stock price.
- Compare ARIMA (univariate) and ARIMAX (multivariate with Google Trends).
- Evaluate the impact of exogenous variables (public interest) on financial forecasting.

---

## Data Sources

- **Amazon Stock Data**: Downloaded from [Kaggle](https://www.kaggle.com/datasets/aenes95/amazon-stock-price-prediction)
- **Google Trends**: Retrieved from [Google Trends](https://trends.google.com)  for the keyword _"Amazon"_

---

## Tools and Libraries

- `pandas`, `numpy` — data manipulation  
- `matplotlib`, `seaborn` — visualization  
- `statsmodels` — ARIMA and ARIMAX modeling  
- `sklearn` — error metrics (MSE, MAD)  

---

## Methodology

1. Data Collection and Merging  
2. Stationarity Testing using ADF  
3. ARIMA Modeling (order selection using ACF, PACF)  
4. ARIMAX Modeling with Google Trends as exogenous regressor  
5. Forecasting & Evaluation on Test Set  

---

## Performance Comparison

| Model  |   MSE   |   MAD  |
|--------|---------|--------|
| ARIMA  | 667486.1| 672.502|
| ARIMAX | 653018.1| 662.212|

> 🔍 *ARIMAX outperforms ARIMA by leveraging external signals from Google Trends.*

---
