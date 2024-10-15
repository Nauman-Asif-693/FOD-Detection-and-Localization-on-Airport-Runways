# Foreign Object Debris Detection and Localization on Airport Runways using Super-Resolution

## Overview
This project aims to develop an automated system for detecting and localizing Foreign Object Debris (FOD) on airport runways. The system utilizes live video streams processed through Super-Resolution models to enhance detection accuracy, focusing on smaller or partially obscured objects that could pose a threat to aircraft safety. The ultimate goal is to improve airport safety by enabling more accurate and timely detection of debris.

## Project Features
- **Real-time FOD Detection**: AI models (such as YOLOv8 or RT-DETR) are used to detect FOD in real-time from multiple video streams.
- **Super-Resolution Enhancement**: Every nth frame from the video streams is enhanced using Super-Resolution techniques for improved detection accuracy, especially for small objects.
- **FOD Localization**: The system identifies the exact coordinates of the detected debris on the runway.
- **Real-time Alerts**: Airport staff is alerted immediately when debris is detected.
- **Dashboard Visualization**: A user-friendly dashboard provides a visual interface for viewing real-time video streams, FOD alerts, and debris locations.

## Functional Requirements
- **Detection Module**: Detect FOD on the runway and classify its type using AI models.
- **Real-time Video Stream Module**: Handle simultaneous video streams from multiple cameras, sending selected frames to the Super-Resolution Module.
- **Super Resolution Module**: Enhance the resolution of the selected frames for better small object detection.
- **Localization Module**: Identify the exact coordinates of detected debris on the runway.
- **Dashboard Module**: Provide real-time alerts and a visual interface for viewing runway conditions and debris locations.

## Evaluation Metrics
To ensure high detection accuracy and performance, the following metrics are monitored:
- **mAP50(B)**: Mean Average Precision at 50% IoU for bounding boxes.
- **mAP50-95(B)**: Mean Average Precision at IoU thresholds ranging from 50% to 95%.
- **Precision**: The ratio of true positives to the total number of detections.
- **Recall**: The ratio of true positives to the total number of actual FOD.
- **Validation Box Loss**: Measures error in predicted bounding boxes during validation.
- **Validation Classification Loss**: Measures error in class predictions during validation.

## Installation and Setup
Clone this repository:
   ```bash
   git clone https://github.com/Nauman-Asif-693/FOD-Detection-and-Localization-on-Airport-Runways.git
   cd FOD-Detection-and-Localization-on-Airport-Runways
