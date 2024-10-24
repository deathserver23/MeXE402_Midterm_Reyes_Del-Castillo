# Midterm Examination

# Introduction 
Linear Regression (Introduction: Overview of Linear and Logistic Regression.)

# Logistic Regression 

Logistic regression is a statistical method used for binary classification tasks, where the goal is to predict the probability of an outcome that can take one of two possible values (e.g., success/failure, yes/no). The logistic regression model predicts the log-odds of the probability of the positive class (typically labeled as 1).

# Dataset Description

Dataset Description in Linear Regression (Dataset Description: Details about the datasets used)

Dataset Description in Logistic Regression

The Adult Census Income dataset, sourced from the UCI Machine Learning Repository, contains demographic information about individuals from the 1994 U.S. Census. It includes features such as age, education, occupation, marital status, race, sex, and hours worked per week, alongside a target variable indicating whether an individual's income exceeds $50,000 per year. This dataset is commonly used for classification tasks in machine learning, particularly to predict income levels based on personal attributes but instead of income the sex is the categorial we used. With a mix of categorical and numerical features, it serves as a rich resource for exploring socio-economic patterns and developing predictive models.

# Project Objectives
Objective for linear Regression Project Objectives: (What you aim to achieve with your analyses.)

Objectives for Logistic Regression
1. Examine Gender Distribution: Analyze the distribution of individuals by sex within different demographic groups (e.g., age, education, occupation).
2. Assess Employment Patterns: Investigate how employment status (e.g., employed, unemployed, never worked) varies by sex to identify any notable trends.
3. Educational Attainment: Explore the relationship between sex and educational levels, analyzing how educational attainment differs across genders.
4. Occupation Analysis: Examine the types of occupations held by different sexes to identify gender-based occupational segregation and its implications.
5. Demographic Correlations: Analyze how sex correlates with other demographic factors, such as race or marital status, to uncover patterns in the data.
6. Visualize Findings: Create visualizations predicted probabilities to clearly communicate model performance and the effects of predictors.

# Data Preproccessing 

![Screenshot 2024-10-24 110235](https://github.com/user-attachments/assets/70d9122b-993b-4fff-99cb-9dd166bd2cb5)


## Documentation 

# Methodology
In the data cleaning phase of the logistic regression analysis, missing values in the dataset were addressed to ensure the completeness of the data. We employed a systematic approach, first identifying missing values across all variables. For continuous variables, we used mean imputation to replace missing entries, while for categorical variables, we replaced missing values with the mode. This method was chosen to minimize bias and retain the overall structure of the dataset. After imputing the missing values, we conducted a final check to confirm that no entries remained missing, ensuring that our dataset was ready for subsequent analysis and model fitting.


