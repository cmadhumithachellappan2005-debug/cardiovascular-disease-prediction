
# Cardiovascular Disease Prediction using Machine Learning

## Project Overview

This project focuses on developing a machine learning-based system for early prediction of cardiovascular disease using patient health data.

The project evaluates multiple machine learning classification algorithms and compares their performance to identify an effective model for cardiovascular disease prediction.

## Objective

- Develop a machine learning system for cardiovascular disease prediction.
- Compare multiple machine learning classification models.
- Apply data preprocessing and feature engineering techniques.
- Use feature selection techniques to identify important features.
- Evaluate model performance using classification metrics.
- Explore explainable AI using SHAP for model interpretation.

## Dataset

The project uses the Heart Disease dataset containing patient health and clinical attributes.

- **Records:** 918
- **Features:** 11
- **Problem Type:** Binary Classification
- **Target:** Heart Disease
  - `1` – Heart Disease
  - `0` – No Heart Disease

### Main Features

- Age
- Sex
- Chest Pain Type
- Resting Blood Pressure
- Cholesterol
- Fasting Blood Sugar
- Resting ECG
- Maximum Heart Rate
- Exercise-Induced Angina
- ST Segment Slope
- Oldpeak

## Data Preprocessing

The project includes the following preprocessing steps:

- Handling missing values
- Encoding categorical variables
- Feature scaling using StandardScaler
- Stratified train-test splitting
- Exploratory Data Analysis (EDA)
- Feature engineering using interaction features

Examples of interaction features explored include:

- Cholesterol × ST Slope
- RestingBP × ST Slope
- Sex × ST Slope
- Age × MaxHR
- RestingBP × Cholesterol
- Oldpeak × Exercise Angina

## Machine Learning Models

Multiple classification algorithms were implemented and evaluated, including:

- Logistic Regression
- K-Nearest Neighbors (KNN)
- Support Vector Machine (SVM)
- Random Forest
- Extra Trees
- AdaBoost
- XGBoost
- LightGBM
- Linear Discriminant Analysis (LDA)
- CatBoost

## Feature Selection and Explainability

SHAP (SHapley Additive exPlanations) was explored to identify important features and improve model interpretability.

This helps understand which clinical attributes contribute more significantly to the model's predictions.

## Model Performance

Different machine learning models were compared based on their prediction performance.

In the project evaluation, CatBoost achieved an accuracy of approximately **90.94%** and was selected as the final model based on the evaluated results.

> Note: Model performance may vary depending on preprocessing, feature selection, hyperparameter settings, and train-test split.

## Project Structure

```text
cardiovascular-disease-prediction/
│
├── heart1.csv
├── KNN.ipynb
├── SVM (1).ipynb
├── Tree_final.ipynb
├── Project_Report.pdf
└── README.md
