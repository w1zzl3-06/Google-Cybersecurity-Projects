SELECT *
FROM log_in_attempts
WHERE login_time > '18:00' AND success = FALSE;

Returns the failed login attempts that occurred after business hours

SELECT * 
FROM log_in_attempts 
WHERE login_date = '2022-05-09' OR login_date = '2022-05-08';

Returns all login attempts that occurred on '2022-05-09' and before ‘2022-05-08'.

SELECT * 
FROM log_in_attempts 
WHERE NOT country LIKE 'MEX%';

Returns login attempts that did not originate in Mexico.

SELECT * 
FROM employees 
WHERE department = 'Marketing' AND office LIKE 'East%';

Returns employees in the 'Marketing' department who are located in all offices in the East building (such as 'East-170' or 'East-320').

SELECT * 
FROM employees 
WHERE department = 'Finance' OR department = 'Sales';

Returns records for employees in the 'Finance' or the 'Sales' department.

SELECT * 
FROM employees 
WHERE NOT department = 'Information Technology';

Returns records for employees who are not in the 'Information Technology' department.



