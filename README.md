# cross-validated-ML-model
A cross validated machine learning model that produces predictions for given testing data. It is a linear model that includes polynomial features.
This is a project completed for my 'Artificial Intelligence with Machine Learning' class. I really enjoyed tweaking the model to optimize the model's prediction results!

Project Overview

This project uses cross-validation and grid search to select an effective regression model for an unfamiliar numerical dataset.
The main objective was to compare different polynomial degrees, regularization methods, and alpha values to identify the model configuration with the lowest estimated prediction error.

Methods

The project uses a Scikit-learn pipeline containing:

Polynomial feature transformation
Feature standardization
Target standardization
Lasso or Ridge regression
Five-fold cross-validation
Grid search for hyperparameter tuning

Using a pipeline ensures that preprocessing and model training are applied consistently during every cross-validation fold.

Models Evaluated

The grid search compared:

Lasso regression
Ridge regression
Polynomial degrees of 1, 2, and 3
Alpha values of 0.01, 0.1, 1, 10, and 100

Model performance was evaluated using root mean squared error (RMSE). A lower RMSE indicates that the model’s predictions are generally closer to the actual target values.

Results

GridSearchCV selected the following configuration:

Regression model: Ridge
Polynomial degree: 2
Alpha: 1
Estimated RMSE: Approximately 22.8

This means that the selected model’s predictions were typically about 23 target units away from the actual values.

The optimized model was then used to generate predictions for a separate grading dataset.

Technologies Used
Python
pandas
NumPy
Scikit-learn
Jupyter Notebook
Kaggle
Key Concepts Demonstrated
Train/test splitting
Machine learning pipelines
Polynomial regression
Feature scaling
Lasso and Ridge regularization
K-fold cross-validation
Hyperparameter tuning with GridSearchCV
Regression evaluation using RMSE and R²
Files
cross-validation-ml-model.ipynb — Complete project notebook
