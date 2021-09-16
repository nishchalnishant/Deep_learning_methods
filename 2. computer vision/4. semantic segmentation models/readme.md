> Semantic segmentations

Image segmentation is a computer vision task in which we label specific regions of an image according to what's being shown.

# Unet -- 2015

# Segnet -- 2015

# Fcn -- 2016

# Deeplabv3 -- 2017

# Espnet -- 2018

> Defining a loss function

- Most common loss function for the task of image segmentation is pixel wise cross entropy loss.

- This loss examines each pixel individually , comparing the class predictions to our one hot encoded target vector.

- Because the cross entropy loss evaluates the class predictions for each pixel vector individually and then averages over all pixels, we're essentially asserting equal learning to each pixel in the image.

- Another popular loss function for image segmentation tasks is based on the Dice coefficient, which is essentially a measure of overlap between two samples.

- This measure ranges from 0 to 1 where a Dice coefficient of 1 denotes perfect and complete overlap.
