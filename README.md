# ⏳ Time Series Forecasting Project

This repository contains my **time series forecasting work**, where I analyze historical data to understand patterns over time and build forecasting models to predict future values. The project focuses on proper data preparation, trend and seasonality analysis, model evaluation, and selecting the best forecasting approach based on performance.

---

## 🧠 Project Overview

The goal of this project is to forecast future values using time-based data by:
- Cleaning and preparing the dataset
- Understanding trends, seasonality, and anomalies
- Building and comparing multiple forecasting models
- Selecting the best model using error metrics

---

## 🧹 Data Preprocessing

- **Missing values** were handled using **interpolation** to preserve continuity in the time series  
- **Anomalies / outliers** were treated using the **quantile-based approach**  
- Applied **moving averages** to smooth the series and understand the underlying trend  

---

## 📊 Time Series Analysis

- Visualized the data to understand overall behavior  
- **Decomposed the time series** to separately analyze:
  - Trend  
  - Seasonality  
  - Residuals  
- Checked for **stationarity** to determine suitable forecasting models  
- Analyzed **autocorrelation and partial autocorrelation** to identify seasonality and determine the value of **m**

---

## 📐 Model Evaluation Metric

- Used **MAPE (Mean Absolute Percentage Error)** to evaluate and compare forecasting models  
- Selected the model with the **lowest MAPE** for final forecasting  

---

## 🤖 Forecasting Models Used

1. **Seasonal Naive Model**  
   - Used as a baseline model for comparison  

2. **Triple Exponential Smoothing (Holt-Winters)**  
   - Captured trend and seasonality effectively  

3. **SARIMA (Seasonal ARIMA)**  
   - Built after identifying stationarity and autocorrelation patterns  
   - Tuned using seasonality (`m`) and ARIMA parameters  
   - Achieved the **lowest MAPE**, making it the final selected model  

---

## 🔮 Final Forecast

- Used the **SARIMA model** to forecast values for the **next one year**
- The forecast captures both **trend and seasonal patterns** observed in the historical data

---

## 🛠️ Tools & Libraries

- Python  
- Pandas, NumPy  
- Matplotlib / Seaborn  
- Statsmodels  

---

## 🎯 Key Takeaways

- Proper preprocessing significantly improves forecasting accuracy  
- Decomposition helps in understanding the structure of time series data  
- Comparing models using error metrics is crucial before final selection  
- SARIMA performed best for this dataset due to clear seasonality and autocorrelation patterns  

---

## 👤 Author

**Tarun Panda**  
Aspiring Data Analyst | Python | EDA | Time Series Forecasting  

Feel free to explore, fork, or suggest improvements!
