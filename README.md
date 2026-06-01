# Quantitative Analysis: Trader Performance vs. Market Sentiment
**Primetrade.ai Data Science Hiring Assignment**  
*Prepared by: Rushikesh Kolla*

---

## 📌 Executive Summary
This project investigates the impact of Bitcoin market sentiment (Fear vs. Greed) on trader performance utilizing historical trade data from Hyperliquid. By analyzing over **211,224 trades** spanning from May 2023 to May 2025, this analysis uncovers hidden behavioral patterns, evaluates profitability across different market regimes, and delivers actionable, data-driven insights for algorithmic trading strategies.

## 🗂️ Project Structure

| File/Resource | Description |
|------|-------------|
| 📓 `trader_sentiment_analysis.ipynb` | Core Jupyter Notebook containing the data pipeline, EDA, statistical analysis, and strategic conclusions. |
| 📦 `data.zip` | Compressed archive containing the raw historical trade data and the Fear/Greed index datasets. |
| 📄 `README.md` | Project documentation and reproduction instructions. |

*Note: Visualizations (Charts 1-6) demonstrating PnL win rates, long/short performance, and fee impacts are dynamically generated within the Jupyter Notebook upon execution.*

## 📊 Datasets Utilized
1. **Hyperliquid Historical Trader Data:** Features include Account ID, Coin Symbol, Trade Direction, Closed PnL, Fees, Timestamps, and Sizing.
2. **Bitcoin Market Sentiment Dataset:** Features include Date, Index Value, and Market Classification (Fear/Greed/Neutral).

## 💡 Key Research Questions Addressed
This analysis provides empirical answers to the following strategic questions:
1. Which market sentiment phase yields the highest average PnL and win rate?
2. How does the performance of *Long* vs. *Short* trades diverge during extreme Fear vs. extreme Greed?
3. Which assets (coins) experience the highest volume concentrations during specific sentiment phases?
4. **Alpha Generation:** Do the Top 10 most profitable traders exhibit different sentiment-based trading patterns compared to the broader retail average?
5. What is the proportionate impact of exchange fees on Gross vs. Net PnL across different market conditions?

## 🚀 How to Run the Analysis

### Option A: Google Colab (Recommended for ease of use)
1. Navigate to [Google Colab](https://colab.research.google.com/).
2. Select **File → Upload notebook** and upload `trader_sentiment_analysis.ipynb`.
3. Extract `data.zip` locally, then use the Colab file explorer (left sidebar) to upload the extracted `.csv` files.
4. *Note: Data paths in Cell 3 are pre-configured for Colab's `/content/` directory.*
5. Select **Runtime → Run all**.

### Option B: Local Environment
Ensure you have Python 3.8+ installed.

1. **Install required dependencies:**
   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```
2. **Unzip the data:** Extract the contents of `data.zip` into the project root directory.
3. **Launch Jupyter:**
   ```bash
   jupyter notebook trader_sentiment_analysis.ipynb
   ```
4. *Note: Update the file paths in Cell 3 of the notebook to match your local extraction directory if different from the root.*

---
*Submitted for the Data Science position at Primetrade.ai.*
