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
  - Performing Data Cleaning to ensure the dataset consistency, handling misssing values and delete unnecessary variables.
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

There are 8 dependent variables in the dataset:
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

| Precipitation Type   | Numerical Value |
|----------------------|-----------------|
| Snow                 | 1               |
| Rain                 | 2               |

- there's 2 categories : snow and rain

| Precip Type                            | Numerical Value  |
|----------------------------------------|------------------|
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

![Screenshot (677)](https://github.com/user-attachments/assets/476a8ab4-c899-4397-a757-b1d139ad6e93)
![Screenshot (678)](https://github.com/user-attachments/assets/cd49b9c9-8d3f-44da-82f9-b07a4bfe18da)

- The train_test_split function from scikit-learn's model_selection module is a tool for dividing datasets into training and testing subsets.In the dataset,x and y are split into training and testing sets. The test_size parameter specifies that 20% of the data should be used for the test set and the 80% is for training set, while the random_state parameter ensures reproducibility of the results.

## Model Implementation

![Screenshot (670)](https://github.com/user-attachments/assets/2e8508a8-ba99-4713-a2f6-4288706667ab)

- The code initializes a simple linear regression model using the scikit-learn library in Python. Linear regression is a technique in machine learning where we create a relationship between a set of inputs (features) and a continuous output, predicting outcomes based on those inputs. The first line, from sklearn.linear_model import LinearRegression, imports the class that represents this model. The second line, model = LinearRegression(), creates an instance of the model, allowing us to train it with data. Once initialized, we can use model.fit() to train the model on data and model.predict() to make predictions on new, unseen data. This linear regression model can help analyze trends, such as predicting sales, stock prices, or temperatures based on past data.

## Evaluation Metrics

![Screenshot (675)](https://github.com/user-attachments/assets/2ecea22c-e3a2-41a1-85f5-c281e98c57fc)
![Screenshot (676)](https://github.com/user-attachments/assets/1176b73c-24b6-4199-83fd-ef8a0f7ee62c)

- The code calculates the R-squared (R²) score, which shows how well the model's predictions match the actual results. After importing r2_score from sklearn.metrics, the line r2 = r2_score(y_test, y_pred) compares the real values (y_test) with the model’s predicted values (y_pred). The R² score ranges from 0 to 1, where a score closer to 1 means the model is doing a good job predicting the results, and a score closer to 0 means the predictions are less accurate.In our model, the accuracy score is 0.99,which is implies that the model is great.
- Adjusted R-squared (Adjusted R²) is an alternative for R-squared score that also considers how many features are in the model. R-squared (R²) measures how well the model's predictions match the real data, but it can go up just by adding more features, even if they don’t actually help. Adjusted R² fixes this by only increasing if new features improve the model's accuracy. This makes it a better way to compare models that use different numbers of features.

## Interpretation
- The dataset contains 96,453 rows and 9 columns, including variables like "Apparent Temperature (C)," "Humidity," "Wind Speed (km/h)," "Visibility (km)," and "Pressure (millibars)," among others, with the target variable likely being "Temperature (C)" as the model’s goal appears to be predicting temperature.Each coefficient in a linear regression model will show how strongly it influences the predicted temperature.The magnitude of each coefficient reflects the feature’s importance in predicting temperature, with larger values indicating a more substantial effect.The R-squared and Adjusted R-squared values will show how well the model predicts temperature based on the chosen coefficient. Higher R² values mean the model explains more of the temperature differences, which indicates it has strong predictive power, while lower values suggest it doesn’t fit the data well.

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
The logistic regression model for sex classification shows a strong ability to differentiate between male and female categories using specific features, with the confusion matrix serving as a valuable tool for interpretation. By displaying true positives, true negatives, false positives, and false negatives, the matrix allows for a nuanced evaluation of the model's performance, indicating where it makes accurate predictions and where it may need improvement. This detailed view aids in interpreting the model's reliability and pinpointing potential adjustments to enhance its precision and effectiveness in classification tasks.

## References
Weather Dataset, Kaggle. https://www.kaggle.com/datasets/muthuj7/weather-dataset

train_test_split. (n.d.). Scikit-learn. https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.train_test_split.html

Adult Cencus Income, Kaggle. https://www.kaggle.com/datasets/uciml/adult-census-income

IBM, What is Logistic Regression https://www.ibm.com/topics/logistic-regression

animesh-agarwal (2018) https://github.com/animesh-agarwal/Machine-Learning-Datasets/blob/master/census-data/census%20income%20logistic%20regression.ipynb, https://towardsdatascience.com/logistic-regression-classifier-on-census-income-data-e1dbef0b5738 



