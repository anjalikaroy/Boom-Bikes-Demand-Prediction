# Boom Bikes Demand Prediction

## Problem Statement
Boom Bikes, a bike-sharing service provider, wants to understand the factors affecting the demand for shared bikes. The goal is to build a model that can accurately predict bike demand based on various environmental and seasonal factors.


## Objective
To identify the key variables influencing bike demand and build a regression model to predict the number of bikes rented.


## Dataset
The dataset contains information about daily bike rentals along with environmental and seasonal variables such as:
- Temperature
- Humidity
- Windspeed
- Season
- Weather conditions
- Working day / Holiday
- Year and month

The target variable is:
- `cnt` → Total number of bike rentals


## Approach
- Data Cleaning and preprocessing
- Handling categorical variables using dummy encoding
- Feature scaling using standardization
- Exploratory Data Analysis (EDA) to understand relationships
- Splitting data into train and test sets
- Model building using Linear Regression
- Feature selection using Recursive Feature Elimination (RFE)
- Model refinement based on statistical significance (p-values)
- Checking assumptions of Linear Regression:
  - Linearity
  - Normality of residuals
  - Homoscedasticity
  - Multicollinearity (using VIF)

## Tech Stack
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Scikit-learn  
- Statsmodels  

## Key Insights
- Temperature is positively correlated with bike demand
- Humidity and windspeed negatively impact demand
- Year (growth trend) significantly increases demand
- Weather conditions such as clear weather lead to higher rentals
- Seasonal variations strongly influence bike usage


## Model
A Multiple Linear Regression model was built to predict bike demand.

Feature selection was performed using:
- RFE (Recursive Feature Elimination)
- Statistical significance (p-values)
- Variance Inflation Factor (VIF)

## Results
- Achieved a good fit with high R-squared value on training data
- Model performed well on test data with minimal overfitting
- Residual analysis confirmed model assumptions were satisfied


## Outcome
Developed a regression model capable of predicting bike demand and identifying key influencing factors.


## Business Impact
This model can help:
- Optimize bike availability across locations
- Improve operational planning
- Understand seasonal and weather-based demand trends
- Support data-driven decision making

## Future Improvements
- Use advanced models like Random Forest or XGBoost
- Include time-based trends and lag features
- Build a real-time prediction system
- Deploy as a web application/dashboard


## Project Structure
```text
boom-bikes-demand-prediction.ipynb
README.md
