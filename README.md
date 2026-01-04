# 🌾 Project DRONEWEED: Precision Vision for a Greener Future 🛰️
### *Revolutionizing Sustainable Agriculture through YOLOv8 Machine Vision*

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white)
![YOLOv8](https://img.shields.io/badge/YOLOv8-00FFAA?style=for-the-badge)
![MIT](https://img.shields.io/badge/Manipal_Institute_of_Technology-Mechatronics-orange?style=for-the-badge)

---

## 🚀 The Vision: Why We Built This
Weed infestation is a global crisis, causing up to **34% annual crop yield loss**. Traditional "blanket spraying" of herbicides is expensive, labor-intensive, and ecologically damaging. 

Our team built a **Real-Time Weed Detection System** that acts as a surgical tool for the sky. By deploying UAV-mounted AI, we've developed a way to spot the "silent thieves" of the field—weeds—before they can steal nutrients from crops. This enables precision herbicide application that can reduce chemical usage by **40-60%** while protecting soil biodiversity.

---

## 🛠️ The Work: Engineering the Edge
We didn't just train a model; we engineered a robust vision pipeline designed for the unpredictable world of outdoor farming.

### 🧠 The YOLOv8 "Brain"
We leveraged the latest evolution of the YOLO family, moving beyond traditional detection to a unified spatial regression approach.
* **Anchor-Free Mechanism**: Our model predicts object centers directly, allowing it to adapt to the irregular growth patterns of weeds without manual anchor box tuning.
* **Decoupled Heads**: By separating classification and localization tasks into separate pathways, we improved prediction accuracy significantly.
* **Advanced Backbones**: Utilizing the **CSPDarknet53** backbone with **C2f modules**, we maximized feature extraction while reducing computational overhead.

### 🌪️ Data "Training Camp" (Augmentation)
To ensure our AI could survive harsh sunlight, deep shadows, and varying altitudes, we implemented a rigorous augmentation strategy:
* **Mosaic Augmentation**: Stitches four training images together to force the model to recognize weeds at various scales and contexts.
* **MixUp Blending**: Linear interpolation between samples that encourages the model to learn broader feature patterns rather than memorizing images.
* **HSV Jittering**: Simulates varying sunlight and moisture conditions (brightness, saturation, hue) to maintain 24/7 field reliability.

---

## 📈 Breakthrough Performance
Our results prove that computational efficiency doesn't have to come at the cost of accuracy.

| Metric | Achievement | Impact |
| :--- | :--- | :--- |
| **Detection Accuracy** | **0.95 - 0.96 mAP** | Near-perfect weed identification. |
| **Real-Time Speed** | **>80 FPS** | Faster than the fastest agricultural drones. |
| **Top-1 Accuracy** | **>99%** | Reliable differentiation in complex fields. |
| **Resolution** | **640x640 px** | Captures weeds as small as 2cm. |

---

## 🌿 Species Spotlight
Our AI is a "botanist in a box," specifically trained on the **DRONEWEED dataset** (67,558 images) to distinguish between crops and these aggressive species:
* **Maize & Tomato Crops**: The primary protected species.
* **The Competitors**: *Atriplex patula*, *Chenopodium album*, *Convolvulus arvensis*.
* **The Invaders**: *Cyperus rotundus*, *Portulaca oleracea*, *Solanum nigrum*.

---

## 🌍 Sustainability (SDG Goals)
We are proud that this work advances the **United Nations Sustainable Development Goals**:
* **SDG 2 (Zero Hunger)**: Protecting yields for a growing population through efficient weed management.
* **SDG 12 (Responsible Production)**: Slashing chemical runoff through precision spraying.
* **SDG 15 (Life on Land)**: Preserving soil biodiversity and ecosystem health by reducing chemical loads.

---

## ⚡ Quick Start
To replicate our results or use our weights, ensure you have the `ultralytics` environment ready:

```bash
# Clone the repository
git clone [https://github.com/yourusername/drone-weed-detection.git](https://github.com/yourusername/drone-weed-detection.git)
cd drone-weed-detection

# Install dependencies
pip install ultralytics

# Run inference on your own drone footage
yolo predict model=best_weights.pt source='path/to/your/video.mp4'
