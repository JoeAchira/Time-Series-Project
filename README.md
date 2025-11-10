# Time-Series-Project
Forecasting Book Sales Using Statistical, Machine Learning, and Hybrid Models

# Book Sales Forecasting

### Project Overview
This project focuses on forecasting weekly book sales for two titles — *The Very Hungry Caterpillar* and *The Alchemist*.  
The goal was to combine traditional statistical and deep learning methods into a **hybrid forecasting model** to capture both linear trends and non-linear patterns in time series data.

This project was completed as part of my **Cambridge Data Science course** and demonstrates advanced time series analysis, model optimisation, and hybrid modelling design.

---

### Objectives
- Forecast weekly book sales for two popular titles using multiple models.
- Compare ARIMA, XGBoost, and LSTM performance.
- Develop and evaluate a **hybrid SARIMA–LSTM** ensemble model.
- Assess forecasting accuracy using MAE, RMSE, and MAPE metrics.

---

### Methods & Tools
- **Languages:** Python  
- **Libraries:** pandas, NumPy, matplotlib, statsmodels, TensorFlow/Keras, scikit-learn  
- **Techniques:**
  - Time series decomposition and stationarity testing
  - SARIMA model for linear trend and seasonality
  - LSTM model for non-linear pattern learning
  - Hybrid ensemble via weighted averaging
  - Hyperparameter tuning with Keras Tuner
  - Rolling forecast and model evaluation

---

### Model Development Steps
1. **Data Preparation:**  
   Aggregated weekly sales data from Nielsen BookScan, handled missing values, and split into train/test sets.
2. **Exploratory Analysis:**  
   Identified seasonality, trends, and outliers in sales patterns for each book.
3. **SARIMA Modeling:**  
   Used ACF/PACF plots and AIC optimisation to determine parameters.
4. **LSTM Modeling:**  
   Scaled data, reshaped for sequential input, and tuned hyperparameters with Keras Tuner.
5. **Hybrid Model:**  
   Combined SARIMA and LSTM predictions using weighted averaging to improve forecast accuracy.
6. **Evaluation:**  
   Compared results across all models and visualised forecast performance.

---

### Results
| Model | MAE | RMSE | MAPE |
|--------|-----|------|------|
| SARIMA | 112.5 | 145.3 | 8.9% |
| LSTM | 98.1 | 129.4 | 7.6% |
| **Hybrid SARIMA–LSTM** | **85.6** | **114.2** | **6.2%** |

**Best performance:** Hybrid SARIMA–LSTM achieved the lowest forecast error across both book titles.

---

### Learning Outcomes
- Applied hybrid modeling to combine statistical and neural network approaches.
- Improved understanding of time series preprocessing and rolling forecasts.
- Strengthened hyperparameter tuning and model evaluation skills.

---

### Next Steps
- Incorporate exogenous variables such as promotions or holidays.
- Deploy the forecasting dashboard with interactive visualisation (Plotly or Streamlit).

---

### Acknowledgment
Completed as part of the **University of Cambridge Data Science Certificate** program.

---

### References
- [Statsmodels SARIMA Guide](https://www.statsmodels.org/stable/examples/notebooks/generated/statespace_sarimax_stata.html)
- [Keras Time Series Forecasting](https://keras.io/examples/timeseries/timeseries_forecasting/)
