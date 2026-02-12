# 📊 Trader Performance vs Market Sentiment Analysis

## 📌 Objective
Analyze how **Bitcoin market sentiment (Fear vs Greed)** affects **trader behavior and profitability** on Hyperliquid and derive **actionable trading strategies** from the findings.

This project was completed as part of the Data Science Intern assignment.

---

# 📁 Datasets

## 1. Market Sentiment (Fear/Greed)
Daily sentiment classification
Columns:
- timestamp
- value
- classification (Fear/Greed)
- date

~2,644 daily records

## 2. Historical Trader Data
Trade-level execution logs
Columns include:
- account
- side
- execution_price
- size_usd
- closed_pnl
- timestamp

~211,224 trades

---

# ⚙️ Methodology

## Data Preparation
- Removed duplicates
- Checked missing values
- Standardized column names (lowercase + underscores)
- Converted timestamps using `unit='ms'`
- Created daily dates
- Merged trades with daily sentiment

## Feature Engineering
Created metrics:
- Daily PnL per trader
- Win rate
- Trade frequency
- Average trade size (risk proxy)
- Long/Short ratio
- Trader volatility (PnL std)

## Segmentation
Traders grouped into:
- Frequent vs Infrequent traders
- High-risk vs Low-risk (size-based)
- Consistent vs Volatile (PnL variability)

---

# 📈 Analysis Performed

## 1. Performance vs Sentiment
Compared:
- Average PnL
- Total PnL
- Win rate
- Trade count

Visualizations:
- Boxplots
- Bar charts
- Daily PnL trends

## 2. Behavioral Changes
Analyzed:
- Trade frequency
- Position size
- Long/Short bias

## 3. Trader Segments
Studied how different trader types behave under Fear and Greed conditions.

---

# 🔍 Key Insights

### Insight 1 — Sentiment impacts profitability
Greed days show higher average PnL and win rates, while Fear days show reduced profitability and fewer trades.

### Insight 2 — Risk appetite changes with sentiment
Traders increase position sizes and trading activity during Greed, indicating higher risk-taking behavior.

### Insight 3 — Trader consistency matters
Consistent traders maintain stable returns across both sentiments, while volatile traders experience large losses during Fear periods.

---

# 💡 Strategy Recommendations (Actionable Rules)

## Strategy 1 — Risk Control During Fear
Reduce trade size and frequency during Fear sentiment to limit drawdowns and protect capital.

Rule of thumb:
→ Cut average position size by 30–50% on Fear days.

---

## Strategy 2 — Momentum Trading During Greed
Increase trade activity when market sentiment is Greed to capitalize on higher win rates and momentum.

Rule of thumb:
→ Increase trade frequency and allow moderately larger position sizes.

---

## Strategy 3 — Segment-Based Capital Allocation
Allocate more capital to consistent traders and restrict exposure for volatile traders.

Rule of thumb:
→ Apply tighter risk limits to high-volatility traders, especially during Fear periods.

---

# ▶️ How to Run

## Install dependencies


---

# 🛠 Tech Stack
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

---

# 👤 Author
Navin Raja

