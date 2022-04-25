https://www.v7labs.com/blog/semantic-segmentation-guide

## Semantic segmentations

- Semantic Segmentation is a computer vision task that involves grouping together similar parts of the image that belong to the same class.

- Essentially, the task of Semantic Segmentation can be referred to as classifying a certain class of image and separating it from the rest of the image classes by overlaying it with a segmentation mask.

- Semantic Segmentation follows three steps:

> Classifying: Classifying a certain object in the image.
> Localizing: Finding the object and drawing a bounding box around it.
> Segmentation: Grouping the pixels in a localized image by creating a segmentation mask.

## Unet -- 2015

- U-Net is an architecture for semantic segmentation.
- It consists of a contracting path and an expansive path.
- The contracting path follows the typical architecture of a convolutional network.
- It consists of the repeated application of two 3x3 convolutions (unpadded convolutions), each followed by a rectified linear unit (ReLU) and a 2x2 max pooling operation with stride 2 for downsampling.
- At each downsampling step we double the number of feature channels.
- Every step in the expansive path consists of an upsampling of the feature map followed by a 2x2 convolution (“up-convolution”) that halves the number of feature channels, a concatenation with the correspondingly cropped feature map from the contracting path, and two 3x3 convolutions, each followed by a ReLU. The cropping is necessary due to the loss of border pixels in every convolution.
- At the final layer a 1x1 convolution is used to map each 64-component feature vector to the desired number of classes. In total the network has 23 convolutional layers.

# Segnet -- 2015

- SegNet is a semantic segmentation model.
- This core trainable segmentation architecture consists of an encoder network, a corresponding decoder network followed by a pixel-wise classification layer.
- The architecture of the encoder network is topologically identical to the 13 convolutional layers in the VGG16 network.
- The role of the decoder network is to map the low resolution encoder feature maps to full input resolution feature maps for pixel-wise classification.
- The novelty of SegNet lies is in the manner in which the decoder upsamples its lower resolution input feature maps.
- Specifically, the decoder uses pooling indices computed in the max-pooling step of the corresponding encoder to perform non-linear upsampling.

# Fcn -- 2016

- Fully Convolutional Networks, or FCNs, are an architecture used mainly for semantic segmentation.
- They employ solely locally connected layers, such as convolution, pooling and upsampling.
- Avoiding the use of dense layers means less parameters (making the networks faster to train).
- It also means an FCN can work for variable image sizes given all connections are local.
- The network consists of a downsampling path, used to extract and interpret the context, and an upsampling path, which allows for localization.
- FCNs also employ skip connections to recover the fine-grained spatial information lost in the downsampling path.

# Deeplabv3 -- 2017

- DeepLabv3 is a semantic segmentation architecture that improves upon DeepLabv2 with several modifications.
- To handle the problem of segmenting objects at multiple scales, modules are designed which employ atrous convolution in cascade or in parallel to capture multi-scale context by adopting multiple atrous rates.
- Furthermore, the Atrous Spatial Pyramid Pooling module from DeepLabv2 augmented with image-level features encoding global context and further boost performance.
- The changes to the ASSP module are that the authors apply global average pooling on the last feature map of the model, feed the resulting image-level features to a 1 × 1 convolution with 256 filters (and batch normalization), and then bilinearly upsample the feature to the desired spatial dimension.
- In the end, the improved ASPP consists of (a) one 1×1 convolution and three 3 × 3 convolutions with rates = (6, 12, 18) when output stride = 16 (all with 256 filters and batch normalization), and (b) the image-level features.
- Another interesting difference is that DenseCRF post-processing from DeepLabv2 is no longer needed.

> Defining a loss function

- Most common loss function for the task of image segmentation is pixel wise cross entropy loss.

- This loss examines each pixel individually , comparing the class predictions to our one hot encoded target vector.

- Because the cross entropy loss evaluates the class predictions for each pixel vector individually and then averages over all pixels, we're essentially asserting equal learning to each pixel in the image.

- Another popular loss function for image segmentation tasks is based on the Dice coefficient, which is essentially a measure of overlap between two samples.

- This measure ranges from 0 to 1 where a Dice coefficient of 1 denotes perfect and complete overlap.
