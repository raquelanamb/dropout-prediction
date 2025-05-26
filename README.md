# dropout-prediction
# Leveraging ML to Predict Dropout Likelihood in Higher Education

Authors: Raquel Ana M Bush and Brian Kade Betterton

This project leverages machine learning to predict the likelihood of student dropout in higher education. Using a real-world dataset from a Portuguese university, we built and evaluated models to help institutions identify at-risk students early and intervene proactively.

## Project Summary

- **Dataset**: 4,424 student records, 36 features  
- **Models**: XGBoost, Random Forest, Logistic Regression, Decision Tree  
- **Goal**: Maximize sensitivity (recall) to identify students at risk of dropping out  
- **Output**: Performance metrics, confusion matrices, AUC-ROC curves, and feature importance analysis

## Key Results

- **Most predictive features**:
  - First and second semester grades
  - Tuition payment status
  - Age at enrollment
- **Best model for sensitivity**: Logistic Regression (89% recall after threshold adjustment)
- **Best balanced models**: XGBoost and Random Forest (high accuracy and specificity)

## Methodology

### Data Preprocessing
- Converted multi-class target into binary: `Dropout (1)` vs. `Enrolled/Graduated (0)`
- Encoded categorical variables (label + one-hot encoding)
- Scaled numerical features (grades, age)
- 80/20 train-test split

### Modeling & Evaluation
- Trained four supervised models
- Used random search hyperparameter tuning
- Evaluated using:
  - Accuracy
  - Sensitivity (Recall)
  - Specificity
  - Precision
  - AUC-ROC curves
  - Confusion matrices

## Files Included Here

- `RaquelAna_Bush_ProjectCode.ipynb` — full code and visualizations
- `DropoutPrediction_ProjectReport.pdf` — formal write-up with figures and detailed analysis


> This project demonstrates the potential of AI to support equity and success in education by enabling data-informed student support systems.
