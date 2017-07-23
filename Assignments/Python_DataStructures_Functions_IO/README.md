<h1>Python: Data structures, Functions, & I/O </h1>

<b>Task:</b> Become familiar with python basics and learn how to read files, manipulate data, and use python functions (def key word).

<b>Due date:</b> TBD

<b>Deliverables:</b>
  - Output files from each part

  - Files of your code

  - All files should be compressed into a zip file before being uploaded

<b>Data files:</b>
  - [part_1_data.csv](data/part_1_data.csv)
  - [part_2_data.txt](data/part_1_data.txt)
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
