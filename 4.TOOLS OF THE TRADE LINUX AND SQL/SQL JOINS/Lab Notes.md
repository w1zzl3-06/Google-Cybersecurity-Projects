SELECT * 
FROM machines 
INNER JOIN employees ON machines.device_id = employees.device_id;

Perform an inner join between the machines and employees tables on the device_id column

SELECT * 
FROM machines 
LEFT JOIN employees ON machines.device_id = employees.device_id;

Returns the information of all employees and any machines that are assigned to them.

Note: In a left join, all records from the table referenced after FROM and before LEFT JOIN are included in the result. In this case, all records from the machines table are included, regardless of whether they are assigned to an employee or not.

SELECT * 
FROM machines 
RIGHT JOIN employees ON machines.device_id = employees.device_id;

Note: In a right join, all records from the table referenced after RIGHT JOIN are included in the result. In this case, all records from the employees table are included, regardless of whether they have a machine or not.

SELECT * 
FROM employees 
INNER JOIN log_in_attempts ON employees.username = log_in_attempts.username;

Perform an inner join on the employees and log_in_attempts tables, linking them on the common username column.


