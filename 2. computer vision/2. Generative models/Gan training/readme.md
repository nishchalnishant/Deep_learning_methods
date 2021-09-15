Training obstacles associated with GAN training as well as several training techniques to improve GAN training for the generation of more realistic data .

> Problems with training GAN

- Gans are deeply hurt from un-stable training due to severeal challenges associated with GAN training.

- Nash equilibrium --

- - State where neither the discriminator nor the generator can improve their cost unilaterally.

- - Generator and discriminator train themselves simultaneously for nash equilibrium.

- - When both G and D update their cost function independently without any coordination , it is hard to achieve Nash-equilibrium. Thus GAN training becomes unstable.

- - Example -- let us assume there are two players A and B which manage the value x and y. Player A desires to minimize the value (xy) while B wants to maximize the value function: 𝑉(x, y) = xy

- - we solve above dunction, ∂xV(x,y) = 0 and ∂yV (x,y)= 0, we can determine that x = y = 0 has a saddle point (Nash-equilibrium).

- - For this, we update the parameter x and y based on the gradient descent of the value function V describes through the partial differential equations system:
    ∆x = α (Ã(Gƒ)/Ã(G)) and ∆y = −α\*(Ã(Gƒ)/Ã(ƒ))

- - By plotting x, y, and xy against the training iterations, we realize that our solution does not converge because after every gradient update causes massive fluctuation and instability becomes poor .

- Internal covariate shift

- - Occurs when the input distribution of network activation differes as a consequence of updating parameters in previous layer.

- - intermediate layer (hidden layers) try to learn to adapt the new distribution.

- - These learning parameters slow down the training of the model due to a change in learning rates.

- - Due to the updated learning rates, the model required much longer training time to counter these shifts.

- - The longer time automatically increases the training cost because the model reserved the resources in higher time.

- Mode collapse

- - Most crucial topic associated with GAN training, where the generator always produced an identical output .

- - MC is a common cause of failure where a generator demonstrates low diversity amongst data or generates only specific types of real samples, which limits the usefulness of learned GAN.

- - It can be of 2 types -- Partial type produces images with small diversity and Compiler type ( worst case senario) provides images of a single kind with no variety .

- - Instead of covering all possible modes at a time, the generator covers only one mode of the goal distribution.

- Vanashing gradient

- - the generator may fail to improve in producing good quality images.

- - VG is due to the gradients of the generator concerning
    weights in earlier layers of the networks becomes very small.

- - The discriminator (well-trained network) rejecting the generator generated samples with confidence due to VG.

- - Optimizing the generator may be hard for the reason that the discriminator is not sharing any information which harms the learning capacity of the models.

- Lack of proper evaluation metrics

- - Still difficult to evaluate which method(s) is better than other methods because there is no standard defined function for evaluation.

> Analysis of GAN training obstacles

> Techniques to improve GAN training

- Feature matching

- Unrolled GAN (UGAN)

- Mini-Batch discrimination

- Historical averaging

- Two time- scale update rule(TTUR)

- Hybrid model

- Self-Attention GAN

- Relativistic GAN

- One-sided label smoothing

- Sampling gan

- Proper optimizer

- Normalization
