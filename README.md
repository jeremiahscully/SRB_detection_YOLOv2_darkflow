# Solar Radio Burst Detection using YOLOv2 and Darkflow
This repository contains code for detecting solar radio bursts using YOLOv2 (You Only Look Once, version 2) implemented with Darkflow. YOLOv2 is a real-time object detection algorithm, and Darkflow is a TensorFlow implementation of YOLO.

# Requirements
- darkflow
- opencv-python
- tensorflow

Install the required packages using the following command:
```
pip install Cython
pip install git+https://github.com/thtrieu/darkflow.git
pip install opencv-python tensorflow
```
# Configuration
The YOLOv2 model is configured using the provided YOLO configuration file (yolov2_Type_III_2.cfg). Make sure to set the appropriate configuration parameters for your use case.

# Model Loading
The YOLOv2 model is loaded using Darkflow. The pre-trained weights are loaded from a checkpoint (step/epoch 40000) to perform solar radio burst detection.

# Detection
The code includes a session configuration for TensorFlow to enable GPU usage. The TFNet object is created with the specified options, including the YOLOv2 model configuration, pre-trained weights, detection threshold, and GPU usage.

# Image Processing
You can use the loaded model to perform solar radio burst detection on images or video frames. Simply input the images or frames to the TFNet object, and it will return the detected objects along with their bounding boxes.

Feel free to adapt the code to your specific needs, and experiment with different detection thresholds and model configurations for optimal performance in solar radio burst detection scenarios.
