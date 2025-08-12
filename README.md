# Tabular-Data-Generation-with-GANs

## Overview
This project explores generating synthetic HR data using Generative Adversarial Networks (GANs) as part of a thesis on tabular data generation. The repository is organized as a series of Jupyter notebooks and data files that walk through data exploration, synthetic data modeling, evaluation, visualization, and privacy analysis.

## Repository Structure

| Path/Notebook | Purpose |
|---------------|---------|
| `01_HR dataset_EDA_Final.ipynb` | Begins the analysis with exploratory data analysis (EDA) and imports the core libraries such as pandas, NumPy, seaborn, and scikit-learn’s label encoder. |
| `02_Synthetic Data Generation.ipynb` | Implements CTGAN-based synthesis, including custom hyperparameters, loss tracking, and sections on utility and privacy evaluation of the generated data. |
| `03_ML classification model synthetic dataset.ipynb` | Trains and compares classification models (e.g., RandomForestClassifier) on synthetic datasets to assess predictive utility. |
| `04_Visualization and Comparison of datasets.ipynb` | Provides visual comparisons (e.g., salary, citizen status, termination) between real and synthetic data across different CTGAN training epochs. |
| `05_Measuring privacy.ipynb` | Discusses privacy metrics, referencing sdmetrics’ “Privacy Inference” and “NLR” methods for quantifying disclosure risk in synthetic data. |
| `metadata.json` | Supplies field definitions and ranges for each column in the HR dataset, guiding the GAN on column types and valid value ranges. |
| `20230301_HR_dataset.csv` & `20230308_Updated_HR_dataset.csv` | Raw HR datasets used throughout the notebooks for real-versus-synthetic comparisons and model training. |

## Usage Notes
1. **Data Preparation** – `01_HR dataset_EDA_Final.ipynb` handles initial profiling and cleaning.
2. **Synthetic Generation** – `02_Synthetic Data Generation.ipynb` trains CTGAN models to produce synthetic tables.
3. **Utility Evaluation** – `03_ML classification model synthetic dataset.ipynb` benchmarks predictive performance of real vs. synthetic data.
4. **Visualization** – `04_Visualization and Comparison of datasets.ipynb` renders side-by-side plots for visual inspection of data fidelity.
5. **Privacy Assessment** – `05_Measuring privacy.ipynb` references privacy-metric resources for evaluating disclosure risk in synthetic outputs.

This notebook-driven workflow enables an end-to-end exploration of synthetic tabular data generation, evaluation, and privacy assessment in an HR context.
