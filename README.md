# Pewlett-Hackard_Analysis

## Purpose
The purpose of this assignment was to create a database by merging files and then querying the results in SQL to provide an analysis of employees eligible to retire. By using ERD and SQL, we now have a number of employees eligible to retire as well as find ones who would be eligible to participate in a mentorship program. 

## Results

First we created an ERD (Entity Relationship Diagram) to map our tables in the database.

![](QuickDBD-export.PNG)

In Deliverable 1, we looked at all employees and then filtered the data to show employees that were born in between certain years (1952-1955). This gave us all employees that are eligible to retire but it contained multiple titles for each employee.

 ![](Resources/retirement_titles.PNG)

Then we used the SQL query "Distinct On" to make sure we were only counting an employee once (if they had switched job titles). This gave us the unique value so each employee was only counted once. The number of employees that are eligible to retire is 90,398. 

 ![](Resources/unique_titles.PNG)
 
 Lastly, we grouped the current employees eligible to retire by job title. Senior engineers was the largest group of titles and second to largest was senior staff. Only 2 employees out of 90,000 were managers. This seems odd to have so few managers with such a large senior staff. 

 ![](Resources/retiring_titles.PNG)

 In Deliverable 2, we looked at all employees that are eligble to participate in the mentorship program. Here we filtered the employee file to only current employees and ones that were born in 1965. There are a total of 1549 mentorship eligible employees. 
 
 ![](Resources/mentorship-eligibility.PNG)
 
 ## Summary
 
 ** How many roles will need to be filled as the "silver tsunami" begins to make an impact?
 
 There would be 90,398 employees eligible to retire which would mean sometime in the next 10 years these roles would need to be filled. 
 
 ** Are there enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees?
 
 There were only 1549 mentorship eligible employees. This is out of 90,0000 employees. I'd suggest widening the mentorship eligible program to more than just employees born  in 1965.
 
The biggest issue with the retirement by title data, was that it included all current and past employees eligible to retire. A better analysis would have been to filter by to-date as well to make sure we were only including current employees to find the true amount of employees eligible to retire. 
 
  ![](Resources/queryforactualemployees.PNG)

 
Another interesting table to look at would be one that showed the groups of titles by the mentorship eligibility group. Here we can see that senior staff is the largest group by title in the mentorship eligibility program.
 
   ![](Resources/mentorshipbytitle.PNG)

  


