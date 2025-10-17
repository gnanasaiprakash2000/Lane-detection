# 🛣️ U-Net Lane Detection

This repository contains a **U-Net based lane detection** model for **Advanced Driver Assistance Systems (ADAS)**.  
It performs **semantic segmentation** to detect road lanes in images or videos using deep learning.

---

## 📘 Overview

Lane detection is a crucial part of ADAS and autonomous vehicles.  
This project uses a **U-Net convolutional neural network (CNN)** to segment lane markings from road scenes.

---

## 🧠 Model Architecture

U-Net consists of two main parts:

- **Encoder (Contracting path)** – Extracts features using convolution + max pooling layers.
- - **Decoder (Expanding path)** – Uses transposed convolutions and skip connections to reconstruct the lane mask.
