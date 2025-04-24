# Stock Market Prediction Using Machine Learning

Author: Travis Johnson  
Course: Machine Learning for Engineering  
Instructor: Arshad Chowdhury  
Semester: Spring 2025

## Project Overview

Investors face significant challenges in predicting market trends due to volatility and the influence of multiple economic and sentiment-driven factors. This project leverages machine learning techniques, including Linear Regression, XGBoost, and Long Short-Term Memory (LSTM) networks, to predict the price of Apple Inc. (AAPL) stock using:

- Historical Stock Data  
- Economic Indicators (FRED)  
- News Sentiment Analysis (VADER)

## Objective

To build, evaluate, and compare multiple ML models to forecast stock price movements, supporting data-driven investment decisions.

---

## Data Sources

- Stock Data: Yahoo Finance API (AAPL, 10+ years)  
- Economic Data: Federal Reserve Economic Database (FRED)  
- Sentiment Data: NewsAPI and Finnhub (VADER sentiment scoring)

### Preprocessing Techniques:

- Normalization  
- Lag Feature Creation (t-1, t-2, t-3)  
- Train/Test Split (80/20)

---

## Models Implemented

| Model | Description |
| :---- | :---- |
| Linear Regression | Baseline model to establish initial performance |
| XGBoost | Nonlinear, tree-based model to capture complex patterns |
| LSTM | RNN-based time-series model for sequential trends |

---

## Evaluation Metrics

- RMSE (Root Mean Squared Error)  
- MAPE (Mean Absolute Percentage Error)  
- MSE (Mean Squared Error)  
- Sharpe Ratio (for assessing trading signal profitability)

---

## Results Summary

| Model | RMSE | MAPE |
| :---- | :---- | :---- |
| Linear Regression | 4.28 | 3.24% |
| XGBoost | 3.12 | 2.15% |
| LSTM | Promising (Needs further tuning) |  |

### Key Insights

- Economic indicators significantly improved prediction accuracy.  
- XGBoost outperformed linear regression by capturing nonlinearity.  
- LSTM models require tuning but show high potential for time-series forecasting.

---

## Future Work

- Refine and tune LSTM model (e.g., adjust units, epochs, lookback window)  
- Integrate real-time data streaming for live predictions  
- Expand model to additional stocks or even cryptocurrencies  
- Experiment with attention mechanisms and reinforcement learning

---

## References

1. Machine Learning Stock Market Prediction Studies – Troy Strader  
   [Link](https://scholarworks.lib.csusb.edu/jitim/vol28/iss4/3/)

2. Stock Market Prediction Using Machine Learning – Ishita Parmar  
   [Link](https://ieeexplore.ieee.org/document/8703332)

3. Applying ML Algorithms to Predict Stock Price Trends – Tran Phuoc  
   [Link](https://www.nature.com/articles/s41599-024-02807-x)

---

## How to Run

1. Clone this repo and open the Jupyter Notebook MLE\_Project.ipynb  
2. Install required packages:

pip install pandas numpy matplotlib scikit-learn xgboost keras yfinance vaderSentiment

3. Run all cells from top to bottom.  
4. View the evaluation metrics and graphs for model performance.

---

## Files Included

- MLE\_Project.ipynb \- Main project notebook  
- README.md \- This file  
- Presentation slides and proposal documentation

