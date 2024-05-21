# DataScienceCapstone

## Project Overview
This project aims to predict obesity levels in individuals based on various physical and dietary attributes using machine learning models. The dataset used was sourced from Kaggle and includes data from individuals in Mexico, Peru, and Colombia.

## Dataset
The dataset consists of 17 attributes and 2111 records. It includes features such as gender, age, weight, height, family history, high-calorie food intake, vegetable intake, number of daily meals, food between meals, smoking, water intake, calorie tracking technology usage, physical activity, alcohol consumption, mode of transportation, and obesity level. Notably, 77% of the data was generated synthetically using the Weka tool and the SMOTE filter, while 23% was collected directly from users via a web platform.

## Key Features
- **Height**
- **Weight**
- **FAF (Physical Activity)**
- **FCVC (Vegetable Intake)**

## Exploratory Data Analysis (EDA)
- **Heatmaps**: Used to identify correlations between numeric features and the target variable.
- **Bar Charts**: Display the relationship between the target variable and the mean values of selected features.

## Data Preprocessing
- No missing values were found in the dataset.
- **Label Encoding**: Categorical data was converted to numerical format.
- **Feature Scaling**: Standardization was applied to selected features to improve model performance and reduce outlier sensitivity.

## Model Building
Three machine learning models were implemented to predict obesity levels:
- **Support Vector Machine (SVM)**: Utilized a linear kernel with a C parameter of 1.0.
- **Decision Tree**: No maximum depth was specified to achieve the best results.
- **Logistic Regression**: Used to find the probability of an instance belonging to a specific class.

## Model Evaluation
The models were evaluated using metrics such as accuracy, precision, recall, and F1-score.

- **SVM**: Accuracy = 0.950, F1-score = 0.950
- **Decision Tree**: Accuracy = 0.947, F1-score = 0.945
- **Logistic Regression**: Accuracy = 0.889, F1-score = 0.887

## Conclusion
The SVM and Decision Tree models outperformed Logistic Regression, making them better choices for predicting multi-class obesity levels. Both SVM and Decision Tree models were better at handling non-linearity and dataset anomalies.
