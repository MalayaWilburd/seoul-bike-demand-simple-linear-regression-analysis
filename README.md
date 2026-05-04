# Seoul Bike Sharing Demand — Simple Linear Regression Analysis

## Overview
This project applies simple linear regression to analyze the relationship 
between temperature and hourly bike rental demand in Seoul, South Korea. 
The analysis was completed as part of a Regression Analysis course and 
demonstrates a full statistical modeling workflow from exploratory data 
analysis through model diagnostics.

## Dataset
The Seoul Bike Sharing Demand dataset contains 8,760 hourly records of 
public bike rentals collected to support demand prediction and ensure 
stable bike availability throughout the city.

**Variables include:**
- Hourly bike rental counts
- Weather conditions (temperature, humidity, wind speed, visibility, 
  solar radiation, rainfall, snowfall)
- Date and time information
- Seasonal indicators
- Holiday and functioning day status

**Source:** UCI Machine Learning Repository

## Methods
- Exploratory Data Analysis (EDA)
- Correlation matrix to identify the strongest linear predictor
- Simple Linear Regression using Least-Squares Estimation
- Hypothesis testing (α = 0.01)
- Confidence and prediction interval construction
- Residual diagnostics and heteroscedasticity evaluation

## Key Findings
- Temperature had the strongest linear correlation with hourly rentals 
  (r = 0.54)
- Estimated regression equation: ŷ = 329.95 + 29.08x
- Every 1°C increase in temperature is associated with approximately 
  29 additional bike rentals per hour
- Temperature is a statistically significant predictor 
  (F = 3,578, p ≈ 0)
- R² = 0.29 — temperature alone explains 29% of the variance, 
  indicating additional predictors are needed for a more complete model
- Residual plot revealed heteroscedasticity, further supporting the 
  need for a multi-variable approach

## Tools
- R
- Quarto

## Full Analysis
The full rendered analysis is available on RPubs:
[View Full Analysis](https://rpubs.com/mwilburd/seoul-bike-analysis)

## Files
- `Seoul_Bike_Regression.qmd` — Quarto source document
- `SeoulBikeData.csv` — Dataset
