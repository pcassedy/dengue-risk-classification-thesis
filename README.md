# A Data Analysis Approach to Dengue Risk Assessment in CALABARZON Using Machine Learning

**Undergraduate Thesis — Bachelor of Science in Data Science**
School of Information Technology, Mapúa University · June 2026

**Authors:** Gio Miguel R. Bihasa · Pam Cassedy T. Dumangeng · Alexandra S. Santos

---

## Overview

This study develops a machine learning approach to classify dengue risk at the municipality
level across CALABARZON, Philippines, using climate, environmental, and socioeconomic
data. Each municipality-year is classified into one of three risk levels:

| Risk Level | Basis |
|---|---|
| High | Municipality's high-risk-month rate ≥ overall 75th percentile |
| Medium | Medium-or-high-risk-month rate ≥ 60th percentile among non-High municipalities |
| Low | Does not meet the above thresholds |

The goal is to support public health planning by identifying which municipalities and
periods are most at risk, using publicly-derivable environmental and socioeconomic
indicators alongside climate data.

## Data Confidentiality Notice

> **The dataset used in this study is not included in this repository.**

The dengue case data was obtained through a formal request to the Department of Health –
CALABARZON, under terms limited to academic research use. Raw and processed data files
are excluded from this repository. The code, methodology, and (documented, aggregated)
results are shared here; the underlying dataset is not redistributable.

## Methodology

1. **Data Cleaning, EDA & Feature Engineering** — descriptive statistics, ANOVA, and
   chi-square testing across climate, environmental, and socioeconomic variables
   (`notebooks/data-cleaning-eda-feature-engineering/`)
2. **Data Modeling** — four classifiers (Logistic Regression, SVM, Random Forest, XGBoost)
   evaluated across single, pairwise, and combined feature sets
   (`notebooks/data-modeling/`)
3. **Additional Findings** — dengue incidence lag models, climate variable lag models, and
   a deliberate data leakage demonstration, run separately from the operational model
   (`notebooks/additional-findings/`)
4. **Feature Importance & SHAP Analysis** — XGBoost gain-based importance and SHAP value
   analysis for model interpretability (`notebooks/feature-importance-shap/`)
5. **Classification Results** — final municipality-level risk classification, generated from
   the selected model (`results/classification/`)

## Repository Structure
# A Data Analysis Approach to Dengue Risk Assessment in CALABARZON Using Machine Learning

**Undergraduate Thesis — Bachelor of Science in Data Science**
School of Information Technology, Mapúa University · June 2026

**Authors:** Gio Miguel R. Bihasa · Pam Cassedy T. Dumangeng · Alexandra S. Santos
**Adviser:** [ADVISER NAME]

---

## Overview

This study develops a machine learning approach to classify dengue risk at the municipality
level across CALABARZON, Philippines, using climate, environmental, and socioeconomic
data. Each municipality-year is classified into one of three risk levels:

| Risk Level | Basis |
|---|---|
| High | Municipality's high-risk-month rate ≥ overall 75th percentile |
| Medium | Medium-or-high-risk-month rate ≥ 60th percentile among non-High municipalities |
| Low | Does not meet the above thresholds |

The goal is to support public health planning by identifying which municipalities and
periods are most at risk, using publicly-derivable environmental and socioeconomic
indicators alongside climate data.

## Data Confidentiality Notice

> **The dataset used in this study is not included in this repository.**

The dengue case data was obtained through a formal request to the Department of Health –
CALABARZON, under terms limited to academic research use. Raw and processed data files
are excluded from this repository. The code, methodology, and (documented, aggregated)
results are shared here; the underlying dataset is not redistributable.

## Methodology

1. **Data Cleaning, EDA & Feature Engineering** — descriptive statistics, ANOVA, and
   chi-square testing across climate, environmental, and socioeconomic variables
   (`notebooks/data-cleaning-eda-feature-engineering/`)
2. **Data Modeling** — four classifiers (Logistic Regression, SVM, Random Forest, XGBoost)
   evaluated across single, pairwise, and combined feature sets
   (`notebooks/data-modeling/`)
3. **Additional Findings** — dengue incidence lag models, climate variable lag models, and
   a deliberate data leakage demonstration, run separately from the operational model
   (`notebooks/additional-findings/`)
4. **Feature Importance & SHAP Analysis** — XGBoost gain-based importance and SHAP value
   analysis for model interpretability (`notebooks/feature-importance-shap/`)
5. **Classification Results** — final municipality-level risk classification, generated from
   the selected model (`results/classification/`)

