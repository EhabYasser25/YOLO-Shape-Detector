# YOLOv8 Shape Detector

![YOLOv8 Logo](https://raw.githubusercontent.com/ultralytics/assets/main/yolov8/banner-yolov8.png)

## Introduction

The YOLOv8 Shape Detector is an open-source computer vision project that uses the YOLO (You Only Look Once) object detection algorithm to detect and classify various shapes. This README provides an overview of the project and explains how to set it up, train the model, and perform inference.

## Getting Started

### Prerequisites

Before you begin, make sure you have the following prerequisites installed:

- Python 3.x
- [Ultralytics](https://github.com/ultralytics/ultralytics) library
- [Roboflow](https://pypi.org/project/roboflow/) library

### Installation

You can install the required libraries using pip:

```bash
pip install ultralytics
pip install roboflow
```

### Data Preparation
- Change the root path to your project directory.
- Discover the dataset and visualize class counts in the training, testing, and validation sets.

### Training
- Choose the YOLOv8 model configuration.
- Train the model using your dataset.
- Load the trained model.
- Display results, including mAP, confusion matrix, and training batch.

### Testing
- Evaluate the model's performance on the test dataset.

### Inference
- Define an inference function to detect and classify shapes in an image.
- Example usage for performing inference on an image.
