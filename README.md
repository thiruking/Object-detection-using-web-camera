# YOLOv4 Real-Time Object Detection Using OpenCV

## Overview

This project implements real-time object detection using the YOLOv4 (You Only Look Once Version 4) algorithm with OpenCV and Python. The system captures video from a webcam, detects objects in real time, and displays bounding boxes with class labels and confidence scores.

## Features

- Real-time object detection using webcam input
- YOLOv4 deep learning model
- Support for 80 object classes from the COCO dataset
- Bounding box visualization
- Confidence score display
- Non-Maximum Suppression (NMS) for removing duplicate detections

## Project Structure

```text
YOLOv4-Object-Detection/
│
├── yolov4.weights
├── yolov4.cfg
├── coco.names
├── object_detection.py
└── README.md
```

## Requirements

The following software and libraries are required:

- Python 3.x
- OpenCV
- NumPy
- Matplotlib
- IPython

Install the required packages:

```bash
pip install opencv-python
pip install numpy
pip install matplotlib
pip install ipython
```

## Required Files

Download and place the following files in the project directory:

### YOLOv4 Weights

- `yolov4.weights`

### YOLOv4 Configuration

- `yolov4.cfg`

### COCO Class Labels

- `coco.names`

## How to Run

1. Clone the repository:

```bash
git clone https://github.com/your-username/YOLOv4-Object-Detection.git
```

2. Navigate to the project directory:

```bash
cd YOLOv4-Object-Detection
```

3. Ensure the following files are present:

```text
yolov4.weights
yolov4.cfg
coco.names
object_detection.py
```

4. Run the application:

```bash
python object_detection.py
```

## Methodology

The object detection pipeline follows these steps:

1. Load the YOLOv4 network architecture and weights.
2. Load COCO class labels.
3. Initialize webcam capture using OpenCV.
4. Capture video frames continuously.
5. Convert frames into blobs suitable for YOLO input.
6. Perform forward propagation through the network.
7. Extract object predictions and confidence scores.
8. Apply Non-Maximum Suppression to eliminate redundant detections.
9. Draw bounding boxes and class labels on detected objects.
10. Display the output frame.

## Output

The application displays:

- Detected object name
- Confidence score
- Bounding box around the object

Example:

```text
Person 0.98
Bottle 0.92
Chair 0.87
```

## Applications

- Video Surveillance Systems
- Autonomous Vehicles
- Traffic Monitoring
- Robotics
- Security Systems
- Smart Cities
- Industrial Automation
- Human Activity Monitoring

## Results

The YOLOv4 model successfully detects and classifies objects from live webcam video streams in real time. Bounding boxes and confidence scores are displayed for each detected object.

## Future Enhancements

- Support for custom-trained YOLO models
- Object tracking integration
- Video file processing
- GPU acceleration using CUDA
- Detection logging and reporting

## Author

**Thirumalai K**  
Saveetha Engineering College

## License

This project is intended for educational and research purposes.
