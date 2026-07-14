# Prompt 1: Forecast 8 Weeks Forward (with Backtest)

> **Instructor note:** One prompt, three models (ARIMA, SARIMA, Prophet) with exogenous drivers, an 8-week backtest, winner per series, forward forecast using the Future Calendar. Notebook stays in the folder for instructor reference.

## Paste this into Codex (venv active)

```
Context: I have a workbook in the dataset/ folder with weekly sales history and a Future Calendar of known future drivers (price, discount, marketing, holidays). I want an 8-week forward forecast per store/category. Before I trust it, I want a backtest so I know which model to use.

Instruction: For each store/category series, train ARIMA, SARIMA, and Prophet using the available driver columns as exogenous regressors. Hold out the last 8 weeks of history as a test set, score each model with MAPE and RMSE, pick the winner per series. Refit the winner on full history and forecast 8 weeks forward using the Future Calendar drivers. Write everything back to the workbook in dataset/.

Input:
- Workbook in dataset/ with sheets: History, Future Calendar, Data Dictionary
- Target: units_sold
- Exogenous drivers: every numeric column except the target (price, discount_pct, marketing_spend, competitor_price_idx, avg_temp_c, is_holiday, stockout)
- Backtest window: 8 weeks
- Forecast horizon: 8 weeks

Output: new sheets inside the workbook
- Backtest Results: per series, MAPE and RMSE for ARIMA / SARIMA / Prophet plus the winner
- Forecast: 8-week forward forecast per series using the winning model
- Forecast vs Actuals: embedded image, 15-panel grid showing each model vs actuals on the held-out window
- Forward Forecast: embedded image, 15-panel grid showing history plus forward forecast

Chart style: lines must be continuous across the train/test boundary. Do not leave a visual gap between history and predictions. Anchor each model's prediction line at the last training point so it connects to history. Same for the forward forecast — anchor it at the last actual point so it continues smoothly from the blue history line. Mark the held-out actuals with black dots so the test region is still obvious.

Keep modeling code in a notebook in this folder. The student-facing artifact is the updated workbook.
```

> **Instructor note:** Open Backtest Results — Prophet usually wins where drivers matter (Essentials, Snacks, Seasonal). ARIMA wins on stable series with weak driver effects. SARIMA picks up weekly seasonality. Average MAPE lands ~14% — realistic for weekly retail. Then open Forecast vs Actuals to show how each model performed on data it had not seen. Forward Forecast is the deliverable.
