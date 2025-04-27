# Overdose Hospital Discharge Cost Prediction

## Project Overview
This project analyzes hospital discharge data from New York State SPARCS and builds machine learning models to predict the mean cost of hospital discharges based on clinical and facility features.

## Dataset
- Source: New York State Department of Health SPARCS Database
- Fields: Facility Name, APR DRG Code, Severity of Illness, Year, Discharges, Mean Cost, etc.
- Cleaned and engineered dataset available in `data/cleaned_data.csv`.

## Structure
- `data/`: Raw and processed datasets
- `notebooks/`: Data cleaning and machine learning notebooks
- `README.md`: Project documentation

## Models
- Linear Regression (Baseline)
- Random Forest Regressor
- XGBoost Regressor

Achieved R² Score of **0.995** using XGBoost.

## Setup
```bash
pip install pandas scikit-learn matplotlib seaborn xgboost
