# Pewlett_Hackard_Analysis




The purpose of the new analysis is well defined. (3 pt)
Results:

There is a bulleted list with four major points from the two analysis deliverables. (6 pt)
Summary:

The summary addresses the two questions and contains two additional queries or tables that may provide more insight. (5 pt)

Now that Bobby has proven his SQL chops, his manager has given both of you two more assignments: determine the number of retiring employees per title, and identify employees who are eligible to participate in a mentorship program. Then, you’ll write a report that summarizes your 
analysis and helps prepare Bobby’s manager for the “silver tsunami” as many current employees reach retirement age.

## Pewlett Hackard Analysis Overview
PewLett Hackard has been woring with Bobby in conducting an over-view of their retiring employees or to be more exact, those who are eligible for retirment. To that end, 3 csv files were created that showed from some originally provided data of ALL employees and the following tables were created for the first part of the analysis:

- current_emp.csv which showed ALL current employees elibible for retirement
- emp_info.csv which included information about those employees salaries
- manager_inf which identified which managers are due for retirement


Because Bobby impressed the PH senior management with the 3 original output files, they wanted him to do 2 additional analysis:
1) 3 queries were requested on some more of the general information about ALL the employees who are retiring: 
- A query was written for employees who are born between January 1, 1952 and December 31, 1955: retirement_titles.csv
- A query was written that contains the employee number, first and last name, and most recent title: unique_titles.csv.
- A query was written to create a table with the number of titles filled by employees who are retiring: retiring_titles.csv. 

2) The second request was for a more targeted program: determine the number of retiring employees per title, and identify employees who are eligible to participate in a mentorship program. For this, the data was more targeted; those employees who were born in 1965, a few years away from the eligibility age. PH would like to capitalize on this group's knowledge base and use it to crate a training or mentorship program. This will also help PH keep a closer eye on those employees whose retirement is approaching.  Bobby created one output file for this second piece:

- mentorship_eligibilty.csv

## PH Analysis Results:
Here are some interestng information that may need some further analysis to fully understand:
1) When you look at the retirement_titles.csv count vs the over-all employees.csv count, it shows an alarming number of employees are eligible to leave the company.  While there are some differences on the data-points of these two tables, a closer look needs to be taken to fully understand the situation with their employees.

![Pewlett_Hackard_Analysis](./ret_titles.png)
![Pewlett_Hackard_Analysis](./employee_count.png)

2) The second file results, unique_titles, did help understand the true number of employees who are reaching retirement eligibility.  This count output brought the original number to 90,398 which nearly 40,000 less than we were gathering from the unfiltered retirement_titles.  While this is a bit more reassuring, it is still a very large number of employees retiring.

![Pewlett_Hackard_Analysis](./actual_ret.png)

3) In looking at the unique_titles file, it is easy to note that many of the employees have risen among the ranks. Some have gone up two or more levels of employment. It would be interesting to see how employees in the past were able to be promoted and perhaps something more could be learned about this process.

4) The mentorship elibility csv really highlighted the remarkable drop in employess from 1952 to 1965. Bobby noticed the relatively low number on the count(*) of this output so created the same output with the 1952 year as input and the difference in number of employees retiring born in the year 1952 vs those born in the year 1965 is quite astounding, those born in 1952 who are eligible for retirement count is 16,981 vs those born in 1965 is 1,549.  That's more than 15 X's the employees who are eligible for retirement who were born in 1952 vs that of 1965. It is a good thing the are starting a mentorship program, but they may want to try something with those born  BEFORE 1965.

![Pewlett_Hackard_Analysis](./ret_1965.png)
![Pewlett_Hackard_Analysis](./ret_1952.png)

## PH Analysis Summary

As noted above in the analysis that has been completed, a closer look should be taken at retirement elibility as the numbers of those who may retire in the next few years is quite staggering:

Bobby ran a few different queries to further the analysis as an introduction as to what needs to be looked at:
Using the SQL for creating the mentorship_eligibilty.csv which was filtering on 1965, Bobby ran the same for 1952, 1953, and 1954;

1) Bobby knows there is an underlying question: How many roles will need to be filled as the "silver tsunami" begins to make an impact?

To answer this, Bobby refactored the SQL he used for the 1965 group and changed the range from January 1st of 1952 through December 31st of 1955, and came up with this number of employees who will be elible for retirement:

![Pewlett_Hackard_Analysis](./ret_silver.png)

2) Are there enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees?






## Resources
- Data Source: city_data.csv 
	       ride_data.csv
- Software: Matplotlib, Scipy, Pandas and Nympy.
# Challenge Overview
There were definitely parts of the challenge that were not clear which resulted in me wasting time on irrelevent points. Otherwise, it was a fun challenge - like a puzzle you are both creating and solving at the same time.
