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
* F Score(XGBoost)

## Algorithms Used
* Logistic Regression
* XGBoost


## Evaluation methods
 * Decile Analysis
 * ROC-Curve
 
## Results and Conclusion
* Using logistic regression, we got 69% of buyers in 1st decile, and 88% buyers within 3 deciles on training set. On test set, we got 45% of buyers in 1st decile and 89%of buyers within 3 deciles.
* Using XGBoost, we got 53% of buyers in 1st decile, and 95% buyers within 3 deciles on training set. On test set, we got 48% of buyers in 1st decile and 94%of buyers within 3 deciles.
* So, XGBoost performed well when compared to Logistic regression, by predicting 94% of buyers in top 3 deciles itself(in top 30%).

* So, a company can focus on that 3 deciles of customers only(those 30% of customers) for their marketing purposes, who are more likely to purchase their products without wasting their time and resources on those remaining 70% customers, who are very less likely to buy.In this way our propensity model can help companies for saving their resources and time, by only targeting on people who are more likely to buy their products.
![image](https://user-images.githubusercontent.com/71011054/124872490-f7ec6600-dfe2-11eb-93dc-d4c0f26ce09e.png)
On test set(using XGBoost)



