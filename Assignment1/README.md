# Assignment 1 — End-to-End Data Science Project

Name: Kalhar Mayurbhai Patel
SJSU ID: 019140511
> Generated on 2025-09-14 20:32
- Github Link: https://github.com/kalhar108/CMPE-255_Data_Mining/edit/main/Assignment1  
- Medium Article Link: https://medium.com/@kalharpatel2002/sweet-sugar-and-data-science-1864a79a93ab


> This Repository includes Python notebook to solve the assignment and chat tanscript (Doc and PDF both).

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
- `Chat_Transcript.pdf` - Full chat summary with ChatGPT 5 Thinking Model.
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
