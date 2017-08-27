<h1>Linear Models & Ensembles - Regression, Logistic Regression, & Classification</h1>

<b>Task:</b> Use data from three [Kaggle](https://www.kaggle.com) datasets to achieve a score that would rank in the top 75th percentile.

<b>Due date:</b> TBD

<b>Datasets:</b>
  - [Regression](https://en.wikipedia.org/wiki/Regression_analysis) - [Allstate Claims Severity]( https://www.kaggle.com/c/allstate-claims-severity/data)
  - [Logistic Regression](https://en.wikipedia.org/wiki/Logistic_regression) - [Springleaf Marketing](https://www.kaggle.com/c/springleaf-marketing-response/data)
  - [Classification](https://en.wikipedia.org/wiki/Statistical_classification) - [Animal Shelter Outcomes](https://www.kaggle.com/c/shelter-animal-outcomes/data)


<b>Deliverables:</b>
  - 3 screenshots of your Kaggle submissions with scores in the top 75th percentile on the LB(leaderboard)

  - File(s) of your code <i>(Students may use any python based machine learning API's for the tasks and are not limited to sci-kit learn. Other technologies students might find useful and more challenging: H2O.ai, Apache Spark (PySpark), XGBoost)</i>


<h3><b>Assignment:</b></h3>

<b>Part 1:</b> Regression

1. Download the dataset from [https://www.kaggle.com/c/allstate-claims-severity/data](https://www.kaggle.com/c/allstate-claims-severity/data)

2. Load the train and test datasets into pandas dataframes

3. Figure out which variables are categorical and which are numeric. Linear models only accept numeric variables. You can either drop the categorical columns OR turn them into numeric variables (one-hot encoding, perturbed rate-by-level, label encoding, BLUP, etc). Many times these columns are vary useful and dropping them will hurt your model.

4. Feed your data in sci-kit learns Linear Regression algorithm. Sample code below:
    ```
    from sklearn import linear_model
    import numpy as np

    # LOAD DATA HERE

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

<b>Part 2:</b> Logistic Regression

1. Download the dataset from [https://www.kaggle.com/c/springleaf-marketing-response/data](https://www.kaggle.com/c/springleaf-marketing-response/data) - note this data set is much larger then the others. Will have a longer processing time.
2. Load the train and test datasets into pandas dataframes

3. Figure out which variables are categorical and which are numeric. Linear models only accept numeric variables. You can either drop the categorical columns OR turn them into numeric variables (one-hot encoding, perturbed rate-by-level, label encoding, BLUP, etc). Many times these columns are vary useful and dropping them will hurt your model.

4. Feed your data in sci-kit learns Logistic Regression algorithm. Sample code below:

    ```
    rom sklearn import linear_model

    # LOAD DATA HERE

    #create model object with one hyperparamater set
    logreg = linear_model.LogisticRegression(C=1e5)

    #Train the model
    logreg.fit(X_train, Y_train)
    ```
5. Run predictions on test set and create a submission csv file to submit to Kaggle.

    ```
    predictions = logreg.predict(X_test)
    # CRATE YOUR SUBMISSION FILE HERE
    ```

<b>Part 3:</b> Classification

1. Download the dataset from [https://www.kaggle.com/c/shelter-animal-outcomes/data](https://www.kaggle.com/c/shelter-animal-outcomes/data)
2. Load the train and test datasets into pandas dataframes
3. Feed your data in sci-kit learns Random Forest Ensemble model algorithm (Note: decision tree based models accept categorical columns and null values. Furthermore, it is much harder to overfit a random forest compared to a linear model.). Students may use any classification algorithm and are not limited to random forest. Advanced students may want to try the XGboost boosting library (one of the best algorithms for Kaggle). Sample code below:
    ```
    from sklearn.ensemble import RandomForestClassifier

    # LOAD DATA HERE

    #create model object with hyperparamater n_estimators
    #this will make 500 trees in the model
    clf = RandomForestClassifier(n_estimators=500)

    # train the model with training frames
    clf = clf.fit(X_train, Y_train)
    ```
4. Run predictions on test set and create a submission csv file to submit to Kaggle.

      ```
      predictions = clf.predict(X_test)
      # CRATE YOUR SUBMISSION FILE HERE
      ```
