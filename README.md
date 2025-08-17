# Remote Sensing Fire Risk Assessment Model Using Continuous Labels and Multi-Task Learning

This repository contains the official PyTorch implementation of our paper **"Remote Sensing Fire Risk Assessment Model Using Continuous Labels and Multi-Task Learning"**.

Our model leverages remote sensing data to assess fire risk through continuous labels using a multi-task learning framework. Both a baseline and an MAE-based model are implemented for comparison.

---

## 🔧 Environment Setup

### General

- Python: **3.9**
- CUDA: **12.4**

### Python Packages

Install the required packages:

```bash
conda create --name contFR --file requirements.txt
```

---

## 🗂️ Data Preparation

The outputs from the following notebooks are already provided, so you **do not need to run them unless you want to regenerate the data**:

- `FireRisk - Relabel-CNT.ipynb`
- `FireRisk - Relabel-CNT-Norm.ipynb`

---

## 📦 Dataset & Pretrained MAE Model

- 🔽 Download the **FireRisk dataset** from:  
  https://github.com/CharmonyShen/FireRisk

- 🔽 Download the **pretrained MAE model** from:  
  https://github.com/facebookresearch/mae

---

## 🚀 Training & Evaluation

### 1. Latent Feature Preparation

```bash
FR_Prep_MAE_Latent.ipynb
```

### 2. Proposed Model (MAE + MTL)

```bash
FR_MAE_MTL_Latent.ipynb
```

### 3. Baseline Model (MAE + Standard Classification)

```bash
FR_MAE_Latent.ipynb
```

---

## 📊 Additional Evaluation & Visualization

### Extra Regression Evaluation

Run the following notebook for additional evaluation metrics and analysis on regression outputs:

```bash
FR_MAE_MTL_Latent_Reg.ipynb
```

### Prediction Mapping

Run this notebook to visualize predictions spatially:

```bash
Mapping.ipynb
```

---
