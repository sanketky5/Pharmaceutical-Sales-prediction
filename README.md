NextHikes - Pharmaceutical Sales Prediction
Overview
This project involves building an end-to-end solution for sales forecasting across multiple stores for Rossmann Pharmaceuticals. The goal is to predict daily sales in various stores six weeks ahead of time. The project includes exploratory data analysis (EDA), data preprocessing, model building, and serving predictions through a web interface.

Table of Contents
Exploration of Customer Purchasing Behavior

Data Cleaning
Visualization and Analysis
Logging
Prediction of Store Sales

Preprocessing
Building Models with Sklearn Pipelines
Choosing a Loss Function
Post Prediction Analysis
Serializing Models
Building Model with Deep Learning
Using MLFlow to Serve Predictions
Serving Predictions on a Web Interface

Web Interface Platforms
Input Parameters
Dashboard Features

Exploration of Customer Purchasing Behavior
Data Cleaning
Cleaned the data to handle outliers and missing values.
Built pipelines for outlier detection and handling missing data.
Visualization and Analysis
Checked the distribution of promotions in both training and test sets.
Compared sales behavior before, during, and after holidays.
Explored seasonal purchase behaviors.
Analyzed the correlation between sales and the number of customers.
Investigated the impact of promotions on sales and customer behavior.
Explored trends during store opening and closing times.
Analyzed the influence of assortment type on sales.
Explored the impact of the distance to the nearest competitor on sales.
Logging
Utilized the logger library in Python to log steps and important information during the analysis.
Prediction of Store Sales
Preprocessing
Processed datetime columns to extract relevant features.
Created new features such as weekdays, weekends, days to holidays, etc.
Scaled the data using the standard scaler in sklearn.
Building Models with Sklearn Pipelines
Used sklearn pipelines for modular and reproducible modeling.
Employed Random Forest Regressor as a starting point for modeling.
Choosing a Loss Function
Chose a loss function for the regression problem and defended the choice.
Post Prediction Analysis
Explored feature importance from the modeling.
Estimated the confidence interval of predictions.
Serializing Models
Serialized models with timestamps for daily predictions.
Building Model with Deep Learning
Created a Long Short Term Memory (LSTM) model for deep learning.
Isolated the Rossmann Store Sales dataset into time series data.
Checked and differenced the time series data.
Checked for autocorrelation and partial autocorrelation.
Transformed the time series data into supervised learning data.
Scaled the data in the (-1, 1) range.
Using MLFlow to Serve Predictions
Used MLFlow to make inferences on test data.
Serving Predictions on a Web Interface
Developed a web interface using Flask to serve predictions.
Integrated input parameters for store_id, CSV file upload, and other relevant features.
Displayed predicted sales amount and customer numbers.
Provided a downloadable CSV table of predictions.
