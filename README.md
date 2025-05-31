# Housing_Data_Feature_Engineering

## Project Overview
This project focuses on improving the performance of a machine learning model through feature engineering using the Kaggle House Prices dataset. The goal is to build a regression model to predict house prices, enhance it by creating new features, and compare its performance against a baseline model without feature engineering.

## Dataset
The dataset used in this project is the Kaggle House Prices dataset, available here: https://drive.google.com/file/d/1U_C-gWb6VwkSHAkru6tzAiufLJLY009B/view?pli=1

## Key Insights

### Data Cleaning & Preprocessing
1. One-Hot Encoding: Converted the furnishingstatus categorical column into numerical features using one-hot encoding (dropping one category to avoid multicollinearity).

2. Boolean Handling: Converted any True/False values to 1/0 for modeling compatibility.

### Feature Engineering
Created the following new features to improve predictive power:
- total_rooms = bedrooms + bathrooms
- area_per_room = area ÷ total_rooms
- total_amenities = Sum of all binary amenity columns (mainroad, basement, airconditioning, etc.)

### Visualizations Created
- Top 10 Feature Importances: A horizontal bar plot showing the most important features (after engineering) ranked by the Random Forest model.
- Model Performance Comparison (R² Score): A bar plot comparing the model performance with and without feature engineering based on the R² metric.

### Model Training & Evaluation
1. Built two Random Forest Regression models:
- Basic Model: Used original features only.
- Enhanced Model: Included new engineered features.

2. Used an 80-20 train-test split for evaluation.

3. Compared model performance using: R-squared (R²) Score

Result: The model with feature engineering showed a clear improvement in predictive performance over the basic model.

## Tools and Libraries Used
- Pandas 
- NumPy 
- Matplotlib
- Seaborn 
- Scikit-learn 
- Jupyter Notebook / Google Colab 
