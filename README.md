# House Prices – Advanced Regression Techniques (Kaggle)

This repository contains my work for the [House Prices: Advanced Regression Techniques](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques) competition on Kaggle.

## Overview
The goal of this competition is to predict the final sale price of homes in Ames, Iowa based on 79 explanatory variables describing various aspects of each house. This is a classic regression problem.

## Approach
- **Data Exploration**: inspected missing values, feature distributions, and the target variable `SalePrice`.
- **Preprocessing**: median imputation, one-hot encoding for categorical variables, scaling of numerical variables, and log-transforming the target variable.
- **Models**:
  - A simple Artificial Neural Network (ANN) with one dense layer.
  - A tuned Random Forest Regressor.
- **Evaluation**: Compared validation metrics; the ANN with log-transformed target performed slightly better.

## Results
On the validation set, the simple ANN with log-transformed target slightly outperformed the Random Forest.
However, on the public leaderboard the tuned Random Forest Regressor achieved a better score:

ANN (validation): RMSE ≈ 23 138; public LB score ≈ 0.15286

Random Forest (validation): RMSE ≈ 24 924; public LB score ≈ 0.13963

Rank (Random Forest submission): 1791 out of 4093 participants at the time of submission

## Files
- `HousePrices_ANN_vs_RF.ipynb`: Jupyter notebook containing data exploration, preprocessing, model training, and submission generation.
- `submission.csv`: my Kaggle submission file.

## Future Work
Further improvements could include deeper neural networks, more extensive feature engineering, and ensemble methods (e.g., blending ANN, Random Forest, and Gradient Boosting).

