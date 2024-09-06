# Vehicle Insurance Customer Response Prediction

This repository contains a project focused on predicting customer responses using vehicle insurance data. The primary objective is to analyze and develop machine learning models that enhance the response rate and optimize marketing efforts for the insurance company.

## Table of Contents

1. [Problem Statement](#problem-statement)
2. [Data Mining](#data-mining)
3. [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
4. [Data Visualization](#data-visualization)
5. [Algorithms Used](#algorithms-used)
6. [Analysis of Results](#analysis-of-results)
7. [Conclusion & Future Work](#conclusion--future-work)
8. [References](#references)

## Problem Statement

The data comprises socio-economic information and insured vehicle details. The objective is to develop machine learning models to predict customer responses, enhancing the response rate and optimizing marketing efforts for the insurance company. The dataset contains both categorical and numerical variables and provides customer lifetime value based on historical data.

**Reference Dataset:** [Kaggle - Vehicle Insurance Customer Data](https://www.kaggle.com/datasets/ranja7/vehicle-insurance-customer-data)

## Data Mining

### Overview

- **Data Types**: 
  - Float: 2 columns
  - Object: 16 columns
  - Integer: 6 columns
- **Dataset Size**: 913,424 rows.
- **Target Variable**: `Response`
- The dataset is balanced with a class ratio of 5.98:1 for the majority to minority class.

### Data Cleaning and Preprocessing

1. Dropped irrelevant columns (`Customer` and `Effective To Date`).
2. Converted categorical variables into numerical using Label Encoding.
3. Scaled the features using MinMaxScaler to a range of 0-1.

## Exploratory Data Analysis (EDA)

- Identified dependent (`Response`) and independent variables.
- Split data into training and testing sets using `train_test_split`.
- Employed training data for model development and testing data for evaluation.

## Data Visualization

Data visualization is performed using Python libraries like Matplotlib and Seaborn to understand the data distribution and relationships better.

## Algorithms Used

The dataset involves a supervised machine learning problem with a categorical target variable. Several classification algorithms were applied:

- Logistic Regression
- Decision Tree Classifier
- Random Forest
- Extra Trees Classifier
- K-Neighbors Classifier
- Naïve Bayes Classifier (Gaussian NB)
- Support Vector Machine (SVM)

**Optimization Techniques:**
- Determined the optimal `k` value for the K-Nearest Neighbors (KNN) algorithm.
- Chose the best kernel type for the SVM algorithm.

## Analysis of Results

- Evaluation based on Confusion Matrix and Classification Report.
- The Extra Trees Classifier achieved the highest accuracy of **99.6%**.
- Models were evaluated on Accuracy, Precision, F1 Score, Recall, and other metrics.

## Conclusion & Future Work

The model has demonstrated excellent results, aiding the insurance company in efficiently predicting customer responses. Future improvements include:

- Integrating real-time data streams and dynamic risk assessment.
- Employing explainable AI techniques for transparent insights.
- Ensuring frequent retraining and monitoring to adapt to changing external factors.

## References

- [Vehicle Insurance Customer Data](https://www.kaggle.com/datasets/ranja7/vehicle-insurance-customer-data)

---

Feel free to add any additional details or modify this README to better suit your needs.
