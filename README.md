# American Sign Language (ASL) Recognition App

A real-time American Sign Language (ASL) alphabet recognition system powered by Transfer Learning (MobileNetV2) and Computer Vision.
The application detects hand gestures from a live camera feed and predicts the corresponding alphabet (A–Z) with high accuracy.

## 📌 Overview

This project captures live video input, detects hand gestures, preprocesses the region of interest, and predicts the corresponding ASL alphabet using a trained deep learning model.

📷 Real-time hand tracking  & Region-of-interest (ROI) extraction

🤖 Image preprocessing aligned with MobileNetV2

🧠 Fast and efficient inference using TensorFlow/Keras

🎯 Single-hand detection and classification

💻 Real-time prediction via Streamlit-based UI for easy interaction

## 🚀 Features

-- Real-time gesture recognition using webcam / IP camera

-- Hand detection using CVZone

-- Transfer Learning with MobileNetV2

-- Fine-tuning of pretrained layers

-- Strong data augmentation pipeline

-- Classification of 26 ASL alphabets

-- Clean UI with prediction display

-- End-to-end pipeline from detection → preprocessing → prediction

## 🧱 Tech Stack

Frontend/UI: Streamlit

Computer Vision: OpenCV, CVZone

Model: MobileNetV2

Deep Learning: TensorFlow / Keras

Language: Python

## 🧠 Model Architecture

The model is built using transfer learning with MobileNetV2, pre-trained on ImageNet.

### 🔹 Fine-Tuning Strategy

  The top 60 layers are unfrozen

   Lower layers remain frozen

👉 This allows:

  Lower layers → General features (edges, textures) → preserved

  Top 60 layers → Task-specific features → learned

  Also prevents overfitting while adapting to the ASL dataset


## 📊 Dataset Details

Total images: ~1815

Training: 1452

Validation: 363

Classes: 26 (A–Z)

## 📈 Training Performance :

📌 Initial training → gradual learning from scratch

📌 Fine-tuning → major accuracy improvement

### Final Metrics (approx):

    -> Training Accuracy: ~85%
    
    -> Validation Accuracy: ~87–89%

##  Key Observations:

📌 Model learns meaningful gesture features

📌 No severe overfitting

📌 Validation > training → augmentation is effective

## 🖥️ Inference Pipeline

1. Detect hand using CVZone

2. Extract bounding box (ROI)
   
3. Resize to (128, 128)
   
4. Apply preprocess_input
   
5. Predict using the trained model

## 📌 Future Scope :

Real-time ASL sentence translation

Gesture-to-speech conversion

Mobile app deployment

Multi-hand interaction system

## APP : 

<img width="1087" height="496" alt="Screenshot 2026-04-26 213143" src="https://github.com/user-attachments/assets/be0cd3b1-59f2-45c9-9fc8-46352ce10fd3" />

<img width="887" height="719" alt="Screenshot 2026-04-26 212257" src="https://github.com/user-attachments/assets/501aa77f-d300-47dd-a4d3-d993d63295ab" />

<img width="937" height="730" alt="Screenshot 2026-04-26 212808" src="https://github.com/user-attachments/assets/ef3ac363-1bde-4cc6-a7e9-4adffc8506de" />

<img width="903" height="717" alt="Screenshot 2026-04-26 215653" src="https://github.com/user-attachments/assets/0c297d6d-e8ba-4770-9c7a-3f30603e6287" />




