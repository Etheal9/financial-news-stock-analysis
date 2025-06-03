
Predicting Price Moves with News Sentiment 📈📰

This repository contains a data pipeline and exploratory framework to analyze how financial news sentiment correlates with stock price movements. The goal is to derive actionable insights and build potential investment strategies using NLP and historical data.

 🔍 Project Overview

- **Sentiment Analysis** of financial news headlines using NLP.
- **Linking Sentiment to Stock Symbols** for companies like AAPL, AMZN, GOOG, META, MSFT, NVDA, TSLA.
- **Analyzing Stock Price Movements** before and after news events.
- **Identifying Patterns** between sentiment polarity and price trends.
- **Building Investment Strategies** based on sentiment-price correlations.
- **Final Report** delivered in PDF format for business stakeholders.



🧭 Project Structure



financial-news-stock-analysis/
├── data/
│   └── yfinance\_data/              # Historical stock CSVs (AAPL, AMZN, etc.)
├── notebooks/                      # EDA and sentiment exploration
│   ├── sentiment\_analysis.ipynb
│   ├── price\_movement\_analysis.ipynb
│   └── pattern\_identification.ipynb
├── reports/
│   └── Predicting\_Price\_Moves\_Report.pdf
├── src/
│   ├── sentiment\_utils.py          # TextBlob and preprocessing functions
│   ├── stock\_price\_utils.py       # Merge and analyze stock + sentiment data
│   └── strategy\_module.py         # Investment logic and pattern scoring
├── raw\_analyst\_ratings.csv        # News headlines dataset
├── requirements.txt               # Project dependencies
└── README.md                      




 📌 Objectives

### Phase 1: Sentiment Analysis
- ✅ Clean and preprocess financial news headlines.
- ✅ Calculate sentiment polarity using TextBlob.
- ✅ Visualize average sentiment per publisher and over time.

### Phase 2: Linking News to Stocks
- ✅ Associate each headline with a specific stock symbol.
- ✅ Merge sentiment scores with historical stock prices.

### Phase 3: Price Movement & Correlation
- ✅ Analyze price change before and after news dates.
- ✅ Compare sentiment direction with price trends.
- ✅ Plot average sentiment vs. average return.

### Phase 4: Strategy Insights
- ✅ Identify strong sentiment-return patterns.
- ✅ Propose rule-based investment ideas.
- ✅ Summarize findings in a business-friendly format.



 📈 Sample Insights

- Publishers like CNBC and MarketWatch have more positive sentiment skew.
- Negative headlines often follow price drops; positive ones sometimes precede short-term gains.
- Average sentiment can mildly correlate with next-day price changes, especially for high-volume stocks.



 ⚙️ Setup Instructions


# 1. Clone the repository
git clone https://github.com/Etheal9/financial-news-stock-analysis.git
cd financial-news-stock-analysis

# 2. Create a virtual environment and install dependencies
python -m venv .venv
source .venv/bin/activate     # On Windows: .venv\Scripts\activate
pip install -r requirements.txt

# 3. Launch the analysis notebooks
jupyter lab


📄 Final Deliverables

 ✅ Cleaned and preprocessed dataset
 ✅ NLP-based sentiment scores
 ✅ Visualized correlation between sentiment and price changes
 ✅ Proposed strategies and insights
 ✅ 📄 [Final PDF Report](./reports/Predicting_Price_Moves_Report.pdf)

 🙌 Author

**Etheal Sintayheu**
GitHub: [Etheal9](https://github.com/Etheal9)
Project Repo: [https://github.com/Etheal9/financial-news-stock-analysis](https://github.com/Etheal9/financial-news-stock-analysis)
