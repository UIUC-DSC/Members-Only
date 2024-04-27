# Members-Only

Designed a predictive model on recidivism among Champaign-Urbana inmates. Determines most influential factors when predicting repeat offenders.

## Data Cleaning

Filtered dataset to Champaign-Urbana inmates and removed any unnecessary columns. We chose descriptive features that work well for our model.

Used MICE (Multiple Imputation by Chained Equations) to convert our categorical variables into numerical (indicator) variables using a label encoder. This allowed us to impute NaN’s accurately.

## Model

With our dataset being primarily discrete data and we want to predict whether or not a specific inmate will be re-incarcerated, we chose classification and used Python’s machine learning library [Pycaret](​​https://pycaret.gitbook.io/docs) to test numerous classification models. from which we chose Gradient Boosting as it had the highest accuracy.

Gradient Boosting uses an iterative approach to improve the model with machine learning by targeting errors. This was an effective and accurate way to deal with our complex dataset (many different categorical and numerical data).

Plan to integrate a UI to search by inmate jacket number or other features to see whether or not they would be incarcerated again in the future.

