#Employee database analysis

This analysis is based on an employee database with 6 given cvs files. Each file holds uniquie information connected to each employee that is needed to retrieve information for each worker and manager.

The very first thing that was needed was to create tables for each csv file and importing that csv into the designated table. All the headers have also been labeled and assigned to a field type. 

First what was asked was to list the employee number, last name, first name, sex, and salary of each employee. Employee number, last name, first name, and sex were selected from the employee table. Salaries was selected from the salary table. Those two were joined to shown the given information while connecting employee number column from both tables.

Next I had to list the first name, last name, and hire date for the employees who were hired in 1986. First name, last name, and hire date were all part of the employees table so only that was used. After selecting the columns needed I neede to filter it only to 1986. I used the split_part method to select the 'hire_date' column, split it by '/', and only take out the third part of the whole date. I then had it equal to only year '1986' so only that information was retrieved from the employees.

Next I had to list the manager of each department along with their department number, department name, employee number, last name, and first name. Three tables were needed for this information. I first joined the department manager table with the employees table by connecting under employee number. Then I joined the departments table with the department manager table connecting with department number. 

Next I had to list the department number for each employee along with that employee’s employee number, last name, first name, and department name. Three tables were also needed to retrieve this information. I first joined the employees tables with the department employee tables connecting it with the employee number column. I also joined the departments table with the department employee table with the department number column.

Next that needed to be listed were first name, last name, and sex of each employee whose first name is Hercules and whose last name begins with the letter B. Only the employee table was needed for this information. I needed to use the where clause to retrieve only specific employees adjusting the filters for the first and last name columns. I also used the like clause to specifiy B% where employees whose last name that show up starting with a B is shown. 

Next I needed to list each employee in the Sales department, including their employee number, last name, and first name. I joined the employees table with the department employee table with the employee number column. I then joined the departments table with the department employee with the department number column. At the end i used the where clause to only show the department under 'Sales'.

Next I listed each employee in the Sales and Development departments, including their employee number, last name, first name, and department name. I joined the employees table with the department employee table with the employee number column. I then joined the departments table with the department employee with the department number column. This was similar to the step above. The only difference was within the where clause I added 'Development' within the where clause so information is shown under development and sales departments.

Lastly I listed the frequency counts, in descending order, of all the employee last names (that is, how many employees share each last name). The employees table was the only one needed for this information. I grouped the table by the last name column. I also used the order by function to makse sure the last name column was shown in descending order as requested.

        
---

© 2023 edX Boot Camps LLC. Confidential and Proprietary. All Rights Reserved.
