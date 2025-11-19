# Ride-Sharing Demand Forecasting Using Machine Learning

Short: Predict hourly ride demand using historical ride data to help ride-sharing platforms optimize driver allocation.

## Project overview
- Problem: Predict hourly ride demand using historical ride data.
- Why it matters: Better demand forecasting helps reduce rider wait times and improves driver utilization.
- Approach: Time-series feature engineering + tree-based regression (example: RandomForestRegressor). See notebook for exact steps.

## Problem statement
Predict hourly ride demand using historical ride records so the platform can pre-position drivers and adjust pricing or incentives.

## Dataset
- Source: Not included in this repository (see `data/README.md` for how to obtain or prepare the dataset).
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

## How to run
1. Clone the repo:

   git clone https://github.com/<your-username>/ride-sharing-demand-forecasting.git

2. Create and activate a Python environment (recommended) and install dependencies:

   python -m venv .venv
   .\.venv\Scripts\Activate.ps1  # in PowerShell
   pip install -r requirements.txt

3. Open the notebook `time-series-ride-demand.ipynb` in Jupyter or VS Code and run all cells.

Notes: If the dataset is large it is NOT included. See `data/README.md` for steps to obtain or generate the data.

## Future improvements
- Try LSTM or transformer-based models for sequence forecasting
- Use external data like weather or events
- Hyperparameter tuning and model ensembling
- Compare with ARIMA/Prophet baselines

## License
This project is available under the MIT License (see `LICENSE`).

---

If you'd like a different repo name from `ride-sharing-demand-forecasting`, tell me and I'll rename files/instructions.
