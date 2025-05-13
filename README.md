# 🧠 Flowchart Shape Detection using YOLOv8 + Roboflow

This repository contains a trained YOLOv8 object detection model fine-tuned using [Roboflow](https://roboflow.com) to detect and classify various flowchart components such as processes, decisions, input/output blocks, and connectors.

![results](https://github.com/user-attachments/assets/50c1c6b7-2aaf-4d9e-86d0-bfbbf7c777cd)
![download (2)](https://github.com/user-attachments/assets/d5df4225-e414-4ff9-b5ba-0d159231895c)
![download (3)](https://github.com/user-attachments/assets/cadfd225-fede-4815-8fe7-e1a265b94cf7)
![download (4)](https://github.com/user-attachments/assets/0ab04d24-9855-49d7-bdb2-40152300a00b)
![download (5)](https://github.com/user-attachments/assets/cd6b1cf8-57c8-4cd3-be7b-f1613cc5d4e7)



## 🚀 Project Overview

This model is designed to:
- Detect hand-drawn or digital flowchart components.
- Enable automated flowchart digitization and editing.
- Integrate with tools like React Flow or diagram editors.

## 🧾 Model Performance

| Metric              | Value |
|---------------------|-------|
| mAP@0.50            | 0.957 |
| mAP@0.50:0.95       | 0.846 |
| Precision           | 0.980 |
| Recall              | 0.933 |

These results indicate high reliability in object localization and classification across a diverse dataset of ~29,000 images.

## 🧠 Classes Detected

- **Process Box**
- **Decision (Diamond)**
- **Start/End**
- **Connector/Arrow**

> *(Update the list based on your dataset labels.)*

## 📂 Project Structure

```bash
├── dataset/                  # Labeled dataset (optional for retraining)
├── weights/                  # Trained YOLOv8 model weights
├── inference/                # Inference scripts and notebooks
├── results.png               # Performance summary image
├── requirements.txt          # Dependencies
└── README.md
