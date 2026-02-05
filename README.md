# Loan Approval Decision Support Analysis

## Overview
This project explores how classification models can support loan approval decisions by balancing predictive performance, interpretability, and financial risk. Rather than automating approvals, the analysis focuses on understanding model tradeoffs and how predictions could be used to inform real-world decision-making.

## Problem Context

Loan approval decisions involve tradeoffs between approving qualified applicants and minimizing default risk. Financial institutions often use predictive models as **decision-support tools**, flagging applications for approval or additional review rather than relying on fully automated decisions.

This project simulates that setting by comparing models with different risk and interpretability profiles

## Data

The dataset consists of historical loan application records containing applicant demographic, financial, and loan-related features. The target variable indicates whether a loan was approved or rejected.

Key preprocessing steps include:
- Handling missing values
- Encoding categorical variables
- Separating features (X) from the target variable (y)

## Modeling Approach

Two classification models were evaluated:

- **Logistic Regression:** Chosen for interpretability and transparency, which are important for regulatory compliance and customer communication.

- **Random Forest Classifier:** Used to capture non-linear relationships and interactions that may improve predictive performance at the cost of reduced interpretability.

Model evaluation emphasized **error tradeoffs** rather than accuracy alone, with particular attention to the financial impact of false approvals versus false rejections.

## Key Findings
- Logistic regression prioritized higher approval rates, resulting in fewer false rejections but more false approvals.
- The Random Forest model reduced false approvals, indicating stronger risk control, but rejected more qualified applicants.
- These results highlight a common tradeoff in credit risk modeling between customer experience and financial risk mitigation.

## Practical Application

In a real-world setting, this analysis could support loan officers by flagging higher-risk applications for additional review rather than automating approval decisions. Model selection would depend on organizational risk tolerance, regulatory requirements, and business priorities.

## Tools Used
- Python
- pandas, NumPy
- scikit-learn
- Jupyter Notebook
