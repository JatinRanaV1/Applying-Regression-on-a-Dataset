# Applying-Regression-on-a-Dataset
Regression consists of a set of machine learning methods that allow us to predict a continuous outcome variable (y) based on the value of one or multiple predictor variables (x).

Briefly, the goal of regression model is to build a mathematical equation that defines y as a function of the x variables. Next, this equation can be used to predict the outcome (y) on the basis of new values of the predictor variables (x).

![Alt text](https://static.javatpoint.com/tutorial/machine-learning/images/simple-linear-regression-in-machine-learning5.png)

Linear regression is the most simple and popular technique for predicting a continuous variable. It assumes a linear relationship between the outcome and the predictor variables.

The linear regression equation can be written as y = c + a*x + e, where:

c is the intercept,
a is the regression weight or coefficient associated with the predictor variable x.
e is the residual error

Technically, the linear regression coefficients are detetermined so that the error in predicting the outcome value is minimized.

When you have multiple predictor variables, say x1 and x2, the regression equation can be written as y = c + a1*x1 + a2*x2 + .... + an*xn + e. In some situations, there might be an interaction effect between some predictors.

Note also that, linear regression models can incorporate both continuous and categorical predictor variables.

When you build the linear regression model, you need to diagnostic whether linear model is suitable for your data.

In some cases, the relationship between the outcome and the predictor variables is not linear. In these situations, you need to build a non-linear regression, such as polynomial and spline regression.

When you have multiple predictors in the regression model, you might want to select the best combination of predictor variables to build an optimal predictive model. This process called model selection, consists of comparing multiple models containing different sets of predictors in order to select the best performing model that minimize the prediction error.

You can apply different regression models on your data, compare the models and finally select the best approach that explains well your data. To do so, you need some statistical metrics to compare the performance of the different models in explaining your data and in predicting the outcome of new test data.

The best model is defined as the model that has the lowest prediction error. The most popular metrics for comparing regression models, include:

Root Mean Squared Error, which measures the model prediction error. It corresponds to the average difference between the observed known values of the outcome and the predicted value by the model. RMSE is computed as RMSE = mean((observeds - predicteds)^2) %>% sqrt(). The lower the RMSE, the better the model.
Adjusted R-square, representing the proportion of variation (i.e., information), in your data, explained by the model. This corresponds to the overall quality of the model. The higher the adjusted R2, the better the model.
