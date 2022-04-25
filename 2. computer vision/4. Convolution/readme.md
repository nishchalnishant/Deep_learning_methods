## Convolutions

- Convolutions are a type of operation that can be used to learn representations from images.
- They involve a learnable kernel sliding over the image and performing element-wise multiplication with the input.
- The specification allows for parameter sharing and translation invariance.
- A convolution is a type of matrix operation, consisting of a kernel, a small matrix of weights, that slides over input data performing element-wise multiplication with the part of the input it is on, then summing the results into an output.
- Intuitively, a convolution allows for weight sharing - reducing the number of effective parameters - and image translation (allowing for the same feature to be detected in different parts of the input space).

## Terms related to convolutions

**Kernel Size**

- The kernel size defines the field of view of the convolution.
- A common choice for 2D is 3 — that is 3x3 pixels.

**Stride**

- The stride defines the step size of the kernel when traversing the image. - While its default is usually 1, we can use a stride of 2 for downsampling an image similar to MaxPooling.

**Padding**

- The padding defines how the border of a sample is handled.
- A (half) padded convolution will keep the spatial output dimensions equal to the input, whereas unpadded convolutions will crop away some of the borders if the kernel is larger than 1.

**Input & Output Channels**

- A convolutional layer takes a certain number of input channels (I) and calculates a specific number of output channels (O).
- The needed parameters for such a layer can be calculated by I*O*K, where K equals the number of values in the kernel.
