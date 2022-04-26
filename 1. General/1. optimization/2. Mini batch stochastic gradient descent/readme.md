## ABOUT

- Mini-batch gradient descent is a variation of the gradient descent algorithm that splits the training dataset into small batches that are used to calculate model error and update model coefficients.

- Implementations may choose to sum the gradient over the mini-batch which further reduces the variance of the gradient.

- Mini-batch gradient descent seeks to find a balance between the robustness of stochastic gradient descent and the efficiency of batch gradient descent.

- It is the most common implementation of gradient descent used in the field of deep learning.

**Pros**

- The model update frequency is higher than batch gradient descent which allows for a more robust convergence, avoiding local minima.

- The batched updates provide a computationally more efficient process than stochastic gradient descent.

- The batching allows both the efficiency of not having all training data in memory and algorithm implementations

**Cons**

- Mini-batch requires the configuration of an additional “mini-batch size” hyperparameter for the learning algorithm.
- Error information must be accumulated across mini-batches of training examples like batch gradient descent.
