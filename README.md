# Predicting Iron Content in Iron Ore Using Machine Learning

## Overview
This project focuses on predicting the iron content in iron ore using machine learning techniques.
The primary goal is to develop a model that can accurately estimate the iron content based on various features extracted from iron ore data.
The project involves data preprocessing, feature engineering, model training, and evaluation.

## Methodology

### Data Preparation

#### 1.Data Import and Exploration: 
The dataset is imported from a CSV file containing raw data on iron ore samples. The data includes features like iron concentration, silica content, and other relevant variables.

#### 2.Data Cleaning: 
Missing values are handled, and outliers are identified and removed using the Z-score method to ensure data quality.

#### 3.Feature Engineering:
New features are created by combining similar columns to reduce dimensionality and improve model performance. For example, air flow and level data from different flotation columns are averaged.

### Model Development

#### 1.Scaling Data:
MinMaxScaler is used to normalize the feature values, ensuring that all features contribute equally to the model.

#### 2.Model Training:
Several regression algorithms are evaluated, including Linear Regression, Ridge Regression, Lasso Regression, K-Nearest Neighbors (KNN) Regressor, and Decision Tree Regressor. Pipelines are created for each algorithm to streamline the process of scaling and fitting the models.

#### 3.Model Evaluation:
Cross-validation is performed to assess model performance, using metrics such as Root Mean Squared Error (RMSE) and R² score. The KNN Regressor is found to have the best performance based on RMSE and accuracy.


## Results
The final model, KNN Regressor, is trained on the scaled data and evaluated on the test set. The performance metrics, including RMSE and R² score, are reported. A scatter plot visualizes the relationship between actual and predicted iron content, providing insights into model accuracy.

## Usage
To run this project, clone the repository and follow these steps:

• Install the required dependencies from requirements.txt.<br>
• Download the Dataset from link "https://www.kaggle.com/datasets/edumagalhaes/quality-prediction-in-a-mining-process".<br>
• Execute the Jupyter notebook or Python script to preprocess the data, train the models, and evaluate their performance.<br>

