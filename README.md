# 💻Midterm Examination

# 🎯Introduction 
Overview of Linear and Logistic Regression

## Linear Regression

Linear regression analysis is used to predict the value of a variable based on the value of another variable. The variable you want to predict is called the dependent variable. The variable you are using to predict the other variable's value is called the independent variable. When a linear model has one independent variable, the procedure is known as simple linear regression. When there are more than one independent variable, statisticians refer to it as multiple regression. These models assume that the average value of the dependent variable depends on a linear function of the independent variables.

## Logistic Regression 

Logistic regression is a statistical method used for binary classification tasks, where the goal is to predict the probability of an outcome that can take one of two possible values (e.g., success/failure, yes/no). The logistic regression model predicts the log-odds of the probability of the positive class (typically labeled as 1).

# 📚Dataset Description

Dataset Description in Linear Regression 

The data set has been selected from Kaggle and it contains real historical weather data with an daily summary for Szeged, Hungary , between 2006 and 2016.This dataset contains information about weather data, including temperature, humidity, wind speed, and precipitation. It can be used to predict weather patterns using linear regression.

Dataset Description in Logistic Regression

The Adult Census Income dataset, sourced from the UCI Machine Learning Repository, contains demographic information about individuals from the 1994 U.S. Census. It includes features such as age, education, occupation, marital status, race, sex, and hours worked per week, alongside a target variable indicating whether an individual's income exceeds $50,000 per year. This dataset is commonly used for classification tasks in machine learning, particularly to predict income levels based on personal attributes but instead of income the sex is the categorial we used. With a mix of categorical and numerical features, it serves as a rich resource for exploring socio-economic patterns and developing predictive models.

# 🔭Project Objectives
Objective for linear Regression Project Objectives: (What you aim to achieve with your analyses.)

Objectives for Logistic Regression
To model the probability of a binary outcome based on one or more independent variables. The aim is to estimate the likelihood that the dependent variable equals one of the categories based on the values of the independent variables, facilitating classification and risk assessment.

# 📸Documentation 
## Methodology
## Data Preproccessing

![Screenshot (648)](https://github.com/user-attachments/assets/898b51aa-5a59-455c-889a-9f8cd1eeb6ee)
![Screenshot (649)](https://github.com/user-attachments/assets/ae083cd0-b1d4-4319-99b0-1834daf77be6)
![Screenshot (650)](https://github.com/user-attachments/assets/4012ffb3-6311-4f2e-963d-c977fce40048)
![Screenshot (651)](https://github.com/user-attachments/assets/c873b63a-21b1-4167-a4d8-1185d112465a)
![Screenshot (652)](https://github.com/user-attachments/assets/900dd410-ac5a-4282-ad9e-35b1f0593d6d)
![Screenshot (653)](https://github.com/user-attachments/assets/6ece1638-7cec-44b2-89f5-7fb4db670d8b)
![Screenshot (654)](https://github.com/user-attachments/assets/645812b6-bf2c-414f-913c-a5106f456a71)
![Screenshot (655)](https://github.com/user-attachments/assets/90c50b76-365a-4da8-bfb9-9e5dd69bc0ce)

## Model Implementation

![Screenshot (660)](https://github.com/user-attachments/assets/698de597-26ae-4f04-81ec-40835ebd068e)

## Evaluation Metrics

![Screenshot (659)](https://github.com/user-attachments/assets/8a4dfcf9-f7b4-4194-8e0a-863aeab02917)
![Screenshot (661)](https://github.com/user-attachments/assets/0783c71b-8308-4c03-978c-eecd474bb890)

## Interpretation

## Data Preproccessing 

![Screenshot 2024-10-24 110235](https://github.com/user-attachments/assets/70d9122b-993b-4fff-99cb-9dd166bd2cb5)
![Screenshot 2024-10-24 121734](https://github.com/user-attachments/assets/36609749-c734-4397-9b13-b43012ce18b3)
![Screenshot 2024-10-24 121753](https://github.com/user-attachments/assets/09786620-fdc7-457c-8217-594d41019add)
![Screenshot 2024-10-24 121810](https://github.com/user-attachments/assets/14cfc02a-a926-4411-a80f-be09cffbc6f8)
![Screenshot 2024-10-24 121824](https://github.com/user-attachments/assets/38d1ffe2-c3ff-47b0-854a-3590107b4281)
![Screenshot 2024-10-24 121834](https://github.com/user-attachments/assets/bb1c0fcb-2e6f-4dd9-880b-c1899e06fac9)
![Screenshot 2024-10-24 121907](https://github.com/user-attachments/assets/60489b51-4671-4cce-b5cb-ef518b3196e9)
![Screenshot 2024-10-24 121928](https://github.com/user-attachments/assets/bb4ac8cd-dfcb-4641-b536-68d332ad5220)
![Screenshot 2024-10-24 121937](https://github.com/user-attachments/assets/bc59d790-c513-44da-9952-ce648b5ea93c)
![Screenshot 2024-10-24 121950](https://github.com/user-attachments/assets/3cb73334-3d16-4851-8662-d9958c8ffb16)
![Screenshot 2024-10-24 121959](https://github.com/user-attachments/assets/1c692c79-5ff9-4d00-9ff6-76338e95111b)
![Screenshot 2024-10-24 122006](https://github.com/user-attachments/assets/20b8c171-b4a5-4916-a37b-06abc61189a5)
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


