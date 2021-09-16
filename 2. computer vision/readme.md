> Covers computer vision topics covering deep learning

# Image models

methods that build representations of images for downstream tasks such as classification and object detection.

There are multiple stages in these models such as feature extraction stages ,combination of those features etc .

- Le-net -- 1998
- Alex net - 2012
- Vgg -- 2014
- Google-net -- 2014
- Resnet -- 2015
- Inception v3 -- 2015
- Dense net -- 2016
- Mobile net v1,v2,v3 -- 2018
- Dark net -53 -- 2018
- Efficient net v0-v7 --2018

# Generative models

A generative model includes the distribution of the data itself, and tells you how likely a given example is.

For example, models that predict the next word in a sequence are typically generative models (usually much simpler than GANs) because they can assign a probability to a sequence of words.

while A discriminative model ignores the question of whether a given instance is likely, and just tells you how likely a label is to apply to the instance.

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

# Object detection models

architecture used to perform the task of object detection [ classification + localization ]

A natural choice to scan the whole image with a multi-scale sliding window, but it is computationally very expensive and produces too amny redundant windows.

> One stage models

requires only a single pass through the neural network and predicts all the bounding boxes in one go.

Make a fixed number of predictions on grid.

Usually have faster inference (at the cost of performance ) than two stage models.

- G-CNN
- YOLO
- SSD
- YOLOv2
- DSSD
- DSOD

> Two stage models

One follows traditional object detection pipeline, generating region proposals at first and then classifying each proposal into different object categories

Similar to human brain , so it gives a coarse scan of whole scenario firstly and then focuses on region of interest.

It inserts cnn into sliding windows method which predicts bounding box directly from location of the topmost feature map after obtaining the confidences of underlying object categories .

- R-CNN
- SPP-net
- Fast R-CNN
- Faster R-CNN
- R-FCN
- FPN
- Mask R-CNN

# Semantic segmentation

Class of methods that address the task of semantically segmenting an image into different object classes.

Goal of semantic image segmentation is to label each pixel of an image with a corresponding class of what is being represented.

As we are predicting for each pixel in the image the task is refered to as dense prediction.

Useful in Autonomous vehicles , Medical image diagnostics etc.

- Unet -- 2015
- Segnet -- 2015
- Fcn -- 2016
- Deeplabv3 -- 2017
- Espnet -- 2018

# Image augmentation

Refers to a class of methods that augment an image dataset to increase the effective size of the training set , or as a form of regularization to help network learn more effective representations.

Used when we have imbalance set of data in training module.

- Random resized crop -- 2000
- Random horizontal flip -- 2000
- Colour jitter --- 2000
- Random gaussian blur -- 2000
- Random scaling -- 2000
- Image scale augmentation -- 2000
- Mixup -- 2017
- Cutout-- 2017
- Autoaugment -- 2018
- Cutmix -- 2019
- Randaugment -- 2019
