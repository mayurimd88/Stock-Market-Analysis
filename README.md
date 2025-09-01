# 📊 Stock Market Analysis Project (Python – Jupyter Notebook)

## 📌 Overview
This project performs **stock market analysis** on four major companies:  
- **Apple (AAPL)**  
- **Microsoft (MSFT)**  
- **Netflix (NFLX)**  
- **Google (GOOG)**  

The analysis uses **Python (Jupyter Notebook)** and covers stock price trends, moving averages, volatility, correlations, and performance comparisons.

---

## 🗂 Dataset
- Daily stock data (Open, High, Low, Close, Adj Close, Volume)  
- Tickers: AAPL, MSFT, NFLX, GOOG  
- Time period: ~3 months  

---

## 🛠️ Libraries Used
- **pandas** – data manipulation  
- **numpy** – numerical operations  
- **matplotlib & seaborn** – visualizations  
- **plotly** – interactive plots  

---

## 📑 Project Workflow

### 1️⃣ Load Dataset
- Imported stock data from CSV  
- Converted `Date` column to datetime  
- Sorted data by `Ticker` and `Date`  
- Previewed 2 rows per company  

**Insight:**  
✔ Dataset structure confirmed → multiple companies with time-series data.

---

### 2️⃣ Exploratory Data Analysis (EDA)
- Used `.info()`, `.describe()` for summary statistics  
- Boxplot of closing prices  

**Insight:**  
✔ Prices range from ~$90 (GOOG) to ~$366 (NFLX).  
✔ Apple & Google are stable, Microsoft is moderately volatile, Netflix is most volatile.  
✔ Trading volume highest in Apple, lowest in Netflix.  

---

### 3️⃣ Stock Price Trends
- Line plots of closing prices  

**Insight:**  
✔ Apple & Microsoft show steady upward trends.  
✔ Google is flat with mild growth.  
✔ Netflix is highest but volatile.  

---

### 4️⃣ Moving Averages
- 10-Day Moving Average (MA) vs Closing Price  

**Insight:**  
✔ AAPL & MSFT align well with MA → steady performers.  
✔ NFLX deviates → volatility.  
✔ GOOG remains flat with weak momentum.  

---

### 5️⃣ Volatility Analysis
- 10-Day Rolling Volatility  

**Insight:**  
✔ NFLX shows highest volatility → riskiest.  
✔ GOOG shows moderate volatility.  
✔ AAPL & MSFT are more stable.  

---

### 6️⃣ Correlation Analysis
- Heatmap of correlations among tickers  

**Insight:**  
✔ AAPL, MSFT, GOOG strongly correlated (0.88–0.95).  
✔ NFLX weakly correlated (0.15–0.22) → independent, useful for diversification.  

---

### 7️⃣ Performance Analysis
- Cumulative returns plotted  
- Percentage change over 3 months  

**Insight:**  
✔ **MSFT: +16.1% → Best performer**  
✔ **AAPL: +12.2% → Strong growth**  
✔ **GOOG: -1.7% → Slightly negative**  
✔ **NFLX: -11.1% → Worst performer**  

---

### 8️⃣ Interactive Plot
- Plotly interactive stock price visualization  

**Insight:**  
✔ Confirms earlier trends.  
✔ MSFT & AAPL rising, GOOG flat, NFLX declining.  
✔ Interactive tool helps zoom & filter by ticker.  

---

## ✅ Final Conclusion
- **Best for conservative investors:** AAPL, MSFT → steady growth, low volatility  
- **For risk takers:** NFLX → high volatility, independent, good for diversification  
- **Moderate option:** GOOG → stable but less dynamic growth  

---

## 🚀 How to Run
1. Clone this repository  
2. Install dependencies:  
   ```bash
   pip install pandas numpy matplotlib seaborn plotly
