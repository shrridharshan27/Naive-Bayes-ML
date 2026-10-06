# ML Lab 03: Bayesian Classification & Naive Bayes

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue.svg?logo=python&logoColor=white)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg?logo=jupyter&logoColor=white)](https://jupyter.org/)
[![Scikit-Learn](https://img.shields.io/badge/scikit--learn-F7931E.svg?logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)
[![Pandas](https://img.shields.io/badge/pandas-150458.svg?logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![NumPy](https://img.shields.io/badge/numpy-013243.svg?logo=numpy&logoColor=white)](https://numpy.org/)

---

## Academic Details
- **Student Name:** Shrri Dharshan D R
- **Register Number:** 23BPS1090
- **Course Code:** BCSE209P
- **Course Title:** Machine Learning Laboratory
- **Faculty:** Dr. S. Shridevi
- **Institution:** School of Computer Science and Engineering (SCOPE), VIT Chennai

---

## Overview
This repository contains laboratory implementations and empirical evaluations of **Bayesian Classification** and **Naive Bayes models** applied to real-world scientific datasets from the UCI Machine Learning Repository.

The laboratory explores Bayes' Theorem, conditional class independence assumptions, Gaussian probability density functions for continuous features, prior and posterior calculation, and comparative performance analysis against imbalanced real-world distributions.

---

## Experiments & Datasets

### 1. MAGIC Gamma Telescope Dataset
- **Dataset:** MAGIC Gamma Telescope ([UCI ID: 159](https://archive.ics.uci.edu/dataset/159))
- **Objective:** Discriminate between primary gamma rays (signal: `g`) and hadronic cosmic rays (background: `h`) detected via atmospheric Cherenkov radiation showers.
- **Features:** 10 continuous morphometric Hillas parameters (`fLength`, `fWidth`, `fSize`, `fConc`, `fAsym`, etc.).
- **Data File:** `magic04.data`
- **Algorithms:** Gaussian Naive Bayes (GNB) with prior probability estimation, posterior decision thresholding, and continuous Gaussian likelihood modeling.

### 2. HTRU2 Pulsar Candidate Dataset
- **Dataset:** High Time Resolution Universe Survey 2 (HTRU2) ([UCI ID: 372](https://archive.ics.uci.edu/dataset/372))
- **Objective:** Identify true pulsar radio emissions from radio frequency interference (RFI) and noise across integrated pulse profiles and dispersion measure (DM-SNR) curves.
- **Algorithms:** Gaussian Naive Bayes under extreme class imbalance.

---

## Evaluation Metrics
- **Confusion Matrix:** True/False Positives and Negatives.
- **Classification Accuracy:** Overall accuracy across validation folds.
- **Precision, Recall & F1-Score:** Macro and Weighted averages.
- **ROC-AUC Score & ROC Curve:** Diagnostic ability across confidence thresholds.
- **Log-Loss / Cross-Entropy:** Probabilistic calibration performance.

---

## Repository Structure
```text
ML-Lab-03-Naive-Bayes/
├── lab-3.ipynb
├── magic04.data
├── .gitignore
└── README.md
```

---

## How to Run
1. **Clone the repository:**
   ```bash
   git clone https://github.com/shrridharshan27/ML-Lab-03-Naive-Bayes.git
   cd ML-Lab-03-Naive-Bayes
   ```
2. **Install dependencies:**
   ```bash
   pip install numpy pandas matplotlib seaborn scikit-learn ucimlrepo jupyter
   ```
3. **Launch Jupyter Notebook:**
   ```bash
   jupyter notebook lab-3.ipynb
   ```
