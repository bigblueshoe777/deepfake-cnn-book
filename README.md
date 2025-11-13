# Deepfake Detection CNN

Lightweight, CPU-only CNN that detects deepfakes with strong baseline metrics and reproducible runs.

## Live site
**https://bigblueshoe777.github.io/deepfake-cnn-book/**

## Results at a glance
- Accuracy ~92–95 percent, Precision/Recall above 90 percent, AUC ~0.95
- Deterministic training, calibration checked, threshold tuned by cost

## Run locally
```bash
conda create -n deepfake-cnn python=3.11 -y
conda activate deepfake-cnn
pip install -r requirements.txt
jupyter-book build .
open _build/html/index.html

![Made with: Python](https://img.shields.io/badge/Python-3.11-blue)
![Framework](https://img.shields.io/badge/Framework-TensorFlow)
![Runs on](https://img.shields.io/badge/Runs_on-CPU-green)

## Responsible use & limitations
- **Intended use:** educational baseline and evaluation scaffold
- **Limitations:** potential dataset bias and domain shift to new manipulation types
- **Mitigations:** calibration checks, threshold tuning by cost, and focused data improvements