# Housing_Price_Prediction_Model
This repository contains a google colab Notebook (Housing_Price_Prediction_Model.ipynb) for predicting housing prices using various regression techniques and data preprocessing methods. The notebook demonstrates a complete workflow—from loading the dataset, performing exploratory data analysis (EDA), feature engineering, encoding categorical variables, to training and evaluating a regression model.

Overview:
The notebook covers the following steps:

1. Data Loading & Exploration
Loads housing data from Housing.csv.
Displays the first few rows to understand the features.

2. Exploratory Data Analysis (EDA)
Visualizes numerical features (area, bedrooms, stories, parking) using boxplots to identify outliers.
Shows distribution of features with histograms.
Displays a correlation matrix heatmap to understand relationships between variables.

3. Data Preprocessing
One-hot encodes categorical variables: mainroad, furnishingstatus, guestroom, hotwaterheating, prefarea, basement, airconditioning.
Feature engineering: creates new features such as total_rooms, price_per_sqft, and area_air.

4. Model Preparation
Splits the data into features (X) and target (Y - price).
Applies polynomial feature transformation for regression.
Splits the dataset into training and test sets.
Scales the features using StandardScaler.

5. Model Training & Evaluation
Trains a LinearRegression model on polynomial features.
Evaluates the model using metrics like Mean Squared Error (MSE), R² score, and Mean Absolute Error.

File Description:

Housing_Price_Prediction_Model.ipynb: Main notebook containing code for EDA, preprocessing, feature engineering, modeling, and evaluation.

Housing.csv: The dataset used for training and testing the model (make sure this file is in the project directory).

Features Used:

Numerical: area, bedrooms, bathrooms, stories, parking

Categorical: mainroad, guestroom, basement, hotwaterheating, airconditioning, prefarea, furnishingstatus

Engineered: total_rooms, price_per_sqft, area_air

Model:

Polynomial Regression using LinearRegression from scikit-learn.

Feature scaling and train-test splitting included.

Visualization:

Boxplots and histograms for feature distribution.

Heatmap for feature correlation.
