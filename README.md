# Trader Performance vs Market Sentiment Analysis

## Overview
This project analyzes how Bitcoin Fear & Greed sentiment influences trader behavior and performance on Hyperliquid.  
The goal is to identify performance patterns, behavioral shifts, and segment-specific risk dynamics to derive actionable trading insights.

---

## Objectives
- Evaluate performance differences across sentiment regimes (Fear vs Greed)
- Analyze behavioral changes in trade size, activity, and directional bias
- Segment traders by frequency and consistency
- Propose actionable strategy recommendations based on findings

---

## Datasets Used
1. **Bitcoin Fear & Greed Index**
   - Date
   - Sentiment classification (Extreme Fear → Extreme Greed)

2. **Hyperliquid Historical Trader Data**
   - Account
   - Trade size (USD & tokens)
   - Side (BUY/SELL)
   - Closed PnL
   - Timestamp
   - Other trade metadata

---

## Methodology

### 1. Data Preparation
- Cleaned and aligned datasets at daily frequency
- Handled missing sentiment labels
- Standardized column names
- Created key metrics:
  - Win rate
  - Daily aggregated PnL
  - Loss-day probability (drawdown proxy)
  - Trade size
  - Daily trade activity
  - Long/Short ratio

### 2. Performance Analysis
Compared:
- Average PnL by sentiment
- Win rate by sentiment
- Loss-day probability by sentiment

### 3. Behavioral Analysis
Evaluated:
- Average trade size
- Average daily trade activity
- Long/Short positioning bias

### 4. Trader Segmentation
Two segmentation approaches were applied:

- **Frequent vs Infrequent Traders** (median trade count split)
- **Consistent vs Inconsistent Traders** (median PnL volatility split)

Performance and downside risk were analyzed across sentiment regimes for each segment.

---

## Key Insights

1. Extreme Greed regimes show the highest profitability and lowest downside risk.
2. Extreme Fear significantly increases loss-day probability.
3. Infrequent traders tend to outperform during bullish sentiment regimes.
4. High-volatility traders amplify sentiment-driven gains and losses.

---

## Strategy Recommendations

- Implement sentiment-based risk scaling (reduce exposure in Fear, expand cautiously in Greed).
- Allocate capital dynamically based on trader segment and sentiment regime.
- Tighten risk controls for high-volatility traders during fearful market conditions.

---

## Tools & Libraries
- Python
- Pandas
- NumPy
- Seaborn
- Matplotlib

---

## Repository Contents
- `trader_sentiment_analysis.ipynb` – Full analysis notebook
- `README.md` – Project documentation
