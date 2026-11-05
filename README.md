# AI-Powered-Customer-Churn-Intelligence-System
End-to-end customer churn project: SQL analysis, ML prediction, SHAP explainability, AI retention recommendations, and an interactive dashboard.

An end-to-end churn analytics project that predicts which telecom customers are likely to leave, explains why, and recommends retention actions. It combines SQL analysis, machine learning, SHAP explainability, an AI recommendation engine, and an interactive dashboard.

## Business Problem
Acquiring a new customer costs much more than keeping an existing one. This project helps a telecom business identify customers at risk of churning, understand the drivers behind it, and act before they leave.

## Dataset
- Telco Customer Churn dataset
- 21 columns and about 7,000 customer records
- Covers customer demographics, services subscribed, contract and billing details, and the churn label

## Data Cleaning
- Found 11 blank values in the `TotalCharges` column during SQL analysis and handled them before modelling.
- Prepared and encoded the data for machine learning.

## Project Workflow
1. **SQL analysis:** explored the data and checked quality, including the blank TotalCharges rows.
2. **Python:** cleaning, exploratory analysis, and feature preparation.
3. **Machine learning:** trained and compared three models.
4. **SHAP:** explained the model's predictions and the main drivers of churn.
5. **AI recommendation engine:** suggests retention actions for at-risk customers.
6. **Dashboard:** an interactive view of churn insights, built with Claude.

## Model Performance

| Model | Accuracy | Precision | Recall | F1 | ROC-AUC |
|---|---|---|---|---|---|
| Logistic Regression | 80.55% | 65.72% | 55.88% | 60.40% | 84.21% |
| Random Forest | 78.28% | 61.89% | 47.33% | 53.64% | 82.32% |
| **XGBoost** | **80.55%** | **67.24%** | 52.14% | 58.73% | **84.52%** |

XGBoost was selected as the final model because it has the highest ROC-AUC (84.52%) and the highest precision (67.24%). Logistic Regression has a slightly higher recall and F1, so it is a strong, simpler alternative.

## Explainability with SHAP
SHAP values show which features push a customer towards or away from churning, so every prediction can be explained to a business team and not treated as a black box.

## AI Recommendation Engine
For customers flagged as high risk, the engine turns the model's findings into suggested retention actions.

## Tools and Technologies
- SQL
- Python: Pandas, NumPy, Scikit-learn, XGBoost, SHAP, Matplotlib
- Jupyter Notebook
- AI recommendation engine
- Interactive dashboard

## Repository Structure
- `sql/`: SQL queries
- `notebook.ipynb`: Python analysis, models, and SHAP
- `data/`: dataset
- `dashboard/`: dashboard file
- `images/`: charts and screenshots

## Dashboard Preview
<img width="538" height="506" alt="image" src="https://github.com/user-attachments/assets/c2300295-34da-405a-b1e3-f7784e18c789" />


## Author
Kumkum
