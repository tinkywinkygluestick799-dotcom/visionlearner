# VisionLearner

**A rigorous benchmark of CNN architectures for image classification on MNIST and CIFAR-10**

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://python.org)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.0+-orange.svg)](https://tensorflow.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

---

## 📌 Overview

VisionLearner is a systematic evaluation of five convolutional neural network architectures — from a simple custom CNN to state-of-the-art pre-trained models (ResNet50, EfficientNetB0, MobileNetV2) — on the MNIST and CIFAR-10 image classification benchmarks.

**Key result:** EfficientNetB0 achieves 80.3% accuracy on CIFAR-10, outperforming custom CNNs by 2.2 percentage points.

---

## ❓ The Problem

Traditional ML models underperform on complex image data. Can deep learning architectures generalise more effectively?

---

## 🔬 Methodology

- **Datasets:** MNIST (digits), CIFAR-10 (objects)
- **Data augmentation:** rotation, flipping, zoom, brightness adjustment
- **Models:** Simple CNN, Deep CNN, ResNet50, EfficientNetB0, MobileNetV2
- **Training:** Adam optimiser, early stopping, 50 epochs

---

## 📊 Results

| Model | MNIST (%) | CIFAR-10 (%) | Parameters (M) |
|-------|-----------|--------------|----------------|
| Simple CNN | 98.9 | 72.4 | 1.2 |
| Deep CNN | 99.3 | 78.1 | 4.8 |
| ResNet50 | 99.4 | 79.2 | 23.0 |
| **EfficientNetB0** | **99.5** | **80.3** | **5.3** |
| MobileNetV2 | 99.1 | 76.8 | 3.5 |

---

## 🚀 How to Run

```bash
git clone https://github.com/tinkywinkygluestick799-dotcom/visionlearner
cd visionlearner
pip install -r requirements.txt
python train_advanced.py --model efficientnet
