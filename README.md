![Conference](https://img.shields.io/badge/Conference-KIICE%20%7C%20ICFICE%202025-blue)
![Task](https://img.shields.io/badge/Task-Medical%20Image%20Segmentation-orange)
![Domain](https://img.shields.io/badge/Domain-Explainable%20AI-success)

# Polyp Segmentation Using Deep Learning Techniques and Explainable AI

📄 **Conference**: KIICE / ICFICE 2025  
👤 **First Author**: Mehedi Hasan Emon
🏫 **Affiliation**: Inje University, Gimhae, Republic of Korea  

---

## Overview

This repository accompanies the paper presented at **KIICE / ICFICE 2025**, which investigates **deep learning–based semantic segmentation** of colorectal polyps and integrates **Explainable Artificial Intelligence (XAI)** to enhance model transparency and clinical interpretability.

The study applies a **state-of-the-art DUCK-Net segmentation framework** and evaluates its performance on publicly available colonoscopy datasets, with a particular focus on **generalization, robustness, and explainability** rather than proposing a new architecture.

---

## Key Contributions

- Applied **DUCK-Net**, a state-of-the-art deep learning model, for colorectal polyp segmentation.
- Conducted extensive evaluation on the **Kvasir-SEG dataset**.
- Achieved strong segmentation performance across **training, validation, and test sets**.
- Integrated **Explainable AI (Grad-CAM)** to visualize decision-making regions.
- Demonstrated alignment between model attention maps and clinically relevant polyp regions, supporting trust in AI-assisted diagnosis.

---

## Dataset

- **Kvasir-SEG**
  - 1000 high-resolution colonoscopy images
  - Pixel-wise ground truth masks
  - Image resolution range: 332×487 to 1920×1072
  - Publicly available:  
    https://www.kaggle.com/datasets/debeshjha1/kvasirseg

---

## Methodology

### Preprocessing
- Image resizing: **352 × 352**
- Normalization using mean and standard deviation
- Data augmentation:
  - Horizontal & vertical flipping
  - Random rotation
  - Random scaling
  - Random cropping

### Model
- **DUCK-Net**
- Supervised learning setup
- Optimized for semantic segmentation accuracy in medical images

---

## Experimental Results

The model demonstrates consistent performance across datasets:

- **Dice Score (Test)**: 0.9156  
- **Mean IoU (Test)**: 0.8443  
- **Accuracy (Test)**: 0.9730  

Results indicate:
- Stable convergence
- Minimal overfitting
- Strong generalization on unseen test data

---

## Explainable AI (XAI)

To improve interpretability, **Grad-CAM** was applied:

- Highlights image regions contributing most to predictions
- Warmer colors (red/yellow) indicate higher model attention
- Demonstrates strong correspondence with annotated polyp regions

📌 *See Figure 2 in the paper for Grad-CAM visualization examples.*

---

## Repository Status

⚠️ **Code Status**: Experimental setup documented  
- This repository focuses on **methodology, dataset usage, and evaluation results**.
- Full training and inference code may be released in the future, subject to institutional and dataset licensing approvals.

---

## Citation

If you use this work, please cite:

```bibtex
@inproceedings{Emon2025KIICE,
  title={Polyp Segmentation Using Deep Learning Techniques and Explainable Artificial Intelligence},
  author={Emon, Mehedi Hasan and Mondal, Proloy Kumar and Mozumder, Md Ariful Islam and Bharti, Ayushi and Kim, Hee-Cheol},
  booktitle={Proceedings of KIICE / ICFICE 2025},
  year={2025}
}
