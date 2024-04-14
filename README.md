# Object_Detection_YOLO_V8
This is the Model in which you just need to install requirements.txt and then RUN the code, 
Object Detection using YOLOv8n
This Python script allows you to perform real-time object detection using the YOLOv8n model. It uses the ultralytics library for YOLO and OpenCV for video capturing and visualization.

Prerequisites
Python 3.6 or later
ultralytics library (install using pip install ultralytics)
OpenCV library (install using pip install opencv-python)
Setup
Clone the repository or download the required files:

bash
Copy code
git clone <repository-url>
cd <repository-folder>
Download the YOLOv8n model weights:

The script expects the YOLOv8n model weights file to be present in the weights directory with the name yolov8n.pt.
You can obtain the YOLOv8n model weights file from the ultralytics repository or other sources.
Create the class list file:

The script requires a text file containing the list of class names that the YOLO model can detect.
Create a text file named coco.txt inside the utils directory, and add each class name on a new line.
Usage
Open a terminal or command prompt and navigate to the script directory.

Run the object detection script with a webcam feed:

Copy code
python object_detection.py
If you want to use a video file for detection, you can modify the cap variable inside the script with the file path of your video.

During runtime, a window will open displaying the live webcam feed with detected objects highlighted and labeled.

Press the 'q' key to exit the detection mode and terminate the script.

Configuration
You can adjust the confidence threshold for detections by changing the conf value inside the script. Lower the value to detect objects with lower confidence scores.

The script resizes the video frames to optimize the runtime. If you want to use the original frame size, uncomment the line that resizes the frame.

Notes
Make sure you have the necessary dependencies installed before running the script (Python 3.6+, ultralytics, OpenCV).

The script is based on the YOLOv8n model, and the performance may vary depending on the hardware and model weights used.

You can customize the colors used for bounding boxes by modifying the detection_colors list inside the script.

The requirements.txt file in this repository lists the required dependencies. You can install them using pip install -r requirements.txt.
