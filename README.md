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
Objective for Linear Regression
  - Performing Data Cleaning to ensure the dataset consistency, handling misssing values and delete unnecessary variables
  - To models the relationships between independent and dependent variable.
  - To choose the suitable the independent variable and it's dependent variable.
  - To test the accuracy of the model in prediction of values.

Objectives for Logistic Regression
  - Performing Data Cleaning to ensure the dataset consistency, handling misssing values and remove duplicates
  - To model the probability of a binary outcome based on one or more independent variables
  - Evaluating the program to classify the accuracy of categorical variable 
  

# 📸Documentation 
## Methodology
## Data Preproccessing

![Screenshot (664)](https://github.com/user-attachments/assets/894cda31-eee7-4971-908d-96cf683f7d8e)

There are 9 dependent variables in the dataset:
 - Summary
 - Precipitation Type
 - Apparent Temperature
 - Humidity
 - Wind Speed
 - Wind Bearing
 - Visibility
 - Pressure

And there's 1 independent variable : Temperature

We change the summary and precipitation types into numerical values as a part of data cleaning.

| Precip Type   | Numerical Value |
|---------------|-----------------|
| Snow          | 1               |
| Rain          | 2               |

- there's 2 categories : snow and rain

| Precip Type                            | Numerical Value |
|----------------------------------------|-----------------|
| Partly Cloudy                          | 10               |
| Mostly Cloudy                          | 11               |
| Overcast                               | 12               |
| Foggy                                  | 13               |
| Breezy and Mostly Cloudy               | 14               |
| Clear                                  | 15               |
| Breezy and Partly Cloudy               | 16               |
| Breezy and Overcast                    | 17               |
| Humid and Mostly Cloudy                | 18               |
| Humid and Partly Cloudy                | 19               |
| Windy and Foggy                        | 20               |
| Windy and Overcast                     | 21               |
| Breezy and Foggy                       | 22               |
| Windy and Partly Cloudy                | 23               |
| Breezy                                 | 24               |
| Dry and Partly Cloudy                  | 25               |
| Windy and Mostly Cloudy                | 26               |
| Dangerously Windy and Partly Cloudy    | 27               |
| Dry                                    | 28               |
| Windy                                  | 29               |
| Humid and Overcast                     | 30               |
| Light Rain                             | 31               |
| Drizzle                                | 32               |
| Clear                                  | 33               |
| Windy and Dry                          | 34               |
| Dry and Mostly Cloudy                  | 35               |
| Breezy and Dry                         | 36               |
| Rain                                   | 37               |

- there's 27 categories

![Screenshot (665)](https://github.com/user-attachments/assets/7061635b-0168-4841-a507-c38107a7c6c4)

- import pandas as pd - for data analysis and manipulation
- dataset = pd.read_csv('the name of the file')
- dataset.info - to get the summary of the dataset, if there's a missing values or null

## Model Implementation

![Screenshot (668)](https://github.com/user-attachments/assets/ca25f2d0-3657-42a6-babb-631d32c523cc)

![Screenshot (669)](https://github.com/user-attachments/assets/77c137d8-1186-43d2-864a-8433864367f6)

![Screenshot (670)](https://github.com/user-attachments/assets/2e8508a8-ba99-4713-a2f6-4288706667ab)

![Screenshot (671)](https://github.com/user-attachments/assets/e45b324f-9526-44f8-9a7e-653986d9cd5e)

![Screenshot (672)](https://github.com/user-attachments/assets/fac709a3-51e1-4c73-b1af-671550916156)


## Evaluation Metrics

![Screenshot (671)](https://github.com/user-attachments/assets/e45b324f-9526-44f8-9a7e-653986d9cd5e)

![Screenshot (672)](https://github.com/user-attachments/assets/fac709a3-51e1-4c73-b1af-671550916156)

## Interpretation


## Data Preproccessing 
  
Converting letters into numerical value 
| Letter        | Numerical Value |
|---------------|-----------------|
| Male          | 0               |
| Female        | 1               |

  
![Screenshot 2024-10-24 121734](https://github.com/user-attachments/assets/36609749-c734-4397-9b13-b43012ce18b3)
import pandas as pd - for Data Manipulation 

The file name depends on your assigned file name - adult.csv

![Screenshot 2024-10-31 002708](https://github.com/user-attachments/assets/0d268bb1-0b77-4a5a-87e2-0be397cc41b1)
This is the preview of your Dataset

![Screenshot 2024-10-31 003031](https://github.com/user-attachments/assets/0a9ef811-48f6-440a-ac4a-6446bdb2e892)
![Screenshot 2024-10-31 003051](https://github.com/user-attachments/assets/feb65710-0b89-435c-8a0f-b40c7362a569)
![Screenshot 2024-10-31 003041](https://github.com/user-attachments/assets/124bf023-2397-4822-ad5b-fbf340f20d55)

For splitting the dataset into train and test sets -from sklearn.model_selection import train_test_split 

![Screenshot 2024-10-31 003437](https://github.com/user-attachments/assets/1fae5f39-a8b3-45a5-a0c6-2a7fd59e1e6e)

For standardizing features - from sklearn.preprocessing import StandardScaler

In the data preprocessing stage of the logistic regression analysis, categorical variables were transformed into numerical format to enable model fitting. Specifically, we utilized one-hot encoding for nominal variables, creating binary indicator variables for each category. This transformation allowed us to incorporate categorical information into the model while ensuring that the logistic regression algorithm could interpret the data appropriately. After these conversions, we verified that all variables were in the correct numerical format.

## Model Implementation
![Screenshot 2024-10-31 003645](https://github.com/user-attachments/assets/5fd5522d-74ff-4c15-bc9c-8772c9ac3352)

For logistic regression implementation - from sklearn.linear_model import LogisticRegression  

the logistic regression analysis, we imported essential libraries to facilitate data manipulation, model training, and evaluation. The pandas library was used for data handling and preprocessing, allowing us to easily read and manipulate our dataset. We employed train_test_split from sklearn.model_selection to divide the dataset into training and testing sets, ensuring that our model could be evaluated on unseen data to assess its performance. The LogisticRegression class from sklearn.linear_model was utilized to fit our logistic regression model, providing a robust implementation of the algorithm. Finally, accuracy_score and classification_report from sklearn.metrics were included to evaluate the model's performance, offering insights into accuracy, precision, recall, and F1-score, which are crucial for understanding the model's predictive capabilities.
## Evaluation Metrics
![Screenshot 2024-10-31 004805](https://github.com/user-attachments/assets/ce80e0b5-b4ef-4923-a536-3f8b3748a8fd)

For evaluating the model performance - from sklearn.metrics import confusion_matrix

For calculating the accuracy of the model - sklearn.metrics import accuracy_score

The calculated accuracy of 0.7326 in the logistic regression model indicates that approximately 73.26% of the predictions made by the model were correct. This metric provides a straightforward measure of how well the model performed on the test dataset, reflecting the proportion of true positive and true negative predictions relative to the total number of observations. While a higher accuracy suggests better model performance and close to 100%.

## Visualization
![Screenshot 2024-10-31 004503](https://github.com/user-attachments/assets/c63445ec-5493-49ca-ac89-5152186e0764)


In logistic regression, plotting a confusion matrix provides a visual representation of the model's classification performance by summarizing the counts of true positive, true negative, false positive, and false negative predictions. This matrix allows us to quickly assess how well the model distinguishes between the two classes. Each cell in the matrix indicates the number of instances predicted by the model, with the diagonal representing correct classifications (true positives and true negatives) and the off-diagonal cells representing misclassifications (false positives and false negatives).

## Interpretation
Logistic regression is a powerful model for classification tasks, as it estimates the probability of a binary outcome based on input features. The importance of features in logistic regression is critical, as each feature contributes to the model’s decision-making process by adjusting the weights associated with it. These weights, also known as coefficients, directly influence the prediction by determining the direction and strength of the relationship between the feature and the target variable. A well-tuned logistic regression model not only classifies observations effectively but also offers insight into which features are most influential, providing interpretability to decision-making.

## References

Adult Cencus Income, Kaggle. https://www.kaggle.com/datasets/uciml/adult-census-income

IBM, What is Logistic Regression https://www.ibm.com/topics/logistic-regression

animesh-agarwal (2018) https://github.com/animesh-agarwal/Machine-Learning-Datasets/blob/master/census-data/census%20income%20logistic%20regression.ipynb, https://towardsdatascience.com/logistic-regression-classifier-on-census-income-data-e1dbef0b5738 


