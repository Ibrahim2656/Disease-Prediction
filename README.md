# Predictive Modeling for Disease Diagnosis

## Overview
This project aims to develop a predictive model to classify individuals into diseased or non-diseased categories based on various health attributes. Leveraging machine learning algorithms, the model serves as a reliable tool for healthcare providers to assist in disease diagnosis and prognosis.

## Table of Contents
- [Overview](#overview)
- [Project Objective](#project-objective)
- [Dataset Description](#dataset-description)
- [Methodology](#methodology)
  - [Data Preprocessing](#data-preprocessing)
  - [Feature Selection](#feature-selection)
  - [Model Selection](#model-selection)
- [Results](#results)
  - [Model Performance](#model-performance)
  - [Confusion Matrix](#confusion-matrix)
- [Conclusion](#conclusion)
- [Future Work](#future-work)
- [Usage](#usage)
- [License](#license)

## Project Objective
The primary objective of this project is to develop a machine learning model that can accurately classify individuals as diseased or non-diseased based on their health attributes. This model can be a valuable tool for healthcare providers in diagnosing diseases and planning treatments.

## Dataset Description
The dataset contains multiple health-related attributes and a binary indicator for disease presence. The key attributes include:

- Cholesterol (mg/dL)
- Hemoglobin
- Platelets
- White Blood Cells (WBC)
- Red Blood Cells (RBC)
- Hematocrit
- Mean Corpuscular Volume (MCV)
- Mean Corpuscular Hemoglobin (MCH)
- Mean Corpuscular Hemoglobin Concentration (MCHC)
- Insulin
- Body Mass Index (BMI)
- Systolic Blood Pressure (SBP)
- Diastolic Blood Pressure (DBP)
- Triglycerides (mg/dL)
- HbA1c (Glycated Hemoglobin)
- LDL Cholesterol
- HDL Cholesterol
- ALT (Alanine Aminotransferase)
- AST (Aspartate Aminotransferase)
- Heart Rate (bpm)
- Creatinine
- Troponin
- C-reactive Protein (CRP)
- Disease (Binary Indicator: 1 = Diseased, 0 = Non-diseased)

## Methodology

### Data Preprocessing
- **Data Cleaning**: Removed missing or null values to ensure data quality.
- **Normalization**: Normalized the data to ensure all features are on a similar scale.
- **Feature Engineering**: Created new features based on domain knowledge.

### Feature Selection
Dropped features with low correlation to the target variable:
- Glucose
- Platelets
- Red Blood Cells
- Mean Corpuscular Volume
- Diastolic Blood Pressure
- Triglycerides
- ALT
- White Blood Cells
- Heart Rate

### Model Selection
The following machine learning algorithms were considered:
- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier
- Support Vector Machine (SVM)
- Gradient Boosting Classifier
- K-Neighbors Classifier
- Gaussian Naive Bayes

## Results

### Model Performance
The performance of each model was evaluated based on accuracy:
- **Logistic Regression**: 93.00%
- **Random Forest**: 95.06%
- **Decision Tree**: 79.42%
- **Gradient Boosting**: 92.59%
- **K-Neighbors**: 62.76%
- **Gaussian Naive Bayes**: 98.15%
- **SVM**: 93.83%

### Confusion Matrix
The confusion matrix for the best-performing model (Gaussian Naive Bayes) was analyzed to assess the model's classification performance.

## Conclusion
- The Gaussian Naive Bayes model achieved the highest accuracy at 98.15%.
- Dropping low-correlation features improved the overall model performance.
- The model can assist healthcare providers in disease diagnosis.

## Future Work
- Incorporate additional data sources to enhance model accuracy.
- Refine the model with advanced feature engineering and hyperparameter tuning.
- Evaluate the model's performance on different datasets.

## Usage
To use this project, follow these steps:

1. Install the required packages:
   ```bash
   pip install -r requirements.txt
