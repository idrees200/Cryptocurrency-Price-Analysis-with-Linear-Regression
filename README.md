# Cryptocurrency Price Analysis with Linear Regression

This repository contains code to analyze cryptocurrency price data using linear regression for forecasting and visualization purposes.

## Overview

The code uses historical price data of Bitcoin from a CSV file (`12_coin_Bitcoin.csv`). It performs the following tasks:

1. **Data Preprocessing**:
   - Loads the data from CSV and calculates the target variable (`Target`) as the average of 'Low' and 'High' prices.
   - Drops unnecessary columns ('Open', 'Close', 'Name', 'Symbol').
   - Converts the 'Date' column to datetime format and converts dates to numerical format using `date2num` from Matplotlib.

2. **Model Training**:
   - Splits the dataset into training and testing sets (70% training, 30% testing).
   - Uses Linear Regression (`LinearRegression` from scikit-learn) to train a model to predict the target variable (`Target`).
   - Evaluates the model using Mean Absolute Error (MAE) and Mean Squared Error (MSE) metrics on the test set.

3. **Forecasting**:
   - Generates a forecast for the next two months using the trained model.
   - Prints the forecasted price at the end of 2 months.

4. **Visualization**:
   - Plots a scatter plot of actual test data points against dates.
   - Fits a polynomial regression line to visualize the trend in cryptocurrency prices over time.

## Instructions to Run

1. Clone or download the repository.
2. Install Python 3.x and necessary libraries (`pandas`, `numpy`, `scikit-learn`, `matplotlib`).
3. Ensure the CSV file (`12_coin_Bitcoin.csv`) is in the same directory as the Python script.
4. Run the Python script (`analysis.py`) to execute the code.
5. The script will display MAE, MSE, forecasted prices, and a visualization of the cryptocurrency price trends.

## Requirements

- Python 3.x
- pandas
- numpy
- scikit-learn
- matplotlib

## Future Improvements

- Include more advanced forecasting techniques such as ARIMA or Prophet.
- Enhance visualization with interactive plots using Plotly or Bokeh.
- Implement cross-validation for model evaluation to ensure robustness.
![image](https://github.com/idrees200/Cryptocurrency-Price-Analysis-with-Linear-Regression/assets/113856749/733ed66a-b5f0-4aff-8bb9-58d0a4510212)

