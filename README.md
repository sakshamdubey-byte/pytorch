# 🚀 PyTorch Learning Journey & Breast Cancer Detection

Welcome to my PyTorch repository! This project tracks my progress from mastering core deep learning operations to building and optimizing real-world medical imaging diagnostics.

---

## 📂 Repository Structure

| Topic | File / Folder | Description |
| :--- | :--- | :--- |
| 🔢 **01. Tensors** | `01_tensors/` | Core tensor operations, initialization, manipulation, and CPU vs. GPU acceleration. |
| 🧮 **02. Autograd** | `Autograd_pytorch.py` | Understanding PyTorch's automatic differentiation engine, tracking gradients, and backward passes. |
| 🎗️ **03. Diagnostics** | `breast_cancer_detection/` | Implementing and scaling breast cancer detection models from baseline networks to advanced architectures. |

---

## 🔬 Feature Project: Breast Cancer Detection Pipeline

This module focuses on evaluating and scaling machine learning models for automated breast cancer detection, transitioning from a basic baseline to state-of-the-art medical imaging architectures.

### Phase 1: The Baseline (Current)
* **Architecture:** Single Multi-Layer Neural Network.
* **Objective:** Establish a core end-to-end pipeline (data loading, preprocessing, training loop, and evaluation).

### Phase 2: Advanced Computer Vision Upgrades (In Progress)
To reduce false negatives and capture subtle tissue patterns, the pipeline is being upgraded with the following architectures:
* **Transfer Learning via DenseNet-121 / ResNet-50:** Leveraging ImageNet pre-trained weights to preserve detailed feature maps.
* **Vision Transformers (ViTs):** Capturing global context across high-resolution mammogram and ultrasound scans.
* **U-Net Segmentation:** Moving beyond binary classification to actively segment and highlight regions of interest (tumors).

### Phase 3: Tabular & Ensemble Integration
* **Hybrid Models:** Extracting deep spatial features using CNNs and passing them into optimized **XGBoost/LightGBM** classifiers.
* **Model Ensembling:** Combining predictions from multiple architectures to maximize the pipeline's overall $F_1$-score and clinical reliability.

---

## 🛠️ Getting Started

### Prerequisites
Make sure you have Python installed on your system. You can install the required dependencies by running:

```bash
pip install torch torchvision xgboost scikit-learn
