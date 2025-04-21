# ConnectTel Customer Churn Prediction

## Overview
This project aims to build a machine learning model that predicts customer churn for **ConnectTel**, a telecommunications company. The prediction system will help the company identify at-risk customers and implement targeted retention strategies to reduce churn and improve customer loyalty.

---

## Dataset Overview
- **Rows:** 7,043 customers 
- **Columns:** 21 features 
- **Target Variable:** `Churn` (Yes/No)

---

## Project Steps

### 1. Problem Definition
Customer churn poses a serious challenge to ConnectTel’s sustainability and growth. The objective of this project is to:
- Predict churn with high accuracy
- Prioritize **recall** to avoid missing potential churners
- Help the business take **data-driven retention actions**

---

### 2. Exploratory Data Analysis (EDA)
EDA was conducted using Python libraries like `pandas`, `seaborn`, and `matplotlib`:
- **Univariate analysis** on features like `Gender`, `PhoneService`, `InternetService`
- **Bivariate analysis** to see how features affect churn (e.g., MultipleLines vs. churn)
- **Multivariate analysis** using correlation matrices, analyzed multiple variables at a go.
- Cleaned missing data and verified data types

---

### 3. Feature Engineering
- Encoded categorical variables using `LabelEncoder`
- Dropped non-informative columns like `CustomerID`
- Converted object-type numerical fields (e.g., `PhoneService`) to int

---

### 4. Model Training and Selection
Trained and evaluated the following models:
- Logistic Regression
- Random Forest Classifier
- Naive Bayes
- SGD Classifier
- XGBoost

Used `train_test_split()` with an 80/20 train-test ratio.

---

### 5. Model Evaluation

**Metrics Evaluated:**
- Accuracy
- Precision
- Recall
- ROC AUC Score
- Confusion Matrix and ROC Curves for visualization

**Best Model:** 
- **Naive Bayes** was selected for its **high recall and ROC AUC**, making it the best model to capture the most churners and help reduce customer loss.

---

### 6. Business Recommendations
- Use the model to flag at-risk customers for retention campaigns
- Prioritize models with **high recall** to reduce false negatives
- Consider integrating churn prediction into CRM workflows

---

## Challenges Faced
- Dealing with class imbalance and metric trade-offs
- Choosing the right model based on business needs (recall vs. accuracy)
- Encoding and transforming complex categorical data

---  
