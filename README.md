# CBCL symptom-onset analysis

This project evaluates analysis-ready CBCL ADHD symptom-onset data with XGBoost/SHAP feature analysis, random-forest tuning, classification metrics, and ROC analysis. Sample selection and cohort construction are not included.

## Setup

Python 3.9 or newer is recommended.

```bash
python -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
export ANALYSIS_DATA_ROOT=/path/to/analysis-data
jupyter lab code.ipynb
```

`ANALYSIS_DATA_ROOT` replaces the machine-specific data prefix. The notebook requires `code/ADHD_dataset.csv` and `code/labels.csv` below this root.

## Data policy

No source data are included. The `.gitignore` excludes common tabular, imaging, model, and generated-output formats. Check the staged files before every push and follow the applicable data-use agreement and the group's access policy.

## Reproducibility note

The notebook outputs were cleared before publication. Run cells in order from a fresh kernel after configuring the data root. Generated figures and feature-importance results are written to `results/`.
