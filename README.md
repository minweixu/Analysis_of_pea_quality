# Analysis of Pea Quality

This repository contains hyperspectral imaging (HSI) and machine-learning analyses for pea quality assessment using flour and intact-seed spectra.

## Dataset

A total of 149 pea samples from the 2024 and 2025 harvest years were used:

- 113 samples for model development
- 36 samples for independent validation

Seven quality indicators were analyzed:

- Protein content
- Moisture content
- Water uptake capacity
- Water binding capacity
- Oil binding capacity
- Protein solubility
- Peak viscosity (RVA)

## Repository structure

```text
1_Flour regression/
1_Seed regression/
2_Individual quality indicator classification/
3_Overall classification/
```

## Analyses

### Flour regression
- Protein regression
- Regression of the other six quality indicators

### Seed regression
- Regression of all seven quality indicators using intact-seed spectra

### Individual indicator classification
- Three-class classification for each quality indicator

### Overall classification
- K-means two-class and three-class classification based on all seven indicators

## Models

Regression models include PLSR, SVR, Ridge, and Elastic Net.

Classification models include Logistic Regression, SVM, Random Forest, Extra Trees, and Soft Voting.

## Requirements

```bash
pip install numpy pandas matplotlib scikit-learn openpyxl joblib jupyterlab
```

## Usage

Clone or download the repository, open the required notebook in Jupyter, and run all cells in order.

```bash
git clone https://github.com/minweixu/Analysis_of_pea_quality.git
cd Analysis_of_pea_quality
jupyter lab
```

Keep all filenames and folder names unchanged so the relative paths work correctly.

## Notes

- Sample-level splitting was used to prevent patches from the same sample appearing in both training and validation sets.
- HSI spectra were used as model inputs.
- Quality measurements were used as regression targets or to define classification labels.
