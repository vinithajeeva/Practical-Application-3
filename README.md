# Practical-Application-3
Application to compare performance of Classifier Models and identify the feature importance that affects the customer acceptance of banking products over the telephone-based marketing.

## Business Objectives
The application is built based on the CRISP-DM framework. The following are the business objective of this application,
1. Identify the performance/accuracy score of Classifier Models
2. Identify the factors that affect the customer acceptance of banking products via telephone marketing
3. Summarize and provide future recommendations (if any)

## Data
The dataset comes from the UCI Machine Learning repository (https://archive.ics.uci.edu/ml/datasets/bank+marketing). The data is from a Portugese banking institution and is a collection of the results of multiple marketing campaigns. The dataset contains 41188 entires with a total of 21 columns.

## Model
The following Classifier Models were used in this application,
1. DummyClassifier() - for baseline prediction
2. LogisticRegression()
3. KNeighborClassifier()
4. DecisionTreeClassifier()
5. RandomForestClassifier()
6. SVC()
After the initial analysis, the GridSearchCV() to identify the best paramater for these models and reevaluate tthe performance of these Classifier Models. Among these, the LogisticRegression() model outperformed the other Classifier models.

### Feature Importance at the model-level

## Conclusion
* In this application, we were able to identify that LogisticRefression() model outperformed the other models for the given dataset
* When improving the models with best hyperparameteres GridSearchCV(), the DecisionTree() model outperformed the other models for the given dataset
* In all the models, the following features exhibits more importance in accepting/rejecting the bank marketing offer - No. of Employees, Duration, Euribor3m
* As notedd in the data documentation, duration should only be included for benchmark purposes and should be discarded if the intention is to have a realistic predictive model

## Content
* Practical_Application_3.pdf          # PDF summary of the final assignment
* prompt_III_VJ.jpynb                  # jupyter notebook with coding pipeline
* README.md                            # this readme file

## Requirements
1. This project is implemented with Python 3.7.13.
2. The final assignment is implemented in Google Colab.
3. The required packages and libraries with their versions are listed in the prompt_III_VJ.jpynb file.
