
# ⚡ Electricity Price Forecasting – Statistical & Machine Learning Models

This repository contains a comprehensive framework for **electricity spot price forecasting**, combining statistical analysis, feature engineering, and predictive modeling using machine learning techniques. The dataset is based on multiple price hubs including *Indiana*, *Mid C*, *SP15 EZ Gen DA LMP Peak*, and *Palo Verde Peak*.

## 🔍 Repository Contents

| File                             | Description |
|----------------------------------|-------------|
| `All_methods_withoutjump.ipynb`  | Main notebook implementing all prediction models (Random Forest, Dense Neural Network, LSTM) on cleaned data without jump events. |
| `jumps.ipynb`                    | Jump detection and exclusion notebook to filter out high-volatility days for robustness evaluation. |
| `Statistics.ipynb`               | Final notebook for computing descriptive statistics (mean, std, skewness, kurtosis, etc.) and generating distribution plots per hub. |
| `Indiana.xlsx`                   | Subset of the dataset focusing on the Indiana hub, used for testing and comparison. |
| `allinone_adjusted_final.xlsx`   | Master dataset used across all notebooks, containing preprocessed hub price data. |
| `deep_nn_sensitivity_results.xlsx`| Complete results of manual hyperparameter tuning for Dense Neural Network models. |
| `lstm_all_results.xlsx`          | Results from extensive hyperparameter tuning for LSTM models. |
| `rf_sensitivity_results.csv`     | Output of sensitivity analysis for the Random Forest model, including MSE/RMSE across configurations. |

## 📌 Features

- **Time-based feature engineering:** Creation of lagged features and rolling averages.
- **Manual hyperparameter tuning:** Detailed tuning of Random Forest, Dense Neural Networks, and LSTM architectures.
- **Statistical analysis:** Computation and visualization of price distribution statistics for each electricity hub.
- **Model evaluation:** Performance assessment using Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and Mean Absolute Error (MAE).
- **Visualization:** Comprehensive visualizations of data distributions, error metrics, and hyperparameter sensitivity.

---
