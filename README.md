# Car_price_prediction_using_gradient_boosting
## Numerical Methods project from Practicum by Yandex

### Goal

Develop a model for Rusty Bargain used car sales service to determine the market value of a car based on historical data (technical specifications, trim versions, and prices).

Key metrics:

- the quality of the prediction
- the speed of the prediction
- the time required for training

### This project's repo includes the following files:

- The project's jupyter notebook (Car_price_prediction_using_gradient_boosting.ipynb);
- A pdf format of the notebook (Car_price_prediction_using_gradient_boosting.pdf);
- Input data (car_data.csv.zip);
- Project description from Practicum (Num_Methods_project_description.pdf);

### We have completed the following steps in this project:

1. Descriptive statistics. We found missing values, wrong features format, 6 categorical features, possible ouliers in several variables.
2. Data preprocessing. We have converted column names to lower case, changed data type, filled in missing values and removed duplicates.
3. EDA. We have checked for outliers 5 variables, created a new featured (car_age) and dropped non-informative columns.
4. Encoding of categorical variables. All categorical variables were one-hot encoded.
5. Splitting data into train, validation and test sets. Data was split into 3 sets to perform best model selection.
6. Standard scaling
7. Model selection. We have compared Linear Regression, Random Forest, XGBoost, LightGBM and CatBoost models. We have also tuned a few hyperparameters for these algorithms. We have chosen the tuned CatBoost model based on RMSE score and training and prediction speed.
8. Retrain the best tuned model. The best model was retrained on the whole training data set in order to increase the volume of data it can learn from. The test score has slightly improved thanks to this step.
9. Sanity check. The test score of the Linear regression model, that we use as a baseline to analyze the model quality, is 43.54% higher than our final chosen model. It means that the modeling was useful.

### Results

**The CatBoost model with the tuned hyperparameters** has shown the best results (test RMSE of 1524, time of training 27 seconds, time of prediction 0.11 seconds) in terms of both quality and speed of training and prediction.

### Logbook

### The logbook of this project can be found [here](https://docs.google.com/spreadsheets/d/1SrGdReexaSEomJGS6yR6cRwJtHA_XqpprnLaE7B6Ayg/edit#gid=14154505) (Num Methods).
Total time spent on the project: 13.7 hours with a daily average of 2.03 hours working for 7 days.
