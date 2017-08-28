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


<b>Grading Rubric:</b>


|    | Unsatisfactory | Satisfactory | Good | Excellent |
|:----------:|:-------------|:-------------| :-------------| :-------------|
| Delivery | ● Completed less than 70% of the requirements. <br> ● Not delivered on time or not in correct format (Blackboard or git) | ● Completed between 70-80% of the requirements. <br> ● Delivered on time, and in correct format (Blackboard or git)| ● Completed between 80-90% of the requirements. <br> ● Delivered on time, and in correct format (Blackboard or git)| ● Completed between 90-100% of the requirements. <br> ● Delivered on time, and in correct format (Blackboard or git) |
| Coding Standards | ● No name, date, or assignment title included <br> ● Poor use of white space (indentation, blank lines). <br> ● Disorganized and messy <br> ●Poor use of variables(many global variables, ambiguous naming). | ● Includes name, date, and assignment title. <br> ● White space makes program fairly easy to read.<br> ●Organized work. <br> ● Good use of variables (few global variables, unambiguous naming).| ●Includes name, date, and assignment title. <br> ●Good use of white space. <br> ● Organized work.<br> ●Good use of variables (no global variables, unambiguous naming) | ●Includes name, date, and assignment title. <br> ●Excellent use of white space. <br> ● Creatively organized work.<br> ●Excellent use of variables (no global variables, unambiguous naming). |
| Documentation | ● No documentation included. | ●Basic documentation has been completed including descriptions of all variables. <br> ●Purpose is noted for each function. | ● Clearly documented including descriptions of all variables. <br> ● Specific purpose is noted for each function and control structure.| ●Clearly and effectively documented including descriptions of all variables. <br> ●Specific purpose is noted for each function, control structure, input requirements, and output results. |
| Runtime | ●Does not execute due to errors. <br> ●User prompts are misleading or non-existent. <br> ● No testing has been completed.| ● Executes without errors(if applicable).<br> ● User prompts containlittle information, poordesign(if applicable).<br> ●Some testing has beencompleted.| ●Executes without errors <br> ●User prompts are understandable, minimum use of symbols or spacing in output(if applicable). <br> ● Thorough testing has been completed  | ●Executes without errors excellent. <br> ●user prompts, good use of symbols, spacing in output(if applicable). <br> ●Thorough and organized testing has been completed and output from test cases is included. |
| Efficiency | ●A difficult and inefficient solution. |  ●A logical solution that is easy to follow but it is not the most efficient. | ●Solution is efficient and easy to follow (i.e. no confusing tricks).| ●Solution is efficient, easy to understand, and maintain. |
