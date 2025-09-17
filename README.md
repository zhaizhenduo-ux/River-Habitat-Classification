# 🛰️ River Habitat Segmentation & Debris Detection Pipeline

This repository provides an end-to-end deep learning pipeline for **river habitat segmentation** and **debris detection** using high-resolution UAV orthomosaic imagery. The workflow integrates:

- ✅ Semantic segmentation using DeepLab (FCN + VGG16)
- ✅ Domain knowledge–based spatial refinement
- ✅ Segment Anything Model (SAM) for further mask enhancement
- ✅ Detectron2-based debris detection
- ✅ Tiling and merging utilities to handle large `.tif` orthomosaics

> 📌 This software runs on Windows via WSL (Ubuntu) and supports GPU acceleration.

---

## 📦 Features

- 🌍 Process ultra-large UAV `.tif` orthomosaics with split/merge support
- 🎯 Multi-stage habitat classification: segmentation → correction → refinement
- 🤖 Object detection for floating debris using Detectron2
- 💻 Designed for both local development and headless server execution
- 🚀 GPU support for all model inference steps (CUDA-compatible)

---

## 🖥️ System Requirements

| Component       | Requirement                  |
|----------------|------------------------------|
| OS             | Windows 10 / 11 with WSL     |
| WSL Linux      | Ubuntu (via `wsl --install`) |
| GPU            | NVIDIA GPU w/ CUDA ≥ 11.0    |
| Python         | Version 3.8 (recommended)    |
| RAM            | ≥ 16 GB (8 GB minimum)       |

---

## ⚙️ Installation Guide (Windows)

### 1. Install WSL & Ubuntu
```powershell
wsl --install
