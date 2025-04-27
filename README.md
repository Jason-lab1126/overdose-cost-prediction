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
📦 Setup Instructions
1. Clone the repository
git clone https://github.com/your-username/overdose-cost-prediction.git
cd overdose-cost-prediction
2. Install required packages
We recommend setting up a virtual environment (optional but cleaner):

# (Optional) Create and activate virtual environment
python3 -m venv env
source env/bin/activate  # On Windows use `env\Scripts\activate`
Install the necessary Python packages:

pip install pandas scikit-learn xgboost matplotlib
If you are using Jupyter Notebooks, also make sure:

pip install notebook
🚀 How to Run
1. Data Cleaning
Open and run the notebook:

notebooks/overdose_data_cleaning.ipynb
This notebook loads the original hospital data, cleans missing values, encodes features, and saves the processed file (cleaned_data.csv) under /data/.

2. Machine Learning Model Training
Open and run:

notebooks/overdose_ml_model.ipynb
This notebook loads data/cleaned_data.csv, trains multiple ML models (Linear Regression, Random Forest, XGBoost), evaluates performance, and visualizes feature importances and predictions.

Key output metrics (e.g., R² scores, MSE) are printed at the end.

🏆 Current Best Model

Model	R² Score	MSE
Linear Regression	0.79	15848.72
Random Forest	0.99	778.14
XGBoost	0.995	362.90
✅ XGBoost is currently the best-performing model.

📜 License
This project is licensed under the MIT License.

✨ Notes
The original raw dataset is too large to upload to GitHub (>25MB). Please contact us if you need access to the original file.

All models are trained using the processed cleaned_data.csv file.
