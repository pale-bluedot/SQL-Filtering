# Filtering Log Activity Using SQL

## Objective
My organization is working to make their system more secure. It is my job to ensure the system is safe, investigate all potential security issues, and update employee computers as needed. The following steps provide examples of how I used SQL with filters to perform security-related tasks.

### Skills Learned
- Advanced understanding of SQL utilization in a security environment
- Proficiency in analyzing and interpreting network logs.
- Ability to generate and recognize potential breaches.
- Enhanced knowledge of network protocols and security vulnerabilities.
- Development of critical thinking and problem-solving skills in cybersecurity.

### Tools Used
- SQL 

## Steps

### 1. Retrieve after hours login attempts
There was a potential security incident that occurred after business hours (after 18:00). All after hours login attempts that failed need to be investigated.

The following code demonstrates how I created a SQL query to filter for failed login attempts that occurred after business hours.

![sql1](https://github.com/pale-bluedot/SQL-Filtering/assets/72536144/e3e16009-d44f-430a-b267-cf7747647e46)

*Ref 1: SQL Query*

### 2. Retrieve login attempts on specific dates
A suspicious event occurred on 2022-05-09. Any login activity that happened on 2022-05-09 or on the day before needs to be investigated.

The following code demonstrates how I created a SQL query to filter for login attempts that occurred on specific dates.

![sql2](https://github.com/pale-bluedot/SQL-Filtering/assets/72536144/0cca8563-5c68-4677-beed-527b0f1f8055)

*Ref 2: SQL Query*

### 3. Retrieve login attempts outside of Mexico
After investigating the organization’s data on login attempts, I believe there is an issue with the login attempts that occurred outside of Mexico. These login attempts should be investigated.

The following code demonstrates how I created a SQL query to filter for login attempts that occurred outside of Mexico. 

![sql3](https://github.com/pale-bluedot/SQL-Filtering/assets/72536144/8d3b2cd5-6329-4d0c-8e07-1f6c6f3fbb82)

*Ref 3: SQL Query*

### 4. Retrieve employees in Marketing Eastern Office
My team wants to update the computers for certain employees in the Marketing department. To do this, I have to get information on which employee machines to update.

The following code demonstrates how I created a SQL query to filter for employee machines from employees in the Marketing department in the East building.

![sql4](https://github.com/pale-bluedot/SQL-Filtering/assets/72536144/525b54d6-71c4-48f9-8e38-ec44149dfee5)

*Ref 4: SQL Query*

### 5. Retrieve employees in Finance or Sales
The machines for employees in the Finance and Sales departments also need to be updated. Since a different security update is needed, I have to get information on employees only from these two departments.

The following code demonstrates how I created a SQL query to filter for employee machines from employees in the Finance or Sales departments.

![sql5](https://github.com/pale-bluedot/SQL-Filtering/assets/72536144/bd1923fd-f63e-4d9a-a70d-e3717cc725d9)

*Ref 5: SQL Query*

### 6. Retrieve all employees not in IT
My team needs to make one more security update on employees who are not in the Information Technology department. To make the update, I first have to get information on these employees.

The following demonstrates how I created a SQL query to filter for employee machines from employees not in the  Information Technology department.

![sql6](https://github.com/pale-bluedot/SQL-Filtering/assets/72536144/f2ea7953-2bce-4f42-90d5-58069b82f3db)

*Ref 6: SQL Query*

## Summary
I applied filters to SQL queries to get specific information on login attempts and employee machines. I used two different tables, `log_in_attempts` and `employees`. I used the `AND`, `OR`, and `NOT` operators to filter for the specific information needed for each task. I also used `LIKE` and wildcard (`%`) to filter for patterns.

