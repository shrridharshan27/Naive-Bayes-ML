# Naive Bayes: Probabilistic & Bayesian Classification

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue.svg?logo=python&logoColor=white)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg?logo=jupyter&logoColor=white)](https://jupyter.org/)
[![Scikit-Learn](https://img.shields.io/badge/scikit--learn-F7931E.svg?logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)
[![Pandas](https://img.shields.io/badge/pandas-150458.svg?logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![NumPy](https://img.shields.io/badge/numpy-013243.svg?logo=numpy&logoColor=white)](https://numpy.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Author
- **Shrri Dharshan D R** — [@shrridharshan27](https://github.com/shrridharshan27)

---

## Overview
This repository contains probabilistic classification pipelines implementing **Gaussian Naive Bayes (GNB)** and **Bayesian decision theory** applied to continuous scientific observation datasets from the UCI Machine Learning Repository.

The project examines prior and posterior probability distributions, Gaussian probability density functions for continuous variables, class conditional independence assumptions, and likelihood-ratio classification under real-world class imbalances.

---

## Datasets & Problem Statements

### 1. MAGIC Gamma Telescope Cherenkov Shower Discrimination
- **Dataset:** MAGIC Gamma Telescope Dataset ([UCI ID: 159](https://archive.ics.uci.edu/dataset/159))
- **Objective:** Differentiate primary gamma rays (signal: `g`) from background hadronic cosmic ray noise (`h`) using 10 continuous morphometric Hillas shower parameters (`fLength`, `fWidth`, `fSize`, `fConc`, `fAsym`, etc.).
- **Data File:** `magic04.data`
- **Methodology:** Continuous Gaussian likelihood density estimation, log-posterior decision rule, and ROC analysis.

### 2. High Time Resolution Universe Survey 2 (HTRU2) Pulsar Detection
- **Dataset:** HTRU2 Dataset ([UCI ID: 372](https://archive.ics.uci.edu/dataset/372))
- **Objective:** Identify candidate radio pulsars from radio frequency interference (RFI) using integrated pulse profile and dispersion measure statistics.
- **Methodology:** Probabilistic decision boundary evaluation under severe class imbalance (~9% pulsar prevalence).

---

## Evaluation Metrics
- **Classification Accuracy:** Overall correct predictions.
- **Precision, Recall, and F1-Score:** Macro and weighted performance across imbalanced labels.
- **Receiver Operating Characteristic (ROC-AUC):** Discriminative threshold sensitivity.
- **Log-Loss / Cross-Entropy:** Calibration quality of predicted posterior probabilities.

---

## Project Structure
```text
Naive-Bayes-ML/
├── Naive_Bayes_Classification.ipynb
├── magic04.data
├── .gitignore
└── README.md
```

---

## Quickstart & Setup
1. **Clone the repository:**
   ```bash
   git clone https://github.com/shrridharshan27/Naive-Bayes-ML.git
   cd Naive-Bayes-ML
   ```
2. **Install requirements:**
   ```bash
   pip install numpy pandas matplotlib seaborn scikit-learn ucimlrepo jupyter
   ```
3. **Run the notebook:**
   ```bash
   jupyter notebook Naive_Bayes_Classification.ipynb
   ```

---

## License
Distributed under the [MIT License](https://opensource.org/licenses/MIT).
