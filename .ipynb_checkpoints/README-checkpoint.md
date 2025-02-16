# Stock Prediction with Machine Learning

This project leverages machine learning to develop an advanced stock trading algorithm. The repository contains tools for data acquisition, feature engineering, model training, backtesting, and advanced analytics to create a robust, factor-based trading strategy. By integrating technical indicators and adaptive machine learning models, this project aims to optimize trading signals and improve risk-adjusted returns.

---

## Project Goals

1. Develop a scalable, machine-learning-driven trading model capable of generating accurate and risk-managed trading signals.
2. Identify predictive factors such as price momentum and volatility.
3. Create a robust framework to model nonlinear market relationships and adapt to changing market conditions.

---

## Methodologies

### 1. **Data Collection**
- Stock price data is sourced from Yahoo Finance using `yFinance` and OpenBB.
- Additional technical indicators such as RSI, Bollinger Bands, and MACD are calculated using the `ta` library.

### 2. **Feature Engineering and Selection**
- Feature importance is assessed using SHAP values, Mutual Information, and Gini Importance.
- Correlation analysis is performed to avoid multicollinearity.

### 3. **Machine Learning Models**
- Random Forest and XGBoost are used for predictive modeling of market direction based on engineered features.
- Recurrent Neural Networks (LSTM) are implemented to capture temporal dependencies in time-series data.

### 4. **Backtesting and Performance Evaluation**
- Strategies are backtested on historical data using Pyfolio, with performance compared against the S&P 500 as a benchmark.
- Key metrics include Precision, Recall, F1 Score, Sharpe Ratio, and Sortino Ratio.
- Walk-forward validation and TimeSeriesSplit are used for robust evaluation.

### 5. **Advanced Analytics and Visualizations**
- SHAP analysis provides interpretability of model predictions.
- Pyfolio tearsheets and Quantstats are integrated for in-depth strategy analysis.

---

## Results and Interpretation

**Key Findings:**  
- The baseline models (Random Forest, XGBoost, LSTM) have shown only modest predictive performance.
- SHAP analysis indicates that certain technical indicators (e.g., MACD, RSI) contribute more to model predictions, although the overall signal remains weak.
- The portfolio optimization module, while currently producing minimal allocations in the early periods, provides a systematic framework for testing risk-adjusted strategies.

**Interpretation and Limitations:**  
- **Model Performance:**  
  The models currently do not produce strong predictive signals. This might be due to a limited feature set or the inherent noise in financial markets.
- **Framework Utility:**  
  The strength of this project lies in its robust, modular framework, which allows for systematic testing and refinement of features, models, and portfolio strategies.
- **Portfolio Optimization:**  
  Early allocations are near zero, but the optimization framework is solid and can be refined as better signals are discovered.

**Future Work:**  
- **Enhance Feature Engineering:**  
  Integrate additional technical and fundamental indicators.
- **Model Tuning:**  
  Explore advanced model architectures, ensemble methods, and hyperparameter tuning.
- **Extended Backtesting:**  
  Refine portfolio optimization techniques to better capture real-world trading constraints.
- **Alternative Data Sources:**  
  Incorporate sentiment data, macroeconomic indicators, or alternative data to boost predictive performance.

---

## How to Use

1. Clone the repository:
   ```bash
   git clone https://github.com/michaelHalloran21/Stock_Prediction_with_Machine_Learning.git
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the notebooks in sequence to:
   - Explore and preprocess data.
   - Train models and generate predictions.
   - Backtest strategies and evaluate performance.
  
---

## Contributors
- Michael Halloran
- Stephen Grivers
- Andrew Dunham
  
This project is part of the DSP 577 - Data Enabled Capstone.
