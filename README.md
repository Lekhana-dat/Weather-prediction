# Seattle Weather Type Classification (XGBoost)
Predicts the day's weather label (drizzle, rain, sun, snow, fog) from same-day precipitation, max/min temperature and wind. This is classification, not forecasting.

| Model | Accuracy |
|---|---|
| Always predict the most common class | 44% |
| XGBoost (default) | 76% |
| XGBoost (grid search, 10-fold CV) | 81% |

**Limitation:** rare classes (drizzle, snow) are barely detected (drizzle recall 0%, snow 33%), so accuracy mostly reflects rain, sun and fog.
**Run:** open `Weather Prediction.ipynb` with `seattle-weather.csv` in the same folder (needs pandas, scikit-learn, xgboost).
