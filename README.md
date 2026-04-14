#  Customer Churn Prediction for Bank Customers

##  Project Overview

This project builds a **machine learning model to predict customer churn** in a banking environment. The objective is to identify customers who are likely to leave the bank and provide actionable insights to improve retention strategies.

Customer churn is a critical business problem, as retaining existing customers is more cost-effective than acquiring new ones.

---

##  Business Problem

Banks face significant revenue loss when customers leave. The ability to predict churn enables:

* Early identification of at-risk customers
* Targeted retention campaigns
* Improved customer lifetime value

---

##  Dataset Description

The dataset contains customer demographic and financial information.

### Key Features:

* `CreditScore` — Customer creditworthiness
* `Geography` — Customer location
* `Gender` — Customer gender
* `Age` — Age of customer
* `Tenure` — Years with the bank
* `Balance` — Account balance
* `NumOfProducts` — Number of bank products used
* `HasCrCard` — Credit card ownership
* `IsActiveMember` — Activity status
* `EstimatedSalary` — Customer income

### Target Variable:

* `Exited` — Whether the customer churned (1) or stayed (0)

---

##  Data Preprocessing

* Standardized column names for consistency
* Removed irrelevant features (`RowNumber`, `CustomerId`, `Surname`)
* Applied encoding techniques:

  * One-Hot Encoding for `Geography`
  * Label Encoding for `Gender`

---

##  Exploratory Data Analysis (EDA)

Key analyses performed:

* Churn distribution across dataset
* Impact of geography on churn
* Relationship between age, balance, and churn
* Behavioral analysis using activity status and product usage

### Key Observations:

* Customers in Germany show higher churn rates
* Older customers are more likely to leave
* High-balance customers are at greater risk
* Inactive customers exhibit significantly higher churn

---

##  Machine Learning Approach

A structured ML pipeline was implemented using:

* **StandardScaler** — Feature scaling
* **Logistic Regression** — Baseline classification model

### Model Workflow:

* Train-test split (80/20)
* Hyperparameter tuning using GridSearchCV
* Cross-validation for stability

---

##  Model Evaluation

The model performance was evaluated using:

* Accuracy Score
* Confusion Matrix
* Classification Report
* ROC Curve
* AUC Score

### Results:

* Strong predictive performance
* Effective separation between churned and retained customers
* High AUC indicating good classification capability

---

##  Feature Importance

Using Random Forest:

* **Age** — Strongest driver of churn
* **Balance** — High-value customers more likely to leave
* **IsActiveMember** — Engagement strongly impacts retention

---

##  Key Insights

* Customer engagement is a critical retention factor
* High-balance customers require special attention
* Geography plays a significant role in churn behavior
* Age is a strong predictor of customer decisions

---

##  Business Recommendations

* Implement targeted retention strategies for high-value customers
* Increase engagement through loyalty programs
* Develop region-specific marketing strategies
* Promote multi-product usage to strengthen customer relationships

---

##  Risk Analysis

* False negatives (missed churners) are costly and impact revenue
* The model should prioritize identifying potential churners early

---

##  Limitations

* Dataset size is limited
* Real-world churn behavior may involve additional external factors
* Model performance may vary in production environments

---

##  Technologies Used

* Python
* Pandas
* NumPy
* Seaborn
* Matplotlib
* Scikit-learn

---

## How to Run

```bash
pip install -r requirements.txt
```

```bash
jupyter notebook
```

Run all cells sequentially.

---

##  Project Structure

```
customer-churn-prediction/
│
├── churn_analysis.ipynb
├── README.md
└── requirements.txt
```
---
##  Screen Shots
<img width="1024" height="677" alt="image" src="https://github.com/user-attachments/assets/e7b86e1f-e960-4f0f-bd88-9ebf126cc288" />
<img width="1015" height="717" alt="image" src="https://github.com/user-attachments/assets/493b772f-b5ff-4820-9fa2-0def594237ca" />
<img width="904" height="720" alt="image" src="https://github.com/user-attachments/assets/d03011f5-21c9-45fe-ba7b-1f47836f4c8c" />


---

##  Conclusion

This project demonstrates a complete **machine learning workflow**, combining data analysis, predictive modeling, and business insights.

The results highlight the importance of **customer engagement, financial behavior, and demographic factors** in predicting churn, enabling organizations to make informed, data-driven decisions.

---

##  Author

Muhammad Shoaib Inksar
Data Analyst | Machine Learning Enthusiast
