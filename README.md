# House Price Prediction – Data Preprocessing & Feature Engineering

This repository contains the solution to the [House Prices - Advanced Regression Techniques](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques) competition on Kaggle. It focuses on **data preprocessing and feature engineering**, essential steps before training any machine learning model.

##  Files Included

- `Data_Preprocessing_&_Feature_Engineering.ipynb` — Notebook containing all steps for preprocessing and feature engineering
- `train.csv`, `test.csv` — Raw data files from Kaggle (not included here, please download from the competition page)

## Steps Performed

### 1. Load & Combine Datasets
- Merge `train` and `test` data for consistent preprocessing.

### 2. Handle Missing Values
- Fill missing categorical values with 'None' or mode.
- Fill missing numerical values with the median.

### 3. Feature Engineering
- Create new features:
  - `TotalSF` – Total square footage of the house.
  - `TotalBath` – Total number of bathrooms.
  - `Age` – Age of the house.
  - `IsRemodeled` – Whether the house was remodeled.

### 4. Label Encoding
- Apply `LabelEncoder` to ordinal categorical features like `FireplaceQu`, `BsmtQual`, etc.

### 5. Transform Skewed Features
- Use log1p transformation for numerical columns with high skewness.

### 6. One-Hot Encoding
- One-hot encode remaining categorical variables.

### 7. Final Output
- `X`: Preprocessed training features.
- `y`: Target variable (`SalePrice`).
- `test_clean`: Cleaned test dataset for future prediction.
- `test_ID`: Test set IDs for submission alignment.

## Next Steps

Use the `X` and `y` outputs from this notebook in Part 2 for model training, evaluation, and generating Kaggle submissions.

##  Resources

- [Kaggle Competition Link](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques)
- [Data Description](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data)

##  Author

*Prepared by Sujith kumar*

