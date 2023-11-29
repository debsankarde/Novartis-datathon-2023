# Novartis-datathon-2023
# Daily Sales Problem: Project Summary

## 1. Context

In our organization, making accurate predictions of future sales is crucial for the finance team. The focus of this challenge, known as the "Daily Sales Problem," is a reflection of a real-world issue that we regularly face. By introducing this challenge to the data science community, we are offering an opportunity to tackle a problem that is of significant importance to us.

Our current strategy for sales prediction relies on monthly forecasts. Due to the dynamic nature of our business, we need to examine daily sales patterns more closely. This approach is particularly important for analyzing the performance of specific country-brand combinations, allowing us to predict whether a particular country-brand will perform above or below the expected target.

## 1.1. Daily Sales Phasing

### 1.1.1. Definition

Daily Sales Phasing is a crucial metric that assists in evaluating the accuracy of our monthly sales forecasts on a daily basis. It represents the ratio of sales for each working day within a month. Ideally, if an equal amount is sold every working day, the phasings for that month would average around 1/20, assuming a standard work month.

### 1.1.2. Importance

Understanding Daily Sales Phasing is essential because sales distribution is not uniform throughout the month. Shipping and sales patterns can vary significantly between different countries and brands. For example, Country A might show a shipping pattern dependent on weekdays, while Country B's pattern could correlate more with the working date number.

## 2. The Challenge

The goal of this challenge is to develop innovative solutions for accurate prediction and analysis of Daily Sales Phasing, taking into account the unique shipping patterns associated with different countries and brands. By achieving this, we aim to enhance the precision of our sales forecasts and align our business strategies more closely with real-time market dynamics.

## 3. Dataset Description
This project includes several datasets, each serving a specific purpose in the analysis and modeling process. Below is a detailed description of each file:

### 3.1. train_data.parquet:

Description: This file contains sales data relevant for Exploratory Data Analysis (EDA).
Time Range: The dataset spans from 2013 to 2022.
Usage: Ideal for initial data exploration and understanding trends, patterns, and anomalies in the sales data over the specified period.

### 3.2. submission_data.parquet:

Description: Testing dataset intended for use with the forecast model.
Time Range: Contains data for the latest available year, 2022.
Usage: Utilized for evaluating the model's forecasting performance on unseen data.

### 3.3. cleaned_training_data.csv:

Description: Cleaned version of the training data.
Details: This file represents the train_data.parquet after preprocessing steps such as handling missing values, outliers, and feature engineering.
Usage: Ready for use in model training, ensuring the model learns from quality data.

### 3.4. cleaned_submission_data.csv:

Description: Cleaned version of the testing data.
Details: Preprocessed form of submission_data.parquet, making it suitable for final model testing.
Usage: To be fed into the trained model for generating predictions.

### 3.5. submission.csv:

Description: Final testing dataset with prediction results.
Details: Contains the output from applying the trained model to cleaned_submission_data.csv.
Usage: Useful for analysis of model performance, comparison with actuals (if available), and for submission in case of competitions or reporting.