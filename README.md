# YOLO v4

## Overview
This project implements **YOLO v4 (You Only Look Once)** for real-time object detection. YOLO v4 is an advanced deep learning model designed for fast and accurate object detection in images and videos. It is optimized for both **CPU** and **GPU** usage, making it suitable for various hardware configurations.

## Features
- **Object Detection**: Detect objects in images and videos.
- **Compatibility**: Supports conversion to **TensorFlow Lite** and **TensorRT** formats for optimized inference on different platforms.
- **Pre-trained Models**: Includes YOLO v4 pre-trained weights for quick setup.
- **Custom Object Detection**: Fine-tune YOLO v4 to detect custom objects.

## Setup and Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/shit-happens/yolo_v4.git
   cd yolo_v4
   ```

2. Install required dependencies:
   - **CPU version**:
     ```bash
     conda env create -f conda-cpu.yml
     ```
   - **GPU version**:
     ```bash
     conda env create -f conda-gpu.yml
     ```

3. Install additional Python dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

- Run object detection on images:
  ```bash
  python detect.py --image <path_to_image>
  ```

- Run object detection on videos:
  ```bash
  python detect_video.py --video <path_to_video>
  ```

- Convert YOLO v4 model to TensorFlow Lite or TensorRT formats:
  ```bash
  python convert_tflite.py
  python convert_trt.py
  ```
