# People Counter with YOLOv3 and OpenCV

## Overview

This repository contains a Python application that utilizes YOLOv3 (You Only Look Once version 3) alongside OpenCV to detect and 
count people in video streams in real-time. The project aims to provide a reliable method for counting individuals in various environments, leveraging the power of deep learning for accurate detection.

## Features

- Real-time people detection in video streams.
- Utilizes the robust YOLOv3 model for detection.
- Counts individuals frame-by-frame.
- Display count of detected individuals on the video output.

## Getting Started

### Prerequisites

- Python 3.6+
- OpenCV 4.0+
- Numpy

### Installation

1. Clone this repository to your local machine:

    ```
    git clone 
    ```

2. Install the required Python packages:

    ```
    pip install -r requirements.txt
    ```

3. Download YOLOv3 pretrained weights and configuration file, and place them in the project directory.

    - Download yolov3.weights from [YOLO website](https://pjreddie.com/darknet/yolo/) and save it to the root of this project.
    - Download yolov3.cfg from the Darknet GitHub repo.
    - Ensure `coco.names` is also in the project directory.

### Usage

Run the script with the path to your video file or camera stream:




For real-time detection from a webcam, you can leave the `--video` argument empty, and the script will default to your device's primary camera.

## How It Works

The application utilizes OpenCV's DNN module to load YOLOv3 trained on the COCO dataset for object detection. It processes each frame of the video stream, detects individuals using YOLOv3, and counts the number of detected people.

## Contributions

Contributions are welcome! Please feel free to submit a pull request or open an issue for any bugs or improvements.

## License

This project is licensed under the MIT License 


