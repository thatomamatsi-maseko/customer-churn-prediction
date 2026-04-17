# Customer Churn Prediction

## 📌 Executive Summary
This project predicts customer churn for a bank and identifies the key factors driving attrition. Customer churn is a critical issue, as losing customers directly impacts revenue and growth.  

Using machine learning models such as **Logistic Regression, Random Forest, and XGBoost**, we achieved a maximum accuracy of approximately **83%**, with XGBoost performing the best overall.  

Key findings indicate that **customer activity status, tenure, and balance** are the strongest predictors of churn. In particular, inactive customers and those with shorter tenure are significantly more likely to leave.  

These insights can help the bank design targeted retention strategies, such as improving customer engagement and focusing on high-risk segments.


## 📊 Problem Statement
Customer churn refers to customers leaving a service provider. For banks, high churn rates can lead to significant financial losses.  

**Objectives:**
- Predict whether a customer will churn  
- Identify the most important factors influencing churn  
- Provide actionable insights to reduce customer loss  


## 📂 Dataset
The dataset contains **10,000 anonymized bank customer records**, including demographic, account, and activity details.  

- Overall churn rate: **20.38%**  
- Features include: Age, Balance, Tenure, Activity Status, Credit Score, etc.  
- Target variable: `Exited` (1 = churned, 0 = stayed)  


## 🔎 Exploratory Data Analysis (EDA)
- **Age Distribution:** Younger customers show higher churn tendency.  
- **Balance:** Customers with higher balances appear more likely to churn.  
- **Geography & Gender:** French customers churn less; females churn more.  
- **Activity Status:** Inactive members are more likely to leave.  
- **Correlation Heatmap:** Identified strong correlations; removed `Complain` to avoid data leakage.  


## ⚙️ Modeling
Models tested:
- Logistic Regression  
- Random Forest  
- XGBoost  

**Evaluation Metrics:**
- Confusion Matrix  
- Precision, Recall, F1-score  
- ROC-AUC  
- 5-fold Cross-Validation  

**Results:**
- Logistic Regression: ~80% mean accuracy  
- Random Forest: ~83% mean accuracy  
- XGBoost: ~82% mean accuracy  
- ROC-AUC (Logistic Regression): 0.81  


## 📈 Key Drivers of Churn
- **Tenure:** Short-tenure customers are more likely to churn.  
- **Activity Status:** Inactive members show higher churn risk.  
- **Balance:** High balances linked to churn, suggesting dissatisfaction among valuable clients.  
- **Age:** Younger customers churn more frequently.  

---

## 💡 Business Insights
- Focus retention efforts on **new and inactive customers**.  
- Develop **loyalty programs** for high-value clients.  
- Investigate dissatisfaction among customers with high balances.  
- Tailor retention strategies by geography and demographics.  


## 🚀 Future Work
- Apply hyperparameter tuning to improve performance.  
- Address class imbalance using techniques such as SMOTE.  
- Deploy the model in a real-time prediction system.  

---

## 🛠️ Tech Stack
- Python (pandas, numpy, scikit-learn, seaborn, matplotlib, xgboost)  
- Jupyter Notebook  

---

## 📌 How to Run
1. Clone the repository:
   git clone https://github.com/thatomamatsi-maseko/customer-churn-prediction.git
