# 🎯 Multi-Object Detection and Persistent ID Tracking (Colab Implementation)

## 📌 Overview
This project implements a computer vision pipeline to detect and track multiple objects in sports/event footage. Each detected subject is assigned a **unique and persistent ID** that remains consistent across frames.

The implementation is executed using **Google Colab**, ensuring ease of use without local setup.

---

## 🚀 Features
- ✅ Object detection using YOLOv8  
- ✅ Multi-object tracking using DeepSORT  
- ✅ Persistent ID assignment across frames  
- ✅ Handles occlusion, motion, and scale changes  
- ✅ Trajectory visualization for tracked objects  
- ✅ Processed annotated output video  

---

## 🧠 Methodology

### 🔹 Object Detection
We use **YOLOv8 (Ultralytics)** for detecting objects such as players, athletes, or vehicles in each frame.

### 🔹 Multi-Object Tracking
We use **DeepSORT**, which combines:
- Motion prediction (Kalman Filter)  
- Appearance-based matching (deep features)  

---

## 🏗️ Pipeline Architecture
Input Video → Frame Extraction → YOLOv8 Detection → Feature Extraction → DeepSORT Tracking → ID Assignment → Annotated Output Video

---

## 📂 Project Structure
multi-object-tracking/
│
├── main.ipynb
├── README.md
├── outputs/
│   └── output.mp4
└── screenshots/

---

## ⚙️ How to Run (Google Colab)

1. Open notebook:
(https://colab.research.google.com/drive/1WVkxpGlR1oxBOVcGrNewmppd3W3xDTGf?usp=sharing)

2. Install:
!pip install ultralytics opencv-python-headless deep-sort-realtime

3. Upload video  
4. Run all cells  
5. Download output  

---

## 🎥 Demo Video
(https://drive.google.com/file/d/1Nc__rd-ZEb9qC-Fh7BOkbfb429gJNNvT/view?usp=sharing)

---

## 📹 Input Video Source
(https://drive.google.com/file/d/1ANhcxu1WXoy5mfGp5w2awJl-rNE9kp3P/view?usp=sharing)

---
## 📹 Output Video
(https://drive.google.com/file/d/1O3rDgtrAobjfO10dGbBTgZ3BdF_snnUp/view?usp=sharing)

---

## 🛠️ Tech Stack
Python, OpenCV, YOLOv8, DeepSORT, Google Colab
