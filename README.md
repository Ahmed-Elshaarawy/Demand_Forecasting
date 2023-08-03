# Demand_Forecasting
Link to the Dataset:https://www.kaggle.com/competitions/store-sales-time-series-forecasting/data?select=train.csv

# Time Series Forecasting with Prophet

**Summary**
The `forecasting.ipynb` notebook demonstrates a time series forecasting process using the Prophet library. It focuses on forecasting demand for different product families based on historical sales data.

**Data Preprocessing**
- The notebook begins by reading the sales data from a CSV file and performs data cleaning and column renaming.
- The date column is converted to a datetime format, and the data is aggregated at the daily level for each family of products.

**Exploratory Data Analysis (EDA)**
- The EDA section visualizes the historical sales trends for each product family using line plots.

**Data Split and Volume Classification**
- The data is split into training and testing sets, with the testing set representing future time periods for forecasting evaluation.
- The product families are categorized into low, mid, and high volume based on their average daily sales.

**Forecasting with Prophet**
- The Prophet library is used to create time series forecasting models for each product family.
- The models are trained on the historical data for each family.
- The forecasts are made for a specific prediction horizon (30 days in the example).

**Model Evaluation**
- The models' performance is evaluated using Mean Absolute Percentage Error (MAPE) on the testing set.
- Cross-validation is applied to test the models over various time periods to evaluate their robustness.

**Hyperparameter Tuning**
- The notebook demonstrates hyperparameter tuning for the Prophet model to find the best combination of parameters.
- The tuning is done using cross-validation and evaluating the RMSE metric for different parameter combinations.

**Example Usage**
The notebook showcases an example usage for demand forecasting, specifically focusing on the "PRODUCE" product family. It demonstrates how to create a forecast for this specific product using the trained Prophet model.