## Repository Structure
# A Data Analysis Approach to Dengue Risk Assessment in CALABARZON Using Machine Learning

**Undergraduate Thesis — Bachelor of Science in Data Science**
School of Information Technology, Mapúa University · June 2026

**Authors:** Gio Miguel R. Bihasa · Pam Cassedy T. Dumangeng · Alexandra S. Santos
**Adviser:** [ADVISER NAME]

---

## Overview

This study develops a machine learning approach to classify dengue risk at the municipality
level across CALABARZON, Philippines, using climate, environmental, and socioeconomic
data. Each municipality-year is classified into one of three risk levels:

| Risk Level | Basis |
|---|---|
| High | Municipality's high-risk-month rate ≥ overall 75th percentile |
| Medium | Medium-or-high-risk-month rate ≥ 60th percentile among non-High municipalities |
| Low | Does not meet the above thresholds |

The goal is to support public health planning by identifying which municipalities and
periods are most at risk, using publicly-derivable environmental and socioeconomic
indicators alongside climate data.

## Data Confidentiality Notice

> **The dataset used in this study is not included in this repository.**

The dengue case data was obtained through a formal request to the Department of Health –
CALABARZON, under terms limited to academic research use. Raw and processed data files
are excluded from this repository. The code, methodology, and (documented, aggregated)
results are shared here; the underlying dataset is not redistributable.

## Methodology

1. **Data Cleaning, EDA & Feature Engineering** — descriptive statistics, ANOVA, and
   chi-square testing across climate, environmental, and socioeconomic variables
   (`notebooks/data-cleaning-eda-feature-engineering/`)
2. **Data Modeling** — four classifiers (Logistic Regression, SVM, Random Forest, XGBoost)
   evaluated across single, pairwise, and combined feature sets
   (`notebooks/data-modeling/`)
3. **Additional Findings** — dengue incidence lag models, climate variable lag models, and
   a deliberate data leakage demonstration, run separately from the operational model
   (`notebooks/additional-findings/`)
4. **Feature Importance & SHAP Analysis** — XGBoost gain-based importance and SHAP value
   analysis for model interpretability (`notebooks/feature-importance-shap/`)
5. **Classification Results** — final municipality-level risk classification, generated from
   the selected model (`results/classification/`)

## Repository Structure
├── notebooks/
│   ├── data-cleaning-eda-feature-engineering/
│   ├── data-modeling/                  # machine learning models + final classification notebook + featureimportance + shap
│   ├── additional-findings/            # lag models, data leakage demo
├── results/
│   └── classification/                 # final risk classification outputs, maps
│   └── feature-importance-shap/        # excel results
├── index.html                          # dashboard entry point (GitHub Pages)
└── README.md

## Key Files for Review

| File | What to Look For |
|---|---|
| `notebooks/data-modeling/Thesis__XGB_Model_.ipynb` | Representative XGBoost training workflow: hyperparameter search, cross-validation |
| `notebooks/data-modeling/Thesis__Final_With_Classification_.ipynb` | Final selected model, municipality-level classification, feature importance, and SHAP output generation |
| `results/classification/` | Final risk classification results and maps |

## Results Summary

Across single-feature, pairwise, and combined-feature experiments, **XGBoost consistently
outperformed** Logistic Regression, SVM, and Random Forest. The **Socioeconomic +
Environmental** pairwise combination achieved the highest standalone accuracy (0.8230,
F1 = 0.8157). The study selected the **XGBoost model trained on the full combined feature
set** (Climate + Socioeconomic + Environmental) as the final model — accuracy 0.8206,
precision 0.8091, recall 0.8206, F1-score 0.8105 — prioritizing holistic representation of
dengue risk factors over the marginal accuracy gain of the narrower feature set.

SHAP analysis identified **Temperature** (SHAP = 0.234), **Relative Humidity** (0.186), and
**Total Population** (0.175) as the most influential individual features, with environmental
land-use variables (Forest Cover, Built-up/Barren areas) also ranking highly — indicating
dengue risk in CALABARZON is shaped by the interaction of climate, environment, and
human exposure rather than any single factor group.

## Dashboard

An interactive dashboard presenting the classification results and dengue risk maps.

- **Embedded version (GitHub Pages):** (https://pcassedy.github.io/dengue-risk-classification-thesis/)
- **Original Looker Studio link:** (https://datastudio.google.com/reporting/6e3beb04-ea35-44c4-94a5-7dfef0352eec)
