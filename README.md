# Engineering Graduate Salary Prediction

A machine learning project to predict the annual salary of engineering graduates in India using regression models and data-driven analysis.

## Overview

This project aims to build a predictive model for estimating the annual salary of engineering graduates based on various factors such as academic performance, technical skills, and personal attributes.

By leveraging machine learning techniques, this project provides a data-driven approach to salary prediction, helping improve decision-making in recruitment and education.

## Problem Background

Determining fair and competitive salaries is a complex task influenced by multiple factors:

* Academic performance
* Technical and soft skills
* Educational background
* Demographic and institutional factors

Traditional approaches can be subjective and inconsistent. This project applies machine learning to generate more objective and reliable salary predictions.

## Dataset

* Source: Kaggle - *Engineering Graduate Salary Prediction*
* Link: https://www.kaggle.com/datasets/manishkc06/engineering-graduate-salary-prediction
* Data includes:

  * Academic scores (10th, 12th, GPA)
  * Skill assessments (English, Logical, Quant, Programming, Domain)
  * Demographic and educational attributes

## Data Preprocessing

* Handling missing values:

  * Numerical features → mean imputation
  * Categorical features → mode imputation
* Feature scaling:

  * Standardization using StandardScaler
* Encoding:

  * One-Hot Encoding for categorical variables
* Data split:

  * 80% training, 20% testing

## Models Used

Three regression models were implemented and compared:

### Random Forest Regressor

* Ensemble method using multiple decision trees
* Produces stable and accurate predictions through averaging

### Gradient Boosting Regressor

* Sequential learning approach that corrects previous errors
* Strong performance in capturing complex patterns

### Support Vector Regression (SVR)

* Uses kernel functions to model linear and non-linear relationships
* Effective for high-dimensional data but sensitive to tuning

## Model Evaluation

Models were evaluated using:

* **MAE (Mean Absolute Error)**
* **MSE (Mean Squared Error)**
* **R² Score (R-squared)**

## Results

### Before Hyperparameter Tuning

* Gradient Boosting showed the best performance
* Random Forest performed moderately well
* SVR had the lowest performance

### After Hyperparameter Tuning

* All models improved significantly
* **Gradient Boosting Regressor remained the best model**
* Random Forest became a strong alternative
* SVR improved but still underperformed compared to others

### Hyperparameter Tuning

Grid Search was used with parameters such as:

* Random Forest:

  * n_estimators, max_depth, min_samples_split
* Gradient Boosting:

  * n_estimators, learning_rate, max_depth
* SVR:

  * C, kernel, gamma

## Objectives

* Predict graduate salaries using machine learning
* Compare multiple regression models
* Identify the best-performing model
* Support data-driven decision-making

## Conclusion

Gradient Boosting Regressor achieved the best performance across all evaluation metrics, making it the most reliable model for this task. The model demonstrates strong predictive capability and can be applied in decision support systems for recruitment and education sectors.
