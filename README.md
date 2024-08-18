# Real-Time-Object-Detection-with-OpenCV-




Real-Time Object Detection with OpenCV and SSD MobileNet







This project implements a real-time object detection system using OpenCV and the SSD MobileNet model. The system captures video from a webcam, detects various objects in the video feed, and displays bounding boxes with labels around the detected objects. The project uses a pre-trained SSD MobileNet model, which is capable of recognizing objects from the COCO dataset.

Features
Real-Time Object Detection: Detects objects in a live video feed in real-time.
COCO Dataset Support: Recognizes objects based on the COCO dataset, which includes 80 common objects such as persons, cars, chairs, etc.
Color-Coded Bounding Boxes: Each detected object is highlighted with a uniquely colored bounding box.
Customizable Detection Threshold: Allows setting a confidence threshold for detection to reduce false positives.
Requirements
Python 3.x
OpenCV 4.x (opencv-python package)
Pre-trained SSD MobileNet model files (ssd_mobilenet_v3_large_coco_2020_01_14.pbtxt, frozen_inference_graph.pb)
COCO class names file (coco.names)
Installation
To set up this project, follow these steps:

Install Required Python Packages:

Install the necessary Python packages using pip:

bash
Copy code
pip install opencv-python
Download the Pre-trained Model Files:

Ensure you have the following files in the Object Detection directory:

ssd_mobilenet_v3_large_coco_2020_01_14.pbtxt
frozen_inference_graph.pb
coco.names
You can find these files from the official TensorFlow Model Zoo or other sources online.

Usage
Run the Object Detection Script:

Execute the objectDetection.py script to start the object detection system:


























bash
Copy code
python objectDetection.py
Quit the Application:

Press q on the keyboard to exit the application and close the video feed.

How It Works
Loading Class Names: Loads the class names from the coco.names file, which represents the 80 object categories in the COCO dataset.
Model Initialization: Initializes the SSD MobileNet model using the provided configuration and weight files.
Video Capture: Captures video from the default webcam.
Object Detection: Processes each frame to detect objects, drawing bounding boxes and labeling them with the detected object's class name and confidence score.
Display Results: Displays the processed video feed with detected objects highlighted.
File Descriptions
objectDetection.py: The main Python script that runs the real-time object detection using OpenCV.
ssd_mobilenet_v3_large_coco_2020_01_14.pbtxt: The configuration file for the SSD MobileNet model.
frozen_inference_graph.pb: The pre-trained model weights for the SSD MobileNet.
coco.names: A text file containing the class names from the COCO dataset.
Contributing
Contributions to improve the project are welcome. Please fork the repository and submit a pull request with your changes.
