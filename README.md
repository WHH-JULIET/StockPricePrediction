# 📈 Stock Price Prediction using LSTM

This project builds a Long Short-Term Memory (LSTM) deep learning model to predict future stock prices based on historical closing price data. It uses **Apple (AAPL)** stock data fetched from Yahoo Finance via the `yfinance` API.

---

## 🔍 Overview

- 📅 Data Range: 2015–2024
- 📊 Target Feature: `Close` price
- 🧠 Model: LSTM Neural Network (2 layers)
- 🔧 Libraries: TensorFlow, scikit-learn, yfinance, NumPy, pandas, matplotlib

---

## 📦 Installation

Before running the notebook, install the necessary Python libraries:

```bash
pip install yfinance pandas numpy matplotlib scikit-learn tensorflow
import yfinance as yf
df = yf.download('AAPL', start='2015-01-01', end='2024-12-31')

Input -> LSTM (50 units, return_sequences=True)
      -> LSTM (50 units)
      -> Dense (1 output)

## 📈 Visualization

The output includes a plot of **actual vs predicted stock prices**:

![Prediction Plot](prediction_plot.png)


from sklearn.metrics import mean_squared_error
rmse = np.sqrt(mean_squared_error(actual, predictions))
RMSE: 2.4567
