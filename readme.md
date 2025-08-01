# Regression Models Comparison

A comprehensive comparison of multiple regression algorithms for predicting California housing prices.

## Overview

This project evaluates the performance of various regression models on the California Housing dataset to identify the most effective algorithm for housing price prediction.

## Dataset

- **Source**: California Housing dataset from scikit-learn
- **Target**: Median house value (MedHouseVal)
- **Features**: 8 numerical features (income, age, rooms, bedrooms, population, occupancy, latitude, longitude)
- **Additional**: Synthetic categorical feature (Region: North/South based on latitude)

## Models Evaluated

| Model | R² Score | Test RMSE | Performance |
|-------|----------|-----------|-------------|
| XGBRegressor | 0.830 | 0.472 | ⭐ Best |
| RandomForestRegressor | 0.807 | 0.503 | ⭐ Second |
| GradientBoostingRegressor | 0.776 | 0.542 | ⭐ Third |
| SVR | 0.730 | 0.595 | Good |
| KNeighborsRegressor | 0.672 | 0.655 | Fair |
| DecisionTreeRegressor | 0.631 | 0.695 | Fair |
| LinearRegression | 0.585 | 0.738 | Poor |
| Ridge | 0.585 | 0.738 | Poor |
| ElasticNet | 0.203 | 1.022 | Very Poor |
| Lasso | -0.0002 | 1.145 | Failed |

## Key Findings

- **Ensemble methods** (XGBoost, Random Forest, Gradient Boosting) significantly outperform linear models
- **XGBoost** achieves the best performance with R² = 0.830
- **Linear models** struggle with the non-linear relationships in housing data
- **Lasso regression** completely fails (negative R² score)

## Installation

```bash
pip install pandas numpy scikit-learn xgboost matplotlib
```

## Usage

1. Open `Regression_models.ipynb`
2. Run all cells to reproduce the analysis
3. Results will be displayed in a formatted table

## Files

- `Regression_models.ipynb` - Main analysis notebook
- `README.md` - This file

## Dependencies

- pandas
- numpy
- scikit-learn
- xgboost
- matplotlib

## License

MIT License# all_regression_models
# all_regression_models
