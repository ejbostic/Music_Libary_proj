
# 🎧 Music Library Analysis & Prediction

This project analyzes a digital music store database using SQLite and Python, and builds regression models to predict invoice totals based on customer and track metadata. The analysis incorporates data cleaning, transformation, and model evaluation using Random Forests and other ensemble methods.

## 📦 Project Overview

- Connects to the **Chinook SQLite database**.
- Performs SQL joins to combine customer, invoice, track, and genre data.
- Cleans and transforms the dataset for regression modeling.
- Encodes categorical variables.
- Builds machine learning models to predict **invoice totals**.
- Evaluates model performance using metrics like **RMSE** and **cross-validation**.
- Includes experiments with **Random Forest**, **Gradient Boosting**, and **XGBoost**.
- Feature importance is analyzed using **SHAP values**.

## 📁 Files

- `Music_Library_proj.ipynb`: Main notebook with all steps—SQL query, data prep, modeling, and evaluation.
- `Chinook_Sqlite.sqlite`: (Expected) SQLite database file.
- `README.md`: Project documentation (you are here!).

## 🛠 Technologies Used

- Python 3
- SQLite (via `sqlite3`)
- Pandas, NumPy
- Scikit-learn
- XGBoost
- SHAP (SHapley Additive exPlanations)
- Matplotlib

## 🚀 How to Run

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/music-library-analysis.git
cd music-library-analysis
```

### 2. Set up your environment

Make sure you have the necessary packages installed:

```bash
pip install pandas numpy matplotlib scikit-learn xgboost shap
```

### 3. Run the Notebook

Open the notebook in Jupyter:

```bash
jupyter notebook Music_Library_proj.ipynb
```

Make sure `Chinook_Sqlite.sqlite` is in the same directory or update the file path accordingly in the notebook.

## 📊 Model Highlights

- Feature engineering includes encoding categorical fields and dropping nulls.
- Trained models:
  - `RandomForestRegressor`
  - `GradientBoostingRegressor`
  - `XGBRegressor`
- Evaluated using:
  - RMSE (Root Mean Squared Error)
  - GridSearchCV for hyperparameter tuning
  - SHAP plots for model explainability

## ✅ Status

✔️ Initial analysis complete  
🔍 Model tuning and interpretability implemented  
🧪 Future work: Incorporate time features and advanced pipeline automation

