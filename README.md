# Regression
#Problem Statement
Wrong estimate or prediction of real estate/ housing properties leads to wrong budgeting and delay of payment for both customers and brokers. Hence the problem is to have an accurate method or model to have justified and correct pricing of real estate.
#Motivation
In real estate, there is usually a discrepancy between real pricing and expected pricing. As a result, it's preferable to utilise precise and best machine learning models based on historical records to forecast sales and purchase pricing. But various models can be used for predicting the price hence a comparative examination of the various models is required. Thus we planned to compile a short simulation on Comparative Analysis Of Various Models For House Sales Price  Prediction.
#Literature
House Price Index (HPI)-The House Price Index (HPI) is a broad measure of the movement of single-family property prices in the United States. In addition to serving as a trend indicator, it also serves as an analytical tool for estimating changes in mortgage default, prepayment, and housing affordability rates [1].
Housing Price Prediction via Improved Machine Learning Techniques-Before building models, the data should be processed accordingly so that the models could learn the patterns more efficiently. Specifically, numerical values were standardised, while categorical values were one-hot-encoded[2].

Housing Price Prediction Based on Multiple Linear Regression-According to economics principles, the market price of properties is attained when the demand and supply curves intersect with each other, which is subject to various factors, both subjectively and objectively[3]. 


#Models used/proposed(Flow Diagram)

#Linear Regression:


Linear Regression is a supervised machine learning algorithm. It carries out a regression task. Based on independent variables, regression models a goal prediction value. It is mostly used in forecasting and determining the link between variables. Different regression models differ in terms of the type of relationship they evaluate between dependent and independent variables and the number of independent variables they employ.
Linear regression performs the task to predict a dependent variable value (y) based on a given independent variable (x). So, this regression technique finds out a linear relationship between x (input) and y(output). Hence, the name is Linear Regression. 
Hypothesis function for Linear Regression:
   y =1+ 2.x
While training the model we are given :
x: input training data (univariate – one input variable(parameter))
y: labels to data (supervised learning)
When training the model – it fits the best line to predict the value of y for a given value of x. The model gets the best regression fit line by finding the best θ1 and θ2 values.
1 : intercept
2 : coefficient of x
How can the θ1 and θ2 values are updated to acquire the greatest fit line?
Cost Function (J):
The model seeks to predict the y value in such a way that the error difference between the predicted and true value is as small as possible by reaching the best-fit regression line. As a result, it is critical to update the θ1 and θ2 values in order to find the ideal value that minimises the difference between the predicted y value (pred) and the true y value (y).
minimize 1ni=1n (predi - yi )2
J = 1ni=1n (predi - yi )2
Cost function(J) of Linear Regression is the Root Mean Squared Error (RMSE) between predicted y value (pred) and true y value (y).





Least Squares Method


Gradient Descent Method


The model employs Gradient Descent to update θ1 and θ2 values in order to minimise Cost function (minimising RMSE value) and achieve the best fit line. The goal is to start with random θ1 and θ2 numbers and then update the values iteratively until the minimal cost is reached.

Multivariate Regression:

Multivariate Regression comes under the class of Supervised Learning Algorithms i.e when we are provided with a training dataset. In the case of multivariate linear regression, the output value is dependent on multiple input values. The relationship between input values, the format of different input values and the range of input values plays an important role in linear model creation and prediction.

For multiple input values, the hypothesis function will look like,

 y =1+ 2*x2  + 3* x3 + ……………n* xn
where x2, x3...xn  are multiple feature values


hθ(X)=Xθ 

If we consider the house price example then the factors affecting its price like house size, no of bedrooms, location etc are nothing but input variables of the above hypothesis function.

Cost Function:

A hypothesis is a predicted value of the response variable represented by h(x). Cost function defines the cost for wrongly predicting hypotheses. It should be as small as possible. We choose a hypothesis function as a linear combination of features x. 
J = 12ni=1n (predi - yi )2

Gradient Descent:
The model employs Gradient Descent to update θ1 and θ2 values in order to minimise Cost function (minimising RMSE value) and achieve the best fit line. The goal is to start with random θ1 and θ2 numbers and then update the values iteratively until the minimal cost is reached.


where, X0 = 1
     α = Learning rate
If α is too small, the gradient descent can be slow. It will require more iterations (hence time) to reach the minimum.

If α is too large, the gradient descent can overshoot the minimum. In that case, it may fail to converge or even diverge. If this happens when you run your Python code, NaN values are returned for θ0 , θ1. In that case, you should decrease the value of α and run the algorithm again.




RSS(Residual Sum of Squares):

The residual sum of squares (RSS), also known as the sum of squared residuals (SSR) or the sum of the squared estimate of errors (SSE), is the sum of the squares of residuals (deviations predicted from actual empirical values of data). It is a measure of the discrepancy between the data and an estimation model, such as linear regression. A small RSS indicates a tight fit of the model to the data.


R-squared(coefficient of determination):

R-squared is a statistical measure of how close the data are to the fitted regression line. It is also known as the coefficient of determination. Its value lies in the range (0,1). The ideal value for r-square is 1. The closer the value of r-square to 1, the better is the model fitted.

Residual Sum of Squares					Total Sum of Squares 
			

   	
