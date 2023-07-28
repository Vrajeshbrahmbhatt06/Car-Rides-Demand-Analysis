# Cab Rides Demand Analysis

This repository contains the analysis of cab ride demand data using various machine learning models. The dataset contains timestamps and various attributes related to cab rides, such as the number of rides, pick-up and drop-off locations, trip duration, and other relevant information. The main goal is to predict the number of cab rides based on different time intervals and explore the best model that fits the data.

## Libraries Used

The following Python libraries were used in this analysis:

- pandas: For data manipulation and analysis.
- numpy: For numerical computations and array operations.
- matplotlib: For creating visualizations and plots.
- seaborn: For enhancing the visualizations.
- scikit-learn: For machine learning models and evaluation metrics.
- xgboost: For XGBoost regression model implementation.
- statsmodels: For time series modeling and ARIMA regression.
- pmdarima: For automatic ARIMA model selection.

## Analysis Steps

1. Data Loading and Preprocessing:
   - Load the dataset from a JSON file and convert it into a pandas DataFrame.
   - Simplify the DataFrame and convert timestamps into a suitable format for analysis.

2. Exploratory Data Analysis (EDA):
   - Visualize the data to gain insights into the distribution of cab ride demand.
   - Use KDE plots to identify regions with the highest number of trips.
   - Create bar plots to understand the nature of the data and its trends.

3. Time Interval Transformation:
   - Split the original DataFrame into different time interval DataFrames (e.g., 15 minutes, 30 minutes, 1 day).
   - Resample the data to aggregate it into the desired time intervals.

4. Model Building:
   - Implement four regression models: Linear Regression, XGBoost Regression, ARIMA, and ARIMA AutoRegression.
   - Train each model on the data and evaluate their performance using MAE (Mean Absolute Error) and RMSE (Root Mean Square Error) metrics.

5. Model Comparison and Conclusion:
   - Compare the performance of all models based on the evaluation metrics and visualizations.
   - Conclude which model outperforms the others in capturing the trend of cab ride demand.

## Acknowledgments

Special thanks to the dataset provider for making the data available for analysis and research purposes.
