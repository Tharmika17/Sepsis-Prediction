# Machine Learning for Early Sepsis Prediction with Clinical Dashboard Support

This project presents an end-to-end pipeline for early sepsis prediction using synthetic ICU time-series data generated from the MIMIC-III demo dataset, followed by model development, evaluation, explainability (SHAP), and a clinical decision-support dashboard built in Power BI.

---

## Project Pipeline

1️. Synthetic dataset generation (Gaussian Copula)

2️. Model development, evaluation and explainability (ML models+ SHAP)

3️. Clinical dashboard development (Power BI)

---

## 1. Synthetic Data Generation

Notebook: `Dataset_Creation.ipynb`

* Source: MIMIC-III Demo ICU dataset
* Method: Gaussian Copula
* Generated privacy-preserving synthetic time-series clinical data
* Preserved statistical relationships between clinical variables for realistic modelling

---

## 2. Model Development, Evaluation and Explainability

Notebook: `Sepsis_Prediction.ipynb`

### Models Implemented

* Logistic Regression - Baseline model
* XGBoost - Ensemble/Boosting model
* Long Short-Term Memory (LSTM) - Deep learning time-series model
* Temporal Convolutional Network (TCN) - Deep learning temporal model

### Key Components

* Data preprocessing and feature engineering on clinical time-series data
* Sequential tensor preparation for deep learning (TCN)
* Train–test split for performance assessment
* Evaluation using Accuracy, Precision, Recall, and F1-score
* Comparative performance analysis across models developed in this stage
* SHAP integrated for feature importance and model interpretation

---

## 3. Clinical Dashboard (Power BI)
Dashboard: `Sepsis_clinical dashboard.pdf`

An interactive clinical decision-support dashboard for interpreting model outputs:

* Sepsis vs Non-Sepsis analysis
* Clinical trends and treatment insights
* Hourly physiological trends 
* Patient and ICU stay level filtering

---

## Tech Stack

 Python • Pandas • NumPy • Scikit-learn • Machine learning • Deep Learning • SHAP • Gaussian Copula • MIMIC-III Demo        
 • Synthetic time-series dataset • Power BI • Jupyter Notebook

---

## Key Contributions

* Synthetic ICU time-series dataset generation using Gaussian Copula
* Time-series sepsis prediction using different ML models
* Integrated SHAP-based explainability within the modelling pipeline
* End-to-end workflow from data synthesis to clinical dashboard

---

## Data & Ethics Note

This repository does not contain raw MIMIC-III clinical data.
The study uses synthetically generated time-series data for privacy-preserving research purposes only.

---


