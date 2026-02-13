# Helmet and Jacket Detection with YOLOv8 (x86_64 CPU)

This repository contains scripts and trained models for detecting **safety helmets and jackets** in images, video files, or live video streams using **Ultralytics YOLOv8**, optimised for **x86_64 CPU-based edge systems**.

The solution supports containerised and Kubernetes-based deployments with built-in observability using **Prometheus** and **Grafana**.

---

## Repository Structure

```text
.
├── app.py
│   └── Main application for PPE detection
│
├── wrapper_script.sh
│   └── Utility script for running inference
│
├── templates/
│   └── Template files (configuration / HTML templates)
│
├── scripts/
│   └── Additional utility scripts for setup or automation
│
├── ppe-cpu-helm/
│   └── Helm charts for deploying PPE detection on Kubernetes
│
├── prometheus/
│   └── Prometheus configuration for observability
│
├── grafana/
│   └── Grafana dashboards for visualising metrics
│
├── inference_v1.py
│   └── Base inference script for YOLOv8 detection
│
├── inference_helmet.py
│   └── Helmet-only detection script (latest)
│
├── inference_helmet_safety.py
│   └── Helmet and safety jacket detection script
│
├── inference.py
│   └── General inference script for custom YOLOv8 models
│
├── helmet_detection_yolov8_latest_v1.pt
│   └── Earlier helmet detection model
│
├── helmet_detection_yolov8_latest_v2.pt
│   └── Intermediate helmet detection model
│
├── helmet_detection_yolov8_latest_v3.pt
│   └── Latest helmet detection model
│
├── helmet_jacket_detection_yolov8_latest_v2.pt
│   └── Helmet + jacket model (do not use)
│
├── best_jacket.pt
│   └── Previous jacket detection model
│
├── best_jacket_v1.pt
│   └── atest helmet + safety jacket detection model
│
└── Dockerfile
    └── Dockerfile for containerised deployment

