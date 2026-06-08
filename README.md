# Hackthon
# 💉 H1N1 Vaccination Prediction using Machine Learning

🚀 Data Science Hackathon Project

📊 Machine Learning | 🤖 Explainable AI | 🏆 Model Comparison

---

## 📖 Project Overview

This project was developed as part of a Data Science Hackathon with the objective of predicting whether an individual would receive the H1N1 vaccine based on demographic, behavioural, health-related and opinion-based survey data.

The project follows a complete machine learning workflow including Exploratory Data Analysis (EDA), data preprocessing, model development, performance evaluation and Explainable Artificial Intelligence (XAI) using SHAP.

---

## 🎯 Objectives

* Predict H1N1 vaccination status.
* Compare multiple machine learning models.
* Evaluate models using classification metrics.
* Interpret model predictions using Explainable AI techniques.
* Generate prediction files for hackathon submission.

---

## 📊 Dataset

The dataset contains information related to:

* Demographic characteristics
* Employment information
* Health conditions
* Vaccination opinions
* Behavioural factors
* Household information

### 🎯 Target Variable

`h1n1_vaccine`

* 0 → Not Vaccinated
* 1 → Vaccinated

---

## 🔍 Exploratory Data Analysis (EDA)

The following analyses were performed:

* Dataset overview and structure inspection
* Missing value analysis
* Target variable distribution analysis
* Correlation analysis
* Feature relationship exploration

### Key Findings

* Several features contained significant missing values.
* Vaccination classes showed some imbalance.
* Health and opinion-related features demonstrated stronger relationships with vaccination behaviour.
* Correlation analysis helped identify influential predictors.

---

## ⚙️ Data Preprocessing

A preprocessing pipeline was implemented to ensure consistent data preparation across all models.

### 🧹 Missing Value Handling

* Mode Imputation
* KNN Imputation

### 🔄 Feature Transformation

* One-Hot Encoding for categorical variables
* Standard Scaling for ordinal variables

### ✂️ Data Splitting

* Training Set: 80%
* Validation Set: 20%

### ✅ Benefits

* Reduced data quality issues
* Improved model reliability
* Prevented data leakage through pipeline implementation

---

## 🤖 Machine Learning Models

The following machine learning models were trained and evaluated:

1. Logistic Regression
2. Random Forest
3. XGBoost
4. Tuned XGBoost
5. Gradient Boosting

### 🎛️ Hyperparameter Tuning

RandomizedSearchCV was used to optimise XGBoost hyperparameters.

Configuration:

* 20 parameter combinations
* 5-Fold Cross Validation
* F1 Score optimisation metric

### Best Parameters

```python
{
    'subsample': 0.8,
    'n_estimators': 300,
    'max_depth': 5,
    'learning_rate': 0.03,
    'colsample_bytree': 0.7
}
```

---

## 📈 Model Performance

| Model               | Accuracy | Precision | Recall | F1 Score |
| ------------------- | -------- | --------- | ------ | -------- |
| Logistic Regression | 0.759    | 0.727     | 0.624  | 0.671    |
| Random Forest       | 0.756    | 0.741     | 0.587  | 0.655    |
| XGBoost             | 0.758    | 0.713     | 0.648  | 0.679    |
| Tuned XGBoost       | 0.755    | 0.713     | 0.635  | 0.671    |
| Gradient Boosting   | 0.767    | 0.727     | 0.653  | 0.688    |

### 🏆 Best Performing Model

**Gradient Boosting**

✅ Accuracy: 76.7%

✅ F1 Score: 0.688

✅ Best balance between Precision and Recall

---

## 🧠 Explainable AI (XAI)

SHAP (SHapley Additive exPlanations) was used to improve model interpretability and understand the factors influencing predictions.

### Key Insights

* Doctor recommendation was one of the strongest predictors.
* Perceived vaccine effectiveness significantly influenced vaccination decisions.
* Perceived H1N1 risk strongly contributed to model predictions.
* Health-related and behavioural variables affected vaccination uptake.

### Why SHAP?

* Improves model transparency
* Explains feature contributions
* Increases trust in machine learning predictions
* Supports data-driven decision making

---

## 🔄 Project Workflow

1️⃣ Data Loading

2️⃣ Exploratory Data Analysis (EDA)

3️⃣ Missing Value Analysis

4️⃣ Train-Test Split

5️⃣ Data Preprocessing

6️⃣ Model Training

7️⃣ Model Evaluation

8️⃣ Model Comparison

9️⃣ Prediction Generation

🔟 Explainable AI Analysis

---

## 🛠️ Technologies Used

🐍 Python

🐼 Pandas

🔢 NumPy

📊 Matplotlib

📈 Seaborn

🤖 Scikit-Learn

⚡ XGBoost

🧠 SHAP

---

## 🚀 Future Improvements

* Explore advanced feature engineering techniques.
* Apply Bayesian optimisation and Optuna for hyperparameter tuning.
* Investigate ensemble stacking methods.
* Evaluate additional Explainable AI approaches.
* Improve handling of highly incomplete features using advanced imputation techniques.

---

## 👥 Team Contributions

This project was completed as part of a collaborative Data Science Hackathon.

Contributions included:

* Data exploration and preprocessing
* Model development and evaluation
* Hyperparameter tuning
* Prediction generation
* Explainable AI analysis
* Presentation preparation and project documentation

---

## 🎓 Conclusion
This project demonstrates how effective preprocessing, ensemble machine learning techniques and Explainable AI can be combined to develop accurate and interpretable models for predicting H1N1 vaccination behaviour.

Among all evaluated models, **Gradient Boosting achieved the strongest overall performance**, while SHAP analysis provided valuable insights into the key factors influencing vaccination decisions.

---
