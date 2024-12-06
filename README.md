# CS-675-Project-3-Time-Series-Forecasting-SunspotPrediction

# 1. Data Loading and Cleaning

The dataset is loaded from a CSV file.
Non-numeric values in the Sunspots column are handled.
Negative values in the dataset are treated as missing and removed.
Date columns are combined to form a datetime index for time-series operations.

# 2. Time Unit Analysis

A function (determine_time_unit) checks whether the dataset is daily or irregular.
This ensures the time-series data is consistent for analysis.

# 3. Basic Analysis and Visualization

Calculates statistics like mean and median of sunspots.
Identifies the day with the maximum sunspot count.
Visualizes the distribution of sunspot counts using a histogram.

# 4. Time-Series Forecasting

Prophet Configuration: The library is configured for linear, logistic, and flat growth.
Seasonality Customization:
Adds custom seasonalities for cycles like 1 year, 11 years (solar cycle), and other periods.
Changepoint Detection: Adjusts parameters to handle abrupt changes in trends.

# 5. Forecasting and Visualization

Extends the dataset into the future by generating placeholder dates.
Generates forecasts for 1 year, 10 years, and specific intervals (100, 200, 365 days).
Compares forecasts using different growth models and seasonal patterns.
Visualizes results to interpret the forecasts effectively.

# 6. Advanced Features

Includes functions to analyze the impact of parameters like n_changepoints and changepoint_prior_scale.
Provides flexibility for users to adjust seasonality, growth models, and forecast horizons.

The same is followed for month (specific intervals - 1,6,9 months) and year dataset (specific intervals - 1,10,20 years)
