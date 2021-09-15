> Covers general topics covering deep learning

# optimization

For a deep learning problem, we usually define a loss function first. Once we have a loss function, we can use a optimization algorithm in an attempt to minimize the loss.

By tradition most optimization algorithm are concerned with minimization , but if we ever need to maximize an objective we just flip the sign on the objective.

- Scholastic gradient discent
- Rms prop
- Adam
- Scholastic gradient discent with momentum

# Skip Connection blocks

while training deep NN , ther performance of model drops down with the increase in depth of the artitecture, there can be many reson for the same .

One of them is can be because of Vanashing or exploding gradients but these can be taken care by using Batch Normalization and proper initialization of weights through normalization.

But above solution doesnt works for deeper network and this is because of inability of deeper layer to learn even identity mappings.

For the same comes the skip connections.

- Residual block
- Bottleneck residual block
- Dense block
- Inverted residual block

# Attention

Attention models , or attention mechanisms, are input processing techniques for neural networks that allows the network to focus on specific aspects of a complex input, one at a time until the entire dataset is categorized.

Goal is to break down complicated tasks into smaller areas of attention that are processed sequentially.

- self attention
- Additive attension
- Multi head attention
- Scaled dot product attention

# Stochastic optimization

Stochastic optimization refers to a collection of methods for minimizing or maximizing an objective function when randomness is present.

Stochastic optimization algorithms provide an alternative approach that permits less optimal local decisions to be made within the search procedure that may increase the probability of the procedure locating the global optima of the objective function.

- Sgd
- Sgd with momentum
- Ada Grad
- Ada delta
- Rms prop

# Regularization

Technique used for tuning the function by adding an additional penalty term in the error function.

The additional term controls the excessively fluctuating function such that coefficients don't take extreme values.

- Weight decay
- Label smoothing
- L1 regularization
- Early stopping
- Dropout
- Entropy regularization
- Attention dropout

# Activation function

Most of the activation function belongs to the similar families i.e. has some differences between them

Used to add the non linearity in the NN as a NN without an activation function is essentially just a linear regression model.

- ReLU
- Sigmoid activation
- Tanh
- Softplus
- Leaky ReLU
- P ReLU
- Swish

# Normalization

Normalization is an approach which is applied during the preparation of data in order to change the values of numeric columns in a dataset to use a common scale when the features in the data have different ranges.

- Batch Normalization
- Weight normalization
- Layer normalization
- Instance normalization
- Group normalization

# Loss functions

loss function is the function that computes the distance between the current output of the algorithm and the expected output.

Method to evaluate how your algorithm models the data.

Based on the kind of probelm [ classification or regression ] , loss can be classification or regression loss.

In addition to the custom made loss functions we can also make our own custom loss function.

- Ctc loss
- Gan least squares loss
- Cycle consistency loss
- Focal loss
- Triplet loss

# Learning rate schedules

Adapting the learning rate for your stochastic gradient descent optimization procedure can increase performance and reduce training time.

- Linear warm up with linear decay
- Linear warmup with cosine annealing
- Stop decay
- Exponential decay

# Feed forward networks

A Feed Forward Neural Network is an artificial neural network in which the connections between nodes does not form a cycle.

- Dense connections
- Feed forward network
- linear layer
- highway newtork
