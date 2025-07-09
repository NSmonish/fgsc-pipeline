# FGSC Pipeline: Feature-Guided Stellar Classification

This repository contains the implementation of the **Feature-Guided Stellar Classification (FGSC)** pipeline. The method integrates **fractal geometry** and **topological data analysis (TDA)** to improve the classification of astronomical spectra.

## 🛰️ Overview

FGSC extracts noise-resilient features from stellar spectra using:
- **Fractal Geometry**: Box-counting dimension, Higuchi fractal dimension, multiscale fractal analysis
- **Topological Data Analysis**: Persistent homology from Vietoris-Rips complexes

These features are then used to train:
- A **Random Forest classifier**, or
- A **hybrid model** combining a shallow neural network and RF

Tested on the **SDSS** dataset (with STAR, GALAXY, QSO classes), FGSC achieves up to **98% accuracy**.

## 📁 Contents

- `FGSC_pipeline.ipynb` – Complete training pipeline (Colab compatible)
- `utils/` – Feature extraction scripts for fractal and TDA descriptors
- `data/` – Sample preprocessed spectra (optional placeholder)
- `models/` – Trained model checkpoints (optional)

## 🧪 How to Run

```bash
# Clone this repository
git clone https://github.com/yourusername/fgsc-pipeline.git
cd fgsc-pipeline

# Install dependencies (Python 3.8+)
pip install -r requirements.txt

# Or open the notebook in Google Colab
