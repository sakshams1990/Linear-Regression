# Linear-Regression

The main goal of regression is the construction of an efficient model to predict the dependent attributes from a bunch of attribute variables.


The general line equation is, y =  a * x + b.

![alt text](http://www.mpl.loesungsfabrik.de/images/linear-regression.png)

Sum of squared residuals = ((a * x1 + b) -y1)^2 + ((a * x2 + b) -y2)^2 + ((a * x3 + b) -y3)^2 + ...

Since we want the line that will give us the smallest sum of squares, this method will find the best values for "a" and "b" is called "Least Squares".

The important concepts are :

1. Minimize the square of the distance between the observed values and the line.

2. This is achieved by taking the derivative of the slope and finding where it is equal to 0.

**Cost Function**

The cost function helps us to figure out the best possible values for a and b which would provide the best fit line for the data points. Since we want the best values for a and b, we convert this search problem into a minimization problem where we would like to minimize the error between the predicted value and the actual value.

![alt text](https://miro.medium.com/max/972/1*wQCSNJ486WxL4mZ3FOYtgw.png)

This cost function is also known as the Mean Squared Error(MSE) function.

**Residual** is the distance between the slope and the datapoint.

**R-squared** is a goodness-of-fit measure for linear regression models. This indicates the percentage of the variance in the dependent variable that the independent variables explain collectively. R-squared measures the strength of the relationship between your model and the dependent variable on a convenient 0 – 100% scale.

R2 = (Variance(Mean)-Variance(Fit))/Variance(Mean)

**Adjusted R2** is a modified version of R2 that gets adjusted as per the number of independent variables. Adjusted R2 increases only if the newly added variable improves the model.Adjusted R-squared is used to determine how reliable the correlation is and how much is determined by the addition of independent variables.
