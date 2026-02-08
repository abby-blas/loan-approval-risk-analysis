# Loan Approval Decision Support Analysis

## Overview
This project explores how classification models can support loan approval decisions by balancing predictive performance, interpretability, and financial risk. Rather than automating approvals, the analysis focuses on understanding model tradeoffs and how decision thresholds can be adjusted to align predictions with real-world business and risk considerations.

## Problem Context
Loan approval decisions involve tradeoffs between approving qualified applicants and minimizing default risk. This project simulates a decision-support setting by comparing models  and analyzing how their differences impact approval outcomes and potential risk exposure.

## Data
The dataset consists of loan application records containing applicant demographic, financial, and loan-related features. The target variable indicates whether a loan was approved or rejected.

Key preprocessing steps include:
- Handling missing values
- Encoding categorical variables
- Defining features (X) from the target variable (y)

## Modeling Approach

Two classification models were evaluated:

- **Logistic Regression:** Chosen for interpretability and transparency, which are important for clear communication with stakeholders.

- **Random Forest Classifier:** Used to capture non-linear relationships and interactions that may improve predictive performance at the cost of reduced interpretability.

Model evaluation emphasized error tradeoffs rather than accuracy alone, with particular attention to the financial impact of false approvals versus false rejections. In addition to standard model evaluation metrics, the analysis includes a cost-sensitive decision threshold assessment. This approach examines how adjusting probability thresholds affects approval rates and error tradeoffs when false approvals are treated as more costly than false rejections.

## Key Findings
- Logistic regression produced higher approval rates, resulting in fewer false rejections but more false approvals.
- The Random Forest model reduced false approvals, indicating stronger risk control, but rejected more qualified applicants.
- These results highlight a common tradeoff in credit risk modeling between customer experience and financial risk mitigation.
- Cost-sensitive threshold analysis showed that the Random Forest model allowed for greater control over financial risk through threshold tuning, while logistic regression was less responsive to threshold changes.

## Practical Application

In a real-world setting, this analysis could support loan officers by flagging higher-risk applications for additional review rather than automating approval decisions. Model selection would depend on business priorities. Decision thresholds can be adjusted to reflect organizational risk tolerance, allowing the same model to support different approval strategies without retraining.

## Tools Used
- Python
- pandas, NumPy
- scikit-learn
- Jupyter Notebook
