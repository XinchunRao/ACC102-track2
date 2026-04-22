# ACC102-track2
Data analysis project for ACC102 mini task

## 1. Problem & User
This project completes the ACC102 mini task by conducting data analysis to support business decision-making for accounting students and course instructors.

## 2. Data
- Source: Kaggle (Rohit Sahoo, Sales Forecasting Dataset)
- Access Date: April 2026
- Key Fields: Order Date, Sales, Profit, Discount, Region, Category, Sub-Category

## 3. Methods (main Python steps)
1. Use pandas to load, clean, and preprocess the dataset
2. Perform exploratory data analysis with pandas and matplotlib
3. Calculate key financial ratios and visualize trends
4. Summarize findings to meet ACC102 mini task requirements

## 4. Key Findings
-The time series analysis confirms clear daily and monthly seasonal patterns in historical sales data.
-The SARIMA model successfully captures sales trends and seasonal fluctuations, with a final RMSE of 269.87, showing reliable prediction performance.
-The model generates accurate 7-day future sales forecasts, which can directly support store inventory planning and staffing arrangements.
-Pandas is used throughout the project to clean, sort, and resample time series data, ensuring the accuracy of model input.
-The sales forecasting results provide actionable, data-driven insights for store daily operation decisions.

## 5. How to run
1. Clone this repository: `git clone https://github.com/XinchunRao/ACC102-track2.git`
2. Install dependencies: `pip install pandas numpy matplotlib jupyter`
3. Open `notebook.ipynb` in Jupyter and run all cells to reproduce the analysis

## 6. Product link / Demo


## 7. Limitations & next steps
- Limitations: The dataset only covers one fiscal year, without external market factors
- Next steps: Expand the dataset, add advanced financial models, build an interactive dashboard
