# Customer Churn Detection ML Project 🔄

Predict whether a telecom customer will churn using Machine Learning.
Built with IBM Telco Customer Churn Dataset.

## 📊 Dataset
- **Source:** IBM Telco Customer Churn Dataset
- **Size:** 7,043 customers, 21 features
- **Target:** Churn (Yes/No)
- **Class Distribution:** No Churn 73.5% / Churn 26.5%

## 📋 Steps
1. Data Loading & Exploration
2. Data Cleaning (TotalCharges conversion)
3. Feature Engineering (Label Encoding + One-Hot Encoding)
4. Class Imbalance Handling (SMOTE)
5. Model Training & Evaluation

## 🤖 Models Compared

| Model | F1 Score (Churn) | Recall |
|-------|-----------------|--------|
| Random Forest | 0.562 | 0.49 |
| Random Forest + SMOTE | 0.571 | 0.53 |
| **XGBoost** ✅ | **0.612** | **0.70** |

## 🏆 Best Model: XGBoost
- **F1 Score:** 0.612
- **Recall:** 0.70
- **Key Config:** scale_pos_weight=2.77

## 💡 Key Findings
- Month-to-month customers churn most
- Higher tenure = lower churn rate
- F1 Score prioritized over Accuracy (class imbalance)

## 🛠️ Tech Stack
- Python 3.13, scikit-learn, XGBoost
- imbalanced-learn (SMOTE)
- pandas, numpy, matplotlib, seaborn

## 🚀 How to Run
1. Clone this repo
2. Open notebook/churn_prediction.ipynb in Google Colab
3. Run all cells
