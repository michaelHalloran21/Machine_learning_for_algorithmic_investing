# Stock Prediction with Machine Learning

This project leverages machine learning to develop an advanced stock trading algorithm. The repository contains tools for data acquisition, feature engineering, model training, backtesting, and advanced analytics to create a robust, factor-based trading strategy. By integrating technical indicators, macroeconomic factors, and adaptive machine learning models, this project aims to optimize trading signals and improve risk-adjusted returns.

---

## Project Goals

1. Develop a scalable, machine-learning-driven trading model capable of generating accurate and risk-managed trading signals.
2. Identify predictive factors such as price momentum, volatility, and macroeconomic indicators.
3. Create a robust framework to model nonlinear market relationships and adapt to changing market conditions.

---

## Methodologies

### 1. **Data Collection**
- Stock price data and macroeconomic indicators are sourced from Yahoo Finance using `yFinance` and OpenBB.
- Additional technical indicators such as RSI, Bollinger Bands, and MACD are calculated using the `ta` library.

### 2. **Feature Engineering and Selection**
- Feature importance is assessed using SHAP values, Mutual Information, and Gini Importance.
- Recursive Feature Elimination (RFE) and BorutaPy are used to identify relevant features and eliminate noise.
- Correlation analysis is performed to avoid multicollinearity.

### 3. **Machine Learning Models**
- **Random Forest** and **XGBoost** are used for predictive modeling of market direction based on engineered features.
- **Recurrent Neural Networks (LSTM)** are implemented to capture temporal dependencies in time-series data.
- Hyperparameter tuning and cross-validation ensure optimal model performance.

### 4. **Backtesting and Performance Evaluation**
- Strategies are backtested on historical data using Pyfolio, with performance compared against the S&P 500 as a benchmark.
- Key metrics include Precision, Recall, F1 Score, Sharpe Ratio, and Sortino Ratio.
- Walk-forward validation and TimeSeriesSplit are used for robust evaluation.

### 5. **Advanced Analytics and Visualizations**
- SHAP analysis provides interpretability of model predictions.
- Pyfolio tearsheets and Quantstats are integrated for in-depth strategy analysis.

---

## Project Outcomes

1. A robust and adaptive trading strategy that integrates key predictive factors.
2. Tools for identifying market drivers and optimizing trading signals.
3. A comprehensive framework for evaluating performance against benchmarks and market conditions.

