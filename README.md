# Trader Performance vs Market Sentiment — Analysis
**By Rushi**

---

## Overview
This project explores whether Bitcoin market sentiment (Fear vs Greed) has a measurable impact on trader performance using Hyperliquid's historical trade data.

**Dataset size:** 211,224 trades | **Period:** May 2023 – May 2025

---

## Files in this folder

| File | Description |
|------|-------------|
| `trader_sentiment_analysis.ipynb` | Main analysis notebook |
| `README.md` | This file |
| `chart_01_pnl_winrate.png` | Avg PnL and win rate per sentiment phase |
| `chart_02_long_short_pnl.png` | Long vs Short PnL across sentiment phases |
| `chart_03_coins_by_sentiment.png` | Most traded coins by sentiment |
| `chart_04_top_traders_sentiment.png` | Top 10 vs all traders sentiment distribution |
| `chart_05_cumulative_pnl.png` | Cumulative PnL over time with sentiment overlay |
| `chart_06_fee_impact.png` | Gross PnL vs fees vs net PnL by sentiment |

---

## Datasets Used

| File | Columns Used |
|------|-------------|
| `historical_data.csv` | Account, Coin, Direction, Closed PnL, Fee, Timestamp IST, Size USD |
| `fear_greed_index.csv` | date, value, classification |

---

## How to Run (Google Colab)

1. Go to [colab.research.google.com](https://colab.research.google.com)
2. File → Upload notebook → select `trader_sentiment_analysis.ipynb`
3. Upload both CSVs using the folder icon on the left sidebar
4. The paths in Cell 3 are already set to `/content/` (Colab default) — no changes needed
5. Runtime → Run all

---

## How to Run (Local)

```bash
pip install pandas numpy matplotlib seaborn jupyter
jupyter notebook trader_sentiment_analysis.ipynb
```

Update Cell 3 paths to your local file locations.

---

## Key Questions Answered

1. Which sentiment phase produces the highest average PnL per trade?
2. Do long or short trades perform better in Fear vs Greed?
3. What coins do traders prefer in each sentiment phase?
4. Do top traders have a different sentiment trading pattern vs average traders?
5. What is the fee impact by sentiment phase?

---

*Submitted as part of the Primetrade.ai Data Science Hiring Assignment*
