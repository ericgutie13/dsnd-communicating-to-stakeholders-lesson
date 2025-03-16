
### Table of Contents

1. [Installation](#installation)
2. [Project Motivation](#motivation)
3. [File Descriptions](#files)
4. [Results](#results)
5. [Licensing, Authors, and Acknowledgements](#licensing)

## Installation <a name="installation"></a>

There should be no necessary libraries to run the code here beyond the Anaconda distribution of Python.  The code should run with no issues using Python versions 3.*.

## Project Motivation<a name="motivation"></a>

For this project, I was interestested in using Stack Overflow data from 2017 to better understand:

1. How other developers suggested breaking into the field (what education to pursue)?
2. What factors about an individual contributed to salary?
3. How bias played a role in the suggestions of developers for how to break into the field?
4. What was the state of bootcamps for assisting individuals with breaking into developer roles?
5. How were bootcamps assisting with increasing diversity in tech careers?

The full set of files related to this course are owned by Udacity, so they are not publicly available here.  However, you can see pieces of the analysis here.  This README also serves as a template for students to follow in creating their own project README files.


## File Descriptions <a name="files"></a>

There are 3 notebooks available here to showcase work related to the above questions.  Each of the notebooks is exploratory in searching through the data pertaining to the questions showcased by the notebook title.  Markdown cells were used to assist in walking through the thought process for individual steps. 

1. HowToBreakIntoTheField.ipynb: This notebook dives into the Stack Overflow public survey results and takes a deeper look into what advice would be given to a cousin who wanted to get into the software development field with little to no experience. This notebook looks to answer the first question above. 
2. BootcampStats.ipynb: This notebook dives into the Stack Overflow public survey results and looks to understand how being a graduate of this Bootcamp impacted job placement and salary.
3. Salary.ipynb: This notebook dives into the Stack Overflow public survey results and looks breakdown the relationship between salary and job satisfaction. 

There is an additional `.py` file that runs the necessary code to obtain the final model used to predict salary.

1. Salary_ML.py: Contains two functions clean_data and find_optimal_lm_mod.
    * clean_data: cleans the dataframe input using the following steps:
        1. Drop all the rows with no salaries
        2. Create X as all the columns that are not the Salary column
        3. Create y as the Salary column
        4. Drop the Salary, Respondent, and the ExpectedSalary columns
        5. For each numeric variable, fill the column with the mean value.
        6. Create dummy columns for all the categorical variables, drop the original columns
    * find_optimal_lm_mod: input is dataframe attributes and pertinent model information. output are several scoring metrics.


## Results<a name="results"></a>

The main findings of the code can be found at the post available [here](https://medium.com/@josh_2774/how-do-you-become-a-developer-5ef1c1c68711).

## Licensing, Authors, Acknowledgements<a name="licensing"></a>

Must give credit to Stack Overflow for the data.  You can find the Licensing for the data and other descriptive information at the Kaggle link available [here](https://www.kaggle.com/stackoverflow/so-survey-2017/data).  Otherwise, feel free to use the code here as you would like! 

