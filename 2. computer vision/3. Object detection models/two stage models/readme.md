## R-CNN

- The Region-based Convolutional Network method (RCNN) is a combination of region proposals with Convolution Neural Networks (CNNs).
- R-CNN helps in localising objects with a deep network and training a high-capacity model with only a small quantity of annotated detection data.
- It achieves excellent object detection accuracy by using a deep ConvNet to classify object proposals.
- R-CNN has the capability to scale to thousands of object classes without resorting to approximate techniques, including hashing.

## Fast R-CNN

- Written in Python and C++ (Caffe), Fast Region-Based Convolutional Network method or Fast R-CNN is a training algorithm for object detection.
- This algorithm mainly fixes the disadvantages of R-CNN and SPPnet, while improving on their speed and accuracy.

**Advantages of Fast R-CNN: –**

- Higher detection quality (mAP) than R-CNN, SPPnet
- Training is single-stage, using a multi-task loss
- Training can update all network layersNo disk storage is required for feature caching

## Faster R-CNN

- Faster R-CNN is an object detection algorithm that is similar to R-CNN.
- This algorithm utilises the Region Proposal Network (RPN) that shares full-image convolutional features with the detection network in a cost-effective manner than R-CNN and Fast R-CNN.
- A Region Proposal Network is basically a fully convolutional network that simultaneously predicts the object bounds as well as objectness scores at each position of the object and is trained end-to-end to generate high-quality region proposals, which are then used by Fast R-CNN for detection of objects.

## R-FCN

Region-based Fully Convolutional Networks or R-FCN is a region-based detector for object detection. Unlike other region-based detectors that apply a costly per-region subnetwork such as Fast R-CNN or Faster R-CNN, this region-based detector is fully convolutional with almost all computation shared on the entire image.

R-FCN consists of shared, fully convolutional architectures as is the case of FCN that is known to yield a better result than the Faster R-CNN. In this algorithm, all learnable weight layers are convolutional and are designed to classify the ROIs into object categories and backgrounds.

- FPN
- Mask R-CNN
