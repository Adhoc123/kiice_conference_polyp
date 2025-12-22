# Polyp Segmentation Using Deep Learning Techniques and Explainable AI

📄 Conference: KIICE / ICFICE 2025
👤 Authors: Mehedi Hasan Emon, Proloy Kumar Mondal, Md Ariful Islam Mozumder, Ayushi Bharti, Hee-Cheol Kim
🏫 Affiliation: Inje University, Gimhae, Republic of Korea

Overview

This repository accompanies the conference paper:

Polyp Segmentation Using Deep Learning Techniques and Explainable Artificial Intelligence
KIICE / ICFICE 2025

The study investigates deep learning–based semantic segmentation of colorectal polyps using a DUCK-Net architecture, combined with Explainable AI (XAI) techniques to improve model transparency and clinical interpretability.

The focus of this work is benchmarking segmentation performance and interpretability, rather than proposing a new architecture.

Key Contributions

Applied a state-of-the-art DUCK-Net segmentation model for colorectal polyp segmentation.

Conducted extensive evaluation on the Kvasir-SEG dataset (1000 annotated colonoscopy images).

Achieved strong generalization performance across train, validation, and test sets:

Dice (Test): 0.9156

mIoU (Test): 0.8443

Accuracy (Test): 0.9730

Integrated Explainable AI (XAI) using Grad-CAM to visualize model decision regions.

Demonstrated alignment between model attention maps and clinically relevant polyp regions, supporting trust in AI-assisted diagnosis.

Methodology
Dataset

Kvasir-SEG

1000 high-resolution colonoscopy images

Pixel-wise ground truth masks

Image resolution ranges from 332×487 to 1920×1072

Preprocessing

Image resizing to 352 × 352

Normalization using mean and standard deviation

Data augmentation:

Horizontal & vertical flipping

Random rotation

Random scaling and cropping

Model

DUCK-Net (Deep U-Net with enhanced convolutional kernels)

Supervised learning setup

Optimized for semantic segmentation accuracy

Evaluation Metrics

The following metrics were used to evaluate performance:

Dice Coefficient (DSC)

Mean Intersection over Union (mIoU)

Precision

Recall

Accuracy

Performance trends across epochs show:

Stable convergence

Minimal overfitting

Strong generalization on unseen test data

Explainable AI (XAI)

To enhance interpretability, Grad-CAM was applied:

Highlights image regions contributing most to predictions

Warm colors (red/yellow) indicate high model attention

Demonstrates strong correspondence with annotated polyp regions

📌 See Figure 2 (Grad-CAM analysis) in the paper.

Repository Status

⚠️ Code Status: To Be Released

This repository currently focuses on:

Experimental setup

Dataset description

Evaluation protocol

Explainability analysis

Full training and inference code will be released in a future update, subject to dataset licensing and institutional approval.

Publication

📄 Polyp Segmentation Using Deep Learning Techniques and Explainable Artificial Intelligence
KIICE / ICFICE 2025

📎 Paper PDF included in this repository 

Polyp Segmentation Using Deep L…

License

This repository is intended for academic and research use only.

Contact

Email: mehedihasanemon3913@gmail.com

LinkedIn: LinkedIn

Google Scholar: Google Scholar
