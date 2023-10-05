SELECT device_id, operating_system 
FROM machines;

The output lists only the selected columns from all the rows in the machines table

SELECT device_id, operating_system 
FROM machines 
WHERE operating_system = 'OS 2';

Select all the records from the machines table with a value of 'OS 2' in the operating_system column

SELECT * 
FROM employees 
WHERE department = 'Finance';

Filter the rows returned from department column in the employees table to include only employees from the 'Finance' department

SELECT * 
FROM employees 
WHERE department = 'Sales';

Returns employees who are in the 'Sales' department.

SELECT * 
FROM employees 
WHERE office = 'South-109';

Returns employees who are in the 'South-109’ office.

SELECT * 
FROM employees 
WHERE office LIKE 'South%';

Returns information on all the employees in the 'South' building

NOTE: The LIKE keyword in SQL performs simple string matches. The matching pattern may include the wildcard % to represent a string of any length. This wildcard may be placed both before and after the targeted substring.





