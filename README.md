Overview
This notebook explores the AI job trends dataset, focusing on the impact of AI on various job roles. The analysis combines data exploration, statistical analysis, clustering, regression, and demonstrative classification.
The notebook is designed for technical learning and exploratory analysis, not for production-grade predictions.

Dataset
Source: Kaggle – AI Impact on Job Market 2024–2030

Key columns include:
Job Title, Industry, Job Status
AI Impact Level, Median Salary (USD)
Experience Required (Years), Job Openings (2024), Projected Openings (2030)
Automation Risk (%), Remote Work Ratio (%), Gender Diversity (%)

Sections
Imports
Loads all necessary libraries for data analysis, visualization, and machine learning.
Data Loading & Inspection
Displays basic information, first rows, and summary statistics.
Checks for missing values and duplicates.
Exploratory Data Analysis (EDA)
Distribution plots for salaries, experience, and other numeric columns.
Boxplots comparing salary vs AI Impact Level or Automation Risk.
Correlation heatmaps for numeric features.
Categorical value counts.
Preprocessing
Encodes categorical variables.
Fills missing numeric values with median.
Scales numeric features for ML models.
Clustering
Performs K-Means clustering based on key numeric features.
Visualizes clusters and identifies patterns in salary vs automation risk.
Opportunity Scoring
Calculates Opportunity_Score = Median Salary / (Automation Risk + 1).
Ranks job opportunities by industry or role.
Regression (ML)
Predicts Median Salary (USD) using Linear Regression and Random Forest Regressor.
Evaluates using R² and RMSE.
Shows feature importance for insights.
Classification (Demonstrative)
Predicts AI Impact Level using Random Forest Classifier.
Focuses on feature importance rather than predictive performance.
Accuracy is low (~33%) due to weak correlation between features and AI Impact Level.
