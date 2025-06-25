<img width="1428" alt="image" src="https://github.com/user-attachments/assets/c59e3fa3-228e-4c8f-86fb-4306d97e55df" />

## Project Overview

This project aims to predict the selling prices of used vehicles for a dealership named "Cars Cars Cars".  
By applying machine learning regression techniques, the goal is to build accurate and interpretable models that assist in pricing strategy and profitability.  
The analysis includes data cleaning, exploratory data analysis, feature engineering, and a comparison of multiple regression algorithms.

## Objectives

- Load and prepare real-world vehicle data  
- Clean duplicates, check for nulls, and address skewed distributions  
- Visualize trends and feature relationships with respect to price  
- Train and compare several regression models:
  - Linear Regression  
  - Random Forest  
  - Gradient Boosting Regressor  
  - XGBoost Regressor  
- Evaluate model performance using:
  - Root Mean Squared Error (RMSE)  
  - Mean Absolute Error (MAE)  
  - R² Score  
- Select the best model and communicate findings with visual explanations

## Tools and Libraries

- Python 3.x  
- pandas  
- numpy  
- matplotlib  
- seaborn  
- scikit-learn  
- xgboost

## Project Structure

car-price-prediction-ensemble-linear-models/  
├── used_car_price_prediction_lr_rf_xgb_gb.ipynb   – Main notebook with modeling pipeline  
├── car data.csv                                   – Dataset containing used car listings  
├── README.md                                      – Project documentation  

## Dataset Description

- Features:
  - Year of manufacture  
  - Present Price (price when new)  
  - Kms Driven  
  - Fuel Type  
  - Seller Type  
  - Transmission  
  - Owner history  
- Target:
  - Selling Price (current estimated resale value)

- Insights:
  - Prices range widely (0.10 to 35 lakh) with a skew toward lower values  
  - Outliers exist for high mileage and luxury vehicles  
  - Older vehicles and diesel engines show predictable depreciation patterns

## Analysis Workflow

1. Load and inspect dataset  
2. Remove duplicate rows  
3. Handle categorical encoding (e.g. fuel, seller, transmission)  
4. Visualize price distributions and feature correlations  
5. Split into train/test sets  
6. Train the following models:
   - Linear Regression  
   - Random Forest  
   - Gradient Boosting  
   - XGBoost  

7. Evaluate each model using standard regression metrics  
8. Rank and select the best model based on lowest RMSE and highest R²  
9. Plot actual vs. predicted prices for interpretability

## How to Run

1. Clone this repository  
2. Install dependencies using pip:  
   pip install pandas numpy matplotlib seaborn scikit-learn xgboost  

3. Place `car data.csv` in the project root  
4. Open and run the notebook:  
   `used_car_price_prediction_lr_rf_xgb_gb.ipynb`

## Requirements

Install required packages with:  
pip install pandas numpy matplotlib seaborn scikit-learn xgboost

## License

This project is licensed under the MIT License. See the LICENSE file for details.
