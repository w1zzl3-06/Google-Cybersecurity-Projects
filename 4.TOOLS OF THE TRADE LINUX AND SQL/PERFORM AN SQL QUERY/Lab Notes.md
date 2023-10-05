SELECT *
FROM machines;

Returns all device information from the machines table

SELECT device_id, email_client
FROM machines;

Returns only the device_id and email_client columns from the machines table

SELECT device_id, operating_system, OS_patch_date
FROM machines;

Returns only the device_id, operating_system, and OS_patch_date columns from the machines table

SELECT event_id, country
FROM log_in_attempts;

Returns the event_id and country columns from the log_in_attempts table

SELECT username, login_date, login_time
FROM log_in_attempts;

Returns the username, login_date, and login_time columns from the log_in_attempts table.

SELECT *
FROM log_in_attempts
ORDER BY login_date;

Orders log_in_attempts data by login_date

SELECT *
FROM log_in_attempts
ORDER BY login_date, login_time;

Orders log_in_attempts data by login_date and login_time


