<h1 align="center">Shivam Dapkekar</h1>

<p align="center">
  <b>Applied AI &nbsp;·&nbsp; AI Vision Research &nbsp;·&nbsp; Multimodal Learning (VLM / VLA)</b><br>
  B.Tech, Vishwakarma Institute of Technology, Pune (2023 – 2027)
</p>

<p align="center">
  <a href="https://shivamd2502.github.io/"><img src="https://img.shields.io/badge/Portfolio-shivamd2502.github.io-22D3EE?style=flat&logo=googlechrome&logoColor=white"></a>
  <a href="https://scholar.google.com/citations?user=zGBbdiYAAAAJ&hl=en"><img src="https://img.shields.io/badge/Google%20Scholar-Publications-4285F4?style=flat&logo=googlescholar&logoColor=white"></a>
  <a href="https://www.linkedin.com/in/shivam-dapkekar-370980292/"><img src="https://img.shields.io/badge/LinkedIn-Shivam%20Dapkekar-0A66C2?style=flat&logo=linkedin&logoColor=white"></a>
  <a href="https://x.com/shivam_d2502"><img src="https://img.shields.io/badge/X-@shivam__d2502-000000?style=flat&logo=x&logoColor=white"></a>
  <a href="https://www.kaggle.com/shivamdapkekar"><img src="https://img.shields.io/badge/Kaggle-shivamdapkekar-20BEFF?style=flat&logo=kaggle&logoColor=white"></a>
  <a href="https://medium.com/@shivamdapkekar25"><img src="https://img.shields.io/badge/Medium-Articles-000000?style=flat&logo=medium&logoColor=white"></a>
  <a href="mailto:shivamdapkekar25@gmail.com"><img src="https://img.shields.io/badge/Email-shivamdapkekar25%40gmail.com-D14836?style=flat&logo=gmail&logoColor=white"></a>
</p>

I research and build AI systems that see and understand: computer vision, vision-language
models and multimodal learning, taken from idea to a working, measured system.
Every repository below documents its method, results and limitations.

