<h1 align="center">Hi, I'm Shivam Dapkekar 👋</h1>
<p align="center">
  <b>AI / Computer Vision · Remote Sensing · Control Systems</b><br>
  4th-year B.Tech, Instrumentation &amp; Control Engineering, Vishwakarma Institute of Technology, Pune (2023–2027)
</p>

<p align="center">
  <a href="mailto:shivamdapkekar25@gmail.com"><img src="https://img.shields.io/badge/Email-shivamdapkekar25%40gmail.com-D14836?style=flat&logo=gmail&logoColor=white"></a>
  <a href="https://www.linkedin.com/in/shivam-dapkekar-370980292/"><img src="https://img.shields.io/badge/LinkedIn-Shivam%20Dapkekar-0A66C2?style=flat&logo=linkedin&logoColor=white"></a>
  <a href="https://x.com/shivam_d2502"><img src="https://img.shields.io/badge/X-@shivam__d2502-000000?style=flat&logo=x&logoColor=white"></a>
</p>

I build end-to-end pipelines that turn **sensor and image data into decisions**: satellite SAR
calibration and land-cover mapping, medical and industrial vision, and learning-based control.
I care about reproducible results, so every repo below runs on Windows and documents how its
numbers were measured.

---

## 💼 Experience

**AI & Computer Vision Intern, Biorad Medisys**, *Aug 2026 – present*
*Automated vision inspection of DJ stents*
- OpenCV inspection pipeline on a Dino-Lite digital microscope: stent segmentation,
  contour and centre-line extraction, marker-distance and tapered-length measurement.
- Calibrated vision metrology: 960×540 imaging, 15.7 × 7.4 mm field of view, 61.15 px/mm.
- Faster image stitching through high-overlap concatenation: 57.96 s for 124 images down to 0.53 s for 12 images.

**Research Intern, ISRO EOS-04 SAR Research Project** (remote), *May 2026 – present*
- EOS-04 Level-2B ARD radiometric calibration implemented from the ISRO format document:
  - β⁰ / σ⁰ / terrain-normalised γ⁰ with local incidence angle correction;
  - noise-bias removal;
  - layover/shadow masking for 160 km MRS scenes.
- QGIS patch-generation and labelling pipeline: about 1,000 (256 px) to 11,700 (64 px)
  georeferenced training patches for 3 land-cover classes.
- Multi-input **EfficientNet-B0 + MLP** fusing image features with calibrated SAR descriptors:
  **93.9–94.5 % validation accuracy** across four patch sizes.
