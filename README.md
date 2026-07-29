# Explainable Machine Learning for Heart Disease Prediction

## Overview

This repository contains the implementation developed for my Bachelor's thesis:

**Explainable Machine Learning for Heart Disease Prediction: A Comparative Analysis of Logistic Regression, Random Forest, and XGBoost**

The project investigates explainable machine learning for binary heart disease prediction using the processed Cleveland Heart Disease dataset. Three supervised machine learning algorithms—Logistic Regression, Random Forest, and XGBoost—were developed and evaluated within a consistent experimental workflow. Model behaviour was interpreted using SHAP (SHapley Additive exPlanations) through both global and local explainability analyses.

The implementation was developed and executed using **Google Colab**.

---

## Repository Structure

```text
.
├── Heart_Disease_XAI_Thesis.ipynb
├── processed.cleveland.data
├── heart.dat
├── requirements.txt
└── README.md
```

---

## Datasets

This project uses two publicly available datasets obtained from the UCI Machine Learning Repository.

### Primary Dataset

- **Dataset:** Heart Disease Dataset (Processed Cleveland subset)
- **File:** `processed.cleveland.data`
- **Observations after preprocessing:** 297
- **DOI:** https://doi.org/10.24432/C52P4X

### Supplementary Evaluation Dataset

- **Dataset:** Statlog (Heart)
- **File:** `heart.dat`
- **Observations:** 270
- **DOI:** https://doi.org/10.24432/C57303

During the implementation, a record-level comparison showed that all Statlog observations were also present in the processed Cleveland dataset used in this study. Consequently, the Statlog analysis is reported as a **supplementary evaluation** rather than an independent external validation. This methodological decision is explained in both the notebook and the accompanying thesis.

---

## Experimental Workflow

The notebook follows the complete workflow presented in the thesis:

1. Dataset loading and inspection
2. Data preprocessing
3. Exploratory Data Analysis (EDA)
4. Data preparation
5. Model development
   - Logistic Regression
   - Random Forest
   - XGBoost
6. Comparative model evaluation
7. SHAP explainability
   - Global feature importance
   - Cross-model comparison
   - Local explanation (XGBoost)
8. Supplementary evaluation using the Statlog Heart Disease dataset

---

## Evaluation Metrics

The models were evaluated using multiple complementary performance measures:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Confusion Matrix
- ROC Curves

---

## Explainability

Model interpretability was investigated using **SHAP (SHapley Additive exPlanations)**.

The notebook includes:

- Global SHAP analysis for Logistic Regression
- Global SHAP analysis for Random Forest
- Global SHAP analysis for XGBoost
- Cross-model comparison of feature contribution patterns
- Local SHAP explanation for the selected XGBoost model

---

## Main Python Libraries

- Python
- pandas
- numpy
- matplotlib
- scikit-learn
- xgboost
- shap

---

## Reproducibility

The implementation follows a reproducible workflow using:

- Consistent data preprocessing
- Stratified train-test split
- Fixed random state (`42`)
- Standardised evaluation metrics
- SHAP-based explainability
- Fully documented analysis workflow

---

## Thesis

This repository accompanies the Bachelor's thesis submitted as part of the **B.Sc. Applied Artificial Intelligence** programme at **IU International University of Applied Sciences**.

**Author:** Negin Hezarjaribi

---

## License

This repository is provided for academic and educational purposes.