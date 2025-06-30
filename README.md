# 📊 Predicting Customer Attrition: Data-Driven Insights for Retention

This project focuses on predicting customer churn in the banking sector using machine learning. The objective is to empower organizations with a **data-driven framework** to proactively identify high-risk customers and improve retention strategies.

The solution was designed to prioritize both **model performance** and **interpretability**, ensuring it can deliver business value. The analysis highlights the **key behavioral drivers of churn** and delivers a **reliable, explainable model** ready for deployment.

---

## 🧠 Project Goals

- Detect customers likely to **churn (attrite)** from the bank  
- Understand **why customers leave** by identifying the most influential features  
- Build a predictive model that balances **accuracy, recall, and interpretability**  
- Equip business teams with insights to design **targeted retention campaigns**

---

## 🛠️ Key Steps Undertaken

### 🔹 Data Cleaning & Preprocessing

- Removed ID columns to avoid data leakage  
- Encoded categorical features using **One-Hot Encoding**  
- Addressed class imbalance using **SMOTE** to ensure fair learning for churn cases

### 🔹 Exploratory Data Analysis

- Visualized churn patterns across **demographic and transactional variables**  
- Identified key churn signals such as **transaction count**, **spending trends**, and **utilization ratios**

### 🔹 Modeling

Three models were trained and evaluated:

| Model             | Purpose                             | ROC-AUC | Recall (Churn) |
|------------------|--------------------------------------|---------|----------------|
| Random Forest     | Robust baseline model               | 0.986   | 85.4%          |
| XGBoost (Base)    | Improve recall, regularization      | 0.987   | 90.2%          |
| XGBoost (Tuned)   | Best performance, hyperparameter tuned | **0.993** | **90.7%**      |

---

## 🔍 Model Explainability

- Applied **SHAP values** and **feature importance charts**  
- **Top churn predictors**:  
  - `Total_Trans_Ct`  
  - `Total_Trans_Amt`  
  - `Total_Revolving_Bal`  
  - `Avg_Utilization_Ratio`

---

## 📈 Evaluation

- Used **ROC-AUC** as the primary metric for threshold-independent evaluation  
- Final tuned model achieved **97.2% accuracy** and strong recall — ideal for minimizing missed churn cases

---

## 📌 Key Takeaways for Stakeholders

Transaction behavior is the strongest predictor of churn. Customers with low transaction counts (Total_Trans_Ct) and lower total amounts spent (Total_Trans_Amt) were significantly more likely to leave the bank. These metrics consistently ranked among the top features in both SHAP and model-based importance analyses.

Lower relationship depth increases churn risk. Customers with fewer products (Total_Relationship_Count) and longer inactivity periods (Months_Inactive_12_mon) exhibited higher attrition, suggesting disengagement or limited banking engagement.

Certain customer segments are more vulnerable. Income groups like "Less than $40K" and single individuals showed above-average churn rates. These insights could support segmentation-based retention campaigns.

Premium expectations may not be met. Surprisingly, churn was higher among Platinum cardholders, indicating that premium clients might not perceive sufficient value — a signal to revisit service offerings for this segment.
---

## 🏁 Final Note

This project bridges **data science and business strategy**. By identifying patterns that drive customer attrition and using predictive models to flag churn risk, organizations can **shift from reactive to proactive** customer retention — improving satisfaction and loyalty.
