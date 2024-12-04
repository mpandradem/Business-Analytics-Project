# Business-Analytics-Project

# Machine Learning applied to a medical dataset

As the final project for the course of Business Analytics, students were assigned a medical dataset for them to analyze and apply machine learning models to generate predictions.

The objective is to determine whether a patient is likely to develop heart disease based on information such as their weight, height, eating habits, and current medical conditions.

## File Outline

#### Exploratory Data Analysis (EDA)

The first section of the file is dedicated to the clean up and pre-processing of the original database. This includes handling missing values, null values, outliers, and categorical variables. A correlation matrix was created to determine which predictor variables have the highest correlation with the response variable. All the variables are visualized in different graphs for a better understanding of their structure and behavior. The clean data is stored in a new dataframe that will be used in the next steps.

#### Spliting data into training, validation, and testing sets

This section focuses on spliting the data into three subsets: training (50%), validation (25%), and testing (25%). This is done for the response variable and for the set of predictor variables. The graphs included show the class distribution between the different subsets of data.

#### Application of SMOTE and Random Under-Sampling

In this section we apply the Random Forest Classifier model to find whether SMOTE or RUS should be used to handle the unbalanced dataset. This is done by scoring the accuracy of these two techniques and comparing the results.

#### Application of machine learning algorithms

Four different algorithms are applied using the SMOTE training technique. The algorithms are the following:
- Logistic Regression
- Desicion Tree Classifier
- Naive Bayes Classifier
- Ensemble
    - Combination of Logistic Regression, Random Forest, and XGBoost

For the algorithms of Decision Tree Classifier and Logistic Regression two hyperparameter optimization methods were used: random search and grid search respectively.

#### Evaluation of the models

To score the models, an evaluation function was created. This includes a subfunction to calculate metrics such as accuracy, presicion, sensitivity, specificity, and auc score using the sklearn.metrics library. Another subfunction is used to print the results obtained. The last subfunction graphs the ROC curve. The main function is later called on with each of the four algorithms explored in the previous section.

## Authors

- María Paula Andrade
- Mateo Herrera
- Iván Olaizola


