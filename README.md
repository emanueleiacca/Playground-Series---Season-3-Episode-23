# Defect Prediction using Machine Learning

This repository contains code for predicting software defects using machine learning models. It includes data preprocessing, exploratory data analysis, feature selection, model training, hyperparameter tuning, model stacking, and result analysis. 

## Table of Contents

- [Introduction](#introduction)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Dataset](#dataset)
  - [Synthetically-Generated Datasets](#synthetically-generated-datasets)
- [Data Preparation](#data-preparation)
- [Data Exploration](#data-exploration)
- [Feature Selection](#feature-selection)
- [Model Training](#model-training)
- [Hyperparameter Tuning](#hyperparameter-tuning)
- [Model Stacking](#model-stacking)
- [Results](#results)
- [Conclusion](#conclusion)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Software defect prediction is essential for improving software quality and reducing maintenance costs. In this project, we aim to predict defects in software using various machine learning algorithms.

## Dataset
The dataset used in this project is available in the data directory. It includes train.csv and test.csv for training and testing data, respectively.

Synthetically-Generated Datasets like every Kaggle Competition, you can find more info here: https://www.kaggle.com/competitions/playground-series-s3e23/data

## Data Preparation
We start by loading the dataset and checking for missing values. Fortunately, there are no missing values in the dataset.

## Data Exploration
We perform data exploration, including visualizing the distribution of the 'defect' variable. This helps us understand the class distribution and the balance between defects and non-defects.

## Feature Selection
To reduce the dimensionality of the dataset, we calculate the correlation matrix and identify highly correlated features. We also use Principal Component Analysis (PCA) to select the most important features for modeling and have a better understanding of our variables

## Model Training
We train several machine learning models, including Random Forest, LightGBM, XGBoost, and CatBoost. These models are trained on the preprocessed dataset and evaluated for their predictive performance.

## Hyperparameter Tuning
To improve model performance, we use hyperparameter tuning with the Optuna library to find the best hyperparameters for each model.

## Model Stacking
We apply a stacking technique to combine the predictions from multiple models with different weights. This ensemble approach helps to further improve predictive accuracy.

## Results
After extensive model training and hyperparameter tuning, we evaluate the best model's performance using the ROC AUC score, which is the evaluation metric. Submissions are evaluated based on the area under the ROC curve between the predicted probability and the observed target.




