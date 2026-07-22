# Project Workflow

The project is organized into four notebooks corresponding to different stages of the workflow.

## Notebooks

### 1. Structured Data Preprocessing
- Extracted structured clinical data from the MIMIC-IV database.
- Performed data cleaning, feature engineering, and missing value imputation.

### 2. Unstructured Data Preprocessing
- Processed discharge summaries and radiology reports.
- Generated TF-IDF features and BioBERT embeddings.
- Applied SVD and PCA for dimensionality reduction.

### 3. Structured Data Modeling
- Performed feature selection using LASSO and XGBoost.
- Built and evaluated logistic regression models using structured clinical variables.

### 4. Multimodal Modeling
- Combined structured and text-derived features.
- Developed the final multimodal mortality prediction model.
- Evaluated performance using ROC-AUC, Accuracy, Precision, Recall, and F1-score.
