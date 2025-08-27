# 🏦 Banking Customer Churn 

This project analyzes customer data to predict **churn** (customers leaving the bank) and provides actionable insights for retention strategies.

---

## 📌 Project Overview
Customer churn is a critical challenge for banks. Retaining customers is more cost-effective than acquiring new ones.  
This project explores **EDA, customer segmentation, and predictive modeling** to understand churn behavior and identify at-risk customers.

---

## 🎯 Objectives
- Perform **Exploratory Data Analysis (EDA)** to uncover churn patterns.  
- Apply **K-Means clustering** for customer segmentation.  
- Build predictive models to classify customers likely to churn.  
- Recommend **strategies to reduce churn** based on insights.

---

## 📊 Dataset
- **Source:** Kaggle – [Bank Customer Churn Prediction Dataset](https://www.kaggle.com/)  
- **Size:** 10,000 rows × 14 columns  
- **Target Variable:** `Exited` (1 = churned, 0 = retained)  

**Key Features**  
- Demographics: `Age`, `Gender`, `Geography`, `Tenure`  
- Financial: `CreditScore`, `Balance`, `EstimatedSalary`  
- Engagement: `NumOfProducts`, `HasCrCard`, `IsActiveMember`

---

## 🔍 Exploratory Data Analysis (EDA)
- Churn rate ~20%.  
- **Age:** Older customers more likely to churn.  
- **Geography:** Germany has the highest churn.  
- **Gender:** Female customers churn at higher rates.  
- **Engagement:** Inactive members have higher churn risk.  
- **Products:** Customers with 2 products are least likely to churn.  

---

## 👥 Customer Segmentation (K-Means)
- Optimal clusters: **5**.  
- **Cluster 4**: Older, high-balance customers → **highest churn (~44%)**.  
- **Cluster 1**: Loyal, long-tenure customers → **lowest churn (~12%)**.  

---

## 🤖 Machine Learning Models
**Best Model: Random Forest**  
- Accuracy: **82%**  
- Recall: **66%** (focus on capturing churners)  
- AUC: **0.84**  

📌 Recall prioritized to maximize identification of at-risk customers.

---

## 📈 Key Insights
- **Age** is the strongest churn driver.  
- **Inactive members** churn more frequently.  
- **Geographic differences** affect churn (Germany highest).  
- **More than 3 products** → higher churn risk.  

---

## 💡 Recommendations
- Create **retention programs for older customers** (e.g., retirement plans).  
- Re-engage **inactive customers** with targeted campaigns.  
- Launch **female-focused financial products** to address higher churn rates.  
- Improve **services in high-churn regions** (Germany).  

---

## 🛠️ Tech Stack
- **Python**  
- Libraries: pandas, numpy, matplotlib, seaborn, scikit-learn, imbalanced-learn, xgboost, lightgbm  
- **Jupyter Notebook** for analysis  
