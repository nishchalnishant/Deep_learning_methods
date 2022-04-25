## Normalization

- Normalization is an approach which is applied during the preparation of data in order to change the values of numeric columns in a dataset to use a common scale when the features in the data have different ranges.

- Suppose an input dataset contains data in one column with values ranging from 0 to 10 and the other column with values ranging from 100,000 to 10,00,000. In this case, the input data contains a big difference in the scale of the numbers which will eventually occur as errors while combining the values as features during modelling. These issues can be mitigated by normalization by creating new values and maintaining the general or normal distribution in the data.

**Batch Normalization**

- Batch normalization, it is a process to make neural networks faster and more stable through adding extra layers in a deep neural network.
- The new layer performs the standardizing and normalizing operations on the input of a layer coming from a previous layer.

- But we call this process as batch becauce the normalizing process in batch normalization takes place in batches, not as a single input.

- Advantages of Batch Normalization

> Speed Up the Training By Normalizing the hidden layer activation the Batch normalization speeds up the training process.

> Handles internal covariate shift It solves the problem of internal covariate shift.Through this, we ensure that the input for every layer is distributed around the same mean and standard deviation.

> Internal covariate shift Suppose we are training an image classification model, that classifies the images into Dog or Not Dog.

> Smoothens the Loss Function Batch normalization smoothens the loss function that in turn by optimizing the model parameters improves the training speed of the model.

**Weight Normalization**

- Weight normalization is a process of reparameterization of the weight vectors in a deep neural network which works by decoupling the length of those weight vectors from their direction.
- In simple terms, we can define weight normalization as a method for improving the optimisability of the weights of a neural

- The advantages of weight normalization are mentioned below

> Weight normalization improves the conditioning of the optimisation problem as well as speed up the convergence of stochastic gradient descent.
> It can be applied successfully to recurrent models such as LSTMs as well as in deep reinforcement learning or generative models

**Layer normalization**

- Layer normalization is a method to improve the training speed for various neural network models.

- Unlike batch normalization, this method directly estimates the normalisation statistics from the summed inputs to the neurons within a hidden layer.

- Layer normalization is basically designed to overcome the drawbacks of batch normalization such as dependent on mini batches, etc.

- The advantages of layer normalization are mentioned below:

> Layer normalization can be easily applied to recurrent neural networks by computing the normalization statistics separately at each time step

> This approach is effective at stabilising the hidden state dynamics in recurrent networks

**Instance normalization**

- Instance normalization, also known as contrast normalization is almost similar to layer normalization.
- Unlike batch normalization, instance normalization is applied to a whole batch of images instead for a single one.

- The advantages of instance normalization are mentioned below

> This normalization simplifies the learning process of a model.
> The instance normalization can be applied at test time.

**Group normalization**

- Group normalization can be said as an alternative to batch normalization.
- This approach works by dividing the channels into groups and computes within each group the mean and variance for normalization i.e. normalising the features within each group.
- Unlike batch normalization, group normalization is independent of batch sizes, and also its accuracy is stable in a wide range of batch sizes.

- The advantages of group normalization are mentioned below:

> It has the ability to replace batch normalization in a number of deep learning tasks
> It can be easily implemented in modern libraries with just a few lines of codes
