## Regularization

- One of the most important aspects when training neural networks is avoiding overfitting.

- Overfitting refers to the phenomenon where a neural network models the training data very well but fails when it sees new data from the same problem domain.
- Overfitting is caused by noise in the training data that the neural network picks up during training and learns it as an underlying concept of the data.
- There are many ways to prevent overfitting the model , one such way is to use regularization.
- There are many techniques to perform regularization during model training , four of the most important are discussed below.

**L2 regularization**

- It is the most common type of all regularization technique and is also known as weight decay .
- For the L2 regularization we alter the Loss function and add an extra term to the loss function known as regularization term.
- In case of L2 regularization, we use the L2 norm of the weight matrices , which is the sum of square of weight matrix, then the regularization term is multiplied by alpha and divided by 2 leading to the final loss as

- Advantages of L2 over L1 norm

> Mathematical derivations of the L2 norm are easily computed. Therefore it is also easy to use gradient-based learning methods.

> L2 regularization optimizes the mean cost (whereas L1 reduces the median explanation) which is often used as a performance measurement. This is especially good if you know you don't have any outliers and you want to keep the overall error small.

> The solution is more likely to be unique. This ties in with the previous point: While the mean is a single value, the median might be located in an interval between two points and is therefore not unique.

> While L1 regularization can give you a sparse coefficient vector, the non-sparseness of L2 can improve your prediction performance (since you leverage more features instead of simply ignoring them).

> L2 is invariant under rotation. If you have a dataset consisting of points in a space and you apply a rotation, you still get the same results.

**L1 regularization**

- L1 regularization also known as Lasso regression is similar to the L2 regularization , but here insterad of using sum of suare of weight matrix we use the sum of weight matrix as the regularization term.
- Also in case of L1 we don't divide the regularization term by 2.
- All other process remains the same, resulting into the final loss function as

- Advantages of L1 over L2 norm

> The L1 norm prefers sparse coefficient vectors.
> This means the L1 norm performs feature selection and you can delete all features where the coefficient is 0.
> A reduction of the dimensions is useful in almost all cases.
> The L1 norm optimizes the median. Therefore the L1 norm is not sensitive to outliers.

**Dropout**

- In aqddition to the above discussed regularization methods , we also have another simple techniqu of dropout, where we define a probability P which is the probability of the neurons in a neural network layer getting turned off while training .
- For example if we declare P as 0.5 then half of the neurons in a layer get ramdomly turned off ( weights of such neurons are not updated during training)
- This is a simple yet effective dropout method.

- Advantages of the dropout layers

> The main advantage of this method is that it prevents all neurons in a layer from synchronously optimizing their weights.
> This adaptation, made in random groups, prevents all the neurons from converging to the same goal, thus decorrelating the weights.
