# 🏠 Loan Approval Prediction

## 📌 Overview
This project aims to automate loan eligibility decisions for a finance company using machine learning. The dataset includes applicant details such as income, education, credit history, and employment status. The goal is to predict whether a home loan application will be approved, and to identify the most reliable model for doing so.

---

## 🎯 Objective
- Build and compare machine learning models for binary classification.
- Tune hyperparameters to improve model performance.
- Evaluate using robust metrics (AUC-ROC, precision, recall, F1).
- Present insights and model performance in a business-relevant way.

---

## 🛠 Tools & Technologies
- Python, Jupyter Notebook
- scikit-learn, pandas, matplotlib
- Pipelines, GridSearchCV, cross-validation
- Random Forest, Logistic Regression, AdaBoost, Bagging

---

## 📊 Model Performance

| Model                        | AUC-ROC (Train) | AUC-ROC (Test) | F1 Score (Train) | F1 Score (Test) |
|-----------------------------|-----------------|----------------|------------------|-----------------|
| RandomForest (tuned)        | 0.76            | 0.79           | 0.88             | 0.88            |
| **Logistic Regression**     | 0.73            | **0.82**       | 0.87             | **0.88**        |
| AdaBoost                    | 0.75            | 0.73           | 0.83             | 0.81            |
| Bagging                     | 0.76            | 0.75           | 0.87             | 0.88            |

🔍 **Conclusion**: The simplest model — Logistic Regression — outperformed more complex models on test data, achieving the highest AUC and F1 score.

---

## 🧠 Problem-Solving Process

1. Defined the business goal: automate loan approval screening.
2. Explored and cleaned the data using EDA and histograms: found the data is balanced.
3. Preprocessed features using scikit-learn Pipelines (imputation, scaling, encoding).
4. Trained multiple models and used cross-validation for comparison.
5. Tuned Random Forest using GridSearchCV.
6. Evaluated models on a separate test set to assess generalization.

---

## 🧑‍💼 Explanation for audience

This project predicts whether a home loan will be approved using historical customer data. I tested several models and found that **Logistic Regression**, a simple and explainable algorithm, performed the best. It achieved 98% recall, meaning it successfully identified nearly all eligible applicants, minimizing the risk of mistakenly rejecting someone who qualifies.

