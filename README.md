<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0a1628,40:0d3d6e,100:00bcd4&height=200&section=header&text=DroneWeed&fontSize=52&fontColor=ffffff&animation=twinkling&fontAlignY=36&desc=UAV-Based%20Weed%20Species%20Detection%20%7C%20YOLOv8&descAlignY=56&descAlign=50&descSize=16" />

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=18&duration=2800&pause=1000&color=00BCD4&center=true&vCenter=true&width=700&lines=Real-time+weed+detection+from+UAV+imagery.;YOLOv8+%E2%80%94+0.95%2B+mAP+%7C+80%2B+FPS.;Reduces+herbicide+usage+by+40-60%25.;DRONEWEED+dataset+%E2%80%94+67%2C558+images." alt="Typing SVG" />

<br/>

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![YOLOv8](https://img.shields.io/badge/YOLOv8-00FFAA?style=for-the-badge&logoColor=black)
![OpenCV](https://img.shields.io/badge/OpenCV-27338e?style=for-the-badge&logo=OpenCV&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![MIT Manipal](https://img.shields.io/badge/MIT_Manipal-Mechatronics-orange?style=for-the-badge)

</div>

---

## The Problem

Weed infestation causes up to **34% annual crop yield loss** globally. Traditional blanket spraying is expensive, labor-intensive, and ecologically destructive. This project builds a **surgical AI solution** — a UAV-mounted real-time detection system that targets only weeds, enabling precision herbicide application.

---

## Results

<div align="center">

| Metric | Achievement |
|:---|:---|
| **Detection Accuracy** | **0.95 – 0.96 mAP** |
| **Real-Time Speed** | **> 80 FPS** |
| **Top-1 Classification Accuracy** | **> 99%** |
| **Input Resolution** | 640 × 640 px (detects weeds as small as 2 cm) |
| **Herbicide Reduction (est.)** | **40 – 60%** via precision targeting |

</div>

---

## Model Architecture

### YOLOv8 — Key Design Choices

| Component | Detail |
|:---|:---|
| **Anchor-Free Detection** | Predicts object centers directly — adapts to irregular weed growth patterns |
| **Decoupled Heads** | Separate classification & localization pathways for higher accuracy |
| **Backbone** | CSPDarknet53 with C2f modules — maximum feature extraction, low overhead |

### Data Augmentation Pipeline

| Technique | Purpose |
|:---|:---|
| **Mosaic Augmentation** | Forces multi-scale weed recognition |
| **MixUp Blending** | Prevents memorization, improves generalization |
| **HSV Jittering** | Simulates varying sunlight, moisture, and altitude conditions |

---

## Dataset

**DRONEWEED** — 67,558 UAV images across 8 classes:

- **Crops (protected):** Maize, Tomato
- **Weeds (targets):** *Atriplex patula*, *Chenopodium album*, *Convolvulus arvensis*, *Cyperus rotundus*, *Portulaca oleracea*, *Solanum nigrum*

---

## Impact — UN SDG Alignment

| Goal | Contribution |
|:---|:---|
| **SDG 2** Zero Hunger | Protects yields through early precision weed management |
| **SDG 12** Responsible Production | Slashes chemical runoff via targeted spraying |
| **SDG 15** Life on Land. | Reduces chemical load, preserves soil biodiversity |

---

<div align="center">

*Mechatronics Engineering — MIT Manipal '26*

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:00bcd4,60:0d3d6e,100:0a1628&height=100&section=footer" />

</div>
