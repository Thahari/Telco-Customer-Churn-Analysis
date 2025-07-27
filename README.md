# 📉 Customer Churn Prediction – Telco Dataset

This project predicts customer churn for a telecom company using Python (pandas, sklearn, SQL), Power BI, and various machine learning models. The goal is to identify customers likely to churn and understand the key drivers behind their behavior.

---

## 📊 Dataset

- **Source**: Telco Customer Churn dataset (CSV)
- **Size**: 7,043 rows, 21 columns
- **Target variable**: `Churn` (Yes/No)

---

## 🧠 Project Workflow

1. **Data Cleaning & Exploration**
   - Handled missing values, duplicates
   - Converted `TotalCharges` to numeric
   - Explored churn patterns with SQL and Python

2. **Feature Engineering**
   - Encoded categorical variables
   - Scaled numerical features
   - Addressed class imbalance with `class_weight` and hyperparameters

3. **Model Training & Evaluation**
   - Trained 7 models: Logistic Regression, Naive Bayes, Decision Tree, Random Forest, AdaBoost, XGBoost, MLP
   - Applied **hyperparameter tuning** using GridSearchCV / RandomizedSearchCV
   - Created a **Voting Ensemble**
   - Final model: **CatBoostClassifier**

4. **Performance Metrics (Class 1: Churn)**

| Model            | F1-Score |
|------------------|----------|
| ✅ **CatBoost**     | **0.615**  
| Voting Ensemble  | 0.610  
| Random Forest    | 0.605  
| XGBoost          | 0.603  
| Decision Tree    | 0.597  

5. **Dashboard & Business Insights**
   - Created interactive Power BI dashboard
   - Identified churn patterns by contract, tenure, charges
   - Estimated revenue loss by customer segment

---

## 🚀 Final Model: CatBoost

```python
CatBoostClassifier(learning_rate=0.05, iterations=200, depth=5, class_weights=[1,2])
