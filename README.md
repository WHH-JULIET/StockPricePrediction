# 📈 Stock Price Prediction using LSTM

This project builds a Long Short-Term Memory (LSTM) deep learning model to predict future stock prices using historical data. The model is trained on Apple (AAPL) stock prices from 2015 to 2024, obtained via the Yahoo Finance API.

---

## 🔍 Overview

- **Data**: Apple (AAPL) historical stock prices (2015–2024)
- **Target**: `Close` price
- **Model**: 2-layer LSTM Neural Network
- **Libraries**: TensorFlow, scikit-learn, yfinance, NumPy, pandas, matplotlib

---

## ⚙️ Installation & Setup

1. **Install required libraries**:

   ```bash
   pip install yfinance pandas numpy matplotlib scikit-learn tensorflow
import yfinance as yf
df = yf.download('AAPL', start='2015-01-01', end='2024-12-31')

from sklearn.metrics import mean_squared_error
rmse = np.sqrt(mean_squared_error(actual, predictions))
print("RMSE:", rmse)

Input (60 time steps)
    ↓
LSTM (50 units, return_sequences=True)
    ↓
LSTM (50 units)
    ↓
Dense (1 output)


---

✅ **Summary**:  
This `README.md` tells the user exactly:
- What the project does  
- What libraries to install  
- How to load and process data  
- How the model is structured  
- How to train and evaluate it  
- Optional improvements

Let me know if you want this in a downloadable file or Jupyter template too!
