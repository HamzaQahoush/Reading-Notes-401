# Read 13: Linear Regressions :
## How to run Linear regression in Python scikit-Learn:
* **Regression analysis** is one of the most important fields in statistics and machine learning. There are many regression methods available. Linear regression is one of them.
* **Regression** searches for relationships among variables.
* **Linear regression** is a basic and commonly used type of **predictive analysis**.The overall idea of regression is to examine two things:
 1. does a set of predictor variables do a good job in predicting an outcome (dependent) variable?
 2. Which variables in particular are ignificant predictors of the outcome variable, and in what way do they–indicated by the magnitude
 sign of the beta estimates–impact the outcome variable? 
 * These regression estimates are used to explain the relationship between one **dependent variable** and one or more **independent variables**.
* Dependent variables -> outputs-> responses.
* Independent variables-> inputs-> predictors.
* **Scikit-learn** is a powerful Python module for machine learning. It contains function for regression, classification, clustering, model selection and dimensionality reduction.
* If you want to implement linear regression and need the functionality beyond the scope of scikit-learn, you should consider **statsmodels**. It’s a powerful Python package for the estimation of statistical models, performing tests, and more. It’s open source as well.
* Important functions to keep in mind while fitting a linear regression model are:
1. **.fit()**-> fits a linear model
2. **.predict()** -> Predict Y using the linear model with estimated coefficients
3. **.score()** -> Returns the coefficient of determination (R^2). A measure of how well observed outcomes are replicated by the model, as the proportion of total variation of outcomes explained by the model.
* If you wont implement linear regression on the entire data set, you will have to split the data sets into training and test data sets. So that you train your model on training data and see how well it performed on test data.

## Simple Linear Regression With scikit-learn :
* There are five basic steps when you’re implementing linear regression:
1. Import the packages and classes you need.
2. Provide data to work with and eventually do appropriate transformations.
3. Create a regression model and fit it with existing data.
4. Check the results of model fitting to know whether the model is satisfactory.
5. Apply the model for predictions.
