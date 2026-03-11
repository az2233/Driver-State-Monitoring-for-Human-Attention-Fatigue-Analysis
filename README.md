
## Overview

This project implements a computer-vision–based driver monitoring system designed to analyze driver attention and behavior in real time. The system detects facial cues and driving actions such as eye state, gaze direction, yawning, and phone usage.

---

## System Design

The solution is composed of two main modules:

### 1. Facial Analysis Module
A facial tracking pipeline built using **MediaPipe** processes facial landmarks to determine:

- Eye condition (open or closed)  
- Gaze orientation (left, right, or center)  
- Yawning detection based on facial movement patterns  

This module continuously evaluates driver alertness through facial features.

### 2. Behavior Recognition Module
A deep learning–based action recognition component identifies driver activities such as:

- Phone calling  
- Texting while driving  

A **MobileNet-based classifier** is used for behavior prediction, while **YOLOv5** assists by detecting mobile phones to improve recognition accuracy.

---

## Requirements

The project was developed using the following environment:

- Python 3.8  
- TensorFlow 2.8.0  
- PyTorch 1.11.0  
- OpenCV 4.5.5  
- MediaPipe 0.8.9.1  
- Matplotlib 3.5.1  
- NumPy 1.22.3  
- Scikit-learn 1.0.2  

Install dependencies:

```bash
pip install tensorflow==2.8.0 torch==1.11.0 opencv-python==4.5.5 mediapipe==0.8.9.1 matplotlib==3.5.1 numpy==1.22.3 scikit-learn==1.0.2
