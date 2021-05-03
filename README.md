# Propensity-Modelling( Propensity to buy)
Propensity modeling is a popular technique that tries to estimate the likelihood of customers performing specific actions using predictive analytics. That means we can use this technique to estimate the likelihood of a customer buying a product, the likelihood of a customer reacting to a particular email, the likelihood of a customer leaving our service etc.
This likelihood is calculated as probability, and this probability is called propensity score in propensity modeling.
By assigning different propensity scores to different customers based on the features we have selected, the propensity model will produce accurate predictions of future behavior.
This technique is used in various fields such as marketing, health care, economics, business etc.
Propensity modeling includes several techniques like Propensity Score Matching, Propensity Score Weighting, Propensity Score Stratification. However, in this course, we are only focusing on Propensity Score Matching(PSM), which is mostly used in business.
In this project we had build a propensity to buy model using [Online Shoppers Intention data set](https://archive.ics.uci.edu/ml/datasets/Online+Shoppers+Purchasing+Intention+Dataset).

## Feature Selection Methods Used
* Correlation coefficient : for removing correlated features
* Backward Elimination

## Algorithms Used
* Logistic Regression
* XGBoost

## Evaluation methods
 * Decile Analysis
