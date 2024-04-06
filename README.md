# Indoor Temperature Forecasting Project

This project aims to forecast indoor temperatures based on various environmental and sensor data. It encompasses data preprocessing, exploratory data analysis (EDA), statistical testing, feature selection, and the application of multiple forecasting models.

## Table of Contents

- [Overview](#overview)
- [Libraries and Tools](#libraries-and-tools)
- [Data Preprocessing](#data-preprocessing)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Feature Engineering and Selection](#feature-engineering-and-selection)
- [Model Development](#model-development)
- [Challenges and Considerations](#challenges-and-considerations)
- [Conclusion](#conclusion)

## Overview

The project develops forecasting models to predict future indoor temperatures using a time series dataset containing various environmental and sensor measurements. It explores statistical methods, machine learning algorithms, and deep learning approaches for time series forecasting.

## Libraries and Tools

- **Data Handling and Analysis**: `pandas`, `numpy`, `statsmodels`
- **Machine Learning**: `scikit-learn`, `xgboost`, `lightgbm`, `catboost`
- **Deep Learning**: `PyTorch`
- **Visualization**: `matplotlib`, `seaborn`
- **Others**: `pmdarima` for ARIMA modeling, `shap` for model explainability, Google Colab tools

## Data Preprocessing

- Data is loaded from CSV files and processed to combine date and time into a datetime index.
- Missing timestamps are checked and handled appropriately.
- Data normalization and logarithmic transformations are applied to certain variables.

## Exploratory Data Analysis (EDA)

- Visualization techniques such as boxplots, violin plots, and line plots are used to explore the distributions and trends of the dataset's variables.

## Feature Engineering and Selection

- **VIF Analysis**: Conducted to reduce multicollinearity among features by removing highly correlated variables.
- **Lagged Features**: Created to incorporate past observations as features for forecasting future values.
- **PCA**: Employed for dimensionality reduction on the reshaped time series data.

## Model Development

- **Statistical Methods**: Includes Exponential Smoothing, ARIMA, and VAR.
- **Machine Learning**: Utilizes Random Forest, XGBoost, and LightGBM models.
- **Deep Learning**: Applies LSTM models using PyTorch for forecasting.
- **Evaluation**: Models are compared using metrics such as RMSE, MAE, and R2.

## Challenges and Considerations

- **Computational Resources**: Limitations encountered with ARIMA and SARIMAX models, leading to data reduction.
- **Data Stationarity**: Augmented Dickey-Fuller test applied to ensure stationarity, a key assumption for time series models.

## Conclusion

The project demonstrates a thorough approach to forecasting indoor temperatures, showcasing the workflow from preprocessing and EDA to modeling and evaluation. It highlights the versatility and complexity of time series forecasting in real-world scenarios.

