# Analysis_of_pea_quality
This repository contains a structured analysis pipeline for pea quality assessment using hyperspectral imaging (HSI) combined with chemometric and machine learning methods. The workflow progresses from quantitative prediction to single-attribute classification and finally to integrated quality clustering.

The repository is intended to provide a transparent and reproducible framework for evaluating pea quality at both seed and flour levels.

Repository Structure

The repository is organized according to the analytical workflow:

1. Regression
PLSR models for quantitative prediction of pea quality attributes using hyperspectral data. Models are developed at both seed and flour levels.

2. Classification – Single Parameter
Supervised classification models built separately for individual quality attributes (e.g., protein content, moisture, solubility, WBC, WUC, OBC, RVA parameters) to evaluate the discriminative capability of HSI for each trait.

3. HCA Cluster
Hierarchical cluster analysis (HCA) based on multiple quality attributes to derive integrated pea quality classes.

4. K-means Cluster
K-means clustering for multivariate quality integration and overall quality classification, with PCA-based visualization and model performance comparison.

pea_patch_dataset.zip
Patch-level hyperspectral dataset used for patch-level model training and sample-level prediction via soft voting.

Analysis Workflow

Quantitative Modeling
PLSR is used as a baseline chemometric approach to model spectral–quality relationships at seed and flour levels.

Single-Attribute Classification
Each quality parameter is classified independently to assess its spectral observability and classification performance.

Integrated Quality Classification
HCA and k-means clustering are applied to combine multiple quality attributes and derive holistic pea quality classes.


Notes

Scripts use relative paths for portability.

Large raw hyperspectral images are not included and should be provided separately if needed.

This repository is intended for research and methodological demonstration.
