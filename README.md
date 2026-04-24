# Superstore Sales Forecasting Tool

## 1. Problem & User
Retail managers often struggle with inventory and staffing due to unpredictable daily demand; this project builds a SARIMA-based forecasting model to provide a 7-day sales outlook for **Store Operations Managers** to optimize daily resources.

## 2. Data
* **Source**: [Kaggle - Sales Forecasting Dataset](https://www.kaggle.com/datasets/rohitsahoo/sales-forecasting) by Rohit Sahoo.
* **Access Date**: April 2026.
* **Key Fields**: `Order Date` (Temporal index), `Sales` (Target variable).

## 3. Methods
1. **Data Cleaning**: Handled missing values and converted `Order Date` to datetime.
2. **Aggregation**: Resampled data into a daily frequency.
3. **EDA**: Visualized historical trends and seasonal decomposition.
4. **Modeling**: Implemented a **SARIMA** model via `statsmodels`.
5. **Output**: Generated a 7-day forecast saved as `prediction.csv`.

## 4. Key Findings
* **Upward Growth**: The store exhibits a consistent year-on-year growth trend.
* **High Seasonality**: Sales peak significantly in late Q4 due to holiday shopping.
* **Weekly Patterns**: Higher volatility on weekends compared to stable mid-week performance.
* **Accuracy**: SARIMA successfully captured the 7-day seasonal lag.

## 5. How to run
1. Ensure Python 3.x is installed.
2. Install libraries: `pip install pandas numpy matplotlib seaborn statsmodels`.
3. Place `Sample - Superstore.csv` in the `/data` folder.
4. Run `ACC102 Track2 (1).ipynb` to generate `prediction.csv`.

## 6. Product link / Demo
* **Main Notebook**: [Track2 .ipynb](./Track2%20.ipynb)
* **Forecast Output**: [prediction.csv](./prediction.csv)
* **Dataset Source**: [View on Kaggle](https://www.kaggle.com/datasets/rohitsahoo/sales-forecasting)

## 7. Limitations & next steps
* **External Factors**: Does not account for local holidays or competitor discounts.
* **Linear Constraints**: Future iterations could use **XGBoost** for non-linear spikes.
* **Granularity**: Next steps include building category-specific models (e.g., Technology).
