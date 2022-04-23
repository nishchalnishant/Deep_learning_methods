# About Optimization techniques --

# Scholastic gradient discent

- Objective function is usually the average of the loss function for each example in the training dataset.

- For an objective function f(x) , we can find the gradient of the function .

- If gradient descent is used the computational cost for each independent variable iteration is O(n), which grows linearly with n.

- If we have the larger training dataset cost of gradient descent for each iteration will be higher , thus when the training dataset is larger , the cost of gradient descent for each iteration will be higher .

- SGD reduces the computational cost at each iteration.

- At each iteration of SGD , we uniformly sample an index for data samples at random, and compute the gradient to update x.

![alt text](https://github.com/nishchalnishant/Deep_learning_methods/blob/main/img/sgd.png?raw=true)

# Mini batch stochastic gradient descent

- We can iterate over complete data and update the weights at once or we can iterate over one sample at once each of them has their drawbacks.

- SGD is not computationally efficient as CPUs and GPUs cannot exploit the full power vectorization.

- In case of mini batch SGD we read minibatches of data rather that single observations to update the parameters.

![alt text](https://github.com/nishchalnishant/Deep_learning_methods/blob/main/img/mini_batch.png?raw=true)

# Adagrad --

- Adagrad decreases the learning rate dynamically on a per-coordinate basis.

- It uses the magnitude of the gradient as a means of adjusting how quickly progress is achieved - coordinates with large gradients are compensated with a smaller learning rate.

- Computing the exact second derivative is typically infeasible in deep learning problems due to memory and computational constraints. The gradient can be a useful proxy.

- If the optimization problem has a rather uneven structure Adagrad can help mitigate the distortion.

- Adagrad is particularly effective for sparse features where the learning rate needs to decrease more slowly for infrequently occurring terms.

- On deep learning problems Adagrad can sometimes be too aggressive in reducing learning rates.

# Ada delta

- Adadelta has no learning rate parameter. Instead, it uses the rate of change in the parameters itself to adapt the learning rate.

- Adadelta requires two state variables to store the second moments of gradient and the change in parameters.

- Adadelta uses leaky averages to keep a running estimate of the appropriate statistics.

# Adam

- Adam combines features of many optimization algorithms into a fairly robust update rule.

- Created on the basis of RMSProp, Adam also uses EWMA on the minibatch stochastic gradient.

- Adam uses bias correction to adjust for a slow startup when estimating momentum and a second moment.

- For gradients with significant variance we may encounter issues with convergence.

- They can be amended by using larger minibatches or by switching to an improved estimate for st . Yogi offers such an alternative.

# Rms prop

- RMSProp is very similar to Adagrad insofar as both use the square of the gradient to scale coefficients.

- RMSProp shares with momentum the leaky averaging. However, RMSProp uses the technique to adjust the coefficient-wise preconditioner.

- The learning rate needs to be scheduled by the experimenter in practice.

- The coefficient γ determines how long the history is when adjusting the per-coordinate scale.

# Scholastic gradient discent with momentum

- For noisy gradients we need to be extra cautious when it comes to choosing the learning rate in the face of noise. If we decrease it too rapidly, convergence stalls.

- Momentum is an extension to the gradient descent optimization algorithm that allows the search to build inertia in a direction in the search space and overcome the oscillations of noisy gradients and coast across flat spots of the search space.

- If we are too lenient, we fail to converge to a good enough solution since noise keeps on driving us away from optimality.

- Earlier we fixed the learning rate thuse we had same learning rate initially ( when we can take longer steps ) and at the end ( when we need to take small steps till we reach local minima ).

- We add a term called Beta multiplied with the previous update to the initial gradient g(t) .
  thus , vt ← βvt − 1 + gt,t−1

- if we look at it and put beta as 0 we get the regular gradient descent.
