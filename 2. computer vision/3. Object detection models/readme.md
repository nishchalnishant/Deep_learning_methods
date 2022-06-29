- One stage models

  - G-CNN
  - YOLO
  - SSD
  - YOLOv2
  - DSSD
  - DSOD

- Two stage models

  - R-CNN
  - SPP-net
  - Fast R-CNN
  - Faster R-CNN
  - R-FCN
  - FPN
  - Mask R-CNN

**Problems in Object detection**

- The goal of this detection technique is to determine where objects are located in a given image called object localisation and which category each object belongs to, which is called object classification.

- Object detection is the task of detecting instances of objects of a certain class within an image.

- The state-of-the-art methods can be categorized into two main types: one-stage methods and two stage-methods.

- One-stage methods prioritize inference speed, and example models include YOLO, SSD and RetinaNet.

- Two-stage methods prioritize detection accuracy, and example models include Faster R-CNN, Mask R-CNN and Cascade R-CNN.

- The most popular benchmark is the MSCOCO dataset. Models are typically evaluated according to a Mean Average Precision metric.

- Object detection is more tricky than classification.

- One of the problems you’ll encounter is that a training image can have anywhere from zero to dozens of objects in them, and the model may output more than one prediction, so how do you figure out which prediction should be compared to which ground-truth bounding box in the loss function?

- It’s common for object detection to predict too many bounding boxes. Each box also has a confidence score that says how likely the model thinks this box really contains an object.

https://analyticsindiamag.com/top-8-algorithms-for-object-detection/

https://neptune.ai/blog/object-detection-algorithms-and-libraries
