# Create README.md content
readme = """# 🚧 PotholeAI — Road Intelligence System
Multi-Modal Deep Learning System for **Pothole Detection** using **CNN + YOLO + Hybrid Fusion**

---

## 📌 Overview
PotholeAI is a real-time road surface monitoring system that detects potholes using deep learning models and provides analytics through an interactive dashboard.

Features:
- 📷 Image Upload Detection
- 🎥 Live Webcam Detection
- 🧠 CNN Classification
- 🎯 YOLO Object Detection
- 🔀 Hybrid (YOLO + CNN)
- 📊 Analytics Dashboard

---

## 🧠 Detection Modes
### 1. CNN Classifier
- Classifies entire image
- Output: normal / pothole
- Input size: 128 × 128
- Threshold: 0.6

### 2. YOLO Object Detection
- Detects pothole bounding boxes
- Multiple detections supported

### 3. Hybrid (YOLO + CNN)
- YOLO → finds region
- CNN → confirms pothole
- Highest accuracy mode

---

## 🏗️ System Architecture
Input Image/Webcam → YOLO → CNN → Annotated Output → Dashboard

---

## 📂 Project Structure
PotholeAI/
│
├── frontend.py
├── pothole_model.h5
├── runs/detect/train12/weights/best.pt
├── requirements.txt
└── README.md

---

## ⚙️ Requirements
pip install gradio opencv-python numpy ultralytics tensorflow

---

## 📥 Model Files Required
YOLO Model:
runs/detect/train12/weights/best.pt

CNN Model:
pothole_model.h5

---

## ▶️ Run
python frontend.py

Open:
http://127.0.0.1:7860

---

## 📊 Dashboard Metrics
- Total scans
- Potholes detected
- Clear roads
- Avg confidence
- Mode usage
- Detection log

---

## 🛠️ Tech Stack
- Gradio
- YOLOv8
- TensorFlow CNN
- OpenCV
- NumPy

---

## 🚀 Use Cases
- Smart city monitoring
- Road maintenance
- Autonomous driving
- Infrastructure analytics

---

## 👨‍💻 Author
Yash Singh
"""

path = "/mnt/data/README_PotholeAI.md"
with open(path, "w") as f:
    f.write(readme)

path
