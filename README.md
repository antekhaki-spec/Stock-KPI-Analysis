# Stock-KPI-Analysis
Antoni Hakizimana Stock Market Analisys
# Stock Data Quality Analysis (KPI Assignment)
**Author:** Antoni Hakizimana

## Data Card Information

### 1. Source of Data: Full Description
This dataset contains historical stock market data for 5 selected NASDAQ companies: **Microsoft (MSFT), Netflix (NFLX), Palantir (PLTR), Tesla (TSLA), and Apple (AAPL)**. 

The data was programmatically retrieved using the `yfinance` library, which fetches data from the **Yahoo Finance API**. The dataset focuses on the daily "Close" price, which is the standard benchmark for financial model training. Each company has a **different time period** to ensure diversity in the dataset, ranging from 3 months to a full year.

### 2. All the KPIs (Quantitative Assessment)
Below are the quality metrics measured for each dataset:

| Company | Ticker | Completeness (%) | Latency (Data Span) | Consistency (%) | Accuracy (ADF Statistic) |
| :--- | :--- | :--- | :--- | :--- | :--- |
| Microsoft | MSFT | 100% | 362 Days | 100% | -1.16 |
| Netflix | NFLX | 100% | 213 Days | 100% | -1.45 |
| Palantir | PLTR | 100% | 184 Days | 100% | -1.82 |
| Tesla | TSLA | 100% | 105 Days | 100% | -2.01 |
| Apple | AAPL | 100% | 184 Days | 100% | -0.95 |

**Metric Definitions:**
*   **Completeness:** Ratio of non-missing values to total records (0 nulls found).
*   **Latency:** The duration of the historical window; data is updated daily (Low Latency).
*   **Consistency:** Percentage of data points following the `float64` format with standardized timestamps.
*   **Accuracy:** Verified through visual inspection and the **Augmented Dickey-Fuller (ADF) Test** for price trend stability.

### 3. Conclusion
The dataset assessment shows high-quality results across all 5 tickers. With **100% completeness** and **consistent formatting**, this data is highly reliable for training AI models, performing trend analysis, or building financial visualizations. The varied time ranges provide a robust foundation for testing model adaptability to different market conditions.
