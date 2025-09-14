# Assignment 1 — End-to-End Data Science Project

> Generated on 2025-09-14 20:32

This repository contains a complete beginner-to-intermediate data science workflow:

- **Part 1:** Kaggle dataset suggestions + chosen dataset
- **Part 2:** EDA & preprocessing with plots
- **Part 3:** Baseline and advanced models (Linear Regression, RandomForest, MLPRegressor)
- **Part 4:** Insights & storytelling
- **Part 5:** Medium-style article draft

## Chosen Dataset
We use the **Diabetes** dataset bundled with scikit‑learn for full reproducibility. Task: **Regression** — predict a disease progression score from clinical measurements.

## Quickstart
1. Create a fresh Python 3.9+ environment
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Open the notebook:
   ```bash
   jupyter notebook Assignment1.ipynb
   ```

## Repository Contents
- `Assignment1.ipynb` — the full, commented notebook
- `plots/` — exported figures you can paste into reports or Medium
    - `target_distribution.png`
    - `hist_bmi.png`
    - `hist_bp.png`
    - `hist_s5.png`
    - `hist_s1.png`
    - `correlation_heatmap.png`
    - `model_comparison_rmse.png`
    - `rf_feature_importances.png`
- `Medium_Article_Draft.md` — polished, beginner-friendly article
- `README.md` — this file

## EDA Highlights
- No missing values; all features are numeric and already normalized by scikit‑learn.
- **BMI** and **blood pressure** show strong relationships with the target.

## Modeling Results (Test Set)
| Model | MAE | RMSE | R² |
|---|---:|---:|---:|
| LinearRegression (scaled) | 42.7941 | 53.8534 | 0.4526 |
| RandomForestRegressor | 44.2761 | 54.4612 | 0.4402 |
| MLPRegressor (64,32) | 48.1606 | 60.4706 | 0.3098 |

**Best (by RMSE):** LinearRegression (scaled) — RMSE=53.8534, MAE=42.7941, R²=0.4526

## How to Reproduce
The notebook is self-contained and uses a dataset bundled with scikit‑learn. Run all cells in order.
