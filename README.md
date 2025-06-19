WEATHER PREDICTION WITH AIML

DESCRIPTION:

This project involved building a machine learning model to predict the next day’s maximum temperature (tmax) using historical weather data spanning from 1970 to 2022. The dataset was cleaned, enriched with rolling averages, percentage changes, and seasonal patterns, and a Ridge Regression model was used for prediction. The model was evaluated using a custom backtesting strategy to simulate real-world forecasting.

🔍 Key Insights & Highlights
> Data Preprocessing & Feature Engineering:

* Removed high-missing-value columns and filled missing values using forward-fill.

* Engineered features: rolling averages (3 & 14 days), monthly & daily averages, and percent changes.

* Created target variable as the next day’s tmax.

> Modeling & Backtesting:

* Ridge Regression (alpha=0.1) used with 5 predictors (tmin, tmax, prcp, snow, snwd).

* Custom backtest trained the model incrementally and tested over 90-day periods to mimic time-series forecasting.

> Performance Metrics:

* Achieved a Mean Absolute Error (MAE) of 4.79°C and Mean Squared Error (MSE) of 37.6.

* Showed consistent predictions across decades of data, with error distribution largely centered around ±5°C.

> Feature Importance:

* tmin and tmax were strong positive predictors.

* prcp (precipitation) had a negative influence on next day’s temperature — aligning with weather patterns.
