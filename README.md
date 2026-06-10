# Stress Prediction Pipeline

This repository contains an end-to-end machine learning workflow for student stress classification using questionnaire and demographic data.

## Repository Contents

- `Stress_Preprocessing_Modeling.ipynb` — full preprocessing, feature engineering, model training, evaluation, and comparison notebook.
- `Stress.csv` — source dataset used by the notebook.
- `Machine_REPORT.md` — detailed technical report of the complete pipeline and modeling decisions.
- `VISUAL_SUMMARY.md` — concise visual summary of results and model comparison updates.

## What This Project Covers

- Data cleaning and preprocessing
- Encoding strategy for mixed feature types
- Feature scaling for scale-sensitive models
- Feature selection using multiple statistical/model-based methods
- Training and evaluation of multiple classifiers (Random Forest, XGBoost, Logistic Regression, SVM, KNN)
- Train/test performance comparison and overfitting analysis

## Main Outcome

The notebook compares full-feature and reduced-feature pipelines and recommends the best-performing model based on weighted F1-score and generalization behavior.
