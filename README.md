# Stock-KPI-Analysis
Antoni Hakizimana Stock Market Analisys
# Stock Data Quality Analysis (KPI Assignment)
**Author:** Antoni Hakizimana

## Data Card Information

### 1. Source of Data: Full Description
The dataset consists of historical financial data for 5 major companies listed on the NASDAQ exchange: Microsoft (MSFT), Netflix (NFLX), Palantir (PLTR), Tesla (TSLA), and Apple (AAPL). 

The primary source is the **Yahoo Finance API**, accessed via the `yfinance` Python library. The data points collected include daily **Closing Prices** adjusted for splits and dividends. Each company was purposely analyzed over a unique time period to ensure variety in the training dataset.

### 2. Key Performance Indicators (KPIs)
| Company | Ticker | Date Range | Completeness | Latency | Accuracy | Consistency |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Microsoft | MSFT | 2023-01-01 to 2023-12-31 | 100% | Low | Verified | High |
| Netflix | NFLX | 2023-06-01 to 2023-12-31 | 100% | Low | Verified | High |
| Palantir | PLTR | 2023-08-01 to 2024-02-01 | 100% | Low | Verified | High |
| Tesla | TSLA | 2024-01-01 to 2024-04-15 | 100% | Low | Verified | High |
| Apple | AAPL | 2023-03-01 to 2023-09-01 | 100% | Low | Verified | High |

### 3. Conclusion
The dataset assessment confirms high quality across all established KPIs:
* **Completeness:** There are zero missing values in the "Close" price columns.
* **Latency:** Data latency is categorized as **Low**, as the records are fetched directly from the exchange's digital feed with updates available immediately after each trading session.
* **Accuracy:** Statistical descriptions (`describe()`) confirm the price values are within realistic market ranges.
* **Consistency:** All data formats (Date as index and Float64 for prices) are uniform across all five datasets.

This dataset is fully prepared and recommended for training AI models or conducting financial trend visualizations.
