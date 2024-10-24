## Midterm Examination

## Introduction 
Linear Regression (Introduction: Overview of Linear and Logistic Regression.)

## Logistic Regression 

Logistic regression is a statistical method used for binary classification tasks, where the goal is to predict the probability of an outcome that can take one of two possible values (e.g., success/failure, yes/no). The logistic regression model predicts the log-odds of the probability of the positive class (typically labeled as 1).

## Dataset Description

Dataset Description in Linear Regression (Dataset Description: Details about the datasets used)

Dataset Description in Logistic Regression

The Adult Census Income dataset, sourced from the UCI Machine Learning Repository, contains demographic information about individuals from the 1994 U.S. Census. It includes features such as age, education, occupation, marital status, race, sex, and hours worked per week, alongside a target variable indicating whether an individual's income exceeds $50,000 per year. This dataset is commonly used for classification tasks in machine learning, particularly to predict income levels based on personal attributes but instead of income the sex is the categorial we used. With a mix of categorical and numerical features, it serves as a rich resource for exploring socio-economic patterns and developing predictive models.

## Project Objectives
Objective for linear Regression Project Objectives: (What you aim to achieve with your analyses.)

Objectives for Logistic Regression
1. Examine Gender Distribution: Analyze the distribution of individuals by sex within different demographic groups (e.g., age, education, occupation).
2. Assess Employment Patterns: Investigate how employment status (e.g., employed, unemployed, never worked) varies by sex to identify any notable trends.
3. Educational Attainment: Explore the relationship between sex and educational levels, analyzing how educational attainment differs across genders.
4. Occupation Analysis: Examine the types of occupations held by different sexes to identify gender-based occupational segregation and its implications.
5. Demographic Correlations: Analyze how sex correlates with other demographic factors, such as race or marital status, to uncover patterns in the data.
6. Visualize Findings: Create visualizations predicted probabilities to clearly communicate model performance and the effects of predictors.

# Documentation 

## Methodology

## Data Preproccessing 

![Screenshot 2024-10-24 110235](https://github.com/user-attachments/assets/70d9122b-993b-4fff-99cb-9dd166bd2cb5)

In the data preprocessing stage of the logistic regression analysis, categorical variables were transformed into numerical format to enable model fitting. Specifically, we utilized one-hot encoding for nominal variables, creating binary indicator variables for each category. This transformation allowed us to incorporate categorical information into the model while ensuring that the logistic regression algorithm could interpret the data appropriately. After these conversions, we verified that all variables were in the correct numerical format.

## Model Implementation
![Screenshot 2024-10-24 110022](https://github.com/user-attachments/assets/129c8545-a07d-401d-9984-e3975a4a9cde)

the logistic regression analysis, we imported essential libraries to facilitate data manipulation, model training, and evaluation. The pandas library was used for data handling and preprocessing, allowing us to easily read and manipulate our dataset. We employed train_test_split from sklearn.model_selection to divide the dataset into training and testing sets, ensuring that our model could be evaluated on unseen data to assess its performance. The LogisticRegression class from sklearn.linear_model was utilized to fit our logistic regression model, providing a robust implementation of the algorithm. Finally, accuracy_score and classification_report from sklearn.metrics were included to evaluate the model's performance, offering insights into accuracy, precision, recall, and F1-score, which are crucial for understanding the model's predictive capabilities.
## Evaluation Metrics

![Screenshot 2024-10-24 105901](https://github.com/user-attachments/assets/e0065624-d538-4b6b-a1ec-16c6257ac427)

The calculated accuracy of 0.7326 in the logistic regression model indicates that approximately 73.26% of the predictions made by the model were correct. This metric provides a straightforward measure of how well the model performed on the test dataset, reflecting the proportion of true positive and true negative predictions relative to the total number of observations. While a higher accuracy suggests better model performance and close to 100%.

## Visualization
![Screenshot 2024-10-24 111738](https://github.com/user-attachments/assets/1bd25147-57aa-4389-b841-d29b6f90025e)

In logistic regression, plotting a confusion matrix provides a visual representation of the model's classification performance by summarizing the counts of true positive, true negative, false positive, and false negative predictions. This matrix allows us to quickly assess how well the model distinguishes between the two classes. Each cell in the matrix indicates the number of instances predicted by the model, with the diagonal representing correct classifications (true positives and true negatives) and the off-diagonal cells representing misclassifications (false positives and false negatives).

## Interpretation
Logistic regression is a powerful model for classification tasks, as it estimates the probability of a binary outcome based on input features. The importance of features in logistic regression is critical, as each feature contributes to the model’s decision-making process by adjusting the weights associated with it. These weights, also known as coefficients, directly influence the prediction by determining the direction and strength of the relationship between the feature and the target variable. A well-tuned logistic regression model not only classifies observations effectively but also offers insight into which features are most influential, providing interpretability to decision-making.


