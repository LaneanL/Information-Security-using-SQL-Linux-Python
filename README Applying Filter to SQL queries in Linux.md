## Project description
You recently discovered a potential security incident that occurred after business hours. To investigate this, you need to query the log_in_attempts table and review after hours login activity. Use filters in SQL to create a query that identifies all failed login attempts that occurred after 18:00. (The time of the login attempt is found in the login_time column. The success column contains a value of 0 when a login attempt failed; you can use either a value of 0 or FALSE in your query to identify failed login attempts.)
Retrieve after hours failed login attempts
There was a potential security incident that occurred after business hours (18:00). All after hours login attempts that failed needed to be investigated.
  
.  
.  
.  
.  
.  
.  

### Example from file: Apply filter to SQL queries:
Retrieve after hours failed login attempts
There was a potential security incident that occurred after business hours (18:00). All after
hours login attempts that failed needed to be investigated.

SELECT * 
FROM log_in_attempts 
WHERE login_time > ‘18:00’ AND success = False;

![image](https://github.com/LaneanL/CyberSecurity/assets/132226337/a5483295-9013-4ac0-a1c6-d498caae77f0)

Start  selecting all data from the log_in_attempts table. A WHERE clause with an AND operator to filter the results to display only login attempts that occurred after 18:00 and were unsuccessful. The first condition is login_time > '18:00' which filters times outside of 18:00. The second condition is success = FALSE, which filters for the failed login attempts. 
