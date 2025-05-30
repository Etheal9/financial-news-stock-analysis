
# Financial News Stock Sentiment Analysis

This repository analyzes the sentiment of financial news headlines and links them to stock price movements to discover patterns and develop predictive strategies for investment.

---

## 🛍️ Project Structure

```
financial-news-stock-analysis/
├── data/
│   ├── raw_analyst_ratings.csv                 # News headlines dataset
│   └── yfinance_data/
│       ├── AAPL_historical_data.csv
│       ├── AMZN_historical_data.csv
│       ├── GOOG_historical_data.csv
│       ├── META_historical_data.csv
│       ├── MSFT_historical_data.csv
│       ├── NVDA_historical_data.csv
│       └── TSLA_historical_data.csv
├── notebooks/                                  # Future analysis and reports
├── src/                                        # Core processing and utils (planned)
├── outputs/                                    # Cleaned or merged data (planned)
├── requirements.txt
└── README.md
```

---

## 📌 Project Objectives

Main goal: Analyze how financial news sentiment impacts stock prices and develop data-driven investment strategies.

### ✅ Goals

* **Sentiment Analysis:** Assign polarity scores to each news headline.
* **Ticker Matching:** Match each headline with a relevant stock symbol.
* **Stock Price Linkage:** Link stock closing prices to the date of the news.
* **Pattern Discovery:** Analyze correlation between sentiment and price movement.
* **Strategy Design:** Recommend trading strategies based on sentiment insights.
* **Reporting:** Deliver a final report with actionable insights for Nova.

---

## 📈 Current Progress

### ✅ Data Loading & Initial Exploration

* Loaded `raw_analyst_ratings.csv` with financial news headlines.
* Performed basic profiling: headline length, publisher frequency, date distribution.

### ✅ Text Vectorization

* Used `CountVectorizer` to extract top keywords from headlines.

### ✅ Sentiment Analysis

* Applied `TextBlob` to calculate sentiment polarity scores per headline.
* Plotted average sentiment per day and by publisher.

### ✅ Data Cleaning & Transformation

* Converted `date` column to datetime.
* Extracted publishing time and frequency.
* Removed timezone and ensured uniform datetime formats.

### ✅ Stock Price Data Integration

* Loaded historical price data for 7 tickers (AAPL, AMZN, GOOG, META, MSFT, NVDA, TSLA).
* All files are parsed, cleaned, and stored under `yfinance_data/`.

---

## 📆 Next Steps

### ⏳ Merge News with Price Data

* Match headlines to stock prices by date and ticker symbol.
* Calculate next-day return from price data.

### 🔄 Correlation Analysis

* Run correlation between sentiment score and 1-day stock return.
* Explore lagging sentiment vs. price (0-day, +1-day, +2-day).

### 🧹 Strategy Development

* Build simple sentiment-based trading signals.
* Backtest basic rules (e.g., buy when sentiment > 0.5).

### 📄 Final Report

* Summarize findings.
* Include charts: sentiment distributions, returns vs. sentiment, etc.
* Deliver to Nova with clear investment recommendations.

---

## ⚙️ Setup Environment

```bash
git clone https://github.com/Natty4/financial-news-stock-analysis.git
cd financial-news-stock-analysis
python -m venv .venv
source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install -r requirements.txt
```

---

## 🙌 Acknowledgments

Built for Nova as part of a financial data analysis initiative. Thanks to the Nova team for support and challenge framing.
