# DL-Project-SimSiam-reimplementation-
# 🧠 SimSiam: Reproduction and Extension on CIFAR-10

This project reproduces and extends the core findings of the paper **"Exploring Simple Siamese Representation Learning" (SimSiam)** using the CIFAR-10 dataset and PyTorch. The aim is to verify that meaningful representations can be learned without negative samples, large batches, or momentum encoders — and to go further with modern enhancements.

---

## 📌 Project Objectives

- ✅ Reproduce SimSiam from scratch in PyTorch
- ✅ Verify performance using **linear probing** and **k-NN evaluation**
- ✅ Perform **ablation studies** on:
  - Removing stop-gradient
  - Removing prediction head
- ✅ Compare SimSiam with:
  - BYOL
  - SwAV
  - SimCLR
- ✅ Test performance with **advanced augmentations**:
  - Mixup
  - CutMix
  - RandAugment

---

## 🗂️ Files Included

| File | Description |
|------|-------------|
| `DL_project_final.ipynb` | Full implementation of SimSiam, experiments, and evaluations |
| `proposal_DL.pdf` | Original project proposal (received full score) |
| `results/` *(optional)* | Visualizations (e.g., accuracy bar plots) |
| `checkpoints/` *(optional)* | Model weights (if any saved) |
| `final_report.pdf` *(if applicable)* | Full report with analysis and conclusions |

---

## 🧪 Summary of Results

| Model                  | Linear Accuracy (%) | k-NN Accuracy (%) |
|-----------------------|---------------------|-------------------|
| SimSiam               | 64.27	              |  60.13             |   
| SimSiam (No Predictor)| 58.74               |  55.02             |
| BYOL                  | 70.91               |  67.45             |
| SwAV                  | 69.42               |  65.33             |
| SimCLR                | 72.30               |  68.90             |


---

## ⚠️ Note on DINO

DINO was part of the original proposal. However, it was excluded from final evaluation due to practical challenges in dataset compatibility and model integration. Other comparisons (BYOL, SwAV, SimCLR) were completed as planned.

---

## 🛠️ How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/SiddharthTanwar1/DL-Project-SimSiam-reimplementation.git
   cd DL-Project-SimSiam-reimplementation
Install required packages:
pip install torch torchvision matplotlib tqdm


## Authors

Siddharth Tanwar
Vraj Mayur Parekh
Project for Deep Learning Course @ York University
Winter Semester 2025

## REFERENCES
Chen, X., & He, K. (2020). Exploring Simple Siamese Representation Learning. arXiv preprint arXiv:2011.10566.

## Pretrained Model Sources
# DINO ResNet-50 Pretrained Weights:
https://dl.fbaipublicfiles.com/dino/dino_resnet50_pretrain.pth

# SwAV ResNet-50 Pretrained Weights (800 epochs):
https://dl.fbaipublicfiles.com/deepcluster/swav_800ep_pretrain.pth.tar

# BYOL ResNet-50 Pretrained Weights:
https://github.com/yaox12/BYOL-PyTorch
(Note: The specific file resnet50_byol_imagenet2012.pth.tar can be found in the releases or linked resources of this repository.)

# SimSiam Pretrained Weights:
https://github.com/facebookresearch/simsiam
(Note: The checkpoint_100.tar file is available in the releases or linked resources of this repository.)

## SimSiam-Reproduction/
├── DL_project_final.ipynb
├── proposal_DL.pdf
├── README.md
└── final_report.pdf        
