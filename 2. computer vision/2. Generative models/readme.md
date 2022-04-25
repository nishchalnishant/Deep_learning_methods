> Generative models --

Model data generatively ( rather than discriminatively), i.e. they aim to approximate the probability distribution of the data.

Overall Generative model framework --

- We have dataset of observations x

- We assume that the observations have been generated according to some unknown distribution p_delta

- A generative model tries to mimic p_delta , if we achieve this goal , we can sample from p_model to generate observations that appear to have been drawn from p_delta

- Finally we are impressed if --

- - We can generate examples that appear to have been drawn from p_delta

- - We can generate examples that are suitably different from the observations in x [ model shouldn't reproduce what it has already seen]

**Restricted Boltzmann machine -- 1986**

- Restricted Boltzmann Machines, or RBMs, are two-layer generative neural networks that learn a probability distribution over the inputs.
- They are a special class of Boltzmann Machine in that they have a restricted number of connections between visible and hidden units.
- Every node in the visible layer is connected to every node in the hidden layer, but no nodes in the same group are connected.
- RBMs are usually trained using the contrastive divergence learning procedure

**Auto encoder -- 2006**

- An Autoencoder is a bottleneck architecture that turns a high-dimensional input into a latent low-dimensional code (encoder), and then performs a reconstruction of the input with this latent code (the decoder).

- There are several types of autoencoders , but for generative modelling variational autoencoders are used.

**Vae -- 2013**

- VAE stands for variational autoencoders.
- Standard and variational autoencoders learn to represent the input just in a compressed form called the latent space or the bottleneck.
- Variational autoencoders deal with specific topic and express their latent attributes as a probability distribution, leading to the formation of a continuous latent space that can be easily sampled and interpolated.
- When fed the same input, a variational autoencoder would construct latent attributes, The latent attributes are then sampled from the latent distribution formed and fed to the decoder, reconstructing the input.

https://www.v7labs.com/blog/autoencoders-guide#:~:text=An%20autoencoder%20is%20an%20unsupervised,even%20generation%20of%20image%20data.

**Gan -- 2014**

- A GAN, or Generative Adversarial Network, is a generative model that simultaneously trains two models: a generative model G that captures the data distribution, and a discriminative model D that estimates the probability that a sample came from the training data rather than .
- The training procedure for G is to maximize the probability of D making a mistake.
- This framework corresponds to a minimax two-player game.
- In the space of arbitrary functions G and D, a unique solution exists, with G recovering the training data distribution and D equal to 1/2 everywhere.
- In the case where G and D are defined by multilayer perceptrons, the entire system can be trained with backpropagation.

## Some other generative models are --

- Dcgan -- 2015
- Pix2pix-- 2016
- Cycle gan -- 2017
- Wgan -- 2017
- Style gan -- 2018
- Sagan -- 2018
- Bigggan -- 2018
- Glow -- 2018
- Style gan 2-- 2019
