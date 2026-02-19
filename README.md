# Geospatial Risk Modeling & Classification Analysis

## Overview

This project builds an end-to-end geospatial data science pipeline to analyze spatial patterns and predict risk using structured geographic and tabular data.

The objective is to integrate geospatial features with machine learning models to understand how location-based factors influence classification outcomes.

We focus on:

• Spatial feature engineering
• Imbalanced classification modeling
• Performance evaluation beyond simple accuracy
• Translating spatial patterns into actionable insights

---

## Problem Statement

Many real-world prediction problems contain geographic signals that are not captured by traditional tabular models.

This project investigates:

How can spatial proximity, geographic density, and location-based features improve classification performance?

We designed a modeling framework that integrates:

• Geospatial data processing
• Distance-based feature engineering
• Imbalanced learning techniques
• Model benchmarking

---

## Methodology

### 1. Data Processing & Cleaning

* Standardized coordinate systems using consistent CRS (UTM)
* Cleaned missing and inconsistent spatial records
* Normalized structured and geospatial variables
* Performed exploratory data analysis (EDA)

---

### 2. Geospatial Feature Engineering

Engineered spatial signals including:

* Nearest neighbor distance features using SciPy cKDTree
* Density-based spatial measures
* Coordinate transformations using GeoPandas
* Spatial joins and region-level aggregations

This step significantly improved model signal strength.

---

### 3. Handling Class Imbalance

The dataset exhibited imbalance in the target variable.

We applied:

* SMOTE (Synthetic Minority Oversampling Technique)
* Focused on Recall and F1-score instead of accuracy

---

### 4. Modeling & Evaluation

Implemented and compared:

* Logistic Regression
* XGBoost

Evaluation Metrics:

* Accuracy
* Precision
* Recall
* F1-score

Tree-based models captured nonlinear spatial interactions more effectively.

---

## Tech Stack

**Languages & Libraries**

* Python
* Pandas
* NumPy
* Scikit-learn
* XGBoost
* GeoPandas
* SciPy (cKDTree)
* imbalanced-learn (SMOTE)

**Concepts**

* Feature Engineering
* Geospatial Data Processing
* Imbalanced Learning
* Classification Modeling
* Model Evaluation

---

## Key Learnings

1. Spatial feature engineering often contributes more performance gain than model switching.
2. Evaluation metrics must align with business objectives when dealing with imbalanced data.
3. Clean preprocessing pipelines significantly improve model robustness.
4. Geospatial context provides strong predictive signals when properly engineered.

---

## Results

* Improved minority class recall using SMOTE
* XGBoost outperformed linear models in capturing nonlinear spatial relationships
* Distance-based features meaningfully increased predictive performance

---

## Future Improvements

* Add cross-validation with spatial splits
* Incorporate time-series spatial drift analysis
* Deploy as an interactive dashboard
* Experiment with deep learning models for spatial embeddings

