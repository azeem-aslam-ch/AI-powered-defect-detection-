# 🛠️ AI-Powered Defect Detection using YOLOv8 & YOLOv9

A deep learning-based system to automatically detect industrial or manufacturing defects using YOLOv8 and YOLOv9. This project leverages custom-trained models to localize and classify various defects from visual input such as camera feeds, product images, or 3D printing layers.

---

## 📌 Features

- ✅ Real-time defect detection using YOLOv8 & YOLOv9
- 🔍 Supports multiple defect types (e.g. cracks, shifts, warping, misalignment)
- 📊 Model performance comparison (accuracy, speed, robustness)
- 📦 Dataset preparation via Roboflow
- 🚀 Works in Google Colab or local Python setup
- 📁 Visual results with bounding boxes and labels

---

## 🧠 Models Used

| Model   | Version | Architecture | Strength              |
|---------|---------|--------------|------------------------|
| YOLOv8s | v8.1    | CSPDarknet   | Speed + Accuracy       |
| YOLOv9s | v9.0    | RT-DETR      | Higher Recall, Robust  |

---

## 🏭 Dataset Overview

- **Source**: Custom-labeled using Roboflow
- **Classes**: Cracking, Layer Shifting, Warping, Off-Platform, Stringing
- **Format**: YOLO (bounding box), split into train/val/test
- **Augmentations**: Flip, blur, mosaic, rotation

---

## ⚙️ Google Colab Setup



## 🛠️ Training in Colab

### YOLOv8

```python
!yolo task=detect mode=train model=yolov8s.pt data=data.yaml epochs=100 imgsz=640
