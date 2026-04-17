# Trader Performance vs Market Sentiment

## Overview
In this project, I analyzed how market sentiment (Fear and Greed) affects trader behavior and performance using real trading data from Hyperliquid.

The main goal was to understand whether traders behave differently during Fear vs Greed conditions and how that impacts their profitability.

---

## Datasets Used
I used two datasets:

1. **Market Sentiment Data**
   - Contains daily sentiment classification (Fear, Greed, Extreme Fear, etc.)

2. **Trader Data**
   - Includes trade details like account, trade size, price, side, timestamp, and PnL

---

## What I Did

### 1. Data Cleaning
- Renamed columns for easier handling
- Converted timestamps into proper datetime format
- Created a common `date` column in both datasets
- Merged both datasets on date

---

### 2. Feature Creation
I created some useful metrics:
- **Win column** (whether trade was profitable or not)
- **Average PnL**
- **Win rate**
- **Trade size (Size_USD)**
- **Trade count**

---

### 3. Analysis

I compared trader behavior across different sentiment categories.

#### Key observations:
- Average PnL changes based on sentiment
- Win rate also varies with sentiment
- Trade size shows how risky traders are under different conditions

I also used graphs (boxplots and bar charts) to visualize the patterns.

---

## Key Insights

1. **Better performance during Greed**
   Traders achieve higher profits and better win rates during Extreme Greed conditions.

2. **Poor performance during Fear**
   Both PnL and win rate drop during Fear and Extreme Fear phases.

3. **Higher risk-taking during Fear**
   Surprisingly, traders take larger positions during Fear periods, which may indicate emotional or recovery-driven trading.

---

## Strategy Suggestions

- During Fear periods, traders should reduce position sizes to control losses.
- During Greed phases, traders can participate more, but should avoid overtrading.
- Risk management should be stricter when the market sentiment is negative.

---

## Tools Used
- Python
- Pandas
- Matplotlib
- Seaborn
- Google Colab

---

## How to Run
1. Open the notebook in Google Colab
2. Upload the datasets
3. Run all cells step by step

---

## Final Thoughts
This analysis shows that market sentiment has a clear impact on trader behavior. Understanding these patterns can help traders make better decisions and manage risk more effectively.
