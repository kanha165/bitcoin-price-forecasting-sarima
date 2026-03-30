# 🚀 Bitcoin Price Forecasting using SARIMA & Auto ARIMA

## 📌 Project Overview

This project focuses on **Time Series Forecasting** of Bitcoin prices using classical statistical models like **ARIMA, SARIMA, and Auto ARIMA**.

The goal is to analyze historical Bitcoin data and predict future prices while understanding the limitations of traditional models on highly volatile data.

---

## 🎯 Objectives

* Perform time series analysis on Bitcoin data
* Apply ARIMA and SARIMA models
* Use Auto ARIMA for optimal parameter selection
* Compare model performance
* Generate future forecasts

---

## 📊 Dataset

* Source: Yahoo Finance (via `yfinance`)
* Asset: **BTC-USD (Bitcoin)**
* Duration: Last 5 Years
* Frequency: Daily

---

## 🛠️ Tech Stack

* Python 🐍
* Pandas
* NumPy
* Matplotlib
* Statsmodels
* pmdarima (Auto ARIMA)
* yfinance

---

## ⚙️ Workflow

### 1️⃣ Data Collection

* Fetched Bitcoin data using `yfinance`
* Extracted closing price for analysis

### 2️⃣ Data Visualization

* Plotted time series graph
* Observed **trend and volatility**

### 3️⃣ Stationarity Check

* Used **ADF (Augmented Dickey-Fuller Test)**
* Found data **non-stationary**

### 4️⃣ Differencing

* Applied first-order differencing
* Converted data into **stationary form**

### 5️⃣ ACF & PACF Analysis

* Determined AR (p) and MA (q) values
* Observed weak autocorrelation

### 6️⃣ ARIMA Model

* Applied basic ARIMA
* Result: **Flat predictions (baseline model)**

### 7️⃣ SARIMA Model

* Included seasonal components
* Slight improvement observed

### 8️⃣ Auto ARIMA Optimization

* Used `auto_arima()` to find best parameters
* Applied those parameters in SARIMA

### 9️⃣ Forecasting

* Predicted next 30 days
* Compared results across models

---

## 📈 Results & Observations

| Model       | Performance         |
| ----------- | ------------------- |
| ARIMA       | Flat prediction ❌   |
| SARIMA      | Slight variation ⚠️ |
| Auto SARIMA | Best among all ✅    |

### 🔥 Key Insight:

Bitcoin data is highly volatile and lacks strong seasonality, making it difficult for traditional models to capture patterns effectively.

---

## ⚠️ Limitations

* High volatility of cryptocurrency data
* Weak seasonality
* Linear models struggle with non-linear patterns

---

## 🚀 Future Improvements

* Implement **LSTM (Deep Learning Model)**
* Use **Facebook Prophet**
* Hybrid models (SARIMA + ML)

---

## 📂 Project Structure

```
📦 Bitcoin-Forecasting
 ┣ 📜 SARIMA.ipynb
 ┣ 📜 README.md
 ┗ 📜 requirements.txt
```

---

## ▶️ How to Run

```bash
# Clone repo
git clone https://github.com/your-username/bitcoin-forecasting.git

# Install dependencies
pip install -r requirements.txt

# Run notebook
jupyter notebook
```

---

## 📦 Requirements

```
pandas
numpy
matplotlib
statsmodels
pmdarima
yfinance
```

---

## 💡 Key Learnings

* Time series preprocessing is critical
* Stationarity is required for ARIMA models
* Auto ARIMA helps in parameter tuning
* Traditional models struggle with crypto data

---

## 👨‍💻 Author

**Kanha Patidar**
B.Tech (CSIT) Student | Aspiring AI/ML Engineer

Passionate about Machine Learning and Data Science, with hands-on experience in building real-world projects like time series forecasting using ARIMA and SARIMA.

📫 LinkedIn: www.linkedin.com/in/kanha-patidar-837421290
💻 GitHub: https://github.com/kanha165

---

## ⭐ If you found this useful, give it a star!
