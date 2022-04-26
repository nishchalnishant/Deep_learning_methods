**About**

- AdaGrad is a stochastic optimization method that adapts the learning rate to the parameters.

- It performs smaller updates for parameters associated with frequently occurring features, and larger updates for parameters associated with infrequently occurring features.

- In its update rule, Adagrad modifies the general learning rate at each time step for every parameter based on the past gradients

**Advantages**

- The benefit of AdaGrad is that it eliminates the need to manually tune the learning rate; most leave it at a default value of .

**Disadvantages**

- Its main weakness is the accumulation of the squared gradients in the denominator.
- Since every added term is positive, the accumulated sum keeps growing during training, causing the learning rate to shrink and becoming infinitesimally small.
