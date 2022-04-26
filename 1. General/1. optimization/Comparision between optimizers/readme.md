# How to choose optimizers ?

- If the data is sparse, use the self- applicable methods, namely Adagrad, Adadelta, RMSprop, Adam.

- RMSprop, Adadelta, Adam have similar effects in many cases.

- Adam just added bias- correction and momentum on the basis of RMSprop

- As the gradient becoms sparse, Adam performs better that RMSprop.

- But, overall Adam is the best choice.

- SGD is used in many papers, without momentum, etc. Although SGD can reach a minimum value, it takes longer than other algorithms and my be trapped in the saddle point.

- If faster convergence in needed or deeper and more complex neural network are trained, an adaptive algorithm is needed.

- RMSprop, Adadelta, Adam have similar effects in many cases.

- If the data is sparse, use methods, like Adagrad, Adadelta, RMSprop, Adam.

- Adam added momentum and learning rate on the basis of RMSprop.

- As the gradient becomes sparse, Adam will perform better than RMSprop.

- If we need faster convergence or for deeper and complex neural networks an adaptive algorithm is needed.
