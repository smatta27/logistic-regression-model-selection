income-prediction
This project predicts whether an individual earns more than $50K annually using demographic information from census data. I worked on data cleaning, feature engineering, model selection, evaluation, and tried to address issues like class imbalance and fairness.

Project Overview
The goal of this project was to build and evaluate different machine learning models that can classify whether a person earns over $50K based on features like age, education, occupation, and hours worked per week. I explored multiple algorithms and preprocessing techniques to improve performance and interpretability.

Objectives and Goals
Preprocess and clean the census dataset

Try different classification models

Evaluate and compare model performance

Handle class imbalance

Look into potential model bias

Dataset
Source: censusData.csv

Contains demographic and income-related features (e.g., age, workclass, education, marital status, occupation, sex, hours-per-week)

Target variable: income (binary — <=50K or >50K)

Methodology
Data Cleaning:

Removed rows with missing or unknown values

Encoded categorical variables using one-hot encoding

Normalized continuous features

Modeling:

Tried Logistic Regression, Random Forest, XGBoost, and SVM

Used grid search for hyperparameter tuning

Addressed class imbalance using class weights

Evaluation:

Compared models using accuracy, F1-score, precision, recall, and ROC AUC

Analyzed performance specifically for the positive class (>50K)

Results and Key Findings
Best Model: XGBoost

Accuracy: ~86%

F1 Score (positive class): ~0.72

XGBoost outperformed other models after tuning

Class imbalance impacted recall, but weighting helped

Model showed some bias across gender, which is a possible area for improvement

Visualizations
Confusion matrices for each model

Feature importance plots for XGBoost

ROC curves for performance comparison

Next Steps
Explore SHAP or LIME for interpretability

Evaluate fairness across subgroups more thoroughly

Try deep learning models or ensembling methods

How to Run
Clone the repo

Open income_prediction.ipynb in Jupyter or Colab

Make sure censusData.csv is in the same directory

Run the notebook top to bottom to see results

Individual Contributions
I worked on every part of this project including:

Exploring and preprocessing the dataset

Training and tuning all models

Running evaluation metrics and generating plots

Writing the documentation and README
