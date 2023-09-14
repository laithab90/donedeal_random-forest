# Car Price Prediction using DoneDeal.ie Data

This repository contains two Jupyter notebooks that demonstrate the training of machine learning models on scraped car data from the DoneDeal.ie car website. The training dataset used in both notebooks is attached under the name "car_listing_combined.csv". These models aim to predict car prices based on various features.

## Table of Contents
- [Notebooks](#notebooks)
- [Performance Metrics](#performance-metrics)
- [Main Steps Covered](#main-steps-covered)
- [Usage](#usage)
- [Contribution](#contribution)

## Notebooks

1. **Random Forest Classifier (RFC) Notebook (`rfc.ipynb`)**: 
   - This notebook uses a classification approach to predict car prices. It categorizes the prices into different bins and then predicts which bin a car's price falls into based on its features.

2. **Random Forest Regressor (RFR) Notebook (`rfr.ipynb`)**: 
   - This notebook uses a regression approach to predict the exact price of a car based on its features.

## Performance Metrics

- **RFC Notebook**:
   - The model's performance is evaluated using the accuracy score and a confusion matrix is produced for further insights.

- **RFR Notebook**:
   - The regressor's performance is evaluated using metrics like mean squared error (MSE) and R2 score.

## Main Steps Covered

- **Data Loading**: 
   - Both notebooks load data from the attached CSV file named "car_listing_combined.csv".
  
- **Data Preprocessing**: 
   - Both notebooks preprocess the data by handling missing values, infinity values, and encoding categorical features like 'Make', 'Model', 'Transmission', 'Fuel Type', and 'Body Type' using label encoding.

- **Model Training**: 
   - The RFC notebook trains a Random Forest Classifier, whereas the RFR notebook trains a Random Forest Regressor. Both models are trained using a train-test split approach.

- **Model Evaluation**: 
   - The RFR notebook evaluates the regressor's performance using metrics like mean squared error (MSE) and R2 score.

- **Model Saving and Loading**: 
   - Both notebooks demonstrate how to save the trained models and associated preprocessing tools, like label encoders, for future use. They also show how to load these saved models and tools to make predictions on new data.

## Usage

1. Ensure you have the necessary libraries installed. Both notebooks mainly use `pandas`, `numpy`, `seaborn`, `sklearn`, and others.
2. Load your data or use the provided "car_listing_combined.csv".
3. Run the notebooks to train the models and make predictions.

## Contribution

Feel free to fork this repository and contribute by adding more features, optimizing the current models, or adding new models.
