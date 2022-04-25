## Skip connection blocks

- Skip Connection Blocks are building blocks for neural networks that feature skip connections.
- These skip connections 'skip' some layers allowing gradients to better flow through the network.
- Below you will find a list of commonly used skip connection blocks:

**Resudual block**
Residual Blocks are skip-connection blocks that learn residual functions with reference to the layer inputs, instead of learning unreferenced functions. They were introduced as part of the ResNet architecture.

Formally, denoting the desired underlying mapping as , we let the stacked nonlinear layers fit another mapping of . The original mapping is recast into . The acts like a residual, hence the name 'residual block'.

The intuition is that it is easier to optimize the residual mapping than to optimize the original, unreferenced mapping. To the extreme, if an identity mapping were optimal, it would be easier to push the residual to zero than to fit an identity mapping by a stack of nonlinear layers. Having skip connections allows the network to more easily learn identity-like mappings.

Note that in practice, Bottleneck Residual Blocks are used for deeper ResNets, such as ResNet-50 and ResNet-101, as these bottleneck blocks are less computationally intensive.

**Bottleneck Residual block**

- A Bottleneck Residual Block is a variant of the residual block that utilises 1x1 convolutions to create a bottleneck.
- The use of a bottleneck reduces the number of parameters and matrix multiplications.
- The idea is to make residual blocks as thin as possible to increase depth and have less parameters.
- They were introduced as part of the ResNet architecture, and are used as part of deeper ResNets such as ResNet-50 and ResNet-101.

**Dense block**

- A Dense Block is a module used in convolutional neural networks that connects all layers (with matching feature-map sizes) directly with each other.
- It was originally proposed as part of the DenseNet architecture.
- To preserve the feed-forward nature, each layer obtains additional inputs from all preceding layers and passes on its own feature-maps to all subsequent layers.
- In contrast to ResNets, we never combine features through summation before they are passed into a layer; instead, we combine features by concatenating them.
- Hence, the layer has inputs, consisting of the feature-maps of all preceding convolutional blocks.
- Its own feature-maps are passed on to all subsequent layers.
- This introduces connections in an -layer network, instead of just , as in traditional architectures: "dense connectivity".

**Inverted residual block**

- An Inverted Residual Block, sometimes called an MBConv Block, is a type of residual block used for image models that uses an inverted structure for efficiency reasons.
- It was originally proposed for the MobileNetV2 CNN architecture.
- It has since been reused for several mobile-optimized CNNs.
- A traditional Residual Block has a wide -> narrow -> wide structure with the number of channels.
- The input has a high number of channels, which are compressed with a 1x1 convolution.
- The number of channels is then increased again with a 1x1 convolution so input and output can be added.
- In contrast, an Inverted Residual Block follows a narrow -> wide -> narrow approach, hence the inversion. We first widen with a 1x1 convolution, then use a 3x3 depthwise convolution (which greatly reduces the number of parameters), then we use a 1x1 convolution to reduce the number of channels so input and output can be added.
