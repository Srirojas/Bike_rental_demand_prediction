# Bike Rental Demand Prediction

## Project Overview
This project focuses on predicting bike rental demand using machine learning algorithms. By analyzing historical rental data, we determine the best-performing model to help rental companies optimize their operations and plan resources efficiently.

## Objective
 - Identify the key factors influencing bike rentals.
 - Compare multiple machine learning models to determine the most accurate predictor.
 - Help businesses forecast demand based on seasonality, weather, and working days.

## Dataset
 - Shape: (731, 14) → 731 days of bike rental data
 - Features:
#### Categorical Columns (Encoded):
season, mnth, holiday, weekday, workingday, weathersit
#### Numerical Columns (Normalized):
temp, atemp, hum, windspeed
 - Target Variable: rentals (Number of bikes rented)
 - Excluded Columns: instant, dteday, yr (Not relevant for prediction)

## Machine Learning Approach

1.Data Preprocessing
 - Encoded categorical features
 - Normalized numerical variables

2.Model Selection & Training
 - Applied Linear Regression
 - Compared with Random Forest Regressor & XGBoost Regressor

3.Performance Evaluation
 - Used R² Score to measure model accuracy
 - Random Forest Regressor performed best, achieving the highest accuracy

## Key Observations
### Feature Impact:
 - Weather & temperature have a significant effect on rentals.
 - Weekends & holidays see different rental trends.
### Model Comparison:
 - Linear Regression → Decent fit but underperforms on complex relationships.
 - XGBoost Regressor → Strong performance but slightly less than Random Forest.
 - Random Forest Regressor → Best model with the highest accuracy.
### Takeaway:
A comparative study of models helps in choosing the most optimal algorithm for real-world deployment.

## Visualization
Feature importance plot shows the impact of different variables on bike rental predictions:

## Technologies Used
 - Python
 - Pandas, NumPy – Data handling
 - Matplotlib, Seaborn – Data visualization
 - Scikit-learn – ML models & evaluation
 - XGBoost, Random Forest, Decision Trees – Predictive models

## Results & Impact
 - Random Forest Regressor achieved the highest accuracy.
 - Feature importance analysis helped understand rental trends.
 - Insights can help rental companies optimize pricing & inventory.
