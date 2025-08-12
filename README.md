# Trader Behavior Insights

### Project Overview

This project explores the relationship between trader performance and market sentiment using two primary datasets: historical trading data from Hyperliquid and the Bitcoin Fear & Greed Index. The objective is to uncover hidden patterns and deliver actionable insights that can drive smarter trading strategies in the Web3 space.

### Datasets

The analysis was performed using two datasets:
1.  **Historical Trader Data from Hyperliquid:** Contains detailed transaction-level data, including account information, execution prices, trade sizes, and closed PnL.
2.  **Bitcoin Market Sentiment Dataset:** A daily record of the market's sentiment, classified as Fear, Greed, Extreme Fear, Extreme Greed, or Neutral.

### Methodology

The analysis followed a structured data science workflow:
1.  **Data Loading & Cleaning:** Loaded the CSV files into pandas DataFrames. Converted date and timestamp columns to the correct `datetime` format.
2.  **Data Aggregation:** Aggregated the granular trader data to a daily level, calculating the total PnL and number of trades for each trader per day.
3.  **Data Merging:** Merged the aggregated trader performance data with the daily sentiment data on the common date column.
4.  **Exploratory Analysis:** Conducted an exploratory analysis to identify relationships and patterns between trader PnL and market sentiment.

### Key Findings & Insights

Based on the analysis, here are the key insights that can be used to inform trading strategies:

* **Fear Outperforms Greed:** Traders in this dataset performed better, on average, during periods of **Fear** and **Extreme Fear** compared to periods of general **Greed**.
* **Extremes of Sentiment are Key:** The most profitable trading days were associated with the extremes of market sentiment (both high and low values), suggesting that volatile market conditions are more conducive to high returns for these traders.
* **No Simple Linear Correlation:** The analysis revealed no strong linear relationship between a trader's daily PnL and the numerical value of the Fear & Greed Index.

### Technologies Used

* Python
* Pandas
* Matplotlib