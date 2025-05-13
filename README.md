# 🧠 Flowchart Shape Detection using YOLOv8 + Roboflow

This repository contains a trained YOLOv8 object detection model fine-tuned using [Roboflow](https://roboflow.com) to detect and classify various flowchart components such as processes, decisions, input/output blocks, and connectors.

<p align="center">
  <img src="results.png" width="600" alt="Model Performance">
</p>

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
