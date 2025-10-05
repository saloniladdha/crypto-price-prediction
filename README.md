#  Cryptocurrency Price Prediction (BTC-USD)

This project applies **Linear Regression** to predict the **closing price of Bitcoin (BTC-USD)** using historical data.
It demonstrates how regression models can be applied to financial time series for short-term forecasting.

---

#  Project Overview

* Goal: Predict Bitcoin closing price using historical price data.
* Method: Linear Regression with lag features (previous days' prices) and moving averages.
* Dataset: BTC-USD daily data from Yahoo Finance (2020–2025).

---

#  Project Structure

```
crypto-price-prediction/
├── data/
│   └── btc_usd_2020_2025.csv              # Dataset (exported from Yahoo Finance)
├── notebooks/
│   └── crypto_price_prediction.ipynb      # Main Jupyter Notebook
├── README.md                              # Project documentation
```

---

#  Workflow

1. Data Collection

   * Downloaded BTC-USD data using `yfinance`.

2. Data Preprocessing

   * Created lag features (previous day’s close price).
   * Added moving average features.
   * Split dataset into training and testing sets.

3. Modeling (Linear Regression)

   * Trained model on historical features.
   * Evaluated using RMSE and MAE.

4. Visualization

   * Plotted actual vs predicted prices.
   * Highlighted test set predictions.

---

#  Results

* Evaluation Metrics

  * RMSE (Root Mean Square Error)
  * MAE (Mean Absolute Error)
* Final plots show how well the Linear Regression model predicts BTC closing prices.

---

#  Technologies Used

* Python
* Pandas, NumPy
* Scikit-learn (Linear Regression, metrics)
* Matplotlib, Seaborn (visualization)
* yfinance (data collection)

---

#  How to Run

1. Clone this repository:

   ```bash
   git clone https://github.com/yourusername/crypto-price-prediction.git
   cd crypto-price-prediction
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Open the Jupyter Notebook:

   ```bash
   jupyter notebook notebooks/crypto_price_prediction.ipynb
   ```

---

#  Future Work

* Experiment with advanced models (Decision Tree, Random Forest, LSTM).
* Add more features (volume, volatility, technical indicators).
* Extend to other cryptocurrencies (ETH, LTC, etc.).

---

#  License

This project is open-source and available under the **MIT License**.
