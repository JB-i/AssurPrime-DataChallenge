# ENS Data Challenge 2025 – AssurPrime

This repository contains my solution to the **ENS Data Challenge 2025 (AssurPrime)**.  
The goal of the challenge was to **predict insurance premiums** using anonymized client and contract data.

## Project Overview
- Ranked **8th in the global leaderboard**.
- Implemented end-to-end workflow in Python (data cleaning, feature engineering, model training, evaluation).
- Final models: **XGBoost + HistGradientBoosting with Optuna hyperparameter tuning and SHAP feature analysis**.

## Repository Structure



## How to run
1. Place the **3 challenge CSVs** in `data/raw/`:
   - `train_input_Z61KlZo.csv`
   - `train_output_DzPxaPY.csv`
   - `test_input_5qJzHrr.csv`
2. Install deps:
   ```bash
   pip install -r requirements.txt
cd AssurPrime-DataChallenge
pip install -r requirements.txt

3. Open the notebook: AssurPrime_End2End.ipynb

Raw data is not included in the repository and can be found in the challenge website :
https://challengedata.ens.fr/participants/challenges/161/
