# Ride-Sharing Demand Forecasting Using Machine Learning

 Predict hourly ride demand using historical ride data to help ride-sharing platforms optimize driver allocation.

## Project overview
- Problem: Predict hourly ride demand using historical ride data.
- Why it matters: Better demand forecasting helps reduce rider wait times and improves driver utilization.
- Approach: Time-series feature engineering + tree-based regression (example: RandomForestRegressor). See notebook for exact steps.

## Problem statement
Predict hourly ride demand using historical ride records so the platform can pre-position drivers and adjust pricing or incentives.

## Dataset
- Source:kaggle (see `data/README.md` for how to obtain or prepare the dataset).
- Features used: timestamp, location (zone), rolling lags, hour/day encodings, weather (if available).
- Target variable: hourly ride count (or demand per zone/hour).

## Methods
- Time-series feature engineering (lags, rolling means)
- Data preprocessing and cleaning
- Model: RandomForestRegressor (example)
- Train/validation split: time-based split
- Evaluation: MAE, RMSE, and visualizations (actual vs predicted)

## Results
See the notebook `time-series-ride-demand.ipynb` for detailed results, plots (feature importance and actual vs predicted), and discussion.


