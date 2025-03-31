# 📈 Stock Price Prediction and Impact Analysis Using LSTM
## 📌 Contributors
- **Krishnendu Adhikary (055022)**
- **Mohit Agarwal (055024)**


## 📌 Overview
This project develops an **LSTM-based deep learning model** to predict stock prices for **NIFTY 50** and **Reliance Industries**. It also examines the impact of Reliance Industries’ stock movements on the NIFTY 50 index.

## 🎯 Key Objectives
- 📊 Predict future stock prices using historical data.
- 🔍 Analyze the correlation between **Reliance Industries** and **NIFTY 50**.
- ⚡ Assess **LSTM's** effectiveness in capturing market trends.

## 🔄 Approach
### **📂 Data Collection & Preprocessing**
- **Source:** Yahoo Finance (`yfinance` package)
- **Date Range:** 2005-01-31 to 2025-01-31
- **Focus:** Closing prices (normalized using `MinMaxScaler`)

### **🧠 Model Development**
- **LSTM Model Architecture**
  - **Input:** 60-day historical closing prices
  - **Layers:** 3 LSTM layers (**50 units** each) with **Dropout (0.2)**
  - **Dense Layers:** One with **25 units (ReLU)** and one **output layer (single unit)**
  - **Optimizer:** `Adam` (learning rate = **0.001**)
  - **Loss Function:** Mean Squared Error (MSE)

- **Training Details**
  - 🏋️ **80% training**, **20% testing**
  - 📅 **10 epochs**
  - 📉 **MAPE** used for performance evaluation

## 📊 Key Findings
### **📈 Prediction Accuracy**
- **NIFTY 50:** ✅ **97.42% accuracy**
- **Reliance Industries:** ✅ **94.13% accuracy**

### **🔍 Insights**
- 📌 Strong **correlation** between **Reliance Industries** and **NIFTY 50**.
- 📈 Model captures **long-term trends** but struggles with **short-term volatility**.
- ⚠️ Predictions **lag** during sharp market fluctuations.

## 🚀 Future Scope
- 📊 Integrate **technical indicators** (RSI, MACD, Bollinger Bands).
- 🤖 Use **Transformer-based models** for improved accuracy.
- 📰 Incorporate **sentiment analysis** from news & social media.

## ✅ Conclusion
This **LSTM-based** approach effectively predicts **stock price trends** and highlights the influence of **Reliance Industries** on **NIFTY 50**. Further **enhancements** can improve **accuracy** and **real-world applicability**.
