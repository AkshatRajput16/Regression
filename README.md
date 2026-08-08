# Insurance Cost Prediction using Linear Regression

## About

This project revolves around a medical insurance dataset.
The main aim here is to predict a person's insurance charges using Linear Regression.

## Dataset

The dataset includes the following columns:

- age
- sex
- bmi
- children
- smoker
- region
- charges

In this case, `charges` serves as the target variable.

-What I did
Throughout this project, I:

- Loaded the dataset with Pandas
- Conducted some basic data visualization
- Transformed categorical values into numerical ones
- Applied One Hot Encoding to the `region` column
- Divided the data into training and testing sets
- Trained a Linear Regression model
- Made predictions on the test data
- Evaluated the model using the R² score
- Introduced interaction features to enhance the model

## Model

I utilized Linear Regression from Scikit-learn.

```python
from sklearn.linear_model import LinearRegression

model = LinearRegression()

model.fit(X_train, y_train)

y_pred = model.predict(X_test)
