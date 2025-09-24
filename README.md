# ENS Data Challenge 2025 – AssurPrime

This repository contains my solution to the **ENS Data Challenge 2025 (AssurPrime)**.  
The goal of the challenge was to **predict insurance premiums** using anonymized client and contract data.

## Project Overview
- Ranked **8th in the global leaderboard**.
- Implemented end-to-end workflow in Python (data cleaning, feature engineering, model training, evaluation).
- Final models: **XGBoost + HistGradientBoosting with Optuna hyperparameter tuning and SHAP feature analysis**.

## Repository Structure

```
AssurPrime-DataChallenge/
│
├── notebooks/ # Jupyter notebooks
│ ├── 01_data_exploration.ipynb
│ ├── 02_feature_engineering.ipynb
│ ├── 03_modeling_optuna_xgb.ipynb
│ └── 04_results_visualization.ipynb
│
├── src/ # Reusable Python scripts
│ ├── preprocessing.py
│ ├── modeling.py
│ └── evaluation.py
│
├── results/ # Figures and outputs
│ ├── shap_summary.png
│ ├── feature_importance.png
│ └── performance_table.csv
│
└── requirements.txt # Python dependencies
```


## ⚙️ Methods
- **Data preprocessing:** handled missing values, categorical encoding, log transformations.  
- **Feature selection:** SHAP values and domain heuristics.  
- **Modeling:** XGBoost, HistGradientBoostingRegressor, stacking ensemble.  
- **Optimization:** Optuna for Bayesian hyperparameter search.  

## 📊 Results
- Ranked **8th overall** in the official leaderboard.  
- Achieved a significant RMSE improvement compared to baseline linear regression.  
- SHAP visualizations highlight the most predictive features.  

## 🔧 Installation
To run the project locally:

```bash
git clone https://github.com/JB-i/AssurPrime-DataChallenge.git
cd AssurPrime-DataChallenge
pip install -r requirements.txt
