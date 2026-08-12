# Appliance Energy Consumption Forecasting

This project focuses on forecasting household appliance energy consumption for the next 24 hours using different forecasting and machine learning approaches.

## Project Overview

The Appliances Energy Prediction dataset was used for this project. The data contains appliance energy consumption along with indoor temperature, humidity and outdoor weather measurements.

The original data was converted into an hourly time series, and the `Appliances` variable was used as the target.

## Models Used

The following models were implemented and compared:

- Mean Forecast
- Naive Forecast
- Daily Seasonal Naive
- Weekly Seasonal Naive
- Drift
- SARIMAX
- Random Forest
- Chronos-Bolt

## Main Steps

1. Data loading and preprocessing
2. Conversion of data to hourly frequency
3. Exploratory data analysis
4. Seasonality analysis using ACF
5. Stationarity testing using ADF
6. Benchmark forecasting
7. SARIMAX modelling with exogenous variables
8. Feature engineering
9. Random Forest forecasting
10. Chronos-Bolt forecasting
11. Model comparison and evaluation

## SARIMAX Variables

The SARIMAX model used the following exogenous variables:

- `T_out`
- `RH_out`
- `Windspeed`
- `hour_sin`
- `hour_cos`

A 24-hour seasonal period was used to capture daily seasonality.

## Evaluation

The models were evaluated using:

- MAE
- RMSE
- MAPE

Chronos-Bolt achieved the best overall performance in the final comparison.

Dataset

The project uses the Appliances Energy Prediction dataset from the UCI Machine Learning Repository.

Dataset:
https://archive.ics.uci.edu/ml/machine-learning-databases/00374/energydata_complete.csv

Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Statsmodels
- Scikit-learn
- Chronos-Bolt
- Jupyter Notebook

 Project Files

- `forecasting.ipynb` – Main analysis and forecasting notebook
- `README.md` – Project description
- Dataset/code files – Supporting project files

 Conclusion

This project compares traditional forecasting, statistical, machine learning and foundation-model approaches for 24-hour appliance energy forecasting. The results show that different models capture different aspects of energy consumption, with Chronos-Bolt providing the best overall forecasting performance in this analysis.

