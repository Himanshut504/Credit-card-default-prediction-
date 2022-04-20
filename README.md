# Credit-card-default-prediction-
## Introduction
Default credit cards are an important issue that brings negative consequences to both sides, i.e, banks and customers. If a customer does not pay his obligations, banks lose money, the customer will lose credibility in future payments, collection calls start to be made and in last resort, the case may go into court. In order to avoid all of that trouble, effective methods that are able to predict the default of credit cards are needed. Therefore, default credit card prediction is an important, challenging, and useful task that should be addressed.

In recent years, the credit card issuers in Taiwan faced the cash and credit card debt crisis and the delinquency is expected to peak in the third quarter of 2006 (Chou,2006). In order to increase market share, card-issuing banks in Taiwan over-issued cash and credit cards to unqualified applicants. At the same time, most cardholders, irrespective of their repayment ability, overused credit card for consumption and accumulated heavy credit and cash–card debts. The crisis caused a blow to consumer finance confidence and it is a big challenge for both banks and cardholders.

## Standardization of features


## Exploratory Data Analysis
After loading the dataset we compared our target variable that is “Default payment next month” with other independent variables. This process helped us figure out various aspects and relationships among the dependent and the independent variables. It gave us a better idea of which feature behaves in which manner compared to the dependent variable.

## Null values Treatment
Our data set didn’t have any null values to be treated. Outliers treatment Isolation Forest Algorithm: Isolation forest is a tree-based algorithm that is very effective for both outlier and novelty detection in high-dimensional data. Encoding of categorical columns We used One Hot Encoding(converting to dummy variables) to produce binary integers of 0 and 1 to encode our categorical features because categorical features that are in string format cannot be understood by the machine and needs to be converted to the numerical format.

Our main motive through this step was to scale our data into a uniform format that would allow us to utilize the data in a better way while performing fitting and applying different algorithms to it. The basic goal was to enforce a level of consistency or uniformity to certain practices or operations within the selected environment. Fitting different models For modeling, we tried various classification algorithms like:

- Logistic Regression
- SVM
- Decision Tree
- Random Forest Classification
- XGBoost Classification
- CatBoost Classification
- LightGBM Classification
- Tuning the hyperparameters for better recall
- Tuning the hyperparameters of respective algorithms is necessary for getting better accuracy and to avoid overfitting in the case of tree-based models like Random Forest Classifier and XGBoost classifier.

## Features Explainability
We have applied SHAP on the XGBoost and CatBoost model to determine the features that were most important while predicting an instance And also build a feature importance graph to find out which features were important and which were redundant in a model performance matrix
 

## Conclusion
From the project we can conclude that the default rate is higher for males, increases as the education increases, and also increases as the age of a person increases. i.e clients whose age over 60 was higher than mid-age and young people. In all of these models, our recall revolves in the range of 76 to 84%.with the best fit model as random forest
