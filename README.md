# Electricity Demand Forecasting

This project focuses on forecasting electricity demand using time series techniques and machine learning.
A significant portion of the time series analysis and modeling is done using the `skforecast` library.

## General Description

The project performs a comprehensive analysis to predict electricity demand. The main steps include:

1.  **Data Loading and Preprocessing**: Electricity demand data is loaded and prepared for analysis. This includes cleaning the data and converting it to the appropriate format.
2.  **Feature Engineering**: New features are created from the existing data to help the model make better predictions. These features can include information about time (hour, day, month), weather (temperature), and holidays.
3.  **Model Training**: A machine learning model (LightGBM) is used to learn from the data and make predictions of electricity demand.
4.  **Model Evaluation**: The accuracy of the model is measured to ensure the predictions are reliable.

## Summary of Results

The project compares several models to predict electricity demand. The best model achieves a Mean Absolute Error (MAE) of 115.570, indicating good accuracy in the predictions.

| Model                          | MAE     |
|---------------------------------|---------|
| Baseline                        | 308.375 |
| LGBM Base                       | 225.521 |
| LGBM + External Variables       | 141.615 |
| LGBM + Parameter Selection      | 132.742 |
| LGBM + Feature Selection        | 131.857 |
| Multi-Step Forecasting          | 115.570 |
