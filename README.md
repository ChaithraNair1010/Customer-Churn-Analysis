📊 Predicting Customer Attrition: Data-Driven Insights for Retention
This project focuses on predicting customer churn in the banking sector using machine learning. The objective is to empower organizations with a data-driven framework to proactively identify high-risk customers and improve retention strategies.

The solution was designed to prioritize both model performance and interpretability, ensuring it can deliver business value. The analysis highlights the key behavioral drivers of churn and delivers a reliable, explainable model ready for deployment.

🧠 Project Goals
Detect customers likely to churn (attrite) from the bank.

Understand why customers leave by identifying the most influential features.

Build a predictive model that balances accuracy, recall, and interpretability.

Equip business teams with insights to design targeted retention campaigns.

🛠️ Key Steps Undertaken
🔹 Data Cleaning & Preprocessing
Removed ID columns to avoid data leakage.

Encoded categorical features using One-Hot Encoding.

Addressed class imbalance using SMOTE to ensure fair learning for churn cases.

🔹 Exploratory Data Analysis
Visualized churn patterns across demographic and transactional variables.

Identified key churn signals such as transaction count, spending trends, and utilization ratios.

🔹 Modeling
Three models were trained and evaluated:

Model	Purpose	ROC-AUC	Recall (Churn)
Random Forest	Robust baseline model	0.986	85.4%
XGBoost (Base)	Improve recall, regularization support	0.987	90.2%
XGBoost (Tuned)	Best performance, hyperparameter tuned	0.993	90.7%

🔍 Model Explainability
Applied SHAP values and feature importance charts to enhance transparency.

Top churn predictors:

Total_Trans_Ct

Total_Trans_Amt

Total_Revolving_Bal

Avg_Utilization_Ratio

📈 Evaluation
Used ROC-AUC as the primary metric for performance across thresholds.

Final tuned model achieved 97.2% accuracy and high recall — ideal for minimizing missed churn cases.

📌 Key Takeaways for Stakeholders
High churn risk is tied to disengagement — fewer transactions, reduced spending, and declining usage.

The model can flag at-risk customers early, enabling timely actions like rewards, personal outreach, or service upgrades.

The approach is data-backed and explainable, making it suitable for business application and stakeholder trust.

🏁 Final Note
This project bridges data science and business strategy. By identifying patterns that drive customer attrition and using predictive models to flag churn risk, organizations can shift from reactive to proactive customer retention — improving satisfaction and loyalty.

