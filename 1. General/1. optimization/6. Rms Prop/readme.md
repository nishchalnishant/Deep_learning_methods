## RMSProp

- The full name of RMSProp algorithm is called **Root Mean Square Prop**, which is an adaptive learning rate optimization algorithm proposed by Geoff Hinton.

- RMSProp tries to resolve Adagrad’s radically diminishing learning rates by using a moving average of the squared gradient.

- It utilizes the magnitude of the recent gradient descents to normalize the gradient.

- Adagrad will accumulate all previous gradient squares, and RMSprop just calculates the corresponding average value, so it can alleviate the problem that the learning rate of the Adagrad algorithm drops quickly.

- The difference is that RMSProp calculates the **differential squared weighted average of the gradient** .

- This method is beneficial to eliminate the direction of large swing amplitude, and is used to correct the swing amplitude, so that the swing amplitude in each dimension is smaller. On the other hand, it also makes the network function converge faster.

- In RMSProp learning rate gets adjusted automatically and it chooses a different learning rate for each parameter.

- RMSProp divides the learning rate by the average of the exponential decay of squared gradients
