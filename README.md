# 🛒 Store Sales Time Series Analysis

**Author:** Melanie  
**Date:** July 15, 2024  

---

## 📌 What is this project about?

This project analyzes **monthly sales data over 6.5 years** for a new retail store. Using time series methods in R, we explore trends, stationarity, variance stabilization, and autocorrelation. The goal is to extract meaningful patterns and prepare the data for accurate forecasting.

---

## 💡 Why this project?

Understanding long-term sales behavior is vital for retail decision-making. This project:

- Identifies trends and seasonal cycles
- Tests for stationarity (a key assumption in forecasting)
- Applies transformations to stabilize variance
- Explores autocorrelation to inform model selection

It demonstrates my ability to apply **real-world data analysis** techniques using statistical and machine learning concepts.

---

## 🛠️ How was it done?

### 🧪 Tools & Techniques:
- **Language:** R  
- **Libraries:** `ggplot2`, `tseries`, `forecast`, `scales`  

### 🔍 Key Steps:
1. **Data Cleaning & Time Series Conversion**  
   - Monthly sales data converted to time series object (`ts`)

2. **Trend & Seasonality Visualization**  
   - Time series plotted using `ggplot2`  
   - Key patterns over time visually identified

3. **Stationarity Testing (ADF Test)**  
   - Used `adf.test()` from the `tseries` package  
   - Confirmed that raw data is stationary (p < 0.05)

4. **Variance Stabilization**  
   - Performed **Box-Cox Transformation**  
   - Achieved more consistent variance across time

5. **ACF Plotting & Autocorrelation Analysis**  
   - Computed up to 20 lags using `Acf()`  
   - Identified strong autocorrelations suggesting AR components

---

## 📈 Results & Insights

| Step | Key Finding |
|------|-------------|
| 📉 Trend Analysis | Sales show strong long-term trend and recurring seasonal behavior |
| ✅ Stationarity | ADF test confirmed stationarity (p-value = 0.01) |
| 🔁 Variance | Box-Cox transformation stabilized variance |
| 📊 ACF Analysis | Strong autocorrelations up to lag 15 → suitable for AR modeling |

These insights create a solid foundation for **forecasting future sales** using models like ARIMA or SARIMA.

---

## ✅ Skills Demonstrated

- Time series modeling (incl. stationarity and transformations)
- Data wrangling and visualization in R
- Statistical testing and interpretation
- Communicating analytical insights clearly

---

## 🚀 Next Steps (if extended)
- Fit ARIMA/SARIMA models for forecasting
- Perform residual diagnostics
- Deploy a Shiny dashboard for business use

---
