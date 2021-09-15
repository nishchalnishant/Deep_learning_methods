# About learning rate scheduling

- So far we primarily focused on optimization algorithms for how to update the weight vectors rather than on the rate at which they are being updated.

- one way of adjusting the learning rate is to explicitly at each step. We could adjust it downward after every epoch

- Nonetheless, adjusting the learning rate is often just as important as the actual algorithm.

- In addition to the actual algorithm there are number of aspects to consider

- - magnitute of learning rate
- - rate of decay
- - Initialization

- Linear warm up with linear decay
- Linear warmup with cosine annealing
- Stop decay
- Exponential decay
