# 🚗 Road Lane Detection Using UNET

This project focuses on **road lane detection** using a **UNET-based deep learning model** for semantic segmentation.  
The model is trained to identify lane markings from road images and generate corresponding binary lane masks.

---

## 📌 Project Overview

Lane detection is a critical task in:

- **Autonomous Driving**
- **Advanced Driver Assistance Systems (ADAS)**
- **Road Safety Applications**
- **Computer Vision for Transportation**

In this project, a **UNET convolutional neural network** is used to perform **pixel-wise segmentation** of road lanes from input images.

---

## 🧠 Model Used

### **UNET Architecture**
UNET is a powerful deep learning architecture designed for image segmentation tasks.  
It consists of:

- **Encoder (Contracting Path)** → captures context and features
- **Decoder (Expanding Path)** → reconstructs spatial information
- **Skip Connections** → preserve fine details for accurate segmentation

This makes UNET highly effective for detecting lane boundaries in road scenes.
---
![image alt](Images/IMG_20251017_090710.jpg)
---

## 📂 Dataset

The model is trained on **TuSimple Preprocessed Lane Detection Dataset**.

### Dataset Path Used:
```python
train_path = '/kaggle/input/tusimple-preprocessed-data/tusimple_preprocessed/training'


