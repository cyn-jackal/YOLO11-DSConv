<!-- # YOLO11-DSConv: A Detection Framework for Black Soldier Fly Larvae in Agricultural Applications -->

# Enhanced Real-Time Object Detection for Black Soldier Fly Larvae Classification Using YOLO11-DSConv

<!-- ![License](https://img.shields.io/badge/License-MIT-blue.svg) -->

![License: AGPL v3](https://img.shields.io/badge/License-AGPL_v3-blue.svg)
![Python](https://img.shields.io/badge/Python-3.7%2B-blue.svg)
[![Ultralytics YOLO](https://img.shields.io/badge/Built%20With-Ultralytics%20YOLO-orange)](https://github.com/ultralytics/ultralytics)
<!-- [![DOI](https://zenodo.org/badge/922564139.svg)](https://doi.org/10.5281/zenodo.15041711) -->

**Table of Contents**

1. [Abstract](#abstract)
2. [Features](#features)

---

## Abstract

**Food waste** represents a significant global challenge, contributing to resource depletion, greenhouse gas emissions, and climate change. **Black Soldier Fly Larvae (BSFL)** offer an effective solution for managing food waste due to their highly efficient decomposition capabilities. However, precise identification of larval instars is crucial for optimal feeding and resource utilization, as larvae at different stages share similar appearances with only subtle color variations.

This study introduces a **mobile application** designed for the **automatic identification and detection** of BSFL instars. The system distinguishes between:

1. **Instars 1 to 4** — Best suited for food waste processing and animal feed production.
2. **Instars 5 to 6** — Optimal for pupation and other industrial applications.

We employed the **YOLO11** model for larval instar classification and detection, achieving an **mAP<sub>50-95</sub> of 0.811**. Furthermore, we developed a modified **YOLO11-DSConv** variant, which replaces standard convolution with **Depthwise Separable Convolution (DSConv)**. This modification result the **mAP<sub>50-95</sub>** to **0.813** and enhanced computational efficiency. By integrating this system, the application of BSFL in food waste management and broader circular economy initiatives can be significantly improved, offering a more effective and intelligent approach to addressing global food waste challenges.

-   **Repository Link:** [YOLO11-DSConv](https://github.com/cyn-jackal/YOLO11-DSConv)
-   **Supplementary Materials:**
    -   [Server Side (API)](https://github.com/cyn-jackal/YOLO-server-API)
    -   [Mobile Application](https://github.com/cyn-jackal/larva_detector_app_v3)
    -   [Datasets](https://universe.roboflow.com/national-pingtung-university/black-soldier-fly-larvae-5natt)

---

## Features

-   **Instar Classification**: Automatically classify BSFL instars into two main groups (1–4, 5–6).
-   **Enhanced Convolution**: Utilizes **Depthwise Separable Convolution (DSConv)** for improved efficiency.
-   **High Accuracy**: Achieves **mAP<sub>50-95</sub> up to 0.813** while maintaining real-time performance.
-   **Resource-Friendly**: Suitable for mobile and embedded applications in resource-constrained environments.
-   **Open Source**: Built on [Ultralytics YOLO](https://github.com/ultralytics/ultralytics) for a robust detection framework.

---

## Acknowledgement
The code base is built with [Ultralytics YOLO](https://github.com/ultralytics/ultralytics).

Thanks for the great implementations!
---

## How to!

-   **How to run the project**

1. **Installation** : Install [pytorch](https://pytorch.org/get-started/locally/)
2. **Install package and enable editable mode**:

```
  pip install -e .
```

3. **How to train model**:

```
  yolo train data=your_data_path_in_dot_yaml_type model=./ultralytics/cfg/models/mod/yoloModx.yaml  name=your_model_name epochs=200 batch=16 imgsz=640 device=[0]
```

If you have multi-GPU for train use device=[0,1]

---

## Citation

If our code or models help your work, please cite our paper:

```
  @article{Pookunngern2025yolo11dsconv,
    author = {An-Chao Tsai, Chayanon Pookunngern},
    title = {Enhanced Real-Time Object Detection for Black Soldier Fly Larvae Classification Using YOLO11-DSConv},
    journal = {The Visual Computer},
    year = {2025},
    note = {In press}
}
```
