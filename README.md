# Dengue-Fever-Prediction-Using-ML-and-XAI
Hematological Biomarker-Driven Dengue Fever Prediction: A Multi-Algorithm Approach with Explainable Artificial Intelligence

# Dengue Fever Prediction Using Machine Learning and Explainable AI

This project presents a machine learning–based framework for predicting dengue
fever using hematological laboratory data. Multiple machine learning models are
trained and evaluated, and Explainable AI (XAI) techniques are applied to ensure
model interpretability.

---

## 🎯 Project Objective

The objective of this project is to:
- Predict dengue fever using patient blood test parameters
- Compare multiple machine learning classifiers
- Handle class imbalance using SMOTE
- Provide explainability using SHAP and LIME

---

## 🗂️ Dataset Description

- Dataset: Dengue Fever Hematological Dataset
- Source: Kaggle
- Features include platelet count, WBC count, hemoglobin, hematocrit, MCV, MCH, and gender
- Target variable: Dengue test result (Positive / Negative)

---

## ⚙️ Data Preprocessing

- Duplicate removal
- Missing value imputation (mean strategy)
- Label encoding for categorical variables
- Feature scaling using StandardScaler
- Feature engineering using domain-specific ratios
- Class imbalance handling using SMOTE

---

## 🧠 Machine Learning Models Used

The following models were trained and tuned using GridSearchCV with 10-fold cross-validation:

- Logistic Regression
- Decision Tree
- Random Forest
- Support Vector Machine (SVM)
- K-Nearest Neighbors (KNN)
- Neural Network (MLP)
- XGBoost (Best performing model)

---

## 🔁 Cross Validation

- **10-Fold Cross Validation** was applied during hyperparameter tuning
- Ensures robustness and generalization of model performance

---

## 📊 Evaluation Metrics

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix
- ROC Curve and AUC score

---

## 🔍 Explainable AI (XAI)

To interpret model predictions, the following XAI techniques were used:

- **SHAP (SHapley Additive exPlanations)**  
  - Global feature importance
  - Local explanation using force plots

- **LIME (Local Interpretable Model-agnostic Explanations)**  
  - Instance-level explanation for individual predictions

These methods help understand how hematological features influence dengue prediction.

---

## 🚀 How to Run

```bash
pip install -r requirements.txt
jupyter notebook

