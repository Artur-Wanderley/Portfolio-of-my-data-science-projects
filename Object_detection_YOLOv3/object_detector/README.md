
# Accenture's AI Challenge¶
## Implement a module for Accenture logo recognition in an image
##Introduction
The code below implements an object detector for the Accenture logo.
The object detector was built using the yolov3 model;
Yolo stdands for "you look only once". The yolov3 is a state-of-the-art deep learning model for object detection;
The Accenture logo object detector was built on top of pretrained weights (transfer learning) for the coco dataset;
Both the yolov3 model and the pretrained weights where implemented using the darknet neural network framework.
I chose the darknet framework to implement yolov3 because it is easy and fast to install. In addition, darknet supports both CPU and GPU computation.
