# YOLOv8 Shape Detector

![YOLOv8 Logo](https://raw.githubusercontent.com/ultralytics/assets/main/yolov8/banner-yolov8.png)
<br>
<br>

## Introduction

The YOLOv8 Shape Detector is an open-source computer vision project that uses the YOLO (You Only Look Once) object detection algorithm to detect and classify various shapes. This README provides an overview of the project and explains how to set it up, train the model, and perform inference.
<br>

## Prerequisites

Before you begin, make sure you have the following prerequisites installed:

- Python 3.x
- [Ultralytics](https://github.com/ultralytics/ultralytics) library
- [Roboflow](https://pypi.org/project/roboflow/) library

## Installation

You can install the required libraries using pip:
```bash
pip install ultralytics
pip install roboflow
```
<br>
<br>

## Data
- The dataset can be accessed on the [Roboflow Dataset](https://universe.roboflow.com/musa-almaz-p7onb/suas-shape-detection/dataset/1/images/?split=train&numImages=40).
- The total images are 2000 (1700 train, 200 validation, 100 testing)
- The dataset contains 13 classes ['circle', 'cross', 'heptagon', 'hexagon', 'octagon', 'pentagon', 'quartercircle', 'rect', 'semicircle', 'square', 'star', 'trapezoid', 'triangle']

![image](https://github.com/EhabYasser25/YOLO-Shape-Detector/assets/97472134/74efc5dd-4da4-4743-af18-15d0c1da32d2)
<br>
<br>
<br>

## Training
- Choose the YOLOv8 model configuration.
- Train the model using 40 epochs.
- Display training and validation results, including mAP, confusion matrix, and training batch.

The validation confusion matrix using the default confidence level
![image](https://github.com/EhabYasser25/YOLO-Shape-Detector/assets/97472134/7d34c8d7-112a-4b79-9edc-11b2cb29dd55)

The validation confusion matrix using 0.6 confidence level
![image](https://github.com/EhabYasser25/YOLO-Shape-Detector/assets/97472134/8de7100a-01eb-4af6-b328-33fb85c9ee4f)

The validation output (mAP = 95.68%)
![image](https://github.com/EhabYasser25/YOLO-Shape-Detector/assets/97472134/2a5eab47-56a5-451b-9bbb-5ba369a624ab)

First training batch
![image](https://github.com/EhabYasser25/YOLO-Shape-Detector/assets/97472134/e76ff948-1fac-4516-a93b-7964a83a9f1e)

First validation batch
![image](https://github.com/EhabYasser25/YOLO-Shape-Detector/assets/97472134/19b7cd78-473c-4ba4-ac16-5254213b848e)
<br>
<br>
<br>

## Testing
- The testing was done at confidence level 0.6
- Displaying the first 20 test images with predicted annotations

Some of the predicted images

![image](https://github.com/EhabYasser25/YOLO-Shape-Detector/assets/97472134/1170b024-bef9-47e6-9d55-4e8e9bceacff)

![image](https://github.com/EhabYasser25/YOLO-Shape-Detector/assets/97472134/b18dc4f1-cbea-4382-842c-579ee5ceb276)

![image](https://github.com/EhabYasser25/YOLO-Shape-Detector/assets/97472134/c46987f7-9b99-4d9b-a3a7-b9425a5a049c)
<br>
<br>
<br>

## Inference
- Defined an inference function to detect and classify shapes in an image.
- Example usage for performing inference on an image.

The input image

![image](https://github.com/EhabYasser25/YOLO-Shape-Detector/assets/97472134/4e7c1836-50d8-4633-b547-98ae1572bd69)

The output image

![image](https://github.com/EhabYasser25/YOLO-Shape-Detector/assets/97472134/a856813c-6a67-48b1-937a-993a9b0e8afd)
<br>
<br>
<br>

## Encountered Challenges
- Obtaining the Mean Average Precision (mAP) or any measure of accuracy for the testing datasets proved to be challenging.
- Implementing the inference code presented its own set of difficulties; however, I was able to overcome them with a little complex way.

## Contact
If you have any questions, suggestions, or would like to contribute to this project, please feel free to reach out.<br>
We hope you find this project valuable and look forward to your involvement in its development😊.<br>
[Google Colab Notebook](https://colab.research.google.com/drive/1wmgZaqEI0yrFSgNPtNGHov6B9YcT63jq?usp=sharing)
