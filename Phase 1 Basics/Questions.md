# Question - Basics SQL

### Question 1: Retrieve All Columns
Retrieve all columns for all records from the table information.

**Input Description:**
You need to write a SQL query to fetch all the data from the information table.

**Example Output:**
| id  | first_name | last_name  | department              | gender | email                    | salary    | country   | city         | family_members | car   | job_title           | date_of_birth | project_count |
|-----|------------|------------|-------------------------|--------|--------------------------|-----------|-----------|--------------|----------------|-------|---------------------|---------------|---------------|
| 1   | Vassili    | Barfield   | NULL                    | Male   | vbarfield0@cbsnews.com   | $8958.13  | Israel    | Hod HaSharon | NULL           | NULL  | NULL                | 2001-10-16    | 686           |
| 2   | Riannon    | McCloid    | Business Development    | Female | rmccloid1@jiathis.com    | NULL      | France    | Vannes       | 3              | NULL  | NULL                | 2007-09-18    | 240           |
| 3   | Rodrigo    | Nodin      | Research and Development| Male   | rnodin2@sun.com          | $6957.33  | Cambodia  | Kampong Speu | NULL           | Lexus | Environmental Tech  | 1991-09-17    | 259           |

---
### Question 2: Filter by Country
Write a query to retrieve the first_name, last_name, and country of all individuals where the country is 'France'.

**Input Description:**
- Filter the records where country is 'France'.
- Return only the first_name, last_name, and country columns.

**Example Output:**
| first_name | last_name | country |
|------------|-----------|---------|
| Riannon    | McCloid   | France  |

---
### Question 3: Filter by Salary
Write a query to retrieve all columns for individuals whose salary is greater than $8000.

**Input Description:**
- Filter the records where the salary column is greater than $8000.
- Return all columns from the table.

**Example Output:**
| id  | first_name | last_name  | department | gender | email                  | salary    | country | city         | family_members | car   | job_title | date_of_birth | project_count |
|-----|------------|------------|------------|--------|------------------------|-----------|---------|--------------|----------------|-------|-----------|---------------|---------------|
| 1   | Vassili    | Barfield   | NULL       | Male   | vbarfield0@cbsnews.com | $8958.13  | Israel  | Hod HaSharon | NULL           | NULL  | NULL      | 2001-10-16    | 686           |

---
### Question 4: Count the Records
Write a query to count the total number of records in the information table.

**Input Description:**
- Use an aggregate function to count the rows in the table.

**Example Output:**
| total_records |
|---------------|
| 3             |

---
### Question 5: Retrieve Unique Job Titles
Write a query to fetch all unique job_title values from the information table.

**Input Description:**
- Return a list of distinct job_title values.

**Example Output:**
| job_title           |
|---------------------|
| NULL               |
| Environmental Tech |

---
### Question 6: Retrieve Records with Null Values in Department
Write a query to retrieve all columns for individuals where the department is NULL.

**Input Description:**
- Filter the rows where the department column has a NULL value.
- Return all columns from the table.

**Example Output:**
| id  | first_name | last_name | department | gender | email                  | salary    | country | city         | family_members | car   | job_title | date_of_birth | project_count |
|-----|------------|-----------|------------|--------|------------------------|-----------|---------|--------------|----------------|-------|-----------|---------------|---------------|
| 1   | Vassili    | Barfield  | NULL       | Male   | vbarfield0@cbsnews.com | $8958.13  | Israel  | Hod HaSharon | NULL           | NULL  | NULL      | 2001-10-16    | 686           |


---
### Question 7: Retrieve Records for Specific Gender
Write a query to retrieve all columns for individuals whose gender is 'Female'.

**Input Description:**
- Filter the rows where the gender column is 'Female'.
- Return all columns from the table.

