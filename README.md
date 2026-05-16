# VisDrone Object Detection & Tracking 🚁

This repository contains my submission for the Antlings Computer Vision Assessment. 

## 📌 Project Overview
The goal of this project is to detect and count **Persons** and **Vehicles** from high-altitude drone imagery using the VisDrone dataset. 

## 🛠️ Tech Stack
* **Framework:** Ultralytics YOLOv8 (PyTorch)
* **Tracking:** ByteTrack (via `supervision` library)
* **Environment:** Google Colab (T4 GPU)

## 🚀 Workflow & Logic
1. **Dataset Prep:** Filtered the 10 VisDrone classes down to focus only on Humans (pedestrian, people) and Vehicles (car, truck, bus, etc.).
2. **Training:** Fine-tuned a YOLO model for 50 epochs on the YOLO-formatted Kaggle dataset.
3. **Tracking & Counting:** Implemented ByteTrack to assign unique IDs to objects. This prevents double-counting the same person across multiple frames of a video.

## 📁 Files in this Repo
* `Antlings_Assessment.ipynb`: The complete, runnable code (Training, Inference, and Tracking).
* `best.pt`: The fine-tuned custom YOLO weights.
* `tracked.mp4`: The final demo video showing real-time unique ID tracking and HUD counting.

## 📺 Demo Video
*(Paste the link to your YouTube or Google Drive screen-recording here!)*
