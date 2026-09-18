# Healthcare Data Analysis & Stroke Prediction

## Overview
This project analyses healthcare data to identify factors associated with stroke risk and compares machine learning models for stroke prediction.

The project focuses on data cleaning, validation, exploratory analysis, feature preparation, model testing and evaluation.

## Dataset
- 5,110 healthcare records
- 12 original fields
- 201 missing BMI values identified and handled
- 249 stroke cases, representing approximately 4.87% of the dataset

## Tools & Technologies
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- scikit-learn

## What I Did
- Cleaned and validated 5,110 healthcare records.
- Handled 201 missing BMI values using median imputation.
- Performed exploratory data analysis and correlation analysis.
- Prepared categorical and numerical features for modelling.
- Split the dataset into 4,088 training and 1,022 testing records.
- Compared Logistic Regression and Random Forest models.
- Evaluated model performance using accuracy, precision, recall, F1-score and ROC-AUC.
- Fine-tuned the selected model using GridSearchCV.

## Key Results

| Model | Accuracy | Precision | Recall | F1 Score | ROC-AUC |
|---|---:|---:|---:|---:|---:|
| Logistic Regression | 74.46% | 13.75% | 80.00% | 23.46% | 84.36% |
| Random Forest | 95.01% | 0.00% | 0.00% | 0.00% | 79.67% |

Although Random Forest achieved higher overall accuracy, it failed to identify stroke cases in the test set. Logistic Regression achieved 80% recall and was more effective at identifying positive stroke cases.

The results also highlighted class imbalance as an important issue when evaluating classification models.

## Key Insights
- Age showed the strongest positive relationship with stroke prediction in the Logistic Regression model.
- Hypertension was also associated with increased stroke risk.
- High overall accuracy can be misleading when working with highly imbalanced datasets.
- Recall and ROC-AUC were important metrics for evaluating stroke detection performance.

## Project Structure
- `21.ipynb` – data preprocessing, EDA, modelling and evaluation
- `eda_figures/` – charts and model evaluation visualisations
- `Datasets/` – healthcare dataset
