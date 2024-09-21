# Capstone-Walmart
Walmart Sales Forecasting Project
This repository contains the code and documentation for a time series forecasting model aimed at predicting Walmart's weekly sales. The model is designed to help Walmart manage its inventory by forecasting future demand, allowing the company to make informed supply chain decisions.

Table of Contents
Problem Statement
Project Objective
Data Description
Data Preprocessing
Algorithm Selection
Assumptions
Model Evaluation
Inferences
Future Possibilities
Conclusion
Problem Statement
Walmart, a retail chain with multiple outlets, faces challenges in managing its inventory. The goal is to forecast sales for a given number of months or years in order to match demand with supply.

Project Objective
The main objective of this project is to provide insights into weekly sales forecasts starting from January 2013. The model aims to optimize inventory levels and prevent underutilized or undersold items from piling up.

Data Description
Null values and duplicates were handled appropriately.
Features such as Store, Holiday_Flag, Temperature, Fuel_Price, CPI, and Unemployment were dropped to simplify the dataset.
The sales data exhibited a seasonal pattern, particularly with peaks during December-January (Christmas season).
Data Preprocessing
Non-relevant columns were removed.
The date column was converted to datetime format.
The dataset was formatted to be compatible with time series algorithms.
Algorithm Selection
Based on the weekly sales data and the need for time-based forecasting, the Prophet algorithm was chosen for this project. Prophet is particularly suitable for time series forecasting due to its ability to model seasonality and trends without requiring the data to be stationary.

Assumptions
The project is treated as a time series forecasting problem.
Sales peaks are expected every Sunday and drop midweek (Wednesday).
Model Evaluation
The model uses Prophet, which is well-suited for handling seasonality and trends in time series data. Although no formal evaluation metric was used, the seasonality was captured accurately.
Inferences
The model follows the seasonal patterns in the data.
It forecasts weekly sales for Walmart stores in the US.
Future sales forecasts may experience fluctuations due to noise in the data.
Future Possibilities
Expand the model to forecast sales in regions outside the US.
Conduct more thorough evaluations by using historical data to validate the forecasts.
Experiment with other algorithms like ARIMA or SARIMA to compare performance.
Conclusion
This project demonstrates a time series forecasting approach using the Prophet library. While alternative models like ARIMA and SARIMA could have been explored, Prophet was chosen for its simplicity and ease of use. Future iterations of the project may include enhanced visualizations and deeper evaluations of the model's performance.
