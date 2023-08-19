# Lab1 - Scikit-learn

## Goal

The goal of this lab is to become familiar with the scikit-learn library.

You will practice loading example datasets, perform classification and regression with multiple scikit-learn models, and compare results between using all features and two principal components as features.

## What to do

Follow `lab1.ipynb`. Here is an overview.

### Datasets
yellowbrick spam - classification  
https://www.scikit-yb.org/en/latest/api/datasets/spam.html

yellowbrick energy - regression  
https://www.scikit-yb.org/en/latest/api/datasets/energy.html

### Classifiers
sklearn LogisticRegression 

`from sklearn.linear_models import LogisticRegression` 

https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html

sklearn RandomForestClassifier (`random_state=88`)

`from sklearn.ensemble import RandomForestClassifier`

https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html


### Regressors
sklearn LinearRegression 

`from sklearn.linear_models import LinearRegression`

https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LinearRegression.html

sklearn RandomForestRegressor (`random_state=88`)

`from sklearn.ensemble import RandomForestRegressor`  

https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestRegressor.html

### Steps

For each dataset and the corresponding models apply the five step process in _Python Data Science Handbook_ Chapter 5:
1. Load and arrange data into feature matrix and target vector
2. Choose model class (from the list above)
3. Instantiate model as directed
4. Fit model to data
5. Predict values for new data and evaluate results with `accuracy_score()`(classification) or `mean_squared_error()` (regression).

In step 1. use `train_test_split(X, y, random_state=956)` to create a training set (used in step 4.) and validation set (used in step 5.).

Repeat the above process by using only the first two principal components of the feature matrix as features for classification/regression. Include a 2D plot of the data using the first two principal components.

### Specifications
Write the following functions: 
- `get_classifier_accuracy()`
- `get_regressor_mse()`
- `get_n_principal_components()`

Function headers and documentation are included in `lab1.ipynb`. Implement the function body accordingly.

Use these functions to implement the tasks as directed and answer the questions below in the corresponding section in the notebook.

### Questions
1. For each task (classification and regression), which model performs best on the validation data using all features?
2. For each task (classification and regression), which model performs best on the validation data using two principal components?
3. In each task (classification and regression), for each model, how do full feature and two principal component model scores compare on the validation data?
4. Do any of the models underfit or overfit? Provide examples.

Use your results to justify/motivate your answers.

## What to hand in
- In the Jupyter notebook `lab1.ipynb` implement the steps above as indicated. 
- Keep code clean and remove any unnecessary cells. 
- Use the results obtained to answer above questions in a section called *Observations/Interpretation*. 
- In a section *Reflection*, include a sentence or two about what you liked/disliked, found interesting/confusing/challangeing/motivating while working on this assignment.

During development, checkin progress with git and use descriptive commit messages.
