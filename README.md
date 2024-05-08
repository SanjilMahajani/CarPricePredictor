# Car Price Predictor: Project Overview

- This was a project given to us by my client it aims to create a car price predictor when different features like mileage, transmission, engineSize etc is given.
- Engineered features from the dataset to identify different relationships between the dependent and independent variables.
- Compared different models like Linear, Lasso, and Random Forest Regressors using GridsearchCV to find the best model.

## Resources and code used
The data set is from Kaggle where it has different models of Mercedes with their information like mileage, transmisson, price etc

[https://www.kaggle.com/datasets/madhurpant/data-science-jobs-in-india](https://www.kaggle.com/datasets/mysarahmadbhat/mercedes-used-car-listing)

Python Version: 3.7

Packages: pandas, numpy, sklearn, matplotlib, seaborn

 ## Data Cleaning

I needed to clean it up so that it was usable for our model. I made the following changes and created the following variables:

- Handled duplicate values
- Removed unnecessary columns and checked for missing values

## EDA

I looked at the distributions of the data and the value counts for the various categorical variables also found out different relationships between data

<img width="714" alt="Screenshot 2024-05-08 at 11 27 00 PM" src="https://github.com/SanjilMahajani/CarPricePredictor/assets/43502576/7a1db71c-61dc-4ade-add5-fbb896348e71">

<img width="717" alt="Screenshot 2024-05-08 at 11 27 38 PM" src="https://github.com/SanjilMahajani/CarPricePredictor/assets/43502576/31fa77a0-f2e6-4daa-8209-7263eef6549a">

<img width="855" alt="Screenshot 2024-05-08 at 11 28 23 PM" src="https://github.com/SanjilMahajani/CarPricePredictor/assets/43502576/4eaf26a1-618d-49f9-8e47-a40b9b9572f1">

## Model Building

First, I transformed the categorical variables into dummy variables. I also split the data into train and tests sets with a test size of 20%.

I tried three different models and evaluated them using Mean Absolute Error. I chose MAE because it is relatively easy to interpret and outliers aren’t particularly bad in for this type of model.

I tried four different models:

- Multiple Linear Regression – Baseline for the model
- Lasso Regression – Because of the sparse data from the many categorical variables.
- Random Forest – Again, with the sparsity associated with the data, I thought that this would be a good fit.

## Model performance

The Random Forest model far outperformed the other approaches.





