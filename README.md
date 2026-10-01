# ESP32-Epilepsy-Monitor
Real-time epileptic seizure detection system using EEG signal processing and Edge AI deployed on an ESP32 microcontroller.
# Edge AI-based Seizure Detection on ESP32 🧠⚡

![Status](https://img.shields.io/badge/Status-In%20Development-yellow)
![Hardware](https://img.shields.io/badge/Hardware-ESP32-blue)

## 📌 Project Overview
This project aims to develop a real-time embedded system for detecting epileptic seizures using Scalp EEG signals. By extracting Power Spectral Density (PSD) features and deploying a lightweight machine learning model directly onto an ESP32 microcontroller, the system minimizes latency and operates independently of cloud computing. 

This repository bridges the gap between biomedical signal processing and edge computing hardware.

## ⚙️ System Architecture
1. **Signal Preprocessing (PC-side):** 
   - Extracting EEG data from the Siena Scalp EEG Database (.edf).
   - Applying Notch (50Hz) and Bandpass filters to isolate key brainwave frequencies (Delta, Theta, Alpha, Beta, Gamma).
2. **Feature Extraction & Training:** 
   - Computing Welch's PSD to identify critical frequency spikes.
   - Training a lightweight classification model.
3. **Edge Deployment (ESP32):** 
   - Converting the trained model into C/C++ for hardware execution.
   - Simulating real-time signal feeding via Serial communication to trigger hardware alerts (e.g., LED/Buzzer).

## 🛠️ Tech Stack & Hardware
- **Signal Processing & ML:** Python (SciPy, MNE), MATLAB
- **Embedded Systems:** C/C++, ESP32 Microcontroller
- **Simulation/Prototyping:** Proteus / EasyEDA (for hardware layout)

## 🚀 How to Run
*(Phần này bạn sẽ viết hướng dẫn từng bước để tải thư viện và flash code vào ESP32 sau khi làm xong).*

## 📈 Results & Clinical Significance
*(Phần này sẽ chèn hình ảnh phổ tần số so sánh với giáo trình sinh lý và video demo ESP32 nháy đèn khi phát hiện động kinh).*