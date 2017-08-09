<h1>Pandas & Data Handling</h1>

<b>Task:</b>

<b>Due date:</b> TBD

<b>Deliverables:</b>
  - Submission files generated in each part

  - File(s) of your code


<h3><b>Assignment:</b></h3>

<b>Part 1:</b> Pandas

1. Start by creating 4 columns of data. The first should start at 0, last value should be 1000, increment by 1. The second should start at 0, last value should be 25,000, increment by 25. The third column should be a categorical column made by the following rules: it should have two characters, the first character relates to the first column the second relates to the second, if the first column is even then the first character is E otherwise it should be O, follow the same rule for the second column and second character, example if you have column1 = 5 and column2 = 100 then column3 should equal 'OE'. The fourth column of data should be loaded from `part1_column4.csv` (use pandas build in load csv and combine the two dataframes). Export this dataframe to `part1_ouput1.csv` and include this in your submission
    ```
    #Hint use a lambda function you will see them a lot in the data science
    #world. Most data scientists hate writing even one character of extra
    #code. Kaggle examples will be full of code like this; however one
    #could use a for loop.
    #Also note there is a slight problem in this line for making column1
    #that needs to be fixed for it to be accurate
    column = [x for x in range(0,1000)]
    ```

2. Load the columns into a pandas dataframe

3. Create a new dataframe from the current data and filter out rows where column 2 is greater than 1000. Must be done using pandas dataframe querying. Export this dataframe to `part1_ouput2.csv` and include this in your submission

4. Create a new dataframe from the ORIGINAL(step 2) dataframe with a new column named `column1|column2`. This column should contain values of column1 multiplied by column2 (note: for learning, this is called doing variable interactions). Export this to `part1_ouput3.csv` and include it in your submission.
    ```
    #this is the proper way to do this
    #.values gets a series from the dataframe (pandas version of a list)
    df['column1|column2'] = df['column1'].values*df['column2'].values
    ```

<b>Part 2:</b> Pandas and Matplotlib

1. Create a plot with column1 on the x axis and column2 on the y axis. Export this plot to an image and save it as `part2_plot1.png` and include in in your submission.

2. Create another plot with column3 on the x axis and the count of each category on the y axis. Export this plot to an image and save it `part2_plot2.png` and include in in your submission.

3. Create a line graph with three lines one for the columns: column1, column2, and column1|column2. The x axis should an auto incrementing row id variable 1 to X. The Y variable should be the value of the columns. Export this plot to `part3_plot3.png` and include in in your submission.


<b>Part 3:</b> SQL

1. Install the mysql python connector.
    - Documentation: https://dev.mysql.com/doc/connector-python/en/connector-python-example-connecting.html
    - Package home page: https://pypi.python.org/pypi/mysql-connector-python/2.0.4

2. Connect to your mysql database in python code (refer to documentation link for how to do this).

3.
