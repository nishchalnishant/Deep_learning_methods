Metrics that can be used for regression techniques --

**mean absolute error (MAE)**

- sum of all errors and divide them by a total number of observations.
- 1/n\*(sum of (y-y_hat))

**mean squared error (MSE)**

- Sum of all errors squared and dividing them by total number of observations.
- 1/n\*(y-y_hat)^2

**Root mean squared error (RMSE)**

- Square root of mean squared error
- sqrt(1/n\*(y-y_hat)^2)

**R squared**

- 1-(SSr/SSm)
- Squared sum error of regression line
- Squared sum error of mean line

**Adjusted R squares**

- ![alt text](https://github.com/nishchalnishant/Deep_learning_methods/blob/main/img/regression.png?raw=true)

Algorithms for regression --

**Linear regression**

- Assumes linear relationship between the input variables and single ouptu variables .
- There are various methods to fit the linear regression from the data , most common of which is Ordinary least squares.
- We can fit the linear regression model using simple linear regression ,ordinary lelast squares, Gradient descent and regularizations (L1 lasso and L2 ridge)

**Support vector machines**

- can be used in regression as well as for classification
- Objective is to find a hyperplane in a n dimensional space that distinctly classifies the data points .
- If we are unable to split the datset using 2 dimensional hyper plane ,we move onto to the 3 dimensional hyperplane till we suceed.

**Descision tree**

**Random forest**
