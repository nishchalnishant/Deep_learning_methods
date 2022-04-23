# About

- There are three problems with the Adagrad algorithm

- - The learning rate is monotonically decreasing.
- - The learning rate in the late training period is very small.
- - It requires manually setting a global initial learning rate.

- AdaDelta is a stochastic optimization technique that allows for per-dimension learning rate method for SGD.
- It is an extension of Adagrad that seeks to reduce its aggressive, monotonically decreasing learning rate.
- Instead of accumulating all past squared gradients,
- Adadelta restricts the window of accumulated past gradients to a fixed size w.
- Instead of inefficiently storing previous squared gradients, the sum of gradients is recursively defined as a decaying average of all past squared gradients.
- The running average at time step then depends only on the previous average and current gradient:

The main advantage of AdaDelta is that we do not need to set a default learning rate.
