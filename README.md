
# House Price Prediction

A machine learning project that predicts house prices based on property features such as area, number of bedrooms, location, and other attributes. The project includes data preprocessing, exploratory data analysis, feature engineering, model training, and performance evaluation.

## Features

- Data cleaning and preprocessing
- Missing value handling
- Feature encoding and scaling
- Exploratory Data Analysis (EDA)
- Feature engineering
- Model training and evaluation
- Performance comparison using multiple regression models

## Features added
-HouseAge = YrSold - YearBuilt
-RemodeledAge = YrSold - YearRemodAdd
-WasRemodeled = (YearRemodAdd != YearBuilt).astype(int)
-GarageAge = YrSold - GarageYrBlt
-HouseAge2 = HouseAge ** 2

TotalSF = TotalBsmtSF + 1stFlrSF + 2ndFlrSF
TotalPorchSF = OpenPorchSF + EnclosedPorch + 3SsnPorch + ScreenPorch
TotalBathroom = FullBath + 0.5*HalfBath + BsmtFullBath + 0.5*BsmtHalfBath
LivAreaPerRoom = GrLivArea / (TotRmsAbvGrd + 1)
GarageArea_x_Cars = GarageArea * GarageCars

2ndFlrRatio = 2ndFlrSF / (TotalSF + 1)
QualxCond = OverallQual * OverallCond
QualxArea = OverallQual * GrLivArea
QualxAge = OverallQual * (HouseAge + 1)
GarageQualArea = GarageCars * GarageArea

## Tech Stack

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

## Models Used

- Linear Regression
- Random Forest Regressor
- XGBoost (optional)

## Evaluation Metrics

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

## Dataset

The project uses a publicly available House Prices dataset from Kaggle.

## Learning Outcomes

- Data preprocessing
- Feature engineering
- Regression algorithms
- Model evaluation
- Machine learning pipeline

## Exploratory Data Analysis

-An EDA report is generated using `ydata-profiling`.




