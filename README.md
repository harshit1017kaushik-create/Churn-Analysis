# Telecom Churn Prediction & Analytics

## Project Overview

This project analyzes customer churn patterns and uses machine learning to identify customers who may be at risk of leaving a telecommunications service provider.

The project combines data cleaning, exploratory data analysis (EDA), machine learning, AI-assisted customer risk analysis, and Power BI visualization to explore churn behavior and support customer retention planning.

## Project Objectives

- Understand customer churn patterns and key customer characteristics.
- Perform data cleaning and exploratory data analysis.
- Compare machine learning approaches for churn prediction.
- Address class imbalance using resampling and class-weighting techniques.
- Identify customers with different predicted churn-risk levels.
- Build an interactive Power BI dashboard for business analysis.
- Translate analytical findings into customer retention recommendations.

## Tools and Technologies

| Technology | Purpose |
|---|---|
| Python | Data processing and machine learning |
| Jupyter Notebook | Analysis and model development |
| Pandas | Data manipulation |
| Scikit-learn | Machine learning and evaluation |
| XGBoost | Gradient-boosting classification |
| Optuna | Hyperparameter optimization |
| SMOTE, SMOTEENN and ADASYN | Class-imbalance handling |
| My Power BI report | Dashboarding and visualization |
| GitHub | Project documentation and version control |

## Project Workflow

### 1. Data Cleaning and Exploratory Data Analysis

The EDA workflow explores the customer dataset and examines churn distribution and relationships between churn and customer attributes.

The analysis includes:
- Data inspection and preparation
- Univariate analysis
- Bivariate analysis
- Churn-rate comparisons across customer groups
- Identification of patterns relevant to customer retention

### 2. Machine Learning

The model-building workflow explores multiple classification approaches and techniques, including:

- Decision Tree
- Random Forest
- XGBoost
- Class weighting
- SMOTE, SMOTEENN and ADASYN
- RandomizedSearchCV
- Optuna hyperparameter tuning

These approaches are used to investigate how customer churn can be predicted and how class imbalance affects model development.

### 3. AI-Assisted Customer Risk Analysis

The AI Analyst workflow uses saved machine learning models to generate customer churn probabilities, assign risk categories, summarize customer risk, and produce business recommendations.

The analysis compares XGBoost and Optuna-based risk classifications to help identify customers who may benefit from proactive retention efforts.

### 4. Power BI Dashboard

The Power BI report contains four analytical pages.

**Page 1 — Customer Churn Overview**

- Total customers, churned customers, and overall churn rate
- Churn rate by contract type
- Churn rate by internet service
- Churn rate by online security

**Page 2 — AI Customer Risk Analysis**

- XGBoost high-risk customer count
- Optuna high-risk customer count
- Average XGBoost churn probability
- Risk distribution for both models
- Comparison of low-, medium-, and high-risk classifications

**Page 3 — Customer Insights & Recommendations**

- Churn rate by technical support
- Churn rate by tenure group
- Churn rate by payment method
- Customer counts by gender and churn status
- Key insights and customer retention recommendations

**Page 4 — Churn Analysis Dashboard**

A consolidated view of key customer metrics, contract and payment-method churn, XGBoost risk distribution, and business insights.

## Key Findings

The Power BI report presents the following observations from the analyzed dataset:

| Metric | Result |
|---|---:|
| Total customers | 7,032 |
| Churned customers | 1,869 |
| Overall churn rate | 26.58% |
| Month-to-month contract churn | 42.71% |
| Electronic Check payment churn | 45.29% |
| Churn among customers without Online Security | 41.78% |
| Churn among customers without Tech Support | 41.65% |
| Churn among customers in their first 1–12 months | 47.68% |

These results suggest that early-tenure customers and certain contract, payment, and service groups deserve further investigation when designing retention strategies.

The report also shows 1,587 customers classified as high risk by XGBoost and 1,649 classified as high risk by the Optuna-based model.

*Note: These findings describe the analyzed dataset. Associations do not establish causation, and predicted risk classifications are not confirmed future churn events.*

## Business Recommendations

Based on the observed patterns, the project highlights several potential actions:

- Explore retention offers and longer-term contract options for month-to-month customers.
- Investigate whether online security and technical support services can improve customer retention.
- Review the high churn rate among Electronic Check users and explore alternative payment options.
- Develop targeted onboarding and retention initiatives for customers in their first year.
- Use model-generated risk scores to prioritize further review and proactive retention outreach.

These recommendations should be validated against business context and customer outcomes before implementation.

## Repository Contents

The repository includes the following project artifacts:

- `Analysis_EDA.ipynb` — exploratory data analysis
- `ML_Model_Building.ipynb` — machine learning experimentation
- `AI_Analyst.ipynb` — customer risk analysis and recommendations
- `Customer-Churn.csv` — customer dataset
- `churn_predictions.csv` — generated churn prediction output
- `Project1_reports.pbix` — Power BI report

Saved model and preprocessing files may also be required to reproduce the AI Analyst workflow. Check that their filenames and relative paths match the notebook before running it.

## How to Explore the Project

1. Review `Analysis_EDA.ipynb` for the data exploration workflow.
2. Open `ML_Model_Building.ipynb` to review model development and experimentation.
3. Explore `AI_Analyst.ipynb` to understand customer risk scoring and generated insights.
4. Open the Power BI report in Power BI Desktop to explore the four dashboard pages.

The notebooks may require the relevant Python packages, saved model files, and correct dataset paths. Configure these dependencies before rerunning the workflow.

## Future Improvements

- Document model performance using verified evaluation metrics.
- Add reproducible environment and dependency instructions.
- Improve model monitoring and risk-score validation.
- Evaluate retention strategies using observed customer outcomes.
- Automate data processing and prediction generation.

## Author

**Harshit Kaushik**

B.Tech — Computer Science and Engineering

This project demonstrates practical work in data analytics, exploratory data analysis, machine learning, customer risk analysis, and business intelligence visualization.
