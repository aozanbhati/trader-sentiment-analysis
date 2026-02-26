# Trader Performance vs Market Sentiment Analysis

## Overview
This project analyzes how Bitcoin Fear & Greed sentiment influences trader behavior and performance on Hyperliquid.  
The objective is to identify performance patterns, behavioral shifts, and segment-based risk dynamics to derive actionable trading insights.

---

## Key Components

### 1. Data Preparation
- Cleaned and aligned sentiment and trade data at daily frequency
- Handled missing sentiment labels
- Standardized column names
- Created performance and risk metrics (PnL, win rate, loss-day probability)

### 2. Performance Analysis
- Average PnL by sentiment
- Win rate by sentiment
- Loss-day probability (drawdown proxy)

### 3. Behavioral Analysis
- Average trade size
- Average daily trade activity
- Long/Short positioning bias

### 4. Trader Segmentation
- Frequent vs Infrequent traders (median trade count split)
- Consistent vs Inconsistent traders (PnL volatility split)
- Performance and risk comparison across sentiment regimes

---

## Strategy Insights
- Scale risk exposure based on sentiment regime
- Adjust capital allocation based on trader segment and volatility profile

---

## How to Run
1. Clone the repository  
   `git clone (https://github.com/aozanbhati/trader-sentiment-analysis.git)`

2. Install dependencies  
   `pip install pandas numpy matplotlib seaborn`

3. Open and run  
   `trader_sentiment_analysis.ipynb`
