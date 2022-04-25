## SSD

Single Shot Detector (SSD) is a method for detecting objects in images using a single deep neural network. The SSD approach discretises the output space of bounding boxes into a set of default boxes over different aspect ratios. After discretising, the method scales per feature map location. The Single Shot Detector network combines predictions from multiple feature maps with different resolutions to naturally handle objects of various sizes.

**Advantages of SSD**

SSD completely eliminates proposal generation and subsequent pixel or feature resampling stages and encapsulates all computation in a single network.
Easy to train and straightforward to integrate into systems that require a detection component.
SSD has competitive accuracy to methods that utilise an additional object proposal step, and it is much faster while providing a unified framework for both training and inference.

## YOLO

You Only Look Once or YOLO is one of the popular algorithms in object detection used by researchers around the globe. According to the researchers at Facebook AI Research, the unified architecture of YOLO is extremely fast in manner. The base YOLO model processes images in real-time at 45 frames per second, while the smaller version of the network, Fast YOLO processes an astounding 155 frames per second while still achieving double the mAP of other real-time detectors. This algorithm outperforms the other detection methods, including DPM and R-CNN, when generalising from natural images to other domains like artwork.
