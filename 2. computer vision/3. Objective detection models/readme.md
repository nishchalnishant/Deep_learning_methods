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

> Problems in Object detection

Object detection is more tricky than classification.

One of the problems you’ll encounter is that a training image can have anywhere from zero to dozens of objects in them, and the model may output more than one prediction, so how do you figure out which prediction should be compared to which ground-truth bounding box in the loss function?

It’s common for object detection to predict too many bounding boxes. Each box also has a confidence score that says how likely the model thinks this box really contains an object.
