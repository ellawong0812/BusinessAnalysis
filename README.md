# Customer Churn Prediction

## 🎯 Business Problem

Predicting customer churn is critical for businesses — retaining existing customers is more cost-effective than acquiring new ones. By identifying customers at risk of leaving, companies can take proactive steps to improve retention, maintain revenue, and make informed decisions around forecasting, resource planning, and expansion.

We frame this as a **supervised classification problem**: predicting whether a customer will `Exited` (1) or `Not Exited` (0).

## 🛠️ Approach

We explore multiple models, starting with:
- Logistic Regression
- Decision Trees  
Additional models (e.g., Random Forest, XGBoost) may be tested for improved performance.

## 📊 Dataset

**Source**: [Kaggle - Bank Customer Churn Prediction](https://www.kaggle.com/datasets)  
**Size**: 10,000 customer records  
**Features**: 12 attributes (e.g., CreditScore, Geography, Gender, Tenure, Balance, etc.)  
**Target**: `Exited` (1 = churned, 0 = retained)

### Train-Test Split
- **70% Training**: 7,001 samples  
- **30% Testing**: 2,999 samples  
Preprocessing is applied consistently — only fitted on training data to prevent leakage.

## 🔍 Data Understanding

Initial exploration included:
- `.head()` – Preview data structure
- `.info()` – Check data types and missing values
- `.describe()` – Summarize numerical distributions

No significant missing data was found. Categorical variables (e.g., Geography, Gender) will be encoded; numerical features will be scaled as needed.

---

Next steps: feature engineering, modeling, and evaluation.

You can find the full Report in "ISOM 3360 Report (combined).pdf"
