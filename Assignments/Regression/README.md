<h1>Linear Models - Regression and Logistic Regression</h1>

<b>Task:</b> Use data from two [Kaggle](https://www.kaggle.com) datasets to achieve a score that would rank in the top 75th percentile.

<b>Due date:</b> TBD

<b>Datasets:</b>
  - [Regression](https://en.wikipedia.org/wiki/Regression_analysis) - [Allstate Claims Severity]( https://www.kaggle.com/c/allstate-claims-severity/data)
  - [Logistic Regression](https://en.wikipedia.org/wiki/Logistic_regression) - [Springleaf Marketing](https://www.kaggle.com/c/springleaf-marketing-r    esponse/data)


<b>Deliverables:</b>
  - 2 screenshots  of your Kaggle submissions with scores in the top 75th percentile

  - File(s) of your code


<h3><b>Assignment:</b><h3>

<b>Part 1:</b> Regression

1. Download the dataset from [https://www.kaggle.com/c/allstate-claims-severity/data](https://www.kaggle.com/c/allstate-claims-severity/data)

2. Load the train and test datasets into pandas dataframes

3. Figure out which variables are categorical and which are numeric. Linear models only accept numeric continuous variables. You can either drop the categorical columns OR turn them into numeric variables (one-hot encoding, perturbed rate-by-level, label encoding, BLUP, etc). Many times these columns are vary useful and dropping them will hurt your model.

4. Feed your data in sci-kit learns Linear Regression algorithm. Sample code below:
  ```
  from sklearn import linear_model
  import numpy as np
  # Create linear regression object
  regr = linear_model.LinearRegression()

  # Train the model using the training sets
  # you will need to split the data into two data
  # frames one with only the Y column and one with all Xs
  regr.fit(X_train, y_train)

  # Evaluation metrics on test data
  # The coefficients
  print('Coefficients: \n', regr.coef_)
  # The mean squared error
  print("Mean squared error: %.2f"
        % np.mean((regr.predict(X_train) - y_train) ** 2))
  # Explained variance score: 1 is perfect prediction
  print('Variance score: %.2f' % regr.score(X_train, y_train))
  ```

5. Run predictions on test set and create a submission csv file to submit to Kaggle.

  ```
  predictions = regr.predict(X_test)
  # CRATE YOUR SUBMISSION FILE HERE
  ```
