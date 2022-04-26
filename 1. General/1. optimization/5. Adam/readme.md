## Adam

- Adaptive Moment Estimation (Adam) is another method that computes adaptive learning rates for each parameter.
- In addition to storing an exponentially decaying average of past squared gradients like Adadelta and RMSprop.
- Adam also keeps an exponentially decaying average of past gradients, similar to momentum.
- Adam can be viewed as a combination of Adagrad and RMSprop,(Adagrad) which works well on sparse gradients and (RMSProp) which works well in online and nonstationary settings repectively.
- Adam implements the exponential moving average of the gradients to scale the learning rate instead of a simple average as in Adagrad.
- It keeps an exponentially decaying average of past gradients.
- Adam is computationally efficient and has very less memory requirement.
- Adam optimizer is one of the most popular and famous gradient descent optimization algorithms.

## Advantages of ADAM

- Adam implements the exponential moving average of the gradients to scale the learning rate instead of a simple average as in Adagrad.

- Adam is computationally efficient and has very less memory requirement.

- Adam is so far the best optimizer that is known.
