# AI-Driven Early Warning System for Sepsis Detection

## Overview

This project introduces an **AI-Driven Real-Time Early Warning System** designed to detect sepsis in ICU patients. By integrating advanced machine learning (ML) and deep learning (DL) techniques, the system focuses on temporal modeling, explainability, and real-time clinical applicability.

## Features
- **Hybrid ML/DL Models**: Combines Random Forest and Transformer-based architectures for robust and accurate predictions.
- **Explainability**: Utilizes SHAP and LIME to ensure model transparency and clinician trust.
- **Real-Time Interface**: Deploys a Gradio-based interactive tool for real-time sepsis risk assessment.
- **Superior Performance**: Achieves a ROC-AUC score of 0.92 and an F1-score of 0.89.

## Dataset
The model is trained and validated on the **PhysioNet 2019 Challenge Dataset**, comprising 2.5 million hourly observations across 44 clinical variables from ICU patients.

## Methodology
1. **Preprocessing**:
   - Imputation of missing values.
   - Outlier handling.
   - Feature scaling and normalization.
2. **Feature Engineering**:
   - Dimensionality reduction via PCA.
   - Key predictors identified: ICULOS, heart rate, respiratory rate, etc.
3. **Model Development**:
   - Logistic Regression, Random Forest, XGBoost, LSTM, Conv1D, and Transformer models.
   - An ensemble model combining Random Forest and Transformer for optimal results.
4. **Explainable AI**:
   - SHAP visualizations: summary, dependence, decision, and force plots.
   - LIME for localized explanations.

## Deployment
The project leverages **Gradio** for real-time predictions, providing an intuitive interface for ICU settings.

## Results
- **Ensemble Model**:
  - ROC-AUC: 0.92
  - F1-Score: 0.89
  - PR-AUC: 0.90
- **Highlighted Significant Predictors**:
  - ICU Length of Stay (ICULOS)
  - Hospital Admission Time (HospAdmTime)
  - Vital signs such as heart rate and respiratory rate.

## Code Files
1. **`sepsis_project_train.ipynb`**: Code for preprocessing, exploratory data analysis (EDA), and data cleaning.
2. **`sepsiscode3_0.ipynb`**: Code for data modeling and evaluation.    

## Future Enhancements
- Real-time continuous monitoring.
- Validation across diverse datasets and multi-center studies.
- Integration of advanced temporal models like Temporal Convolutional Networks (TCNs).

