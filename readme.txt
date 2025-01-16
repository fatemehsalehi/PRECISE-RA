# Remission Classifier: A Machine Learning Approach for Clinical Predictions

This repository contains the code and environment configuration used in the paper titled:

**PRECISE-RA: Predicting Remission and Stratifying Risk in Rheumatoid Arthritis Patients Treated with bDMARDs—A Robust Machine Learning Approach**

## Overview

The repository includes the following steps and processes as described in the paper:
- Data preprocessing
- Model training and evaluation
- Validation
- Calibration analysis
- Risk stratification

## Files

- **`RemissionClassifier.ipynb`**: Main notebook for training machine learning models, hyperparameter tuning, cross-validation, evaluation, calibration, and risk stratification.
- **`preprocess.ipynb`**: Notebook for preprocessing the clinical data, including feature engineering, missing value handling, and data alignment.
- **`environment.yml`**: Conda environment file to recreate the computational environment used for this project.

## Features

- **Data Preprocessing**:
  - Handles clinical data with missing values and prepares it for analysis.
  - Performs feature engineering and alignment for training and testing datasets.

- **Model Training and Evaluation**:
  - Implements machine learning models, including XGBoost, AdaBoost, SVM, and Random Forest.
  - Hyperparameter tuning using `GridSearchCV`

- **Calibration Methods**:
  - Includes Platt scaling (Sigmoid), Isotonic regression, Beta calibration, and Spline calibration.

- **Performance Metrics**:
  - Accuracy, precision, recall, F1-score, Matthews correlation coefficient (MCC), Brier score, and ROC-AUC.

- **Visualization Tools**:
  - Generates calibration curves, ROC curves, and confusion matrices for internal and external validation.

## How to Use

### 1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/RemissionClassifier.git

Set up the environment:

Using Conda (recommended):

conda env create -f environment.yml
conda activate RAproject
Using Virtual Environment:

python -m venv RAproject
source RAproject/bin/activate  # On Windows: RAproject\Scripts\activate
pip install -r requirements.txt

Open and run the notebooks using Jupyter Notebook or JupyterLab:

jupyter notebook
Replace dataset.csv and dataset_test.csv with your datasets (structured as described in the paper).

Dependencies
The dependencies will be automatically installed when setting up the environment.


Dataset
The repository does not include the datasets used in the study due to privacy concerns. Ensure your datasets are structured as described in the paper when running the code.


Contact
For questions or further information, please contact:

Fatemeh Salehi (author) - fatemeh.salehi.h@gmail.com
