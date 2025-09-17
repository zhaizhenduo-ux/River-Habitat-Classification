# River-Habitat-Classification
# River Habitat Segmentation and Debris Detection Pipeline

An end-to-end deep learning pipeline for habitat segmentation and debris detection from UAV-captured orthomosaics. Combines semantic segmentation (FCN), domain-adjusted postprocessing, SAM refinement, and object detection.

## 🚀 Key Features

- DeepLab-based habitat segmentation
- Domain knowledge–enforced spatial postprocessing
- Integration with [Segment Anything Model (SAM)](https://github.com/facebookresearch/segment-anything)
- Detectron2-based debris detection
- Scalable to large orthomosaics (split-merge utilities)

---

## 🖥️ System Requirements

- **OS**: Windows 10/11 (with WSL)
- **GPU**: NVIDIA with CUDA ≥ 11.0 (≥8GB VRAM recommended)
- **Python**: 3.8
- **Recommended**: Use [Anaconda](https://www.anaconda.com/) + WSL (Ubuntu)

---

## ⚙️ Installation (Windows via WSL)

### 1. Install WSL
```bash
wsl --install
