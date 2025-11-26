# ⚡ Electricity Price Forecasting – Statistical & Machine Learning Models

[![DOI](https://img.shields.io/badge/DOI-10.1016%2Fj.cam.2025.117211-blue)](https://doi.org/10.1016/j.cam.2025.117211)

This repository contains the official code and comprehensive framework for **electricity spot price forecasting** associated with the research paper published in the *Journal of Computational and Applied Mathematics*.

The project combines statistical analysis, feature engineering, and predictive modeling using machine learning techniques. The dataset is based on multiple price hubs including *Indiana*, *Mid C*, *SP15 EZ Gen DA LMP Peak*, and *Palo Verde Peak*.

## 📄 Associated Publication

This code supports the findings presented in:

> **"A novel framework for pricing electricity derivatives: Integrating stochastic models and machine learning"**
> *Panumart Sawangtong, Rahman Taleghani, Mehran Taghipour*
> **Journal of Computational and Applied Mathematics**, Vol 477, 117211 (15 May 2026)
> [**Read the Full Paper via DOI**](https://doi.org/10.1016/j.cam.2025.117211)

---

## 🔍 Repository Contents

| File | Description |
|---|---|
| `All_methods_withoutjump.ipynb` | Main notebook implementing all prediction models (Random Forest, Deep Neural Network, LSTM) on cleaned data without jump events. |
| `jumps.ipynb` | Jump detection and exclusion notebook to filter out high-volatility days for robustness evaluation. |
| `Statistics.ipynb` | Final notebook for computing descriptive statistics (mean, std, skewness, kurtosis, etc.) and generating distribution plots per hub. |
| `Indiana.xlsx` | Subset of the dataset focusing on the Indiana hub, used for testing and comparison. |
| `allinone_adjusted_final.xlsx` | Master dataset used across all notebooks, containing preprocessed hub price data. |
| `deep_nn_sensitivity_results.xlsx` | Complete results of manual hyperparameter tuning for Dense Neural Network models. |
| `lstm_all_results.xlsx` | Results from extensive hyperparameter tuning for LSTM models. |
| `rf_sensitivity_results.csv` | Output of sensitivity analysis for the Random Forest model, including MSE/RMSE across configurations. |

## 📌 Features

- **Time-based feature engineering:** Creation of lagged features and rolling averages.
- **Manual hyperparameter tuning:** Detailed tuning of Random Forest, Deep Neural Networks, and LSTM architectures.
- **Statistical analysis:** Computation and visualization of price distribution statistics for each electricity hub.
- **Model evaluation:** Performance assessment using Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and Mean Absolute Error (MAE).
- **Visualization:** Comprehensive visualizations of data distributions, error metrics, and hyperparameter sensitivity.

---

## 📝 Citation

If you use this code or dataset in your research, please cite the paper using the following BibTeX entry:

```bibtex
@article{Sawangtong2026,
  title={A novel framework for pricing electricity derivatives: Integrating stochastic models and machine learning},
  author={Sawangtong, Panumart and Taleghani, Rahman and Taghipour, Mehran},
  journal={Journal of Computational and Applied Mathematics},
  volume={477},
  pages={117211},
  year={2026},
  publisher={Elsevier},
  doi={10.1016/j.cam.2025.117211}
}
