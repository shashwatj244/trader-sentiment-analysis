# 📊 Trader Performance vs Market Sentiment Analysis

## 🔹 Objective
The goal of this project is to analyze how market sentiment (Fear/Greed) impacts trader behavior and performance on Hyperliquid. The analysis aims to uncover patterns that can help design better trading strategies.

---

## 🔹 Datasets Used
1. Bitcoin Market Sentiment Dataset  
   - Columns: timestamp, value, classification, date  

2. Historical Trader Data  
   - Includes: Account, Execution Price, Size_USD, Side, Timestamp, Closed_PnL, etc.

---

## 🔹 Methodology

### 1. Data Cleaning
- Removed inconsistencies in column names  
- Converted timestamps to datetime format  
- Created a common `date` column  
- Merged both datasets on date  

### 2. Feature Engineering
- Created `win` column (profit/loss indicator)  
- Calculated:
  - Average PnL  
  - Win rate  
  - Trade size  
  - Trade frequency  

### 3. Analysis
- Compared trader performance across sentiment categories  
- Analyzed behavior changes (trade size, activity, etc.)  
- Visualized results using seaborn and matplotlib  

---

## 🔹 Key Insights

1. **Higher Profitability in Greed Markets**  
   Traders achieve the highest average PnL during Extreme Greed periods, indicating favorable conditions for profitable trades.

2. **Win Rate Follows Market Sentiment**  
   Win rates are highest in Extreme Greed and lowest in Extreme Fear, showing that traders struggle in bearish conditions.

3. **Risk-Taking Increases During Fear**  
   Traders take significantly larger positions during Fear periods, suggesting emotional or recovery-driven trading behavior.

---

## 🔹 Strategy Recommendations

1. **Reduce Risk During Fear Periods**  
   Traders should limit position sizes as larger trades during Fear lead to lower success rates.

2. **Leverage Favorable Conditions in Greed**  
   Higher participation during Greed phases can improve profitability, but overtrading should be avoided.

---

## 🔹 Tools Used
- Python (Pandas, NumPy)
- Data Visualization (Seaborn, Matplotlib)
- Google Colab

---

## 🔹 How to Run
1. Open the notebook in Google Colab  
2. Upload datasets  
3. Run all cells sequentially  

---

## 🔹 Conclusion
Market sentiment plays a critical role in trader performance and behavior. Understanding these patterns can help traders optimize strategies and manage risk effectively.
