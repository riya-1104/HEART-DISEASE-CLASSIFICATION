# Heart Disease Classification

A machine learning project to predict the presence of heart disease using patient health and clinical features.

## Project Overview

This project follows a complete machine learning workflow, including:

- Data exploration and visualization
- Data cleaning
- Train-test split
- Missing value handling
- Categorical encoding
- Feature scaling
- Feature selection
- Logistic Regression
- Model evaluation

## Dataset

The dataset contains patient health-related features such as:

- Age
- Sex
- Chest Pain Type
- Resting Blood Pressure
- Cholesterol
- Fasting Blood Sugar
- Resting ECG
- Maximum Heart Rate
- Exercise-Induced Angina
- Oldpeak
- ST Slope

**Target:** `HeartDisease`

- `0` → No heart disease
- `1` → Heart disease

## Feature Selection

The following feature selection techniques were explored:

- Correlation analysis for numerical features
- Chi-square test for categorical features
- Mutual Information for numerical features
- Recursive Feature Elimination (RFE)

RFE reduced the processed feature space from 20 features to 10 features. However, the model using all features achieved slightly better overall performance, so the full-feature model was selected as the final model.

## Model

**Logistic Regression**

The data was preprocessed using:

- Simple Imputation for missing values
- One-Hot Encoding for categorical variables
- Feature Scaling for numerical variables

## Results

### Final Model — Logistic Regression

| Metric | Score |
|---|---:|
| Accuracy | 89.13% |
| Precision | 89.42% |
| Recall | 91.18% |
| F1 Score | 90.29% |

### RFE Model

| Metric | Score |
|---|---:|
| Accuracy | 88.59% |
| Precision | 87.85% |
| Recall | 92.16% |
| F1 Score | 89.95% |

The RFE model achieved slightly higher recall, but the full-feature model achieved better accuracy, precision, and F1 score.

## Conclusion

The final Logistic Regression model achieved **89.13% accuracy** and an **F1 score of 90.29%**.

Feature selection was useful for understanding the importance of different features and evaluating whether reducing the feature space improved model performance. In this project, the full-feature model provided the best overall performance.

## Files

- `Heart-Disease-classification.ipynb` — Complete analysis and model development
- `heart.csv` — Dataset
