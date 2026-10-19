# Formula 1 Podium Prediction Companion

**DMET904 |  — Milestone 1**

## Project Overview

This project develops a machine-learning pipeline to predict whether a Formula 1 driver will finish a race on the podium (positions 1–3).

Predictions are made after qualifying and before the race, using only information available at that time.

## Dataset

- Formula 1 World Championship (1950–2024)
- 26,668 driver-race observations after cleaning
- 9 selected pre-race predictors
- Binary classification: Podium (1) / Non-podium (0)

Dataset source: https://www.kaggle.com/datasets/rohanrao/formula-1-world-championship-1950-2020

## Machine Learning Models

Three classifiers were implemented:

1. Logistic Regression
2. Random Forest
3. Shallow Neural Network (MLP)

## Test Results

| Model | F1-score | ROC-AUC | PR-AUC |
|---|---:|---:|---:|
| Logistic Regression | 0.7009 | 0.9299 | 0.7050 |
| Random Forest | 0.6508 | 0.9258 | 0.6703 |
| MLP | 0.6818 | 0.9335 | 0.6922 |

Logistic Regression achieved the highest test F1-score and Average Precision.

## Project Components

- Data cleaning and relational integrity validation
- Exploratory data analysis
- Three Formula 1 data-engineering research questions
- Leakage-safe historical feature engineering
- Chronological train/validation/test splitting
- Model training and hyperparameter optimization
- Feature-group ablation
- Preprocessing-order experiments
- Permutation importance, SHAP, and LIME
- Inference with complete and partially missing records

## Running the Project

The implementation is provided in the Jupyter notebook `F1_Podium_Prediction.ipynb`.

The notebook was developed using Kaggle. To reproduce the analysis, open the notebook in Kaggle, attach the Formula 1 dataset, install any missing dependencies, and run the cells in order.

## Team Members

- Moustafa Mohamed | 58-11800
- Sara Ahmed Elsawy | 58-1857
- Farah Emad Eldin | 58-1980
- Aesha Anwar | 58-0464

## Course

DMET904 — Milestone 1
