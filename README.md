# Practical-Application-3
Application to compare performance of Classifier Models and identify the feature importance that affects the customer acceptance of banking products over the telephone-based marketing.

## Business Objectives
The application is built based on the CRISP-DM framework. The following are the business objective of this application,
1. Identify the performance/accuracy score of Classifier Models
2. Identify the factors that affect the customer acceptance of banking products via telephone marketing
3. Summarize and provide future recommendations

## Data
The dataset comes from the UCI Machine Learning repository (https://archive.ics.uci.edu/ml/datasets/bank+marketing). The data is from a Portugese banking institution and is a collection of the results of multiple marketing campaigns. The dataset contains 41188 entires with a total of 21 columns.
As noted in the data documentation, the 'duration' feature should only be included for benchmark purposes and should be discarded if the intention is to have a realistic predictive model. Hence, this feature is dropped for our model analysis.

## Classification Models Used
The following Classifier Models were used in this application,
1. DummyClassifier() - for baseline prediction
2. LogisticRegression()
3. KNeighborClassifier()
4. DecisionTreeClassifier()
5. RandomForestClassifier()
6. SVC()

In the initial analysis, **KNeighborClassifier()** and **LogisticalRegression()** models outformed the other models.
![image](https://user-images.githubusercontent.com/102641103/179647533-4e8f34a2-98b4-4631-ab8b-d4aa14cc962f.png)

After the initial analysis, the *GridSearchCV()* is applied to identify the best hyperparamaters and improved the performance of these Classifier Models. Among the improved models, **KNeighborClassifier()** and **DecisionTreeClassifier()** model outperformed the other improved classifier models.
![image](https://user-images.githubusercontent.com/102641103/179651030-bed9f6d5-4331-4a0c-bcb5-4af419875d49.png)

### Feature Importance of top models
Based on all the model analysis, the following features exhibited the highest feature importance,
1. euribor3m
2. nr.employed

## Conclusion
* In this application, we were able to identify that **KNeighborClassifier()** and **LogisticalRegression()** models outperformed the other models for the given dataset
* When improving the models with best hyperparameteres *GridSearchCV()*, **KNeighborClassifier()** and **DecisionTreeClassifier()** models outperformed the other models for the given dataset
* Both euribor3m and nr.employed features exhibited high feature importance
* By focusing on these features, will emable the marketing team for better acceptance of bank products to its customers.

## Content
* Practical_Application_3.pdf          # PDF summary report of the practical application
* prompt_III_VJ.jpynb                  # jupyter notebook with coding pipeline
* README.md                            # this readme file

## Requirements
1. This project is implemented with Python 3.7.13.
2. The final assignment is implemented in Google Colab and can be executed in any python notebook apps.
3. The required packages and libraries with their versions are listed in the prompt_III_VJ.jpynb file.