**Example Output:**
| id  | first_name | last_name | department           | gender | email                 | salary | country | city   | family_members | car   | job_title | date_of_birth | project_count |
|-----|------------|-----------|----------------------|--------|-----------------------|--------|---------|--------|----------------|-------|-----------|---------------|---------------|
| 2   | Riannon    | McCloid   | Business Development | Female | rmccloid1@jiathis.com | NULL   | France  | Vannes | 3              | NULL  | NULL      | 2007-09-18    | 240           |

---
### Question 8: Retrieve Individuals by Minimum Project Count
Write a query to fetch the first_name, last_name, and project_count for individuals whose project_count is greater than or equal to 500.

**Input Description:**
- Filter the records where project_count is >= 500.
- Return the first_name, last_name, and project_count columns.

**Example Output:**
| first_name | last_name | project_count |
|------------|-----------|---------------|
| Vassili    | Barfield  | 686           |


---
### Question 9: Sort by Salary in Descending Order
Write a query to retrieve all columns, sorted by the salary column in descending order.

**Input Description:**
- Sort the table by salary in descending order.
- Return all columns.

**Example Output:**

| id  | first_name | last_name | department           | gender | email                  | salary    | country   | city         | family_members | car   | job_title           | date_of_birth | project_count |
|-----|------------|-----------|----------------------|--------|------------------------|-----------|-----------|--------------|----------------|-------|---------------------|---------------|---------------|
| 1   | Vassili    | Barfield  | NULL                 | Male   | vbarfield0@cbsnews.com | $8958.13  | Israel    | Hod HaSharon | NULL           | NULL  | NULL                | 2001-10-16    | 686           |
| 3   | Rodrigo    | Nodin     | Research and Development | Male | rnodin2@sun.com          | $6957.33  | Cambodia  | Kampong Speu | NULL           | Lexus | Environmental Tech  | 1991-09-17    | 259           |
| 2   | Riannon    | McCloid   | Business Development | Female | rmccloid1@jiathis.com    | NULL      | France    | Vannes       | 3              | NULL  | NULL                | 2007-09-18    | 240           |

---
### Question 10: Retrieve Records with Specific Car
Write a query to fetch all columns for individuals who own a Lexus.

**Input Description:**
- Filter the rows where the car column is 'Lexus'.
- Return all columns.

**Example Output:**

| id  | first_name | last_name | department             | gender | email            | salary    | country   | city         | family_members | car   | job_title           | date_of_birth | project_count |
|-----|------------|-----------|------------------------|--------|------------------|-----------|-----------|--------------|----------------|-------|---------------------|---------------|---------------|
| 3   | Rodrigo    | Nodin     | Research and Development | Male   | rnodin2@sun.com | $6957.33  | Cambodia  | Kampong Speu | NULL           | Lexus | Environmental Tech  | 1991-09-17    | 259           |

---
### Question 11: Count Records with Null Values in Car Column
Write a query to count the total number of individuals who do not own a car (car is NULL).

**Input Description:**
- Count the rows where the car column has a NULL value.

**Example Output:**
| total_null_cars |
|-----------------|
| 2               |

---
### Question 12: Retrieve Employees by Country
Write a query to fetch the first_name, last_name, and country for all individuals living in France.

**Input Description:**
- Filter the records where the country column is France.
- Return the first_name, last_name, and country columns.

**Example Output:**
| first_name | last_name | country |
|------------|-----------|---------|
| Riannon    | McCloid   | France  |

---
### Question 13: Retrieve Records with Specific Family Members Count
Write a query to fetch all columns for individuals who have exactly 3 family_members.

**Input Description:**
- Filter the rows where the family_members column equals 3.
- Return all columns.

**Example Output:**
| id  | first_name | last_name | department           | gender | email                 | salary | country | city   | family_members | car   | job_title | date_of_birth | project_count |
|-----|------------|-----------|----------------------|--------|-----------------------|--------|---------|--------|----------------|-------|-----------|---------------|---------------|
| 2   | Riannon    | McCloid   | Business Development | Female | rmccloid1@jiathis.com | NULL   | France  | Vannes | 3              | NULL  | NULL      | 2007-09-18    | 240           |

---