## Loss functions

- Loss Functions are used to frame the problem to be optimized within deep learning.

**L1 and L2 loss**

- L1 and L2 are two common loss functions in machine learning which are mainly used to minimize the error.
- L1 loss function are also known as Least Absolute Deviations in short LAD while L2 loss function are also known as Least square errors in short LS.
- L1 loss is used to minimize the error which is the sum of all the absolute differences in between the true value and the predicted value.
- L2 loss is also used to minimize the error which is the sum of all the squared differences in between the true value and the pedicted value.
- The disadvantage of the L2 norm is that when there are outliers, these points will account for the main component of the loss. For example, the true value is 1, the prediction is 10 times, the prediction value is 1000 once, and the prediction value of the other times is about 1, obviously the loss value is mainly dominated by 1000.

**Huber Loss**

- Huber Loss is often used in regression problems. Compared with L2 loss, Huber Loss is less sensitive to outliers(because if the residual is too large, it is a piecewise function, loss is a linear function of the residual).
- Among them, $\delta$ is a set parameter, $y$ represents the real value, and $f(x)$ represents the predicted value.
- The advantage of this is that when the residual is small, the loss function is L2 norm, and when the residual is large, it is a linear function of L1 norm.
- A smooth approximation of Huber loss to ensure that each order is differentiable.
- Where $\delta$ is the set parameter, the larger the value, the steeper the linear part on both sides.

**Hinge Loss**

- Hinge loss is often used for binary classification problems, such as ground true: t = 1 or -1, predicted value y = wx + b

**Cross- entropy loss**

- The above is mainly to say that cross-entropy loss is mainly applied to binary classification problems. The predicted value is a probability value and the loss is defined according to the cross entropy. Note the value range of the above value: the predicted value of y should be a probability and the value range is [0,1]

**Sigmoid Cross entropy Loss**

- The above cross-entropy loss requires that the predicted value is a probability. Generally, we calculate $scores = x*w + b$. Entering this value into the sigmoid function can compress the value range to (0,1).
- It can be seen that the sigmoid function smoothes the predicted value(such as directly inputting 0.1 and 0.01 and inputting 0.1, 0.01 sigmoid and then entering, the latter will obviously have a much smaller change value), which makes the predicted value of sigmoid-ce far from the label loss growth is not so steep.

**Softmax cross-entropy loss**

- First, the softmax function can convert a set of fraction vectors into corresponding probability vectors. Here is the definition of softmax function.
- As above, softmax also implements a vector of 'squashes' k-dimensional real value to the [0,1] range of k-dimensional, while ensuring that the cumulative sum is 1.
- According to the definition of cross entropy, probability is required as input.
- Sigmoid-cross-entropy-loss uses sigmoid to convert the score vector into a probability vector, and softmax-cross-entropy-loss uses a softmax function to convert the score vector into a probability vector.
- According to the definition of cross entropy loss.
- where $p(x)$ represents the probability that classification $x$ is a correct classification, and the value of $p$ can only be 0 or 1. This is the prior value $q(x)$ is the prediction probability that the $x$ category is a correct classification, and the value range is (0,1)
- So specific to a classification problem with a total of C types, then $p(x_j)$, $(0 <_{=} j <_{=} C)$ must be only 1 and C-1 is 0(because there can be only one correct classification, correct the probability of classification as correct classification is 1, and the probability of the remaining classification as correct classification is 0)
- Then the definition of softmax-cross-entropy-loss can be derived naturally.
