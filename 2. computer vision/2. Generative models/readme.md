> Generative models --

Model data generatively ( rather than discriminatively), i.e. they aim to approximate the probability distribution of the data.

Overall Generative model framework --

- We have dataset of observations x

- We assume that the observations have been generated according to some unknown distribution p_delta

- A generative model tries to mimic p_delta , if we achieve this goal , we can sample from p_model to generate observations that appear to have been drawn from p_delta

- Finally we are impressed if --

- - We can generate examples that appear to have been drawn from p_delta

- - We can generate examples that are suitably different from the observations in x [ model shouldn't reproduce what it has already seen]

- Restricted Boltzmann machine -- 1986
- Auto encoder -- 2006
- Denoising autoencoder -- 2008
- Vae -- 2013
- Gan -- 2014
- Dcgan -- 2015
- Pix2pix-- 2016
- Cycle gan -- 2017
- Wgan -- 2017
- Style gan -- 2018
- Sagan -- 2018
- Bigggan -- 2018
- Glow -- 2018
- Style gan 2-- 2019
