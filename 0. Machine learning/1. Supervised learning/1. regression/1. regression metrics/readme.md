## Metrics that can be used for regression techniques --

**_mean absolute error (MAE)_**

- Simple metric which calculates the absolute difference between actual and predicted values.
- The MAE we get is in the same unit as the output variable
- Most robust to outliers
- Graph of MAE is not differentiable so we have to apply various optimizers like Gradient descent which can be differentiable.

![alt text](https://github.com/nishchalnishant/Deep_learning_methods/blob/main/img/mae.jpg?raw=true)

**_mean squared error (MSE)_**

- Graph of mean squared error is differentiable so we can use it as loss function.
- The value we get afterr calculating MSE is a squared unit of output .
- If we have outliers in the dataset then it penalizes the outliers most and the calculated MSE is bigger. thus MSE is not roboust to outliers which were an advantage in MAE.

![alt text](https://github.com/nishchalnishant/Deep_learning_methods/blob/main/img/mse.jpg?raw=true)

**_Root mean squared error (RMSE)_**

- The outpput we get is the same unit as the required output cariale which makes interpretation of loss easy
- It is not tha roboust to outliers as compared to mean absolute error.
- Most prefered metrics while working with deep learning.
- In other words, it tells you how concentrated the data is around the line of best fit.
- Commonly used in climatology, forecasting, and regression analysis to verify experimental results.
- If the correlation coefficient is 1, the RMSE will be 0, because all of the points lie on the regression line (and therefore there are no errors).

> RMSE has a double purpose:

- To serve as a heuristic for training models
- To evaluate trained models for usefulness / accuracy

![alt text](https://github.com/nishchalnishant/Deep_learning_methods/blob/main/img/rmse.jpg?raw=true)

**_R squared_**

- Tells the performance of the model not the loss in an absolute sense .
- In contrast, MAE and MSE depend on the context as we have seen whereas the R2 score is independent of context.
- So, with help of R squared we have a baseline model to compare a model which none of the other metrics provides.
- So basically R2 squared calculates how must regression line is better than a mean line.
- Hence, R2 squared is also known as Coefficient of Determination or sometimes also known as Goodness of fit.
- If the R2 score is zero then the above regression line by mean line is equal means 1 so 1-1 is zero. So, in this case, both lines are overlapping means model performance is worst, It is not capable to take advantage of the output column.
- Now the second case is when the R2 score is 1, it means when the division term is zero and it will happen when the regression line does not make any mistake, it is perfect. In the real world, it is not possible.
- So we can conclude that as our regression line moves towards perfection, R2 score move towards one. And the model performance improves.

![alt text](https://github.com/nishchalnishant/Deep_learning_methods/blob/main/img/r_squared.jpg?raw=true)

**_Adjusted R squares_**

- Works on the disadvantage of the r squared which is while adding new features in data the r2 score starts increasing or remains constant but it never decreases because it assumes that while adding more data varriance of data increases.
- In adjusted r squared as K increases by adding some features so the denominator will increase n-1 remains constant r^2 score remains constant or increase slightly so the complete answer will increase and when we subtract this from one then the resultant score will decrease. so this is the case when we add an irrelevant feature in the dataset.
- And if we add a relevant feature then the R2 score will increase and 1-R2 will decrease heavily and the denominator will also decrease so the complete term decreases, and on subtracting from one the score increases.

![alt text](https://github.com/nishchalnishant/Deep_learning_methods/blob/main/img/regression.png?raw=true)
