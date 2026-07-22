# Multimodal Mortality Prediction in Cardiac Arrest ICU Patients

A multimodal machine learning framework for predicting in-hospital mortality in cardiac arrest ICU patients by combining structured clinical data with unstructured clinical notes from the MIMIC-IV database.

---

## Overview

Early prediction of mortality in ICU patients can support timely clinical interventions and improve patient management. Traditional prediction models mainly rely on structured clinical variables such as vital signs and laboratory tests, while ignoring valuable information present in clinical notes.

This project integrates structured patient data with physician notes using Natural Language Processing (NLP) and machine learning techniques to build a more accurate and interpretable mortality prediction model.

---

## Project Objectives

- Develop a mortality prediction model for cardiac arrest ICU patients.
- Integrate structured clinical data with unstructured clinical notes.
- Compare structured-only and multimodal prediction models.
- Evaluate the effectiveness of multimodal learning for improving predictive performance.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- Hugging Face Transformers
- BioBERT
- TF-IDF
- Logistic Regression
- Principal Component Analysis (PCA)
- Singular Value Decomposition (SVD)
- Matplotlib

---

## Dataset

This project uses the **MIMIC-IV** database and **MIMIC-IV Clinical Notes** to predict in-hospital mortality among cardiac arrest ICU patients.

The final study cohort consists of **2,307 ICU patients**.

The dataset includes:

- Demographic information
- Vital signs
- Laboratory investigations
- Comorbidities
- Treatment indicators
- Glasgow Coma Scale (GCS)
- Clinical notes (Discharge summaries and Radiology reports)

> **Note:** The MIMIC-IV dataset is not included in this repository because it requires credentialed access through PhysioNet.

---

## Project Workflow

1. Extracted structured clinical data from the MIMIC-IV database.
2. Preprocessed physician notes using TF-IDF and BioBERT.
3. Performed feature engineering and dimensionality reduction.
4. Selected important predictors using LASSO and XGBoost.
5. Built Logistic Regression models for both structured and multimodal datasets.
6. Compared model performance using multiple evaluation metrics.

---

## Results

| Model | ROC-AUC |
|--------|:-------:|
| Structured Data Model | 0.89 |
| Multimodal Model | 0.92 |

The multimodal approach demonstrated improved predictive performance by integrating structured clinical variables with information extracted from physician notes using TF-IDF and BioBERT.

---

## Future Work

- Explore transformer-based multimodal architectures.
- Fine-tune BioBERT for improved clinical text representation.
- Validate the model on external ICU datasets.
- Develop a real-time clinical decision support application.

---

## Repository Structure

```
multimodal-mortality-prediction
│
├── code
│   ├── 01_structured_data_preprocessing.ipynb
│   ├── 02_unstructured_data_preprocessing.ipynb
│   ├── 03_structured_modeling.ipynb
│   ├── 04_multimodal_modeling.ipynb
│   ├── README.md
│   └── requirements.txt
│
├── data
│   └── README.md
│
├── images
│
├── presentation
│   └── Project_Presentation.pdf
│
├── report
│   └── Project_Report.pdf
│
└── README.md
```

---

## Author

**Aman Gupta**

M.Sc. Statistics & Data Science

NSOMASA, SVKM's NMIMS University

