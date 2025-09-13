# 📊 ISAT-Individual-Stock-Analysis-Tool (Stock Market Analysis & Prediction Tool)

A robust **stock market analysis project** built in **Python (Jupyter Notebook)** that integrates **technical indicators, sentiment analysis, and machine learning models (Gradient Boosting & LSTM)** to analyze historical stock data and predict next-day returns.

---

## 🔑 Features

* 📈 **Data Collection**

  * Fetches historical stock data using **Yahoo Finance API (yfinance)**
  * Auto-adjusted prices with validation

* 🧮 **Feature Engineering**

  * Daily & Cumulative Returns
  * Rolling Volatility (21-day, annualized)
  * Moving Averages (7 & 21-day)
  * RSI & MACD indicators

* 📰 **Sentiment Analysis**

  * Scrapes latest Yahoo Finance headlines
  * Applies **TextBlob** to assign sentiment scores

* 🤖 **Machine Learning Models**

  * **Gradient Boosting Regressor** for next-day return prediction
  * **LSTM Neural Network** for sequential return forecasting

* 💡 **Human-Readable Insights**

  * Auto-generated insights on price movement, volatility, moving averages, and sentiment

* 📊 **Visualizations**

  * Interactive **Candlestick Charts** with Plotly
  * Daily Returns & Rolling Volatility plots with Matplotlib

* 📂 **Data Export**

  * Saves enhanced dataset with technical indicators and predictions as `TICKER_Enhanced.csv`

---

## 🛠️ Tech Stack

* **Python 3.10+**
* **Libraries**:

  * `pandas`, `numpy`, `matplotlib`, `seaborn`
  * `yfinance` for stock data
  * `ta` for technical indicators
  * `textblob` + `BeautifulSoup` for sentiment
  * `scikit-learn` for ML
  * `tensorflow` (Keras) for LSTM model
  * `plotly` for interactive charts

---

## 📥 Installation

1. Clone this repo:

   ```bash
   git clone https://github.com/your-username/stock-market-analysis.git
   cd stock-market-analysis
   ```

2. Create a virtual environment (recommended):

   ```bash
   python -m venv venv
   source venv/bin/activate   # Mac/Linux
   venv\Scripts\activate      # Windows
   ```

3. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

---

## 🚀 Usage

1. Open Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

2. Run the main script:

   * Set your stock ticker symbol (default = `AAPL`)
   * Example:

     ```python
     STOCK = 'TSLA'
     ```

3. The notebook will:

   * Fetch and clean stock data
   * Generate features & insights
   * Train ML models (Gradient Boosting & LSTM)
   * Show predictions & visualizations
   * Save enhanced dataset

---

## 📊 Example Outputs

* **Human-Readable Insights**

  ```
  - AAPL closed higher than previous day: 195.67 📈
  - Short-term MA crossed above long-term MA: Bullish ✅
  - Stock volatility is above average: High risk ⚠️
  - Market sentiment: Positive 😊
  ```

* **Predictions**

  ```
  Gradient Boosting Next-Day Return Prediction: 0.00235 (📈 Uptrend expected)
  LSTM Next-Day Return Prediction: -0.00127 (📉 Downtrend expected)
  ```

* **Visualizations**

  * 📉 Interactive candlestick charts
  * 📊 Daily returns & volatility trends

---

## 📂 Project Structure

```
📁 stock-market-analysis
│── 📓 Stock_Analysis.ipynb   # Main Jupyter Notebook
│── 📄 requirements.txt       # Required Python libraries
│── 📄 README.md              # Project documentation
│── 📄 AAPL_Enhanced.csv      # Example enhanced dataset (output)
```

---

## ✅ Future Improvements

* Add more **advanced ML models** (XGBoost, Transformers)
* Integrate **real-time news feeds** for sentiment
* Deploy as a **web dashboard (Streamlit/Flask)**
* Expand to **portfolio optimization & risk management**

---

## 🤝 Contributing

Pull requests are welcome! If you’d like to contribute, please fork the repo and create a feature branch.

---

## 📜 License

This project is licensed under the MIT License.

---

Would you like me to also create a **requirements.txt** for your repo so it’s plug-and-play on GitHub?
