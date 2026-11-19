
# California Housing Price Prediction

## Project Overview
This project focuses on predicting median house values using the California Housing dataset. It applies data preprocessing, feature engineering, multicollinearity analysis, and regression techniques to build and evaluate predictive models.

## Objectives
- Explore and understand the dataset.
- Handle missing values.
- Perform feature engineering.
- Analyze correlations and multicollinearity using VIF.
- Standardize numerical features and encode categorical variables.
- Train and compare OLS, Ridge, and Lasso regression models.
- Tune hyperparameters using GridSearchCV.
- Evaluate model performance using RMSE, MAE, and R².

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Statsmodels
- Jupyter Notebook

## Dataset
The California Housing dataset contains information about housing districts in California.

**Target Variable:** `median_house_value`

**Important Features:**
- Longitude and Latitude
- Housing Median Age
- Total Rooms and Total Bedrooms
- Population and Households
- Median Income
- Ocean Proximity

## Feature Engineering
Created additional features:
- Rooms per Household
- Bedrooms per Room
- Population per Household
- Income × Rooms interaction feature

## Models Implemented
1. Ordinary Least Squares (OLS) Regression
2. Ridge Regression (L2 Regularization)
3. Lasso Regression (L1 Regularization)

GridSearchCV was used to tune Ridge and Lasso regularization parameters.

## Model Performance

| Model | RMSE | MAE | R² Score |
|---|---:|---:|---:|
| OLS | 72977.49 | 51116.28 | 0.59358 |
| Ridge | 72984.40 | 51123.55 | 0.59351 |
| Lasso | 72977.03 | 51116.77 | 0.59359 |

Lasso achieved the lowest RMSE and highest R² score, although the differences between the models were very small.

## Visualizations
- Correlation Heatmap
- Actual vs Predicted Values
- Residual Distribution
- Regression Model Performance Comparison

## Key Learnings
- Data cleaning and missing-value imputation
- Feature engineering and preprocessing
- Multicollinearity analysis using VIF
- Linear regression and regularization techniques
- Hyperparameter tuning using GridSearchCV
- Model evaluation and visualization

## Project Files
- `California Housing Price Prediction.ipynb` – Complete implementation and analysis.
- `California_Housing_Dataset.csv` – Dataset used for modelling.

## Conclusion
This project demonstrates an end-to-end regression workflow, from data exploration and preprocessing to model training, evaluation, and comparison. It provided practical experience with regularized regression techniques and model performance analysis.
