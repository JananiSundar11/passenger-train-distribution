# passenger-train-distribution

People Counter Project - Setup Guide

1. Install Required Dependencies

This project requires Python and the following libraries:

Required Python Libraries

opencv-python - OpenCV is used for image processing and object detection.
numpy - Numpy is used for numerical computations.
Optional (For Headless Systems or GPUs)

opencv-python-headless (Use this instead of opencv-python for servers or systems without a GUI)
Installation Steps

Step 1: Install Python

Ensure you have Python installed on your system. You can download it from Python's official website.

Step 2: Install Required Packages

Run the following command in your terminal or command prompt:

pip install opencv-python numpy
For a headless environment, use:

pip install opencv-python-headless numpy
Step 3: Verify Installation

To confirm that OpenCV and NumPy are installed, run:

python -c "import cv2; import numpy; print('Setup successful!')"
If you see "Setup successful!", your installation is complete.

2. Running the Project

Ensure all dependencies are installed.
Place the following required files in the project folder:
yolov3.weights (YOLO model weights)
yolov3.cfg (YOLO model configuration file)
coco.names (Class labels file)
train.png (Input image for detection)
Run the script:
python people_counter.py
The processed image will be saved as output_image.png.
3. Troubleshooting

ModuleNotFoundError: No module named 'cv2'
Run pip install opencv-python again.
FileNotFoundError: Image not found at path 'train.png'
Ensure the image file exists in the same directory as the script.
Error loading YOLO files
Make sure yolov3.weights and yolov3.cfg are in the correct location.
4. Additional Notes

This script uses the YOLOv3 model for object detection.
Make sure your Python version is 3.7 or higher for best compatibility.
