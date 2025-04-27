---

#  Time Series Forecasting using ARIMA

This project demonstrates **Time Series Forecasting** using the **ARIMA model** in Python.  
The dataset used is the **JPMorgan Chase (JPM) stock prices** fetched using **yfinance** library.

---

##  Project Highlights

- Downloaded **JPMorgan chase stock price data** (2018–2025).
- **Exploratory Data Analysis** (EDA) on stock closing prices.
- Performed **Decomposition** (Trend, Seasonality, Residuals).
- Conducted **Stationarity Test** using **Augmented Dickey-Fuller (ADF)**.
- Built and trained an **ARIMA(1,1,1)** model.
- Evaluated model with **ACF** and **PACF** plots.
- Forecasted future stock prices and compared with actual prices.
- Visualized forecast results.

---

## Libraries Used

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `statsmodels`
- `yfinance`
- `sklearn` (for metrics)

---

##  Steps Followed

1. **Data Collection**:  
   Using `yfinance` to download JPM stock data.

2. **EDA**:  
   Plotting stock closing prices to visualize trends and volatility.

3. **Decomposition**:  
   Applying `seasonal_decompose` to break time series into components.

4. **Stationarity Testing**:  
   Using **ADF Test** to check if differencing is needed.

5. **ACF and PACF Analysis**:  
   Identifying the values for p (AR terms) and q (MA terms).

6. **Model Building**:  
   Trained ARIMA(1,1,1) based on ACF/PACF guidance.

7. **Forecasting and Visualization**:  
   Comparing forecasted vs actual prices using line charts.

---

## Results

- The ARIMA(1,1,1) model captured general stock trends but struggled with sharp upward movements.
- Model residuals are close to random (good for ARIMA).
- Improvements can be made with  **advanced models** (e.g., Prophet, LSTM).

---


##  Future Work

- Try **SARIMA** for seasonal components.
- Use **Rolling Forecasts** for better real-time prediction.
- Experiment with **Deep Learning** models like **LSTM** for higher accuracy.

---

##  Conclusion

This project showcases how ARIMA models work for financial time series and highlights the importance of model selection and validation before real-world forecasting.

---