- Full-scene inference producing georeferenced GeoTIFF land-cover maps for QGIS, plus a U-Net
  pixel-level segmentation model.
  → [EOS04-SAR-Land-Cover-Classification](https://github.com/shivamd2502/EOS04-SAR-Land-Cover-Classification)

---

## 🚀 Featured projects

| Project | What it does | Highlights |
|---|---|---|
| 🛰️ [**EOS04-SAR-Land-Cover-Classification**](https://github.com/shivamd2502/EOS04-SAR-Land-Cover-Classification) | ISRO EOS-04 SAR → calibrated composites → patch classifier → land-cover GeoTIFF maps | ISRO-documented calibration · EfficientNet-B0 + SAR/DEM features · DEM ablation with McNemar test · U-Net |
| 🌍 [**Land-Cover-CLIP-PEFT-Image-Search**](https://github.com/shivamd2502/Land-Cover-CLIP-PEFT-Image-Search) | Parameter-efficient CLIP (ViT-B/32) for satellite land-cover classification + text-to-image search app | **99.88 %** test accuracy with < 1 % trainable parameters · *IEEE OTCON'26* |
| 🩻 [**Automated-X-ray-Stitching**](https://github.com/shivamd2502/Automated-X-ray-Stitching) | Panoramic X-ray stitching: SIFT + FLANN + RANSAC homography + alpha feathering | SSIM 0.998 on a 48-run split-and-restitch benchmark · 0.07 s per stitch at 224² · *IEEE 2025* |
| 🛡️ [**IoT-Intrusion-Detection-Elastic-Autoencoder**](https://github.com/shivamd2502/IoT-Intrusion-Detection-Elastic-Autoencoder) | Intrusion detection on CICIoT2023 with Elastic Deep Autoencoder features vs a raw-feature baseline | **99.42 %** (MLP) · LR / RF / MLP comparison · *IEEE OTCON'25* |
| 🌐 [**Hybrid-Network-Fault-Diagnosis**](https://github.com/shivamd2502/Hybrid-Network-Fault-Diagnosis) | TF-IDF + Random Forest + RFC-grounded expert rules + Bayesian fusion, as a Streamlit troubleshooting app | 8 fault classes · RF **99.58 %** test accuracy · entropy-based uncertainty · *IEEE KALINGACONF'26* |
| 🚗 [**RL-Active-Suspension-Control**](https://github.com/shivamd2502/RL-Active-Suspension-Control) | SAC, DDPG and TD3 controlling a quarter-car active suspension on ISO 8608 road profiles | SAC cuts body velocity **20–35 %** and acceleration **9–12 %** vs passive |

**More work**
- 🧩 [**IMC-25**](https://github.com/shivamd2502/IMC-25): Image Matching Challenge 2025, rank **283 / 5,606** worldwide.
- 🧠 [**LLM_Complete**](https://github.com/shivamd2502/LLM_Complete): LLM building blocks from scratch in PyTorch
  (tokenizer, self-attention, transformer).
- 📄 [**Paper-Implementations**](https://github.com/shivamd2502/Paper-Implementations): research papers re-implemented from scratch in PyTorch.
- 🎛️ **Active bus suspension with full state feedback** (MATLAB/Simulink, ongoing): pole-placement
  controller with integral action, 1.8 s settling time and < 5 mm overshoot for a 0.1 m road step.

---

## 📚 Publications

- **Scalable Land Cover Classification using Parameter-Efficient Vision-Language Models**, *IEEE OTCON'26*
- **Hybrid Bayesian Network Fault Diagnosis using ML and Expert Systems**, *IEEE KALINGACONF'26* (accepted)
- **Elastic Deep Autoencoder-Based Hybrid Intrusion Detection System for IoT Networks**, *IEEE OTCON'25*
- **Automated X-ray Image Stitching for Enhanced Medical Diagnostics and Visualization**, *IEEE, 2025*

---

## 🛠️ Tech stack

<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white">
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat&logo=pytorch&logoColor=white">
  <img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=flat&logo=opencv&logoColor=white">
  <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=flat&logo=scikitlearn&logoColor=white">
  <img src="https://img.shields.io/badge/NumPy-013243?style=flat&logo=numpy&logoColor=white">
  <img src="https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white">
  <img src="https://img.shields.io/badge/Matplotlib-11557C?style=flat">
  <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=flat&logo=streamlit&logoColor=white">
  <img src="https://img.shields.io/badge/QGIS-589632?style=flat&logo=qgis&logoColor=white">
  <img src="https://img.shields.io/badge/rasterio%20%7C%20GDAL-2E5A88?style=flat">
  <img src="https://img.shields.io/badge/MATLAB%20%2F%20Simulink-0076A8?style=flat">
  <img src="https://img.shields.io/badge/Arduino-00878F?style=flat&logo=arduino&logoColor=white">
  <img src="https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white">
</p>

**Areas:** machine learning · deep learning · computer vision · image processing · SAR remote sensing

---

## 🌱 Contributions & outreach

- Open-sourced a **fingerprint classification dataset** on Kaggle: 1,000 images hand-annotated in
  Label Studio across 5 pattern classes.
- Volunteer, **Atmabodh – A Digital Literacy Program**: teaching digital skills to elderly people,
  homemakers and under-privileged children.
