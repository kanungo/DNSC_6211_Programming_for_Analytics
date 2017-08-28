<h1>Clustering: K-Means</h1>

<b>Task:</b> Use data from a [Kaggle](https://www.kaggle.com) dataset to create a cluster.

<b>Due date:</b> TBD

<b>Dataset:</b>
  - [Clustering Dataset](https://en.wikipedia.org/wiki/Cluster_analysis) - [Forest Cover Type Prediction](https://www.kaggle.com/c/forest-cover-type-prediction/data)

<b>Deliverables:</b>
  - `part1_new_feature.csv` file you create from clustering

  - `part1_correlation.txt` correlation value. We will check to make sure that your code outputs this value.

  - File(s) of your code

<h3><b>Assignment:</b></h3>

<b>Part 1:</b> K-Means

1. Download the dataset from [https://www.kaggle.com/c/forest-cover-type-prediction/data](https://www.kaggle.com/c/forest-cover-type-prediction/data). <i>(Remember use the train data for this, because the test isn't labeled (doesn't have a Y variable, or otherwise known as as target variable. Y/Label/Target all mean the same thing, get used to seeing them all being used interchangeably in literature.).</i>

2. Implement a k-means clustering algorithm from scratch (You may not use prewritten algorithms such as in sci-kit or other libraries). [Sample Tutorial - to get started](http://flothesof.github.io/k-means-numpy.html)

3. Submit .csv file named `part1_new_feature.csv` of the new feature for the test dataset made from your cluster - number it 1-X, 1 is the first cluster, 2 is your second cluster, etc. <i>(The hardest part about clustering is figuring out what the right number of clusters is. There are a few mathematical approaches to selecting the right number of clusters, but many times its just a business rule. Visualization of the clusters is important.)</i>

4. Find a new feature that has the highest correlation with the Y variable, Cover_Type. Try many different clusters till you find one with a high correlation. (<i> Hint: Use [scipy's pearsonr](https://docs.scipy.org/doc/scipy-0.15.1/reference/generated/scipy.stats.pearsonr.html) method.</i>) Submit the correlation you achieved to the Y variable in a file named `part1_correlation.txt`.


<b>Grading Rubric:</b>


|    | Unsatisfactory | Satisfactory | Good | Excellent |
|:----------:|:-------------|:-------------| :-------------| :-------------|
| Delivery | ● Completed less than 70% of the requirements. <br> ● Not delivered on time or not in correct format (Blackboard or git) | ● Completed between 70-80% of the requirements. <br> ● Delivered on time, and in correct format (Blackboard or git)| ● Completed between 80-90% of the requirements. <br> ● Delivered on time, and in correct format (Blackboard or git)| ● Completed between 90-100% of the requirements. <br> ● Delivered on time, and in correct format (Blackboard or git) |
| Coding Standards | ● No name, date, or assignment title included <br> ● Poor use of white space (indentation, blank lines). <br> ● Disorganized and messy <br> ●Poor use of variables(many global variables, ambiguous naming). | ● Includes name, date, and assignment title. <br> ● White space makes program fairly easy to read.<br> ●Organized work. <br> ● Good use of variables (few global variables, unambiguous naming).| ●Includes name, date, and assignment title. <br> ●Good use of white space. <br> ● Organized work.<br> ●Good use of variables (no global variables, unambiguous naming) | ●Includes name, date, and assignment title. <br> ●Excellent use of white space. <br> ● Creatively organized work.<br> ●Excellent use of variables (no global variables, unambiguous naming). |
| Documentation | ● No documentation included. | ●Basic documentation has been completed including descriptions of all variables. <br> ●Purpose is noted for each function. | ● Clearly documented including descriptions of all variables. <br> ● Specific purpose is noted for each function and control structure.| ●Clearly and effectively documented including descriptions of all variables. <br> ●Specific purpose is noted for each function, control structure, input requirements, and output results. |
| Runtime | ●Does not execute due to errors. <br> ●User prompts are misleading or non-existent. <br> ● No testing has been completed.| ● Executes without errors(if applicable).<br> ● User prompts containlittle information, poordesign(if applicable).<br> ●Some testing has beencompleted.| ●Executes without errors <br> ●User prompts are understandable, minimum use of symbols or spacing in output(if applicable). <br> ● Thorough testing has been completed  | ●Executes without errors excellent. <br> ●user prompts, good use of symbols, spacing in output(if applicable). <br> ●Thorough and organized testing has been completed and output from test cases is included. |
| Efficiency | ●A difficult and inefficient solution. |  ●A logical solution that is easy to follow but it is not the most efficient. | ●Solution is efficient and easy to follow (i.e. no confusing tricks).| ●Solution is efficient, easy to understand, and maintain. |
