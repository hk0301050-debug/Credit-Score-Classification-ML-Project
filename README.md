# 💳 Credit Score Classification using Machine Learning

```{=html}
<p align="center">
```
![Python](https://img.shields.io/badge/Python-3.10+-blue)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-orange)
![XGBoost](https://img.shields.io/badge/XGBoost-Gradient%20Boosting-green)
![CatBoost](https://img.shields.io/badge/CatBoost-Gradient%20Boosting-yellow)
![License](https://img.shields.io/badge/License-MIT-red)

```{=html}
</p>
```
## 📌 Project Overview

This project develops an end-to-end **Machine Learning pipeline** for
predicting customer **Credit Score** categories (**Good**, **Standard**,
and **Poor**) using financial, behavioral, and credit history
information.

The project demonstrates the complete ML lifecycle including:

-   Data Cleaning
-   Exploratory Data Analysis (EDA)
-   Feature Engineering
-   Model Building
-   Hyperparameter Tuning
-   Model Comparison
-   Feature Importance Analysis
-   Model Selection

------------------------------------------------------------------------

# 📂 Dataset

  Attribute      Value
  -------------- ---------------------------
  Records        100,000
  Target         Credit_Score
  Classes        Good, Standard, Poor
  Problem Type   Multiclass Classification

------------------------------------------------------------------------

# 🚀 Project Workflow

``` text
Raw Dataset
      │
      ▼
Data Cleaning
      │
      ▼
EDA
      │
      ▼
Feature Engineering
      │
      ▼
Encoding
      │
      ▼
Train/Test Split
      │
      ▼
Model Training
      │
      ▼
Hyperparameter Tuning
      │
      ▼
Model Evaluation
      │
      ▼
Model Comparison
      │
      ▼
Final Random Forest Model
```

------------------------------------------------------------------------

# 🧹 Data Preprocessing

-   Removed placeholders (`_`, `-`)
-   Corrected incorrect data types
-   Converted Credit_History_Age into months
-   Missing value imputation
-   Customer-wise median imputation
-   Outlier treatment
-   Removed unrealistic Annual Income values
-   Cleaned impossible Interest Rate values

------------------------------------------------------------------------

# 📊 Exploratory Data Analysis

Performed:

-   Distribution plots
-   Count plots
-   Box plots
-   Correlation Heatmap

Major observations:

-   Outstanding Debt strongly influences Credit Score.
-   Higher Interest Rate generally indicates Poor credit.
-   Credit Mix has high predictive power.
-   Engineered financial ratios improve model performance.

------------------------------------------------------------------------

# ⚙️ Feature Engineering

Created important features including:

-   Debt_to_Income
-   EMI_ratio
-   Investment_Ratio
-   Savings
-   High_Utilization
-   Delayed_Payment
-   High_Inquiry
-   Credit_Health_Index
-   Delinquency_Score
-   Credit_History_Years
-   Customer-level aggregate statistics

------------------------------------------------------------------------

# 🤖 Models Evaluated

  Model                  Accuracy
  ------------------ ------------
  🥇 Random Forest     **83.05%**
  🥈 Extra Trees           82.88%
  🥉 XGBoost               81.99%
  CatBoost                 76.53%

------------------------------------------------------------------------

# 🏆 Final Model

**Random Forest**

### Performance

  Metric             Value
  ----------- ------------
  Accuracy      **83.05%**
  Precision           0.83
  Recall              0.83
  F1 Score            0.83

Class-wise Performance

  Class        Precision   Recall     F1
  ---------- ----------- -------- ------
  Good              0.81     0.79   0.80
  Poor              0.81     0.85   0.83
  Standard          0.85     0.83   0.84

------------------------------------------------------------------------

# ⭐ Top Important Features

1.  Credit_Mix
2.  Interest_Rate
3.  Credit_Health_Index
4.  Outstanding_Debt_max
5.  Outstanding_Debt_mean
6.  CustAvg_Outstanding_Debt
7.  Delinquency_Score
8.  Outstanding_Debt
9.  Changed_Credit_Limit
10. Delay_from_due_date_mean

------------------------------------------------------------------------

# 🛠 Tech Stack

-   Python
-   Pandas
-   NumPy
-   Matplotlib
-   Scikit-Learn
-   XGBoost
-   CatBoost
-   Joblib

------------------------------------------------------------------------

# 📁 Repository Structure

``` text
Credit-Score-Classification/
│
├── data/
├── notebooks/
├── models/
├── reports/
├── README.md
├── requirements.txt
└── LICENSE
```

------------------------------------------------------------------------

# 🔮 Future Improvements

-   Prevent customer-level data leakage
-   Try LightGBM
-   Ensemble Learning
-   Streamlit Web App
-   FastAPI Deployment
-   Docker Containerization

------------------------------------------------------------------------

# 👨‍💻 Author

**Himanshu Kumar**

If you found this project useful, consider giving it a ⭐ on GitHub.
