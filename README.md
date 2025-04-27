# Electricity Price Prediction Using Machine Learning

## Project Overview
This project focuses on predicting electricity prices using machine learning models. The dataset is consolidated from SHMI's weather data, electricity imports/exports, and electricity price.

## Repository Structure
```
├── Electricity_export.ipynb    # Fetches import/export electricity data from API
├── Data_consolidate.ipynb      # Merges multiple CSV files to create final_combined.csv
├── All_models_with_Lagged_TSCV.ipynb   # Runs models with lag features using Time Series Cross-Validation
├── All_models_with_NoLagged_Kfold.ipynb   # Runs models without lag features using K-Fold Cross-Validation
├── final_combined.csv          # Processed dataset used for modeling
├── README.md                   # Project documentation
```

## Dataset
- The **final_combined.csv** file is used for training machine learning models.

## Machine Learning Models
The project employs multiple machine learning models to predict electricity prices:
- **All_models_with_Lagged_TSCV.ipynb**: Uses **lag features** and applies **Time Series Cross-Validation (TSCV)**.
- **All_models_with_NoLagged_Kfold.ipynb**: Excludes lag features and applies **K-Fold Cross-Validation**.

## Key Findings
- The inclusion of **lag features** significantly improves model performance by capturing past trends.

## Prerequisites
The following Python packages should be installed before running the notebooks:

`pip install pandas numpy scikit-learn xgboost matplotlib seaborn requests tensorflow holidays`

## How to Run the Project
1. **Train Models**:
   - To train models **with lag features**, run `All_models_with_Lagged_TSCV.ipynb`.
   - To train models **without lag features**, run `All_models_with_NoLagged_Kfold.ipynb`.


