# 🌞 Week 0 Interim Report

## Task 1: Git & Environment Setup

- ✅ Created GitHub repo: [solar-challenge-week1](https://github.com/rahel-yab/solar-challenge-week0)
- ✅ Initialized Python virtual environment (`venv`)
- ✅ Added `.gitignore` to exclude `data/`, `.csv`, and `.ipynb_checkpoints/`
- ✅ Created `requirements.txt` with core packages: pandas, numpy, matplotlib, seaborn, etc.
- ✅ Set up GitHub Actions CI workflow (`ci.yml`) to:
  - Install dependencies via `pip install -r requirements.txt`
  - Confirm Python version
- ✅ Created `setup-task` branch and merged via Pull Request with 3 commits:
  - `init: add .gitignore`
  - `chore: venv setup`
  - `ci: add GitHub Actions workflow`

## Task 2: Data Profiling, Cleaning & EDA Plan

- ✅ Created branch `eda-eth` and notebook `notebooks/togo_eda.ipynb`
- ✅ Downloaded raw solar dataset for Togo and placed in `raw_data/togo.csv`
- 🔍 Planned EDA steps:
  - Summary statistics and missing-value report
  - Z-score based outlier detection for GHI, DNI, DHI, ModA, ModB, WS, WSgust
  - Impute missing values using median
  - Export cleaned data to `data/togo_clean.csv`
  ---
- 📊 Planned visualizations:
  - Time series plots of GHI, DNI, DHI, Tamb
  - Correlation heatmap and scatter plots
  - Wind rose and histograms
  - Bubble chart: GHI vs Tamb with RH or BP as size
  - Modularize cleaning in `scripts/cleaning_utils.py` 
