
# Project Description

Welcome to the Telecom Customer Churn Prediction project! In today's competitive telecom industry, customer retention is paramount. This project aims to predict customer churn using machine learning, assisting telecom companies in proactively retaining their valuable customers.

## Project Goals

- **Customer Churn Prediction**: Our primary objective is to develop a robust predictive model capable of identifying customers at risk of churning, allowing telecom providers to take timely actions to retain them.

- **Optimizing Retention Strategies**: We seek to optimize customer retention strategies by gaining insights into the key factors that contribute to churn.

- **Cost Reduction**: By retaining existing customers, this project aids telecom companies in reducing the high costs associated with acquiring new ones.

## Project Pipeline Overview

Our project follows a structured pipeline:

### 1.**Problem Statement**: In the telecom industry, customer acquisition costs often exceed retention costs. This project addresses the challenge of predicting customer churn accurately.

### 2.**Data Gathering**: Collecting telecom-related dataset with customer information, behavior data, and switch status for further analysis and model training. Download the data in the .csv file format.

### 3.**EDA (Exploratory Data Analysis)**: The data is meticulously explored to identify patterns, outliers, and critical insights, providing the foundation for subsequent steps.

#### 3.1. Data Frame Shape: Examine the telecom dataset to understand the number of rows and columns.

#### 3.2. Handling Null Values: Identify and handle missing values in the dataset using relevant functions like isnull() and fillna().

#### 3.3. Outlier Detection: Use box plots and IQR (Interquartile Range) function to identify potential outliers in the data

#### 3.4. Outlier Treatment: Replace identified outliers using the Interquartile Range (IQR) method.

#### 3.5. Statistical Information: Calculate mean, median, and other descriptive statistics (e.g., standard deviation) using functions describe() to gain insights into data characteristics.

#### 3.6. Data Insights: Analyze the EDA results to uncover valuable insights and patterns that can inform feature engineering and model training decisions

### 4.**Feature Engineering**: To prepare the data for modeling, we apply techniques such as one-hot encoding and label encoding for categorical variables and handle missing data.

####  4.1. Handling Categorical Variables: Encoded categorical variables using one-hot encoding for the 'state' column and label encoding for 'international plan' and 'voicemail plan' columns.

####  4.2. Customer ID Removal: Dropped the 'Customer ID' column as it didn't contribute significantly to the model.

####  4.3. Normalization: Used Min-Max scaling (MinMaxScaler) to scale features between 0 and 1, ensuring uniformity across different numerical attributes 


 ### 5.**Feature Selection**: We select the most influential features for our model to enhance its predictive accuracy.

#### 5.1. Correlation Analysis: Examined feature correlations using the Pearson correlation coefficient to identify relationships between different attributes. This helped to understand the strength and direction of linear relationships between variables.

#### 5.2. Variance Inflation Factor (VIF): Assessed multicollinearity among features using VIF to ensure independence. VIF values below 5 indicated low multicollinearity, ensuring that the selected features were not highly correlated.

#### 5.3. Train-Test Split: Split the data into training and testing sets (70% training, 30% testing) to evaluate model performance. This allowed us to train the model on one set of data and test its performance on unseen data to avoid overfitting

6. ### **Model Training**: We employ various machine learning algorithms, including Logistic Regression, Decision Trees, Random Forest, and AdaBoost, to develop predictive models.

7. ### **Hyperparameter Tuning**: For Decision Trees, we perform hyperparameter tuning to optimize model performance.

8. ### **Checking for Model Accuracy**: Our chosen model, Decision Tree with Hyperparameters, is evaluated for its predictive accuracy.

## Key Features

- **Logistic Regression**: An initial model with 85% training and 78% testing accuracy.
  
- **Decision Trees**: Decision Tree models, initially showing overfitting on training data, improved through hyperparameter tuning, achieving 96% training and 94% testing accuracy.

- **Random Forest**: Random Forest models, also prone to overfitting, demonstrated 96% training and 90% testing accuracy after hyperparameter tuning.

- **AdaBoost**: AdaBoost models showed 89% training and 86% testing accuracy, with slight improvements following hyperparameter tuning (91% training, 86% testing).

This project offers valuable insights into customer churn prediction, making it a valuable asset for the telecom industry. Explore each section to delve deeper into our process and results.
