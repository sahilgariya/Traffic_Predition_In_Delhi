# Traffic_Predition_In_Delhi
 Machine learning project for analyzing traffic patterns and predicting traffic conditions in Delhi using historical data.

 Traffic Prediction in Delhi

A machine learning project for predicting travel time for trips in
Delhi using trip characteristics such as route, distance, time of day,
day type, weather, traffic density, road type, and average speed.

Project Overview

This project uses a Delhi traffic dataset containing 4,000 trip
records. The feature dataset contains 10 columns, while the target
dataset contains the corresponding travel_time_minutes value. The two
CSV files are connected using Trip_ID.

The notebook explores the data and builds a Linear Regression model
using a preprocessing pipeline with one-hot encoding for categorical
variables.

Dataset

The project uses two CSV files:

delhi_traffic_features.csv --- input features for each trip

delhi_traffic_target.csv --- target travel time in minutes

Feature Columns

Column                    Description

Trip_ID                 Unique trip identifier
start_area              Trip starting area
end_area                Trip destination area
distance_km             Trip distance in kilometers
time_of_day             Time period of the trip
day_of_week             Weekday or weekend
weather_condition       Weather condition
traffic_density_level   Traffic density level
road_type               Type of road
average_speed_kmph      Average speed in km/h

Target

travel_time_minutes --- predicted travel time for the trip.

Machine Learning Workflow

Load the feature and target CSV files.

Explore the dataset.

Separate input features and target.

Split the data into training and testing sets.

Encode categorical variables using OneHotEncoder.

Build a preprocessing and regression pipeline.

Train a Linear Regression model.

Generate predictions.

Evaluate the model using MAE, MSE, RMSE, and R².

Analyze model residuals.

Technologies Used

Python

Pandas

NumPy

Matplotlib

Seaborn

Scikit-learn

Jupyter Notebook / Google Colab

Model Performance

The notebook compares an initial model with an updated model.

Metric     Previous Model   Updated Model

MAE                 10.05        9.15
R²                   0.77        0.82

Updated model metrics:

MAE: 9.15 minutes

MSE: 153.37

RMSE: 12.38 minutes

R²: 0.82

The updated model improved the reported MAE and R² compared with the
previous version.

Repository Structure

Traffic_Prediction_In_Delhi/
│
├── delhi_traffic_features.csv
├── delhi_traffic_target.csv
├── Traffic_Congestion_Prediction_in_Smart_Cities.ipynb
├── README.md
└── requirements.txt

Dataset Source

The uploaded CSV files 

delhi_traffic_features.csv

delhi_traffic_target.csv


Important Note

This repository documents the dataset and analysis contained in the
accompanying notebook. The dataset is designed for machine learning and
urban mobility analysis; it should not be interpreted as a real-time
traffic monitoring system.

Future Improvements

Compare Linear Regression with tree-based regression models.

Perform stronger feature engineering.

Tune model hyperparameters where applicable.

Add cross-validation.

Build an interactive dashboard.

Deploy the prediction model as a small web application.
