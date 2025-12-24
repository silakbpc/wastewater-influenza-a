# Wastewater Influenza A Detection

This project focuses on detecting **Influenza A presence** using
wastewater surveillance data and machine learning techniques.
Wastewater-based epidemiology provides an early indicator of
community-level infection trends before clinical case reports.

The project includes comprehensive data preprocessing, feature
engineering, baseline and advanced classification models, and
extensive evaluation using multiple performance metrics.

---

## Project Overview

The main objective is to predict whether Influenza A is detected
(binary classification) based on wastewater measurements and
contextual features such as flow rate, population served, and
temporal information.

This repository represents an **extended and improved version** of
an earlier baseline analysis, incorporating more advanced models
and evaluation strategies.

---

## Dataset

- **Source:** CDC Wastewater Data for Influenza A  
- **Availability:** Publicly available

⚠️ The dataset is **not included** in this repository due to size and
best practices.  
Please download it directly from the official source and place it
locally if you wish to reproduce the analysis.

---

## Methodology

### Data Processing
- Missing value handling
- Temporal feature extraction (week, month, day of week)
- Log transformations
- Rolling statistics by jurisdiction
- Leakage prevention

### Models
- Logistic Regression (Baseline)
- K-Nearest Neighbors
- Histogram-Based Gradient Boosting
- Bagging Classifier (Decision Trees)

### Advanced Techniques
- Group-aware train/test splitting
- Stratified cross-validation
- Hyperparameter tuning (RandomizedSearchCV)
- Feature selection (SelectKBest, RFE, SelectFromModel)
- Dimensionality reduction (PCA, LDA)

---

## Evaluation Metrics

Models are evaluated using:
- Accuracy
- ROC-AUC
- Precision–Recall (Average Precision)
- Confusion Matrix
- Brier Score (Calibration)

Both hold-out testing and cross-validation results are reported.

---

## Repository Structure

```text
wastewater-influenza-a/
├─ notebooks/
│  └─ influenzaA.ipynb
├─ presentation/
│  └─ Presentation.pptx
├─ LICENSE
└─ README.md
```


## How to Run
Clone the repository
Download the dataset from the official CDC source
Open the notebook:

```text
jupyter notebook notebooks/influenzaA.ipynb
```

All analysis steps, visualizations, and results are contained within
the notebook.

## Presentation
The project presentation slides are available in the presentation/
folder.
