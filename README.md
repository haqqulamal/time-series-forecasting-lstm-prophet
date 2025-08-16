# Time-Series Forecasting — LSTM & Prophet

This repository provides a clean **univariate** forecasting baseline with:
- **windowing** (look_back → horizon),
- **LSTM** (Keras/TensorFlow),
- **Prophet** baseline,
- evaluation using **RMSE / MAE / MAPE / R²** and diagnostic plots.

Notebook: `notebooks/time_series_forecasting_model.ipynb`.

## Pipeline
1. **Prepare:** optional resampling, missing handling, scaling; **time-aware split** (no shuffle).
2. **Windowing:** convert series into supervised samples (`look_back`, `horizon`, `stride`).
3. **Modeling:**
   - **LSTM** with dropout and early stopping (optional).
   - **Prophet** as a quick baseline for trend/seasonality.
4. **Evaluation:** report **RMSE/MAE/MAPE/R²**, plot ŷ vs y & residuals; sav
