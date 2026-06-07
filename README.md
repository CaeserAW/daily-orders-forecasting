# Daily Orders Forecasting Using XGBoost

This notebook forecasts daily orders for the next 7 days using historical order data. The original dataset contains two columns: date and number of orders. Additional calendar, lag, rolling, trend, holiday, and cyclical features are engineered to improve forecasting performance.
## Tools and Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- XGBoost
- Scikit-learn
- holidays
- SHAP
## 5. Feature Engineering

Although the original dataset contains only the date and the number of orders, several predictive features were created from the historical time series. These features help the model capture weekly patterns, monthly effects, holidays, recent demand behavior, and short-term trends.

The engineered features include:

- Calendar features, such as day of week, week of year, month, year, and day of month.
- Weekend, Sunday, holiday, and end-of-month indicators.
- Cyclical date features using sine and cosine transformations.
- Lag features based on previous order values.
- Rolling statistics, such as rolling mean, standard deviation, minimum, and maximum.
- Trend and momentum features, such as differences between recent and older order values.
