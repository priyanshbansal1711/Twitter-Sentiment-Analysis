# Twitter-Sentiment-Analysis
Twitter sentiment analysis trading strategy: ranks stocks by engagement ratio (likes/comments) on Twitter, selects top 5 monthly, equal-weight portfolio. Backtested 2021–2023 vs Nasdaq (QQQ).
Builds a momentum-style strategy using Twitter engagement as a proxy for sentiment: ranks stocks cross-sectionally by likes/comments ratio each month, picks top 5, equal-weights, and rebalances. Compares to QQQ benchmark.​

# What this notebook does
1. Loads daily Twitter data (posts, comments, likes, impressions, sentiment) for ~85 US stocks (2021–2023).​
2. Computes engagement ratio, filters active stocks, aggregates monthly, ranks by engagement.​
3. Selects top 5 stocks per month-end for equal-weight portfolio.​
4. Downloads prices via yfinance, computes daily returns, aggregates to portfolio level.​
5. Plots cumulative strategy returns vs QQQ buy-and-hold.​

# Tech stack
1. Language: Python 3 (Jupyter Notebook).​
2. Core libraries: pandas, numpy, yfinance, matplotlib.​

# How to run
1. Clone repo, open Twitter-Sentiment-Analysis-P2.ipynb in Jupyter/VS Code.​
2. Ensure sentimentdata.csv is in the folder (or adapt loader).​
3. Install deps (pandas, numpy, yfinance, matplotlib), run cells sequentially.​

# Project structure
1. Twitter-Sentiment-Analysis-P2.ipynb – full pipeline from data to backtest.

