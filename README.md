# 📈 Stock Price Prediction using LSTM (Deep Learning)

A time series deep learning project that predicts stock closing prices using an LSTM (Long Short-Term Memory) neural network. This model learns patterns from Apple Inc. (AAPL) stock data between 2015 and 2024.
Predicting future stock prices using machine learning and deep learning techniques in Python.

---

## 📦 Project Files

| File Name                   | Description                                         |
|-----------------------------|-----------------------------------------------------|
| `stock_price_prediction.ipynb` | Jupyter Notebook containing all code for data loading, training, and evaluation |
| `README.md`                | Project documentation                               |

---


## 🛠️ Tech Stack

- Python 🐍
- Pandas
- NumPy
- Matplotlib / Seaborn
- Scikit-learn
- TensorFlow / Keras (for LSTM models)
- yfinance (for fetching stock data)

  
## 🔍 Project Workflow

1. ✅ Load historical stock data using `yfinance`
2. 📊 Use `Close` price as target feature
3. 📏 Normalize data using MinMaxScaler
4. ⛓️ Create sequential data (lookback window = 60 time steps)
5. 🤖 Train a 2-layer LSTM neural network
6. 📉 Evaluate model using RMSE (Root Mean Squared Error)
7. 🧪 Plot actual vs. predicted prices (optional)

---

## 📁 Project Structure

- `data` – contains historical stock price CSV files  
- `notebooks` – Jupyter notebooks for EDA and model building  
- `models` – saved trained models  
- `src` – Python scripts for preprocessing and modeling  
- `README.md` – project documentation  
- `requirements.txt` – list of required packages

---

## 📥 Data Collection

Stock price data is fetched using the `yfinance` library and saved in CSV format for analysis and modeling.

---

## 📊 Exploratory Data Analysis

Visualize trends, check stationarity, analyze moving averages, and understand seasonal patterns in closing prices.

---

## ⚙️ Data Preprocessing

- Normalize the price data using MinMaxScaler  
- Create time-series sequences using a sliding window  
- Reshape input for compatibility with LSTM models

---

## 🧠 Building LSTM Model

- A deep LSTM architecture with dropout regularization  
- Trained on historical closing price sequences  
- Compiled with mean squared error loss and Adam optimizer

---

## 🏋️ Model Training

The model is trained for multiple epochs with a batch size of 32. Model checkpoints and loss evaluation are logged.

---

## 📈 Making Predictions

Once trained, the model predicts future stock prices based on the latest sequences. Predictions are scaled back to original values.

---

## 📉 Visualization

Actual vs. predicted prices are plotted to evaluate model performance visually.

---

## 🧪 Evaluation

Mean Squared Error (MSE) is calculated to quantify prediction error. Lower MSE indicates better performance.

---

## 🧾 Conclusion

This project demonstrates the application of deep learning techniques—particularly LSTM networks—for predicting stock prices based on historical data. While the model shows promising results in capturing trends, it's important to note that stock markets are influenced by countless external factors, and predictions should not be used for real-world trading decisions without further validation.