All links in one place: **[shivamd2502.github.io/links](https://shivamd2502.github.io/links)**

---

## Research Interests

- Applied AI
- Computer vision research
- Multimodal learning: vision-language models (VLM) and vision-language-action models (VLA)
- Representation learning and parameter-efficient fine-tuning

---

## Experience

### AI & Computer Vision Intern, Biorad Medisys
*Aug 2026 – Present*

AI visual inspection of DJ (double-J) ureteral stents: the system watches the stent under a
Dino-Lite microscope and decides **accepted / rejected**.

- Built the end-to-end inspection pipeline: microscope video → sharp-frame extraction every ~2 mm →
  mask transfer → per-region classification → accept / reject decision.
- Designed two quality checks: depth-marker spacing across 11 regions and drainage-hole positions across
  5 regions to a ±0.5 mm tolerance. A stent passes only if all 16 regions pass.
- Developed position-independent mask transfer: a reference mask anchored on the first marker, with the
  best-centred frame selected for every region.
- Trained EfficientNet-B0 classifiers for the marker and hole regions on mask overlays, with a
  tolerance-aware hole mask.
- Calibrated the vision metrology at 67.5 px/mm (8 mm field of view) and optimised inspection to
  ~4–6 s per stent on a standard CPU.
- Delivered an inspection app with per-region overlays and confidence scores.
- Built a stitching and synthetic conveyor-video pipeline (SIFT / RANSAC) to test the system before
  the conveyor line exists.

### Research Intern, ISRO EOS-04 SAR Research Project
*May 2026 – Present · Remote*

Deep learning on ISRO EOS-04 satellite radar imagery.

- Implemented the ISRO-documented radiometric calibration (β⁰ / σ⁰ / γ⁰, incidence-angle correction,
  noise-bias removal, layover/shadow masking) for 160 km scenes.
- Built a patch-generation and labelling pipeline: ~1,000 to 11,700 georeferenced patches across
  4 patch sizes.
- Designed a multi-input EfficientNet-B0 + MLP that fuses image features with calibrated physical
  descriptors, and ran a controlled ablation with McNemar's test.
- Delivered full-scene inference to georeferenced maps, plus a U-Net pixel-level segmentation model.

Repository: [EOS04-SAR-Land-Cover-Classification](https://github.com/shivamd2502/EOS04-SAR-Land-Cover-Classification)

---

## Selected Projects

| Project | Summary | Key points |
|---|---|---|
| [Land-Cover-CLIP-PEFT-Image-Search](https://github.com/shivamd2502/Land-Cover-CLIP-PEFT-Image-Search) | Parameter-efficient fine-tuning of CLIP (ViT-B/32) for satellite scene understanding, plus a natural-language image-search app | Fewer than 1 % of CLIP's parameters trained · joint contrastive + classification objective · IEEE OTCON 2026 |
| [Automated-X-ray-Stitching](https://github.com/shivamd2502/Automated-X-ray-Stitching) | One panoramic X-ray from overlapping shots: SIFT + FLANN, RANSAC homography, alpha feathering | Split-and-restitch benchmark with ground truth · 0.07 s per stitch at 224 × 224 · IEEE 2025 |
| [EOS04-SAR-Land-Cover-Classification](https://github.com/shivamd2502/EOS04-SAR-Land-Cover-Classification) | Raw ISRO EOS-04 radar imagery to georeferenced maps with a multi-input CNN and U-Net | Sensor-documented calibration · image + physical feature fusion · 160 km scenes end-to-end |
| [IoT-Intrusion-Detection-Elastic-Autoencoder](https://github.com/shivamd2502/IoT-Intrusion-Detection-Elastic-Autoencoder) | Elastic Deep Autoencoder representations of IoT traffic for attack detection on CICIoT2023 | 32-d latent code + reconstruction error · LR / RF / MLP comparison · IEEE OTCON 2025 |
| [Hybrid-Network-Fault-Diagnosis](https://github.com/shivamd2502/Hybrid-Network-Fault-Diagnosis) | TF-IDF + Random Forest fused with RFC-grounded expert rules through Bayesian fusion | 8 fault classes · entropy-based uncertainty · explainable rule traces · IEEE KALINGACONF 2026 |
| [RL-Active-Suspension-Control](https://github.com/shivamd2502/RL-Active-Suspension-Control) | SAC, DDPG and TD3 agents controlling an active suspension on ISO 8608 road profiles | SAC lowers body velocity by 20–35 % and acceleration by 9–12 % vs passive |

Each project has a dedicated page (problem, workflow, figures, documents) on the
[portfolio](https://shivamd2502.github.io/#projects).

---

## Publications

| Title | Venue | Status |
|---|---|---|
| Scalable Land Cover Classification using Parameter-Efficient Vision-Language Models | IEEE OTCON 2026 | Published |
| Elastic Deep Autoencoder-Based Hybrid Intrusion Detection System for IoT Networks | IEEE OTCON 2025 | Published |
| Automated X-ray Image Stitching for Enhanced Medical Diagnostics and Visualization | IEEE, 2025 | Published |
| Hybrid Bayesian Network Fault Diagnosis using ML and Expert Systems | IEEE KALINGACONF 2026 | Accepted, publication pending |
| Multi-Input EfficientNet for Land Cover Classification Using EOS-04 SAR Level-2B Data | ISRO EOS-04 research project | In preparation |

Full list: [Google Scholar](https://scholar.google.com/citations?user=zGBbdiYAAAAJ&hl=en)

---

## Competitions and Additional Work

- **Kaggle Image Matching Challenge 2025.** Rank 283 of 5,606 entries.
  [IMC-25](https://github.com/shivamd2502/IMC-25)
- **LLM_Complete.** LLM building blocks implemented from scratch in PyTorch: tokenizer,
  self-attention, multi-head attention and a GPT-style transformer.
  [LLM_Complete](https://github.com/shivamd2502/LLM_Complete)
- **Paper Implementations.** Research papers re-implemented from scratch in PyTorch.
  [Paper-Implementations](https://github.com/shivamd2502/Paper-Implementations)
- **Fingerprint Classification Dataset (Kaggle).** 1,000 images hand-annotated in Label Studio across
  5 pattern classes.

---

## Technical Skills

| Area | Tools and methods |
|---|---|
| AI / ML | PyTorch, scikit-learn, transfer learning, parameter-efficient fine-tuning, representation learning, deep reinforcement learning (SAC, TD3, DDPG) |
| Vision and multimodal | CLIP / ViT, vision-language models, EfficientNet, U-Net, segmentation, retrieval |
| Computer vision | OpenCV, SIFT / FLANN / RANSAC, image stitching, vision metrology, Label Studio |
| Tools | Python, Git and GitHub, Kaggle, Linux, VS Code |

---

## Outreach

- Volunteer, **Atmabodh – A Digital Literacy Program**: teaching digital skills to elderly people,
  homemakers and under-privileged children.
