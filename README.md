# Trader Behavior vs Market Sentiment (Primetrade.ai Assignment)

## 📌 Overview
This project explores how trader behavior (profitability, risk, and volume) aligns or diverges from Bitcoin market sentiment (Fear vs Greed).

**Datasets**
- **Hyperliquid Trader Data**: account, side, size (USD/tokens), execution price, PnL, timestamps.
- **Fear & Greed Index**: daily Bitcoin market sentiment.

> ⚠️ **Note:** The provided datasets do not overlap in time. This repo demonstrates the framework and methodology. On overlapping data, the same pipeline would produce sentiment-aligned insights.

---

## 📂 Project Structure
```
ds_aaysha_sheikh/
├── notebook_1.ipynb # Data preparation & cleaning
├── notebook_2.ipynb # Analysis, plots, and stats tests
├── csv_files/ # Cleaned data & analysis tables
│ ├── hyperliquid_trades_clean.csv
│ ├── fear_greed_clean.csv
│ ├── trades_with_sentiment.csv
│ ├── daily_sentiment_summary.csv
│ ├── sentiment_overall_summary.csv
│ ├── account_sentiment_performance.csv
│ └── side_share_by_sentiment.csv
├── outputs/ # Visual outputs
│ ├── trade_count_by_sentiment.png
│ ├── notional_by_sentiment.png
│ ├── pnl_by_sentiment.png
│ ├── winrate_by_sentiment.png
│ ├── leverage_by_sentiment_box.png
│ ├── side_share_by_sentiment.png
│ ├── accounts_greed_biased.png
│ └── accounts_fear_biased.png
├── ds_report.pdf # Final written report
└── README.md # Project documentation
```

---

## 🚀 How to Run
1. Open the notebooks in **Google Colab**:
   - `notebook_1.ipynb` → data setup, cleaning, merge  
   - `notebook_2.ipynb` → EDA, sentiment alignment, plots, stats tests  

2. Ensure the folder structure is preserved (`csv_files/`, `outputs/`).

3. All outputs (tables & plots) are saved automatically.

---

## 📊 Key Metrics
- **Profitability**: total/avg PnL, win rate  
- **Volume**: total notional traded  
- **Risk**: leverage distributions (if present)  
- **Side bias**: share of longs vs shorts  
- **Account performance**: trader-level breakdown by sentiment  

---

## ⚠️ Limitations
- No overlapping time periods between sentiment & trades (sentiment appears as “Unknown” in this dataset).  
- On overlapping data, this framework would validate if trading performance differs between Fear vs Greed.  
- Statistical testing framework (t-test / Mann–Whitney) included for use when overlap exists.  

---

## ✍️ Author
**Aaysha Sheikh**  
Candidate – Junior Data Scientist (Primetrade.ai Assignment)
