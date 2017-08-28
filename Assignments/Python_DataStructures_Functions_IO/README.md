<h1>Python: Data structures, Functions, & I/O </h1>

<b>Task:</b> Become familiar with python basics and learn how to read files, manipulate data, and use python functions (def key word).

<b>Due date:</b> TBD

<b>Deliverables:</b>
  - Output files from each part

  - Files of your code

  - All files should be compressed into a zip file before being uploaded

<b>Data files:</b>
  - [part_1_data.csv](data/part_1_data.csv)
  - [part_2_data.txt](data/part_2_data.txt)
  - [part_3_data.csv](data/part_3_data.csv)

<h3><b>Assignment:</b></h3>

<b>Part 1:</b> I/O - reading a csv file and creating a function

1. Create a function that reads a csv text file(```part_1_data.csv```) and converts it into a numpy array.

    ```
    import numpy as np
    fileInput (fileName):
      """
      :param string fileName: name of csv text file with comma separated numbers
      :return object: a numpy array
      """
      # WRITE FUNCTION CODE HERE
    if __name__ == '__main__':
      # INVOKE FUNCTION HERE
    ```
2. Output the shape of the numpy array into a text file called ```part_1_output.txt```and submit that along with your py file named ```part_1_code.py```.


<b>Part 2:</b> Reading a text file and plotting word count

1. Create a function that reads a text file(```part_2_data.txt```) and creates a dictionary of the word counts. Each word should be a key and the count of that word being the value.

    Sample dictionary structure:
    ```
    {
      "a_word": 2,
      "some_other_word": 5
    }
    ```
    Function:
    ```
    word_count (fileName):
      """
      :param string fileName: name of text file with words
      :return dict: a dictionary word count
      """
      # WRITE FUNCTION CODE HERE
      # REMEMBER TO STRIP EXTRA WHITE SPACE AFTER SPLITTING
    if __name__ == '__main__':
      # INVOKE FUNCTION HERE
    ```

2. Create another function that plots the word counts using matplotlib. The words should be on the X axis and counts on the Y axis. Title it ```Word Counts``` and include labels on each axis.

    ```
    import matplotlib
    plot_word_counts (dictionary):
      """
      :param dict dictionary: the dictionary of word counts
      :return dict: a matplotlib plot object
      """
      # WRITE FUNCTION CODE HERE

      return plot
    if __name__ == '__main__':
      # INVOKE FUNCTION HERE
    ```

3. Output the the word counts into text file called ```part_2_output.txt``` and save your plot to an image file called ```part_2_plot.png``` - submit both of these files along with py file named ```part_2_code.py```

<b>Part 3:</b> IF statements and FOR loops and JSON

1. Import the function from part one and use it to read the provided ```part_3_data.csv``` file. Do NOT copy and paste the function into a new file you must import it.

2. Loop through the file and calculate mean, standard dev, and median for each row. Use built in numpy functions for at least one of those descriptive statistics.

3. Output this to a json file named ```part_3_output.json```using the structure provided below. Only include rows in the json file that have n < 3 (use an if statement).

    ```
    [
      {
        "Row": 0,
        "Mean": 5.75,
        "Stddev": 2.2,
        "Median": 5
      },
      {
        "Row": 1,
        "Mean": 25.5,
        "Stddev": 5.2,
        "Median": 20
      }
    ]
    ```
4. Submit both the json file from step 3 and a code file named ```part_3_code.py```


<b>Grading Rubric:</b>


|    | Unsatisfactory | Satisfactory | Good | Excellent |
|:----------:|:-------------|:-------------| :-------------| :-------------|
| Delivery | ● Completed less than 70% of the requirements. <br> ● Not delivered on time or not in correct format (Blackboard or git) | ● Completed between 70-80% of the requirements. <br> ● Delivered on time, and in correct format (Blackboard or git)| ● Completed between 80-90% of the requirements. <br> ● Delivered on time, and in correct format (Blackboard or git)| ● Completed between 90-100% of the requirements. <br> ● Delivered on time, and in correct format (Blackboard or git) |
| Coding Standards | ● No name, date, or assignment title included <br> ● Poor use of white space (indentation, blank lines). <br> ● Disorganized and messy <br> ●Poor use of variables(many global variables, ambiguous naming). | ● Includes name, date, and assignment title. <br> ● White space makes program fairly easy to read.<br> ●Organized work. <br> ● Good use of variables (few global variables, unambiguous naming).| ●Includes name, date, and assignment title. <br> ●Good use of white space. <br> ● Organized work.<br> ●Good use of variables (no global variables, unambiguous naming) | ●Includes name, date, and assignment title. <br> ●Excellent use of white space. <br> ● Creatively organized work.<br> ●Excellent use of variables (no global variables, unambiguous naming). |
| Documentation | ● No documentation included. | ●Basic documentation has been completed including descriptions of all variables. <br> ●Purpose is noted for each function. | ● Clearly documented including descriptions of all variables. <br> ● Specific purpose is noted for each function and control structure.| ●Clearly and effectively documented including descriptions of all variables. <br> ●Specific purpose is noted for each function, control structure, input requirements, and output results. |
| Runtime | ●Does not execute due to errors. <br> ●User prompts are misleading or non-existent. <br> ● No testing has been completed.| ● Executes without errors(if applicable).<br> ● User prompts containlittle information, poordesign(if applicable).<br> ●Some testing has beencompleted.| ●Executes without errors <br> ●User prompts are understandable, minimum use of symbols or spacing in output(if applicable). <br> ● Thorough testing has been completed  | ●Executes without errors excellent. <br> ●user prompts, good use of symbols, spacing in output(if applicable). <br> ●Thorough and organized testing has been completed and output from test cases is included. |
| Efficiency | ●A difficult and inefficient solution. |  ●A logical solution that is easy to follow but it is not the most efficient. | ●Solution is efficient and easy to follow (i.e. no confusing tricks).| ●Solution is efficient, easy to understand, and maintain. |
