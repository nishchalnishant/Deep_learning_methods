## ABOUT

- Linear regression shows the linear relationship between the independent(predictor) variable i.e. X-axis and the dependent(output) variable.
- Based on the given data points, we attempt to plot a line that fits the points the best.

- To calculate best-fit line linear regression uses a traditional slope-intercept form which is given below
  Yi = β0 + β1Xi
  where Yi = Dependent variable, β0 = constant/Intercept, β1 = Slope/Intercept, Xi = Independent variable.

- The goal of the linear regression algorithm is to get the best values for B0 and B1 to find the best fit line. The best fit line is a line that has the least error which means the error between predicted values and actual values should be minimum.

> What is the best fit line?

    - In simple terms, the best fit line is a line that fits the given scatter plot in the best way. Mathematically, the best fit line is obtained by minimizing the Residual Sum of Squares(RSS).

- The cost function helps to work out the optimal values for B0 and B1, which provides the best fit line for the data points.

- In Linear Regression, generally Mean Squared Error (MSE) cost function is used, which is the average of squared error that occurred between the ypredicted and yi.

- Using the MSE function, we’ll update the values of B0 and B1 such that the MSE value settles at the minima.

- These parameters can be determined using the gradient descent method such that the value for the cost function is minimum.

- Gradient Descent is one of the optimization algorithms that optimize the cost function(objective function) to reach the optimal minimal solution.

- To find the optimum solution we need to reduce the cost function(MSE) for all data points.

- This is done by updating the values of B0 and B1 iteratively until we get an optimal solution.

**Pros:**

- Performs very well when there is a linear relationship between the independent and dependent variables.
- If overfits, overfitting can be reduced easily by L1 or L2 Norms.

**Cons:**

- Its assumption of data independence.
- Assumption of linear separability.
- Sensitive to outliers.

Credit:
https://www.analyticsvidhya.com/blog/2021/10/everything-you-need-to-know-about-linear-regression/
