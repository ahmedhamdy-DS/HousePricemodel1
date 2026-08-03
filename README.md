# 🏡 House Price Prediction (Advanced Regression Techniques)

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Machine_Learning-orange.svg)
![Kaggle](https://img.shields.io/badge/Kaggle-Competition-blue)
![MLflow](https://img.shields.io/badge/MLflow-Tracking-blueviolet)

##  Project Overview
This project aims to predict the final price of residential homes in Ames, Iowa, using advanced machine learning regression techniques. It is based on the famous [Kaggle Competition](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques).

The pipeline includes comprehensive Data Preprocessing, Feature Engineering, Hyperparameter Tuning, and an advanced Voting Ensemble model tracked via **MLflow**.

##  Dataset Description
- **Source:** Kaggle
- **Train size:** 1460 samples
- **Test size:** 1459 samples
- **Features:** 79 explanatory variables describing (almost) every aspect of residential homes.

##  Project Pipeline
1. **Exploratory Data Analysis (EDA):** Handling skewed distributions (Log transformation on target variable) and analyzing feature correlations.
2. **Data Preprocessing:** Imputing missing values efficiently and handling categorical variables using Scikit-Learn `Pipelines` and `ColumnTransformer`.
3. **Feature Engineering:** Creating new meaningful features (e.g., `TotalSF`, `HouseAge`, `TotalBath`).
4. **Model Building & Tuning:** Implementing robust tree-based models and tuning hyperparameters using `RandomizedSearchCV`.
5. **Experiment Tracking:** Using **MLflow** to log parameters, track model metrics (RMSE, R²), and save learning curve visualizations.

##  Models Implemented

- **LightGBM Regressor** (Tuned)
- **XGBoost Regressor** (Tuned)
-  **Ultimate Voting Ensemble** (LightGBM + XGBoost)

##  Best Performance
- **Winning Model:** Voting Ensemble Regressor 
- **R² Score:** 0.90 
- **Evaluation Metric:** Root Mean Squared Error (RMSE) & Log Error (RMSLE).

##  Repository Structure
```text
├── house_price_model.ipynb   # Main Jupyter Notebook with full code
├── test.csv                  # Test dataset
├── train.csv                 # Training dataset
├── submission.csv            # Final predictions for Kaggle
├── requirements.txt          # Project dependencies
└── README.md                 # Project documentation


