# Loan Approval Classification Analysis

## Overview
This project analyzes loan application data to identify patterns that influence whether a loan is approved or denied. The goal was to compare multiple machine learning models and determine which approach best predicts loan approval outcomes.

## Dataset
The dataset contains applicant financial and demographic features commonly used in loan decision processes, such as income, credit history, loan amount, and related attributes. Data was cleaned and preprocessed to handle missing values and prepare features for modeling.

## Methods
- Performed exploratory data analysis (EDA) to understand feature distributions and relationships.
- Preprocessed data using pandas and NumPy.
- Built and evaluated multiple models:
  - Linear Regression (baseline)
  - Decision Tree Classifier
  - Random Forest Classifier
- Compared model performance to identify the most effective approach.

## Results
- Tree-based models outperformed the linear baseline.
- The Random Forest classifier demonstrated the strongest overall performance, suggesting nonlinear relationships between applicant features and loan approval outcomes.
- Feature analysis indicated that certain financial attributes played a significant role in approval decisions.

## Key Takeaways
- Ensemble models can capture complex patterns in real-world financial data better than linear approaches.
- Careful preprocessing and model comparison are critical for reliable classification results.
- This workflow mirrors real-world decision-support systems used in financial institutions.

## Tools Used
Python, pandas, NumPy, scikit-learn, Matplotlib, Seaborn
