# Predicting_Credit_Card_Approval
Commercial banks receive a lot of applications for credit cards. Many of them get rejected for many reasons, like high loan balances, low income levels, or too many inquiries on an individual's credit report, for example. Manually analyzing these applications is mundane, error-prone, and time-consuming. Therefore, it was created automatic credit card approval predictor using machine learning techniques.

## Steps:
* Data review
* Cleaning data such as copying with missing values, outliers (deletion)
* Checking assumptions (chi-suare test,bonferroni)
* Creating new data
* Encoding categorical features
* Checking VIF
* Parameters tunning
* Creating models (normalization, logistic regression)
  
## Summary: 
The conducted tests (chi-suare test,bonferroni) showed there is high multicollinearity in variables 6,9,11 and medicore in 4,5,7,10. There is no statistically significant relationship between variables 10, 11 and variable 12, which we are going to predict what is undesirable. The lack of multicollinearity is observed in variables 0,1,2,3. However, between variables 0,1 and 12 there is no statistically significant relationship what may negatively affect the prediction. A new variable was created where columns 6,9,11 were removed.

VIF, or Variance Inflation Factor, is a measure that determines the extent to which the variance of an estimator in a multiple regression model is increased due to correlations among the independent variables. VIF greater than or equal to 5 may indicate a multicollinearity problem that can affect the stability of model parameter estimation. VIF values were compared for raw data and cleaned data. In cleaned data there are higher values of VIF which may indicate that relevant variables have been removed.

