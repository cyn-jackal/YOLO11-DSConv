# YOLO11-DSConv: A Detection Framework for Black Soldier Fly Larvae in Agricultural Applications

![License](https://img.shields.io/badge/License-MIT-blue.svg)
![Python](https://img.shields.io/badge/Python-3.7%2B-blue.svg)
[![Ultralytics YOLO](https://img.shields.io/badge/Built%20With-Ultralytics%20YOLO-orange)](https://docs.ultralytics.com/)

**Table of Contents**
1. [Abstract](#abstract)
2. [Features](#features)
---

## Abstract
**Food waste** represents a significant global challenge, contributing to resource depletion, greenhouse gas emissions, and climate change. **Black Soldier Fly Larvae (BSFL)** offer an effective solution for managing food waste due to their highly efficient decomposition capabilities. However, precise identification of larval instars is crucial for optimal feeding and resource utilization, as larvae at different stages share similar appearances with only subtle color variations.

This study introduces a **mobile application** designed for the **automatic identification and detection** of BSFL instars. The system distinguishes between:

1. **Instars 1 to 4** — Best suited for food waste processing and animal feed production.  
2. **Instars 5 to 6** — Optimal for pupation and other industrial applications.

We employed the **YOLO11** model for larval instar classification and detection, achieving an **mAP<sub>50-95</sub> of 0.811**. Furthermore, we developed a modified **YOLO11-DSConv** variant, which replaces standard convolution with **Depthwise Separable Convolution (DSConv)**. This modification increased the **mAP<sub>50-95</sub>** to **0.813** and enhanced computational efficiency. By integrating this system, the application of BSFL in food waste management and broader circular economy initiatives can be significantly improved, offering a more effective and intelligent approach to addressing global food waste challenges.

- **Repository Link:** [YOLO11-DSConv](https://github.com/cyn-jackal/YOLO11-DSConv)  
- **Supplementary Materials:**  
  - [Server Side (API)](https://github.com/cyn-jackal/YOLO-server-API)  
  - [Mobile Application](https://github.com/cyn-jackal/larva_detector_app_v3)
  - [Datasets](https://universe.roboflow.com/national-pingtung-university/black-soldier-fly-larvae-5natt)

---

## Features
- **Instar Classification**: Automatically classify BSFL instars into two main groups (1–4, 5–6).
- **Enhanced Convolution**: Utilizes **Depthwise Separable Convolution (DSConv)** for improved efficiency.
- **High Accuracy**: Achieves **mAP<sub>50-95</sub> up to 0.813** while maintaining real-time performance.
- **Resource-Friendly**: Suitable for mobile and embedded applications in resource-constrained environments.
- **Open Source**: Built on [Ultralytics YOLO](https://docs.ultralytics.com/) for a robust detection framework.

---
