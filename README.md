# YIFE: YC-Inspired Feature Engineering for Startup Success Prediction

> **Paper:** Predicting Early-Stage Startup Success Using ML: A YC-Inspired Feature Engineering Approach  
> **Authors:** Siddharth Gupta, Pratham Namdev, Shubham Nagar, Sunny Kumar, Anjali Deshwal  
> **Institution:** Greater Noida Institute of Technology (GNIOT), GGSIPU

## Overview
This repository contains the code and resources for the YIFE framework — a domain-specific feature engineering approach for predicting early-stage startup success using machine learning on 4,323 YC-funded companies (2005–2024).

## Key Results
| Model | F1-Score | AUROC |
|-------|----------|-------|
| XGBoost (YIFE) ★ | 0.85 | 0.91 |
| Random Forest (YIFE) | 0.80 | 0.88 |
| MLP Neural Network | 0.79 | 0.86 |
| SVM | 0.76 | 0.83 |
| Logistic Regression (Baseline) | 0.66 | 0.74 |

## YIFE Feature Categories
- **Funding Features** — total funding, round count, seed size
- **Team Features** — team size, FAANG experience, elite education
- **Technical Depth** — GitHub repo count, commit frequency
- **Batch Context** — batch year encoding, batch size
- **Industry** — category, AI flag
- **Geography** — geo cluster

## Repository Structure
```
├── notebooks/        # Training and evaluation notebooks
├── data/             # Data sources (raw data not included)
├── paper/            # Published paper (added upon acceptance)
└── requirements.txt  # Dependencies
```

## Dependencies
```
scikit-learn==1.4
xgboost==2.0
shap
torch
pandas
numpy
matplotlib
seaborn
```

## Dataset Sources
Raw data is not included due to licensing restrictions.

| Source | Access |
|--------|--------|
| YC Company Directory | https://www.kaggle.com (search "Y Combinator companies") |
| Crunchbase Open Data Map | https://data.crunchbase.com (free tier / academic access) |
| GitHub Public API | https://api.github.com (public REST API) |
| LinkedIn | Manual collection of 500 public founder profiles |

## Citation
If you use this work, please cite:
> Gupta, S. et al. (2025). Predicting Early-Stage Startup Success Using ML: A YC-Inspired Feature Engineering Approach. PTEMS Conference.
