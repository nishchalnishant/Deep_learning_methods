**Stochastic Gradient Descent**

- Stochastic Gradient Descent is an iterative optimization technique that uses minibatches of data to form an expectation of the gradient, rather than the full gradient using all available data.

- That is for weights and a loss function we have:

![alt text](https://github.com/nishchalnishant/Deep_learning_methods/blob/main/img/sgd_update.jpg?raw=true)

Where is a learning rate. SGD reduces redundancy compared to batch gradient descent - which recomputes gradients for similar examples before each parameter update - so it is usually much faster.

![alt text](https://github.com/nishchalnishant/Deep_learning_methods/blob/main/img/sgd_train.jpg?raw=true)

**Advantages of Stochastic Gradient Descent**

- It is easier to fit in the memory due to a single training example being processed by the network.
- It is computationally fast as only one sample is processed at a time.
- For larger datasets, it can converge faster as it causes updates to the parameters more frequently.
- Due to frequent updates, the steps taken towards the minima of the loss function have oscillations that can help to get out of the local minimums of the loss function (in case the computed position turns out to be the local minimum).

**Disadvantages of Stochastic Gradient Descent**

- Due to frequent updates, the steps taken towards the minima are very noisy. This can often lean the gradient descent into other directions.
- Also, due to noisy steps, it may take longer to achieve convergence to the minima of the loss function.
- Frequent updates are computationally expensive because of using all resources for processing one training sample at a time.
- It loses the advantage of vectorized operations as it deals with only a single example at a time.
