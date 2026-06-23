# Customer Churn Prediction

Predicting which telecom customers are likely to leave using classification models.

## Dataset
Telco Customer Churn — 7,043 customers with 20 features
Source: https://www.kaggle.com/datasets/blastchar/telco-customer-churn

## Tools
- Python (pandas, scikit-learn, imbalanced-learn, matplotlib, seaborn)
- WPS Sheets
- Power BI

## Project Phases
1. EDA in WPS Sheets — churn rate, contract analysis, payment method analysis
2. Data cleaning and encoding in Python
3. SMOTE to balance churned vs non-churned customers
4. Classification modeling with Logistic Regression and Random Forest
5. Churn risk dashboard in Power BI

## Model Results
| Model | Accuracy | AUC |
|---|---|---|
| Logistic Regression | 81% | 0.888 |
| Random Forest | 84% | 0.919 |

## Key Findings
- Overall churn rate is 26.53%
- Month-to-month contracts have the highest churn at 2,220 customers
- Electronic check customers churn at 45.3% — nearly 3x higher than automatic payment methods
- Contract type, TotalCharges and MonthlyCharges are the strongest churn predictors

## Dashboard
![Churn Dashboard](outputs/churn_dashboard.png)

## How to Run
pip install -r requirements.txt
jupyter notebook notebooks/customer_churn_prediction.ipynb
