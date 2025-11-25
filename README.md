# MP2_ImbalancedClassification

<a target="_blank" href="https://cookiecutter-data-science.drivendata.org/">
    <img src="https://img.shields.io/badge/CCDS-Project%20template-328F97?logo=cookiecutter" />
</a>

Project 2

## Project Organization

```
├── LICENSE                    <- Open-source license if used.
├── Makefile                   <- Convenience commands (optional).
├── README.md                  <- The top-level README for developers.
│
├── data
│   ├── raw                    <- Original .arff Mammography dataset.
│   ├── interim                <- Intermediate transformed data (optional).
│   └── processed              <- Final CSV version used for modeling.
│
├── docs                       <- Additional documentation (optional).
│
├── models                     <- Saved Random Forest, tuned models, or metrics.
│
├── notebooks                  <- Jupyter notebooks for EDA, modeling, SHAP, etc.
│                               Naming convention: `1.0-bp-exploration` etc.
│
├── pyproject.toml             <- Python project metadata & formatting config.
│
├── references                 <- Data dictionary, notes, papers, instructions.
│
├── reports
│   ├── figures                <- Generated plots (EDA, metrics, SHAP, etc.)
│   └── results                <- Any generated PDFs, HTML reports, or summaries.
│
├── requirements.txt           <- Requirements file to reproduce environment.
│
├── setup.cfg                  <- Configuration for style tools (flake8, ruff, etc.)
│
└── MP2_ImbalancedClassification
    │
    ├── __init__.py            <- Makes module importable.
    │
    ├── config.py              <- Stores constants: paths, seeds, column lists, etc.
    │
    ├── dataset.py             <- Loads ARFF file, converts to CSV, handles data prep.
    │
    ├── features.py            <- Feature engineering, processing pipelines, encoders.
    │
    ├── modeling
    │   ├── __init__.py
    │   ├── train.py           <- Model training: baseline RF, weighted RF, SMOTE RF,
    │   │                         tuned models, cross-validation, metrics.
    │   └── predict.py         <- Inference or cross_val_predict utilities.
    │
    └── plots.py               <- Visualization functions (EDA, metric plots, SHAP).