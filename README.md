# ENS Data Challenge 2025 – AssurPrime
This repository contains my solution to the **ENS Data Challenge 2025 (AssurPrime)**.  
The goal of the challenge was to **predict insurance premiums** using anonymized client and contract data.

## Project Overview
- Ranked: 8th place on the global leaderboard.
- Objective: Predict insurance charge (CHARGE) = FREQ × CM × ANNEE_ASSURANCE.
- Approach:
   - Data cleaning & categorical encoding.
   - SHAP-based feature selection.
   - Hybrid models: XGBoost (for FREQ) + HistGradientBoosting (for CM).
   - Hyperparameter tuning with Optuna.
   - Custom formula recombination for charge prediction

## Repository Tree
AssurPrime-DataChallenge/
│── data/ # Datasets (not versioned)
│ ├── raw/ # Challenge CSVs (to be downloaded separately)
│ └── processed/ # Encoded & split datasets (generated locally)
│
│── results/ # Outputs (figures, submissions)
│
│── AssurPrime_End2End.ipynb # Main notebook (end-to-end workflow)
│── requirements.txt # Python dependencies
│── README.md # Project documentation
│── .gitignore

## How to run
1. Place the **3 challenge CSVs** in `data/raw/`:
   - `train_input_Z61KlZo.csv`
   - `train_output_DzPxaPY.csv`
   - `test_input_5qJzHrr.csv
   from the official ENS Challenge website: https://challengedata.ens.fr/participants/challenges/161/

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
   
3. Open the notebook: AssurPrime_End2End.ipynb to reproduce preprocessing, training, tuning, and submission generation.
