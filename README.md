# Advertising Sales Prediction Model

## Overview
This project aims to build a regression model to predict sales based on advertising data from 3 different aspects: TV, newspaper, and radio. The dataset first cleaned, analyzed, and preprocessed, then a Linear Regression Model was trained on it.

## Team Members
- Ughur Babayev (Preprocessor)
- Mehdi Shukurtu (Analyst)
- Helia Abedini (Modeler)
- Shahin Safarti (Reporter)

## Dataset
- **Source**: https://www.statlearning.com/resources-first-edition
- **Size**: 200 records
- **Features**: 3 (TV, radio, newspaper)
- **Target**: Sales

## Data Analysis
- **Feature Distributions**: TV and radio spending are roughly normally distributed; newspaper spending is right-skewed.
- **Correlation with Sales**: TV (0.78), Radio (0.58), Newspaper (0.23).

## Preprocessing
- **Outlier Detection**: Outliers in newspaper capped using the IQR method.
- **Scaling**: Features standardized with StandardScaler.
- **Train-Test Split**: 80% training, 20% testing (random_state=42).

## Feature Impact
- TV: 3.839619
- Radio: 2.802285
- Newspaper: 0.057980

## Modeling
- **Algorithm**: Linear Regression
- **Evaluation Metrics**:
  - RMSE: 1.781
  - MSE: 3.171
  - R²: 0.901 (closer to 1 is better)

## Key Findings
- TV is the strongest predictor of sales (coefficient = 3.83).
- Newspaper has the least impact (coefficient = 0.058).

## Visualizations
- Available in report file.
