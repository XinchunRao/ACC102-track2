Superstore Sales Forecasting Tool

1. Problem & User 
Retail managers often struggle with inventory and staffing due to unpredictable daily demand; this project builds a SARIMA-based forecasting model to provide a 7-day sales outlook for Store Operations Managers to optimize daily resources.

2. Data 
Source: Kaggle - Sales Forecasting Dataset by Rohit Sahoo(https://www.kaggle.com/datasets/rohitsahoo/sales-forecasting)

Access Date: April 2026.

Key Fields: Order Date (Temporal index), Sales (Target variable), and Category (for context).


3. Methods (main Python steps)
Data Cleaning: Handled missing values and converted Order Date into a datetime index.

Aggregation: Resampled raw transaction data into a daily frequency to stabilize the time series.

EDA: Visualized historical trends and seasonal decomposition to identify cyclical patterns.

Modeling: Implemented a SARIMA (Seasonal Autoregressive Integrated Moving Average) model via statsmodels.

Output: Generated a 7-day forecast and exported results to prediction.csv.


4. Key Findings (3-5 bullets)
Upward Growth: The Superstore exhibits a consistent year-on-year growth trend in total sales volume.

High Seasonality: Sales peak significantly in late Q4 (November-December), likely driven by holiday shopping behavior.

Weekly Patterns: Analysis shows higher sales volatility on weekends compared to stable mid-week performance.

Model Accuracy: The SARIMA model successfully captured the 7-day seasonal lag inherent in the retail data.


5. How to run (optional but valuable)
Ensure Python 3.x is installed.

Install required libraries: pip install pandas numpy matplotlib seaborn statsmodels.

Place Sample - Superstore.csv in the same directory as the notebook.

Open ACC102 Track2 (1).ipynb and select "Restart & Run All" to generate the new prediction.csv.


6. Product link / Demo
Main Notebook: ACC102 Track2 (1).ipynb

Forecast Output: prediction.csv



7. Limitations & next steps
External Factors: Current predictions rely solely on historical sales and do not account for external shocks like local holiday changes or price promotions.

Linear Constraints: The SARIMA model assumes linear relationships; future iterations could incorporate XGBoost or Prophet to better handle non-linear spikes.

Granularity: Next steps include building sub-models for specific product categories (e.g., Technology vs. Furniture) for more targeted inventory planning.
