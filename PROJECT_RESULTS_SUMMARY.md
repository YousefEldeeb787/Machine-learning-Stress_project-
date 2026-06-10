# Project Summary and Results

## Project Goal
Build a machine learning pipeline to classify student stress levels from questionnaire responses (PSS-10) and demographic features.

## What We Already Did

1. **Data loading and inspection**
   - Loaded `Stress.csv`.
   - Checked shape, data types, and missing values.

2. **Data cleaning and preprocessing**
   - Renamed columns for clarity.
   - Removed `Stress_Value` to avoid target leakage/redundancy.
   - Encoded categorical features (label encoding + one-hot encoding where needed).
   - Prepared numeric feature matrix for modeling.

3. **Train/test preparation**
   - Encoded target labels.
   - Used stratified train/test split.
   - Applied `StandardScaler` for scale-sensitive models.

4. **Feature analysis and selection**
   - Performed correlation review.
   - Computed feature relevance using multiple methods:
     - Chi-square
     - Mutual information
     - ANOVA F-test
     - Tree-based importance
   - Compared **full-feature** vs **reduced-feature** modeling.

5. **Model training**
   - Trained and evaluated five classifiers:
     - Random Forest
     - XGBoost
     - Logistic Regression
     - SVM
     - KNN

6. **Evaluation and validation**
   - Reported Train Accuracy, Test Accuracy, Precision, Recall, F1-score.
   - Generated confusion matrices.
   - Checked overfitting using train–test gap.

## Results Found

- Tree-based models (especially **XGBoost** and **Random Forest**) gave the strongest overall performance.
- The reduced-feature pipeline remained close to full-feature performance in many comparisons, supporting a simpler deployable setup.
- Train–test gaps were generally small, indicating acceptable to good generalization.
- The final recommendation is based on the best weighted F1-score with stable test performance.

## Project Files

- `Stress_Preprocessing_Modeling.ipynb` — full implementation
- `Stress.csv` — dataset
- `VISUAL_SUMMARY.md` — visual comparison and overfitting summary
- `Machine_REPORT.md` — detailed technical documentation
- `README.md` — repository overview

## Conclusion
The project produced a complete and reproducible stress-classification workflow, from preprocessing to model comparison, with clear results and deployment-ready documentation.
