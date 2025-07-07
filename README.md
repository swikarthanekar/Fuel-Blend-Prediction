✈️ Sustainable Fuel Blend Property Prediction

This project was developed as part of a data science hackathon focused on accelerating the transition to sustainable aviation fuels. The objective is to build machine learning models that can accurately predict the properties of fuel blends based on their constituent components and proportions — helping the aviation industry craft sustainable and performance-compliant fuels.

📊 Problem Statement

Blending fuels to meet specific operational, safety, and environmental standards is a complex challenge involving non-linear interactions between base components. The aim is to predict 10 key blend properties from blend composition and component-wise properties using supervised regression techniques.

📁 Dataset

The dataset contains:
- **train.csv**: 2000 samples, with blend compositions, component properties, and target blend properties.
- **test.csv**: 500 samples, with blend compositions and component properties (target values hidden).
- **sample_submission.csv**: Required format for submitting predictions.

📑 Approach

- Exploratory Data Analysis (EDA)
- Baseline LightGBM and XGBoost models
- Hyperparameter tuning with Optuna
- Feature Engineering (interactions, ratios)
- Target transformation (Log1p/Expm1)
- Model Stacking (LightGBM + CatBoost + Ridge)
- K-Fold Cross Validation for robustness
- Optimized final model submission

🏆 Results

Achieved a leaderboard score of **71.96** with an average MAPE of **1.32** on validation. Future improvements involve advanced ensembling, aggressive feature engineering, and deeper hyperparameter tuning to target a 90+ leaderboard score.

📂 Project Structure

sustainable-fuel-blend-prediction/
├── data/ # Datasets
├── notebooks/ # EDA, Baseline and Final Model Notebooks
├── submissions/ # CSV submission files for leaderboard
├── README.md # Project documentation

📦 Setup & Dependencies
To reproduce this project:
pip install -r requirements.txt

Key libraries:
  --pandas
  --numpy
  --scikit-learn
  --lightgbm
  --xgboost
  --optuna
  --seaborn, matplotlib

📌 How to Upload to GitHub

1. Create a new repository on GitHub (e.g., `sustainable-fuel-blend-prediction`)
2. Clone it to your local machine:

git clone (https://github.com/swikarthanekar/Fuel-Blend-Prediction.git)
cd sustainable-fuel-blend-prediction
git add .
git commit -m "Initial project commit with data, notebooks, and README"
git push origin main

