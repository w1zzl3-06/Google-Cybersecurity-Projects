SELECT * FROM 
log_in_attempts 
WHERE login_date > '2022-05-09';

Retrieves data for login attempts made after '2022-05-09'

SELECT * 
FROM log_in_attempts 
WHERE login_date >= '2022-05-09';

Retrieves data for login attempts that were made on or after '2022-05-09'

SELECT * 
FROM log_in_attempts 
WHERE login_date BETWEEN '2022-05-09' AND '2022-05-11';

Return login attempts that were made between '2022-05-09' and '2022-05-11'

SELECT * 
FROM log_in_attempts 
WHERE login_time < '07:00:00';

Retrieves data for login attempts made before '07:00:00'

SELECT * 
FROM log_in_attempts 
WHERE login_time BETWEEN '06:00:00' AND '07:00:00';

Return logins between '06:00:00' and '07:00:00'

SELECT event_id, username, login_date 
FROM log_in_attempts 
WHERE event_id >= 100;

Returns login attempts with event_id greater than or equal to 100.

SELECT event_id, username, login_date
FROM log_in_attempts 
WHERE event_id BETWEEN 100 AND 150;

Return only login attempts with event_id between 100 and 150.
