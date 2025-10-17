# 🛣️ Lane Detection using U-Net

Lane detection is a critical component of **autonomous driving systems**.  
Traditional computer vision methods such as **Hough Transform** can only detect straight lines and often fail under challenging conditions like shadows, varying lighting, or road obstructions.  

This project uses a **Deep Learning–based approach (U-Net)** to achieve more accurate and robust lane detection.

---

## 📘 Description

This project implements **lane detection using a U-Net architecture** — a convolutional neural network designed for image segmentation tasks.  
By learning pixel-wise classification, the model can detect lane markings more effectively than classical methods.

---

## 🗂️ Dataset

The dataset contains **12,764 images** with corresponding lane masks.

- 🖼️ **Images:** [Download Here](https://www.dropbox.com/s/rrh8lrdclzlnxzv/full_CNN_train.p?dl=0)
  🏷️ **Labels:** [Download Here](https://www.dropbox.com/s/ak850zqqfy6ily0/full_CNN_labels.p?dl=0)
 
  - Each image has a resolution of **80 × 160** pixels:
  - - Input images → **3 channels (RGB)**
  - - Label images → **1 channel (grayscale mask)**
     
 - **Example from Dataset:**
     
- ![Dataset Sample](assets/dataset_sample.png)
     
      - ---

## ⚙️ Preprocessing

 Since U-Net expects square inputs, all images were resized to **224 × 224**.

      ```python
      # Example: Resize images to 224x224
      cv2.resize(image, (224, 224))
