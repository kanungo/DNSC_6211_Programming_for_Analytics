<h1>Web Scraping</h1>

<b>Task:</b> Your task is based on scraping the following searches on [Yelp](http://www.yelp.com):

1. Search term: `mexican food` Location: `Washington, DC`
![screenshot](resources/mexican.png)
2. Search term: `chinese food` Location: `Washington, DC`
![graph](resources/chinese.png)

<b>Due date:</b> TBD

<b>Deliverables:</b>
  - `part1_chinese.csv` and `part1_mexican.csv` files you create from scraping

  - `part2_histRatingChinese.pdf` and `part2_histRatingMexican.pdf` plots

  - `part3_CXY1.pdf`, `part3_CXY2.pdf`, `part3_MXY1.pdf`, `part3_MXY2.pdf` plots

  - File(s) of your code

<h3><b>Assignment:</b></h3>

<b>Part 1:</b> Initial Scraping

1. Scrape the following data from ALL restaurants in both searches.
  - Restaurant Name
  - Street Address
  - City
  - State
  - Zip
  - Phone
  - Number of Reviews
  - Rating
  - Price Range


2. Store the data from Mexican restaurants as `part1_mexican.csv` Store the data from Chinese restaurants as `part1_chinese.csv`. Submit these files.

<b>Part 2:</b> Histogram

1. Draw the histogram of  Rating  for both Mexican and Chinese restaurants and save then in separate image files named `part2_histRatingChinese.pdf` and `part2_histRatingMexican.pdf`. Make sure that the plots are labelled - axis labels for both axes and plot title. Submit these files.

<b>Part 3:</b> Correlation Plots

1. For Chinese restaurants: Plot the relationship between  Rating (Y) and  Price Range (X). Label it and save it as `part3_CXY1.pdf`.

2. For Chinese restaurants: Plot the relationship between  Rating (Y) and  Number of reviews (X). Label it and save it as  `part3_CXY2.pdf`.

3. For Mexican restaurants: Plot the relationship between  Rating (Y) and  Price Range (X). Label it and save it as `part3_MXY1.pdf`.

4. For Mexican restaurants: Plot the relationship between  Rating (Y) and  Number of reviews (X). Label it and save it as `part3_MXY2.pdf`.

<b>Part 4:</b> Combined plots

1. Combine  `mexican.csv`  and  `chinese.csv` into one one. Regress  Rating  (Y) on  Price Range  (X) and  Number of reviews  (X). Print out the coefficients and the R squared. Make a 3D plot (with both axes labelled and a title) and save it as  `part4_regress.png`.



<b>Grading Rubric:</b>


|    | Unsatisfactory | Satisfactory | Good | Excellent |
|:----------:|:-------------|:-------------| :-------------| :-------------|
| Delivery | ● Completed less than 70% of the requirements. <br> ● Not delivered on time or not in correct format (Blackboard or git) | ● Completed between 70-80% of the requirements. <br> ● Delivered on time, and in correct format (Blackboard or git)| ● Completed between 80-90% of the requirements. <br> ● Delivered on time, and in correct format (Blackboard or git)| ● Completed between 90-100% of the requirements. <br> ● Delivered on time, and in correct format (Blackboard or git) |
| Coding Standards | ● No name, date, or assignment title included <br> ● Poor use of white space (indentation, blank lines). <br> ● Disorganized and messy <br> ●Poor use of variables(many global variables, ambiguous naming). | ● Includes name, date, and assignment title. <br> ● White space makes program fairly easy to read.<br> ●Organized work. <br> ● Good use of variables (few global variables, unambiguous naming).| ●Includes name, date, and assignment title. <br> ●Good use of white space. <br> ● Organized work.<br> ●Good use of variables (no global variables, unambiguous naming) | ●Includes name, date, and assignment title. <br> ●Excellent use of white space. <br> ● Creatively organized work.<br> ●Excellent use of variables (no global variables, unambiguous naming). |
| Documentation | ● No documentation included. | ●Basic documentation has been completed including descriptions of all variables. <br> ●Purpose is noted for each function. | ● Clearly documented including descriptions of all variables. <br> ● Specific purpose is noted for each function and control structure.| ●Clearly and effectively documented including descriptions of all variables. <br> ●Specific purpose is noted for each function, control structure, input requirements, and output results. |
| Runtime | ●Does not execute due to errors. <br> ●User prompts are misleading or non-existent. <br> ● No testing has been completed.| ● Executes without errors(if applicable).<br> ● User prompts containlittle information, poordesign(if applicable).<br> ●Some testing has beencompleted.| ●Executes without errors <br> ●User prompts are understandable, minimum use of symbols or spacing in output(if applicable). <br> ● Thorough testing has been completed  | ●Executes without errors excellent. <br> ●user prompts, good use of symbols, spacing in output(if applicable). <br> ●Thorough and organized testing has been completed and output from test cases is included. |
| Efficiency | ●A difficult and inefficient solution. |  ●A logical solution that is easy to follow but it is not the most efficient. | ●Solution is efficient and easy to follow (i.e. no confusing tricks).| ●Solution is efficient, easy to understand, and maintain. |
